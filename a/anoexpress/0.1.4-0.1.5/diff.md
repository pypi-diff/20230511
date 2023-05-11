# Comparing `tmp/anoexpress-0.1.4.tar.gz` & `tmp/anoexpress-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anoexpress-0.1.4.tar", max compression
+gzip compressed data, was "anoexpress-0.1.5.tar", max compression
```

## Comparing `anoexpress-0.1.4.tar` & `anoexpress-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1075 2022-11-12 23:31:02.745561 anoexpress-0.1.4/LICENSE
--rw-r--r--   0        0        0       66 2023-03-06 23:08:43.188006 anoexpress-0.1.4/anoexpress/__init__.py
--rw-r--r--   0        0        0    27217 2023-04-19 14:11:43.044076 anoexpress-0.1.4/anoexpress/anoexpress.py
--rw-r--r--   0        0        0      750 2023-04-19 14:11:31.544075 anoexpress-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 anoexpress-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-11-12 23:31:02.745561 anoexpress-0.1.5/LICENSE
+-rw-r--r--   0        0        0       66 2023-03-06 23:08:43.188006 anoexpress-0.1.5/anoexpress/__init__.py
+-rw-r--r--   0        0        0    28444 2023-05-11 11:57:59.581707 anoexpress-0.1.5/anoexpress/anoexpress.py
+-rw-r--r--   0        0        0      750 2023-05-11 11:57:59.585707 anoexpress-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 anoexpress-0.1.5/PKG-INFO
```

### Comparing `anoexpress-0.1.4/LICENSE` & `anoexpress-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `anoexpress-0.1.4/anoexpress/anoexpress.py` & `anoexpress-0.1.5/anoexpress/anoexpress.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,48 +9,48 @@
                     }
 
 index_col = {'fcs':'comparison',
             'pvals': 'comparison',
             'log2counts': 'sampleID'}
 
 
-# Ano-express
+# AnoExpress
 def load_results_arrays(data_type, analysis):
     """
     Load the counts data for a given analysis and sample query
     """
     assert data_type in ['log2counts', 'fcs', 'pvals'], "data_type must be either 'log2counts', 'fcs' or 'pvals'"
     assert analysis in ['gamb_colu', 'gamb_colu_arab', 'gamb_colu_arab_fun', 'fun', 'irtex'], "analysis must be either 'gamb_colu', 'gamb_colu_arab', 'gamb_colu_arab_fun', 'fun' or 'irtex'"
-    df_data = pd.read_csv(f"https://raw.githubusercontent.com/sanjaynagi/Ano-express/main/results/{data_type}.{analysis}.tsv", sep="\t")
-    df_data = df_data.drop(columns=['GeneDescription']).set_index(['GeneID', 'GeneName']) if data_type == 'fcs' and analysis != 'irtex' else df_data.set_index("GeneID")
+    df_data = pd.read_csv(f"https://raw.githubusercontent.com/sanjaynagi/AnoExpress/main/results/{data_type}.{analysis}.tsv", sep="\t")
+    df_data = df_data.set_index('GeneID')
     return(df_data)
 
 def sample_metadata(analysis):
     """
     Load the sample metadata in a pandas dataframe
     """
-    sample_metadata = pd.read_csv("https://raw.githubusercontent.com/sanjaynagi/Ano-express/main/config/sample_metadata.tsv", sep="\t")
+    sample_metadata = pd.read_csv("https://raw.githubusercontent.com/sanjaynagi/AnoExpress/main/config/sample_metadata.tsv", sep="\t")
     sample_metadata = sample_metadata.query(taxon_query_dict[analysis])
     return sample_metadata
 
 def xpress_metadata():
-    comparison_metadata = pd.read_csv("https://raw.githubusercontent.com/sanjaynagi/Ano-express/main/config/comparison_metadata.tsv", sep="\t")
+    comparison_metadata = pd.read_csv("https://raw.githubusercontent.com/sanjaynagi/AnoExpress/main/config/comparison_metadata.tsv", sep="\t")
     return(comparison_metadata)
 
 def irtex_metadata():
     """
     Load the ir-tex fold change data for a given analysis and sample query
     """   
-    comparison_metadata = pd.read_csv("https://raw.githubusercontent.com/sanjaynagi/Ano-express/main/config/irtex_metadata.tsv", sep="\t")
+    comparison_metadata = pd.read_csv("https://raw.githubusercontent.com/sanjaynagi/AnoExpress/main/config/irtex_metadata.tsv", sep="\t")
     return(comparison_metadata)
 
 
 def metadata(analysis, microarray=False):
     """
-    Load the comparisons metadata from both Ano-express and IR-Tex in a pandas dataframe
+    Load the comparisons metadata from both AnoExpress and IR-Tex in a pandas dataframe
 
     Parameters
     ----------
     analysis: {"gamb_colu", "gamb_colu_arab", "gamb_colu_arab_fun", "fun"}
       which analysis to load gene expression data for. analyses with more species will have less genes
       present, due to the process of finding orthologs.
     microarray: bool, optional
@@ -59,15 +59,15 @@
       whether to return the sample metadata in addition to the comparisons metadata. Default is False.
 
     Returns
     -------
     comparisons_df: pandas dataframe
     samples_df: pandas dataframe
     """
-    # load metadata from Ano-express
+    # load metadata from AnoExpress
     metadata = xpress_metadata()   
     metadata = metadata.assign(technology='rnaseq')
 
     # load metadata from IR-Tex
     if microarray == True:
         irtex_meta = irtex_metadata()
         irtex_meta = irtex_meta.assign(technology='microarray')
@@ -75,15 +75,15 @@
 
     # subset to the species of interest
     metadata = metadata.query(taxon_query_dict[analysis])
 
     return metadata
 
 
-def data(data_type, analysis, microarray=False, gene_id=None, sort_by=None):
+def data(data_type, analysis, microarray=False, gene_id=None, sort_by=None, annotations=False, pvalue_filter=None):
     """
     Load the combined data for a given analysis and sample query
 
     Parameters
     ----------
     data_type: {"fcs", "pvals", "log2counts"}
       which data type to load gene expression data for. log2counts are the log2 counts, fcs are the fold changes, and pvals are the adjusted p-values.
@@ -91,14 +91,21 @@
       which analysis to load gene expression data for. analyses with more species will have less genes
       present, due to the process of finding orthologs.
     microarray: bool, optional
       whether to include the IR-Tex microarray data in the requested data. Default is False.
     gene_id: str or list, optional
       A string (AGAP/AFUN identifier), or list of strings, or path to a file containing a list of gene ids in the first column. 
       Input file can be .tsv, .txt, or .csv, or .xlsx.
+    sort_by: {"median", "mean", "agap", "position", None}, optional
+      sort by median/mean of fold changes (descending), or by AGAP, or by position in the genome, or dont sort input gene ids.
+    annotations: bool, optional
+      whether to add gene name and description to the dataframe as index. Default is False.
+    pvalue_filter: float, optional
+      if provided, fold-change entries with an adjusted p-value below the threshold will be set to NaN. Default is None.
+      ignored if the data_type is not 'fcs'. 
     
     Returns
     -------
     results_data: pandas dataframe
     """
     assert analysis in ['gamb_colu', 'gamb_colu_arab', 'gamb_colu_arab_fun', 'fun'], "analysis must be one of 'gamb_colu', 'gamb_colu_arab', 'gamb_colu_arab_fun', 'fun'"
     assert data_type in ['log2counts', 'fcs', 'pvals'], "data_type must be one of 'log2counts', 'fcs', 'pvals'"
@@ -110,15 +117,15 @@
       df_metadata = sample_metadata(analysis=analysis)
 
     # load the data and merge wit microarray data if requested
     df = load_results_arrays(data_type=data_type, analysis=analysis)
     # load ir-tex data and merge
     if microarray == True and data_type != 'log2counts':
         irtex_df = load_results_arrays(data_type=data_type, analysis='irtex')
-        df = df.reset_index().merge(irtex_df, on='GeneID', how='left').set_index(['GeneID', 'GeneName'])
+        df = df.reset_index().merge(irtex_df, on='GeneID', how='left').set_index('GeneID')
 
     # get the sample or comparison ids 
     metadata_ids = df_metadata.loc[:, index_col[data_type]].to_list()
     # subset to the species comparisons of interest
     df = df.loc[:, metadata_ids]
 
     # subset to the gene ids of interest including reading file 
@@ -128,43 +135,58 @@
             gene_id = pd.read_csv(gene_id, sep="\t", header=None).iloc[:, 0].to_list()
         elif gene_id.endswith('.csv'):
             gene_id = pd.read_csv(gene_id, header=None).iloc[:, 0].to_list()
         elif gene_id.endswith('.xlsx'):
             gene_id = pd.read_excel(gene_id, header=None).iloc[:, 0].to_list()
       df = df.query("GeneID in @gene_id")
 
+    if annotations: # add gene name and description to the dataframe as index 
+      df = add_annotations_to_array(df)
+    
+    if data_type == 'fcs' and pvalue_filter is not None:
+      pval_df = data(data_type="pvals", analysis=analysis, microarray=microarray, gene_id=gene_id, sort_by=sort_by, annotations=False)
+      df = null_fold_changes(pval_df=pval_df, fc_df=df, threshold=pvalue_filter)
+
     # sort genes 
     df = _sort_genes(df=df, analysis=analysis, sort_by=sort_by)
     
     return df
 
+def null_fold_changes(pval_df, fc_df, threshold=0.05):
+    fold_changes_null = fc_df.copy() # make a copy of fold_changes to modify
+    fold_changes_null[pval_df > threshold] = np.nan # set values to NaN where pvalue > 0.05
+    return fold_changes_null
+ 
+def add_annotations_to_array(df):
+    df_annots = pd.read_csv("https://raw.githubusercontent.com/sanjaynagi/AnoExpress/main/resources/AgamP4.annots.tsv", sep="\t")
+    df = df.reset_index().merge(df_annots, on="GeneID", how="left").set_index(["GeneID", "GeneName", "GeneDescription"])   
+    return df 
 
 def _sort_genes(df, analysis, sort_by=None):
-  df = df.reset_index()
   if sort_by is None:
      return df.copy()
   if sort_by == 'median':
-    sort_idxs = np.argsort(df.set_index('GeneID').drop(columns='GeneName', errors='ignore').apply(np.nanmedian, axis=1)).values
+    sort_idxs = np.argsort(df.apply(np.nanmedian, axis=1)).values
   elif sort_by == 'mean':
-    sort_idxs = np.argsort(df.set_index('GeneID').drop(columns='GeneName', errors='ignore').apply(np.nanmean, axis=1)).values
+    sort_idxs = np.argsort(df.apply(np.nanmean, axis=1)).values
   elif sort_by == 'agap':
-    sort_idxs = np.argsort(df['GeneID'].values)
+    sort_idxs = np.argsort(df.reset_index()['GeneID'].values)
   elif sort_by == 'position':
     assert analysis != 'fun', "funestus cannot be sorted by position yet"
     
     import malariagen_data
     ag3 = malariagen_data.Ag3()
     gff = ag3.genome_features().query("type == 'gene' & contig in @ag3.contigs")
-    gene_ids = df['GeneID'].to_list()
-    ordered_genes = gff.query(f"ID in '{gene_ids}'")['ID'].to_list()
-    sort_idxs = [np.where(df['GeneID'] == gene)[0][0] for gene in ordered_genes]
+    gene_ids = df.reset_index()['GeneID'].to_list()
+    ordered_genes = gff.query(f"ID in {gene_ids}")['ID'].to_list()
+    sort_idxs = [np.where(df.reset_index()['GeneID'] == gene)[0][0] for gene in ordered_genes]
 
   return df.iloc[sort_idxs, :].copy()
 
-def plot_gene_expression(gene_id, analysis="gamb_colu_arab_fun", microarray=False, title=None, plot_type='strip', sort_by='agap', width=1600, height=None, save_html=None):
+def plot_gene_expression(gene_id, analysis="gamb_colu_arab_fun", microarray=False, title=None, plot_type='strip', sort_by='agap', pvalue_filter=None, width=1600, height=None, save_html=None):
     """Plot fold changes of provided AGAP gene IDs from RNA-Seq 
     meta-analysis dataset
 
     Parameters
     ----------
 
     gene_id : str or list
@@ -193,23 +215,23 @@
     import plotly.subplots as sp
     
     # load the metadata and subset to the species of interest
     df_metadata = metadata(analysis=analysis, microarray=microarray)
     df_samples = sample_metadata(analysis=analysis)
 
     # load fold change data, make long format and merge with metadata for hovertext
-    fc_data = data(data_type="fcs", analysis=analysis, microarray=microarray, gene_id=gene_id, sort_by=sort_by)
+    fc_data = data(data_type="fcs", analysis=analysis, microarray=microarray, gene_id=gene_id, sort_by=sort_by, annotations=True, pvalue_filter=pvalue_filter).reset_index()
     # load count data, make long format and merge with metadata for hovertext
-    count_data = data(data_type="log2counts", analysis=analysis, microarray=microarray, gene_id=gene_id, sort_by=None).set_index('GeneID')
+    count_data = data(data_type="log2counts", analysis=analysis, microarray=microarray, gene_id=gene_id, sort_by=None)
     count_data = count_data.loc[fc_data['GeneID']].reset_index()
     count_data = count_data.melt(id_vars='GeneID', var_name='sampleID', value_name='log2_counts')
     count_data = count_data.merge(df_samples, how='left').assign(counts = lambda x: np.round(2**x.log2_counts, 0))
 
     fc_data.loc[:, 'Label'] = [id_ + " | " + name if name != "" else id_ for id_, name in zip(fc_data['GeneID'].fillna(""), fc_data['GeneName'].fillna(""))]
-    fc_data = fc_data.drop(columns=['GeneName', 'GeneID']).melt(id_vars='Label', var_name='comparison', value_name='log2FC')
+    fc_data = fc_data.drop(columns=['GeneName', 'GeneID', 'GeneDescription']).melt(id_vars='Label', var_name='comparison', value_name='log2FC')
     fc_data = fc_data.merge(df_metadata, how='left')
 
     if not height:
       height = np.min([fc_data.shape[0]*12, 2500])
     
     if not title:
       title = ""
@@ -325,16 +347,16 @@
 
   return(fig)
 
 def load_annotations():
     """
     Load pfam or go annotations for Anopheles gambiae 
     """
-    pfam_df = pd.read_csv("https://github.com/sanjaynagi/ano-express/blob/main/resources/Anogam_long.pep_Pfamscan.seqs.gz?raw=true", sep="\s+", header=None, compression='gzip')
-    go_df = pd.read_csv("https://github.com/sanjaynagi/ano-express/blob/main/resources/Anogam_long.pep_eggnog_diamond.emapper.annotations.GO.gz?raw=true", sep="\t", header=None, compression='gzip')
+    pfam_df = pd.read_csv("https://github.com/sanjaynagi/AnoExpress/blob/main/resources/Anogam_long.pep_Pfamscan.seqs.gz?raw=true", sep="\s+", header=None, compression='gzip')
+    go_df = pd.read_csv("https://github.com/sanjaynagi/AnoExpress/blob/main/resources/Anogam_long.pep_eggnog_diamond.emapper.annotations.GO.gz?raw=true", sep="\t", header=None, compression='gzip')
     pfam_df.columns = ["transcript", "pstart", "pend", "pfamid", "domain", "domseq"]
     go_df.columns = ['transcript', 'GO_terms']
 
     gene_annot_df = pfam_df.merge(go_df)
     gene_annot_df.loc[:, 'gene_id'] = gene_annot_df.loc[:, 'transcript'].str.replace("Anogam_", "").str.replace("-R[A-Z]", "", regex=True)
     return(gene_annot_df)
 
@@ -358,16 +380,16 @@
     query_fc: float, optional
       filter genes by fold change. Defaults to None
     
     Returns
     -------
     fc_ranked: pd.DataFrame
     """
-    fc_data = pd.read_csv(f"https://raw.githubusercontent.com/sanjaynagi/ano-express/main/results/fcs.{analysis}.tsv", sep="\t")
-    fc_data = fc_data.set_index(['GeneID', 'GeneName', 'GeneDescription'])
+    
+    fc_data = data(data_type='fcs', analysis=analysis, microarray=False, annotations=True, sort_by=None)
 
     if query_annotation is not None:
       gene_annot_df = load_annotations()
       gene_ids = _gene_ids_from_annotation(gene_annot_df=gene_annot_df, annotation=query_annotation)
       fc_data = fc_data.query("GeneID in @gene_ids")
       assert not fc_data.empty, "No genes were found for the selection. It is possible these genes were removed by the ortholog finding process"
     
@@ -399,24 +421,24 @@
       percentile of genes to use for the enriched set in hypergeometric test. Defaults to 0.05
 
     Returns
     -------
     go_hypergeo_results: pd.DataFrame
     """
 
-    fc_data = pd.read_csv(f"https://raw.githubusercontent.com/sanjaynagi/ano-express/main/results/fcs.{analysis}.tsv", sep="\t")
+    fc_data = pd.read_csv(f"https://raw.githubusercontent.com/sanjaynagi/AnoExpress/main/results/fcs.{analysis}.tsv", sep="\t")
     fc_genes = fc_data.reset_index()['GeneID'].to_list()
 
     # get top % percentile genes ranked by func
     fc_ranked = load_candidates(analysis=analysis, name=name, func=func)
     percentile_idx = fc_ranked.reset_index()['GeneID'].unique().shape[0] * percentile
     top_geneIDs = fc_ranked.reset_index().loc[:, 'GeneID'][:int(percentile_idx)] 
 
     # load gene annotation file 
-    gaf_df = pd.read_csv("https://raw.githubusercontent.com/sanjaynagi/ano-express/main/resources/AgamP4.gaf", sep="\t")
+    gaf_df = pd.read_csv("https://raw.githubusercontent.com/sanjaynagi/AnoExpress/main/resources/AgamP4.gaf", sep="\t")
     go_annotations = gaf_df[['go_term', 'descriptions']].rename(columns={'go_term':'annotation'}).drop_duplicates()
     gaf_df = gaf_df[['GeneID', 'go_term']].drop_duplicates()
     gaf_df = gaf_df.query("GeneID in @fc_genes")
     N = gaf_df.GeneID.unique().shape[0] #Total number of genes with some annotation 
     k = np.isin(gaf_df.loc[:, 'GeneID'].unique(), top_geneIDs).sum() 
 
     hyper_geo = _hypergeometric(
@@ -447,24 +469,24 @@
     
     Returns
     -------
     pfam_hypergeo_results: pd.DataFrame
     """
 
     # get all genes
-    fc_data = pd.read_csv(f"https://raw.githubusercontent.com/sanjaynagi/ano-express/main/results/fcs.{analysis}.tsv", sep="\t")
+    fc_data = pd.read_csv(f"https://raw.githubusercontent.com/sanjaynagi/AnoExpress/main/results/fcs.{analysis}.tsv", sep="\t")
     fc_genes = fc_data.reset_index()['GeneID'].to_list()
 
     # get top 5% percentile genes ranked by median
     fc_ranked = load_candidates(analysis=analysis, name=name, func=func)
     percentile_idx = fc_ranked.reset_index()['GeneID'].unique().shape[0] * percentile
     top_geneIDs = fc_ranked.reset_index().loc[:, 'GeneID'][:int(percentile_idx)] 
 
     # load gene annotation file 
-    pfam_df = pd.read_csv("https://github.com/sanjaynagi/ano-express/blob/main/resources/Anogam_long.pep_Pfamscan.seqs.gz?raw=true", sep="\s+", header=None, compression='gzip').iloc[:, [0,4]]
+    pfam_df = pd.read_csv("https://github.com/sanjaynagi/AnoExpress/blob/main/resources/Anogam_long.pep_Pfamscan.seqs.gz?raw=true", sep="\s+", header=None, compression='gzip').iloc[:, [0,4]]
     pfam_df.loc[:, 0] = pfam_df.loc[:, 0].str.replace("Anogam_", "").str.replace("-R[A-Z]", "", regex=True)
     pfam_df.columns = ['GeneID', 'pfam']
     pfam_df = pfam_df.query("GeneID in @fc_genes")
     N = pfam_df.GeneID.unique().shape[0] #Total number of genes with some annotation 
     k = np.isin(pfam_df.loc[:, 'GeneID'].unique(), top_geneIDs).sum()  
 
     # run hypergeometric test
@@ -494,24 +516,24 @@
       percentile of genes to use for the enriched set in hypergeometric test. Defaults to 0.05
 
     Returns
     -------
     go_hypergeo_results: pd.DataFrame
     """
 
-    fc_data = pd.read_csv(f"https://raw.githubusercontent.com/sanjaynagi/ano-express/main/results/fcs.{analysis}.tsv", sep="\t")
+    fc_data = pd.read_csv(f"https://raw.githubusercontent.com/sanjaynagi/AnoExpress/main/results/fcs.{analysis}.tsv", sep="\t")
     fc_genes = fc_data.reset_index()['GeneID'].to_list()
 
     # get top % percentile genes ranked by func
     fc_ranked = load_candidates(analysis=analysis, name=name, func=func)
     percentile_idx = fc_ranked.reset_index()['GeneID'].unique().shape[0] * percentile
     top_geneIDs = fc_ranked.reset_index().loc[:, 'GeneID'][:int(percentile_idx)] 
 
     # load gene annotation file 
-    kegg_df = pd.read_csv("https://raw.githubusercontent.com/sanjaynagi/ano-express/main/resources/AgamP4.kegg", sep="\t")
+    kegg_df = pd.read_csv("https://raw.githubusercontent.com/sanjaynagi/AnoExpress/main/resources/AgamP4.kegg", sep="\t")
     kegg_annotations = kegg_df[['kegg_pathway', 'description']].rename(columns={'kegg_pathway':'annotation'}).drop_duplicates()
     kegg_df = kegg_df[['GeneID', 'kegg_pathway']].drop_duplicates()
     kegg_df = kegg_df.query("GeneID in @fc_genes")
     N = kegg_df.GeneID.unique().shape[0] #Total number of genes with some annotation 
     k = np.isin(kegg_df.loc[:, 'GeneID'].unique(), top_geneIDs).sum() 
 
     hyper_geo = _hypergeometric(
@@ -576,15 +598,15 @@
     cbar_pos: {"left", "right", "top", "bottom"}, optional
       position of colorbar. Defaults to None.
     figsize: tuple, optional
       size of figure.
     """
     import seaborn as sns
     # load metadata
-    fc_data = pd.read_csv(f"https://raw.githubusercontent.com/sanjaynagi/ano-express/main/results/fcs.{analysis}.tsv", sep="\t") 
+    fc_data = data(data_type='fcs', analysis=analysis, microarray=False, annotations=True, sort_by=None).reset_index()
     fc_ranked = load_candidates(analysis=analysis, name=query_name, func=query_func, query_annotation=query_annotation, query_fc=query_fc)
     fc_genes = fc_ranked.loc[:, 'GeneID']
     fam_data = fc_data.query("GeneID in @fc_genes").copy()
     
     fam_data.loc[:, 'Label'] = [id_ + " | " + name if name != "" else id_ for id_, name in zip(fam_data['GeneID'].fillna(""), fam_data['GeneName'].fillna(""))]
     fam_data = fam_data.set_index("Label").drop(columns=['GeneName', 'GeneID', 'GeneDescription'])
     fam_data.columns = [c.replace("_log2FoldChange", "").replace("_", " ") for c in fam_data.columns]
```

### Comparing `anoexpress-0.1.4/pyproject.toml` & `anoexpress-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anoexpress"
-version = "0.1.4"
+version = "0.1.5"
 description = "A package to access insecticide resistance gene expression meta analyse in Anopheles mosquitoes"
 authors = [
     "Sanjay Nagi <sanjay.nagi@lstmed.ac.uk>",
     ]
 packages = [
     { include = "anoexpress" }
 ]
```

### Comparing `anoexpress-0.1.4/PKG-INFO` & `anoexpress-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anoexpress
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package to access insecticide resistance gene expression meta analyse in Anopheles mosquitoes
 License: MIT
 Author: Sanjay Nagi
 Author-email: sanjay.nagi@lstmed.ac.uk
 Requires-Python: >=3.7.1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

