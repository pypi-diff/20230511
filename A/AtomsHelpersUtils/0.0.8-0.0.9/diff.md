# Comparing `tmp/AtomsHelpersUtils-0.0.8.tar.gz` & `tmp/AtomsHelpersUtils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AtomsHelpersUtils-0.0.8.tar", last modified: Wed Mar 29 20:27:41 2023, max compression
+gzip compressed data, was "AtomsHelpersUtils-0.0.9.tar", last modified: Thu May 11 05:57:28 2023, max compression
```

## Comparing `AtomsHelpersUtils-0.0.8.tar` & `AtomsHelpersUtils-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 20:27:41.280658 AtomsHelpersUtils-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-03-29 20:27:41.252169 AtomsHelpersUtils-0.0.8/AtomsHelper/
--rw-rw-rw-   0        0        0      605 2023-01-17 02:07:28.000000 AtomsHelpersUtils-0.0.8/AtomsHelper/__init__.py
--rw-rw-rw-   0        0        0    23012 2023-03-29 19:30:43.000000 AtomsHelpersUtils-0.0.8/AtomsHelper/atoms_helper.py
--rw-rw-rw-   0        0        0     4399 2023-02-20 07:03:59.000000 AtomsHelpersUtils-0.0.8/AtomsHelper/ddec6_graph_gen.py
--rw-rw-rw-   0        0        0     8427 2023-03-29 19:34:03.000000 AtomsHelpersUtils-0.0.8/AtomsHelper/mine_subgraphs.py
--rw-rw-rw-   0        0        0    13390 2023-03-29 20:23:21.000000 AtomsHelpersUtils-0.0.8/AtomsHelper/nx_to_rdkit.py
--rw-rw-rw-   0        0        0      494 2023-03-29 19:28:44.000000 AtomsHelpersUtils-0.0.8/AtomsHelper/point_cloud.py
--rw-rw-rw-   0        0        0    23258 2023-02-24 21:13:40.000000 AtomsHelpersUtils-0.0.8/AtomsHelper/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-29 20:27:41.278150 AtomsHelpersUtils-0.0.8/AtomsHelpersUtils.egg-info/
--rw-rw-rw-   0        0        0      583 2023-03-29 20:27:41.000000 AtomsHelpersUtils-0.0.8/AtomsHelpersUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-03-29 20:27:41.000000 AtomsHelpersUtils-0.0.8/AtomsHelpersUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 20:27:41.000000 AtomsHelpersUtils-0.0.8/AtomsHelpersUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-03-29 20:27:41.000000 AtomsHelpersUtils-0.0.8/AtomsHelpersUtils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-01-17 02:07:28.000000 AtomsHelpersUtils-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      583 2023-03-29 20:27:41.280151 AtomsHelpersUtils-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-01-17 02:07:28.000000 AtomsHelpersUtils-0.0.8/README.md
--rw-rw-rw-   0        0        0      538 2023-03-29 20:26:47.000000 AtomsHelpersUtils-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-29 20:27:41.281667 AtomsHelpersUtils-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-03-07 07:47:33.000000 AtomsHelpersUtils-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:57:28.620677 AtomsHelpersUtils-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-05-11 05:57:28.547394 AtomsHelpersUtils-0.0.9/AtomsHelper/
+-rw-rw-rw-   0        0        0      605 2023-01-17 02:07:28.000000 AtomsHelpersUtils-0.0.9/AtomsHelper/__init__.py
+-rw-rw-rw-   0        0        0    23208 2023-04-21 23:03:13.000000 AtomsHelpersUtils-0.0.9/AtomsHelper/atoms_helper.py
+-rw-rw-rw-   0        0        0     5054 2023-05-11 05:51:54.000000 AtomsHelpersUtils-0.0.9/AtomsHelper/ddec6_graph_gen.py
+-rw-rw-rw-   0        0        0     8491 2023-05-03 00:21:21.000000 AtomsHelpersUtils-0.0.9/AtomsHelper/mine_subgraphs.py
+-rw-rw-rw-   0        0        0    13856 2023-05-04 17:30:49.000000 AtomsHelpersUtils-0.0.9/AtomsHelper/nx_to_rdkit.py
+-rw-rw-rw-   0        0        0      494 2023-04-12 22:15:33.000000 AtomsHelpersUtils-0.0.9/AtomsHelper/point_cloud.py
+-rw-rw-rw-   0        0        0    24715 2023-05-03 06:57:03.000000 AtomsHelpersUtils-0.0.9/AtomsHelper/utils.py
+-rw-rw-rw-   0        0        0    27012 2023-04-13 16:40:14.000000 AtomsHelpersUtils-0.0.9/AtomsHelper/utils2.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:57:28.612676 AtomsHelpersUtils-0.0.9/AtomsHelpersUtils.egg-info/
+-rw-rw-rw-   0        0        0      583 2023-05-11 05:57:27.000000 AtomsHelpersUtils-0.0.9/AtomsHelpersUtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-05-11 05:57:28.000000 AtomsHelpersUtils-0.0.9/AtomsHelpersUtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 05:57:27.000000 AtomsHelpersUtils-0.0.9/AtomsHelpersUtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-11 05:57:27.000000 AtomsHelpersUtils-0.0.9/AtomsHelpersUtils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-01-17 02:07:28.000000 AtomsHelpersUtils-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      583 2023-05-11 05:57:28.616668 AtomsHelpersUtils-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-01-17 02:07:28.000000 AtomsHelpersUtils-0.0.9/README.md
+-rw-rw-rw-   0        0        0      538 2023-05-11 05:55:52.000000 AtomsHelpersUtils-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 05:57:28.620677 AtomsHelpersUtils-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      487 2023-03-07 07:47:33.000000 AtomsHelpersUtils-0.0.9/setup.py
```

### Comparing `AtomsHelpersUtils-0.0.8/AtomsHelper/__init__.py` & `AtomsHelpersUtils-0.0.9/AtomsHelper/__init__.py`

 * *Files identical despite different names*

### Comparing `AtomsHelpersUtils-0.0.8/AtomsHelper/atoms_helper.py` & `AtomsHelpersUtils-0.0.9/AtomsHelper/atoms_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,16 @@
                     
         for i in active_site_nn.keys():
             active_site_nn[i] = list(active_site_nn[i])
             
         return active_site_nn
     
         
-    def gen_graph(self, h_surface = False, fill_bonds = True, distances = True, weight = 'bond_index'):
+    def gen_graph(self, h_surface = False, fill_bonds = True, distances = True, 
+                  weight = 'bond_index', verbose=False):
         
         # Create graph from subgraph, giving each node a name by index
         
         valency = {'H': 1, 'O': 2, 'N': 3, 'C': 4, self.surface_type: 99}
         
         self.graph = nx.Graph(bonds_solved = 'solved')
         
@@ -336,27 +337,27 @@
             self.graph.nodes[i]['element'] = self.symbols[i]
             self.graph.nodes[i]['position'] = self.positions[i,:]
             
         for i in self.edge_dict.keys():
             for j in self.edge_dict[i]:
                 
                 if {self.graph.nodes[i]['element'], self.graph.nodes[j]['element']} == {'H', self.surface_type}:
-                    self.graph.add_edge(i,j, bond_index = 0)
+                    self.graph.add_edge(i,j, bond_index = 0.)
                 else:
-                    self.graph.add_edge(i,j, bond_index = 1)
+                    self.graph.add_edge(i,j, bond_index = 1.)
 
         for node in self.graph.nodes:    
             self.graph.nodes[node]['valency'] = valency[self.graph.nodes[node]['element']]
             self.graph.nodes[node]['edges'] = len(self.graph.edges(node))
             self.graph.nodes[node]['unoccupied'] = self.graph.nodes[node]['valency'] - self.graph.nodes[node]['edges']
           
         if not fill_bonds:
             return
             
-        model, results = self.fill_bonds()
+        model, results = self.fill_bonds(verbose = verbose)
         if not model:
             return
         
         self.solver_results = {'model': model, 'results': results}
         
         if self.solver_results['model']:
             
@@ -421,15 +422,15 @@
             for j in periodics:
                 for k in periodics:
                     distances[idx] = np.linalg.norm(np.sum(pos1 + np.array([i,j,k]) * cell.T - pos2, axis = 1))
                     idx +=1
                     
         return min(distances)
 
-    def fill_bonds(self):
+    def fill_bonds(self, verbose = False):
         
         node_dict = dict(self.graph.nodes)
     
         edges_ads, edges_pts, edges_hs, nodes_ads, nodes_pts, nodes_hs= {}, {}, {}, {}, {}, {}
         
         # Sort edges into surface and adsorbate
         for edge in self.graph.edges:
@@ -450,16 +451,17 @@
                 nodes_pts[node] = node_dict[node]['valency']
             elif self.symbols[node] == 'H':
                 nodes_hs[node] = node_dict[node]['valency']
             else:
                 nodes_ads[node] = node_dict[node]['valency']
 
         if not edges_ads and not edges_pts:
-            print('Solving ' + str(self.atoms[self.adsorbate_atoms].symbols) + ' on' + str(self.surface_type))
-            print('No adsorbate/slab edges; trivial solution returned')
+            if verbose:
+                print('Solving ' + str(self.atoms[self.adsorbate_atoms].symbols) + ' on' + str(self.surface_type))
+                print('No adsorbate/slab edges; trivial solution returned')
             return None, None
         
         model = pe.ConcreteModel()
         
         model.nodes_ads = pe.Set(initialize = list(set(nodes_ads.keys())))
         model.nodes_hs = pe.Set(initialize = list(set(nodes_hs.keys())))
         model.edges_ads = pe.Set(initialize = list(set(edges_ads.keys())))
@@ -536,19 +538,21 @@
             constraint_nodes = [i for i in constraint_nodes.union(constraint_nodes_pts) if self.symbols[i] != self.surface_type]
         
         model.con = pe.Constraint(constraint_nodes, rule = valency_cap)
 
         solver = po.SolverFactory('glpk')
         
         try:
-            print('Solving ' + str(self.atoms[self.adsorbate_atoms].symbols))
+            if verbose:
+                print('Solving ' + str(self.atoms[self.adsorbate_atoms].symbols))
             results = solver.solve(model)
                 
         except:
-            print('Solver unable to get solution')
+            if verbose:
+                print('Solver unable to get solution')
             model = None
             results = None
         
         return model, results
 
     def draw_graph(self, cutoff = 0.3, 
                         node_label_type = 'element', edge_labels = False, edge_label_type = 'weight'):
@@ -559,15 +563,15 @@
         
     def get_SMILES_string(self):    
         self.smiles_string = pysmiles.write_smiles(self.graph)
 
         
     def generalize_graph_metal(self):
         if not self.graph:
-            print('No graph generated')
+            print('Generalizing metal error: No initial graph generated')
             return
         
         for n in self.graph.nodes(data=True):
             if self.graph.nodes[n[0]]['element'] == self.surface_type:
                 self.graph.nodes[n[0]]['element']='M'
         
 if __name__=="__main__":
```

### Comparing `AtomsHelpersUtils-0.0.8/AtomsHelper/ddec6_graph_gen.py` & `AtomsHelpersUtils-0.0.9/AtomsHelper/ddec6_graph_gen.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,28 @@
             typ = 'adsorbate'
         
         graph.add_node(count,
                        element = element,
                        system_type = typ,
                        position = [float(x),float(y),float(z)],
                        charge = float(charge))
+        
+    record = False
+    for i in nac:
+        if record:
+            idx, _, _, _,_,_, x, y, z, mag, xy, xz, yz, x2y2, z2, ev1, ev2, ev3 = i.split()
+            idx = int(idx)-1
+            graph.nodes[idx]['dipole'] = [float(x),float(y),float(z)]
+            graph.nodes[idx]['dipole_mag'] = mag
+            graph.nodes[idx]['quadrupole'] = [float(j) for j in [xy, xz, yz, x2y2, z2]]
+            graph.nodes[idx]['tless_q_ev'] = [float(ev1),float(ev2),float(ev3)]
+            if idx + 1 == num_atoms:
+                break
+        if 'atom number, atomic symbol, x, y, z, net_charge, dipole_x,' in i:
+            record = True
 
     bo = open('DDEC6_even_tempered_bond_orders.xyz')
     next(bo)
     
     cell_text = next(bo)
     cell_text_split = re.split('[{}]', cell_text)
     
@@ -137,10 +151,10 @@
         closest = np.argmin(dist_vec)
         graph.nodes[i]['bader charge'] = bader_cha[closest]
 
     return graph
 
 if __name__=='__main__':
     from AtomsHelper.utils import draw_surf_graph
-    graph1 = gen_graph_ddec6('Examples/ddec6')
+    graph1 = gen_graph_ddec6('Examples/ddec6/CHOH')
     draw_surf_graph(graph1)
     graph2 = bader_charge_assign(graph1)
```

### Comparing `AtomsHelpersUtils-0.0.8/AtomsHelper/mine_subgraphs.py` & `AtomsHelpersUtils-0.0.9/AtomsHelper/mine_subgraphs.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,15 +244,18 @@
     
     
 # if __name__=='__main__':
 import pickle as pk
 import pandas as pd
 
 if not 'df' in locals() or 'df' in globals():
-    df = pd.DataFrame(pk.load(open('Examples/graphs/LDAtoPBE_df.pk', 'rb')))
+    
+    with open('Examples/graphs/LDAtoPBE_df.pk', 'rb') as fo:
+    
+        df = pk.load(open('Examples/graphs/LDAtoPBE_df.pk', 'rb'))
     graph = df.loc[147]['Active Graph'][0]
 
 obj = graph_enumerator([graph], substrates = ['Pt'])
 
 obj.regen_check(obj.gen_smiles, 'smiles', regenerate=True)
 obj.regen_check(obj.gen_rdkitmol, 'rdkit_mol', regenerate=True)
 print(obj.systems[0])
```

### Comparing `AtomsHelpersUtils-0.0.8/AtomsHelper/nx_to_rdkit.py` & `AtomsHelpersUtils-0.0.9/AtomsHelper/nx_to_rdkit.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 @author: eccn3
 """
 
 import networkx as nx
 from networkx import weisfeiler_lehman_graph_hash as wlgh
 
-from AtomsHelper.utils import draw_surf_graph
+from AtomsHelper.utils import draw_surf_graph, remove_small_edges
 
 from rdkit import Chem
 from rdkit.Chem.rdmolops import FindAllSubgraphsOfLengthMToN
 from rdkit.Chem.rdchem import BondType
 
 from ase import formula
 from ase.data import chemical_symbols
@@ -195,15 +195,15 @@
                 
                 
             g.add_edge(begin_atom_idx, end_atom_idx,
                        **bond_props)
 
         return g
 
-    def enumerate_subgraphs(self, min_path=1, max_path=4, useHs=True,
+    def enumerate_subgraphs(self, min_path=1, max_path=2, useHs=True,
                             edge_attr='bond_index', node_attr='element'):
         
         """
         Enumerate subgraphs 
         
         In
         -------
@@ -228,29 +228,34 @@
 
         
         for i in self.mol_subgraphs:
             for j in i:
                 subgraph = self.mol_to_nx(self.mol, j)
                 nx_subgraphs.append(subgraph)
                 nx_subgraph_hashes.append(wlgh(subgraph, iterations=max_path,
-                                               edge_attr = edge_attr,
+                                               # edge_attr = edge_attr,
                                                node_attr = node_attr))
                 
         self.nx_subgraphs = nx_subgraphs
         self.nx_subgraph_hashes = nx_subgraph_hashes
         
         self.nx_subgraph_counter = Counter(self.nx_subgraph_hashes)
         
         hash_index= {i: [] for i in self.nx_subgraph_counter.keys()}
         for count, i in enumerate(self.nx_subgraph_hashes):
             hash_index[i].append(count)
         
         self.nx_subgraph_indices = hash_index
         
-        return nx_subgraphs, nx_subgraph_hashes  
+        dic = {'nx_subgraphs': nx_subgraphs,
+               'nx_subgraph_hashes': nx_subgraph_hashes,
+               'nx_subgraph_counter': self.nx_subgraph_counter,
+               'nx_subgraph_indices': self.nx_subgraph_indices}
+        
+        return dic
         
     # def change_metal()
     def remove_small_bonds(self, measure = 'rdkit_bond'):
         
         """
         Enumerate subgraphs 
         
@@ -329,75 +334,81 @@
             return
         else:
             for bond in self.mol.GetBonds():
                 print(bond.GetBeginAtomIdx(),
                       bond.GetEndAtomIdx(),
                       bond.GetPropsAsDict())
                 
-    
-
 def mol_with_atom_index(mol):
     for atom in mol.GetAtoms():
         atom.SetAtomMapNum(atom.GetIdx())
     return mol
+
+def simplify_graph(graph, substrate = 'Pt', cutoff = 0.01):
+        
+    graph = remove_small_edges(graph, cutoff = cutoff)
+    
+    keep = []
+    
+    for node in graph.nodes:
+        if graph.nodes[node]['element'] == substrate:
+            continue
+        else:
+            
+            neighbors = list(graph.neighbors(node))
+            for i in neighbors:
+                if graph.edges[i, node]['weight'] > cutoff:
+                    keep.append(neighbors)
+            
+    keeps = sum(keep, [])
+    keeps = set(keeps)
+    
+    return graph.subgraph(keeps).copy(), keeps    
     
 if __name__ == '__main__':
     import pickle as pk
     
     from rdkit.Chem.Draw import IPythonConsole
     from rdkit.Chem import Draw, AllChem
     from ase.io import read
     
     from AtomsHelper.atoms_helper import geom2graph
     from AtomsHelper.ddec6_graph_gen import gen_graph_ddec6
-    from AtomsHelper.utils import remove_small_edges
+    from AtomsHelper.utils import remove_small_edges, draw_surf_graph
     import numpy as np
     from collections import Counter
-    
-    def simplify_graph(graph):
-        
-        keep = []
-        
-        for node in graph.nodes:
-            if graph.nodes[node]['element'] == 'Pt':
-                continue
-            else:
-                
-                neighbors = list(graph.neighbors(node))
-                keep.append(neighbors)
-                
-        keeps = sum(keep, [])
-        keeps = set(keeps)
-        
-        return graph.subgraph(keeps).copy(), keeps
 
     IPythonConsole.ipython_useSVG=True
     
     # graph = pk.load(open('Examples/nx_mol_helper/OCH3-Pt-hol.pk', 'rb'))
     # ddec6 = gen_graph_ddec6('Examples/CHOH/ddec6')
     # ddec6, _ = simplify_graph(ddec6)
     # ddec6 = remove_small_edges(ddec6)
     # atoms = [read('Examples/ase_to_graph/CONTCAR_Pt_CHOH_ontop'), read('Examples/ase_to_graph/CONTCAR_CHCH_holhol')]
     # geoms = [geom2graph(atoms = atom) for atom in atoms]
     examples = ['Examples/ddec6/CHOH',
                 'Examples/ddec6/CH2CHCH3CH3']
-    ddec6 = [remove_small_edges(gen_graph_ddec6(i)) for i in examples]
+    
+    cutoff = 0.06
+    
+    ddec6 = [gen_graph_ddec6(i) for i in examples]
     for count, i in enumerate(ddec6):
-        ddec6[count], _  = simplify_graph(i)
+        ddec6[count], _  = simplify_graph(i, cutoff = cutoff)
+        draw_surf_graph(ddec6[count], cutoff = cutoff)
     rdhelp = [rdkit_helper(nx_graph=i) for i in ddec6]
     
     for i in rdhelp:
         i.nx_to_mol()
         i.remove_small_bonds()
         
         i.smiles = Chem.MolToSmiles(i.mol)
         g = i.mol_to_nx(i.mol)
         
-        # i.enumerate_subgraphs(min_path=1, max_path = 4)
-        # i.count = Counter(i.nx_subgraph_hashes)
+        i.enumerate_subgraphs(min_path=1, max_path = 4)
+        i.count = Counter(i.nx_subgraph_hashes)
         
     
     
     # rd_help = rdkit_helper(nx_graph = ddec6)
     # rd_help.nx_to_mol()
     # rd_help.remove_small_bonds()
     # # rd_help.mol.UpdatePropertyCache()
```

### Comparing `AtomsHelpersUtils-0.0.8/AtomsHelper/utils.py` & `AtomsHelpersUtils-0.0.9/AtomsHelper/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,19 +18,32 @@
 
 from itertools import compress
 
 from ase.data.colors import jmol_colors
 from ase.data import chemical_symbols
 from ase import formula
 
+from sklearn.neighbors import NearestNeighbors
 
 
 def draw_surf_graph(graph, cutoff = 0.3, 
                     node_label_type = 'element', edge_labels = False, edge_label_type = 'weight'):
    
+    '''
+    Draws graph of atoms system
+    Input:
+        graph: networkx graph of atoms
+        cutoff: min edge value to be drawn
+        node_label_type: what attribute to print as node label
+        edge_labels: boolean to draw edge labels
+        edge_label_type: what attribute to print as edge label
+    Output:
+        prints graph
+    '''
+    
     if edge_label_type !='weight' and edge_labels == False:
         edge_labels=True
     
     if cutoff:
         graph = remove_small_edges(graph, cutoff = cutoff)
 
     plt.figure(figsize=(6,5))
@@ -106,65 +119,65 @@
     copy_graph = copy.deepcopy(graph)
     for i in small_weights:
         copy_graph.remove_edge(*i)
 
     return copy_graph
 
 def data_keep(X, X_names, idx):
+    
+    
+    
     return X[:, idx], X_names[ idx]
 
 def correlation(df, threshold):
-    # try:
-    #     y = df[response]
-    #     df = df.drop(response, axis = 1)
-    # except:
-    #     pass
+
     cor_matrix = df.corr().abs()
     upper_tri = cor_matrix.where(np.triu(np.ones(cor_matrix.shape),k=1).astype(np.bool))
     to_drop = [column for column in upper_tri.columns if any(upper_tri[column] > threshold)]
     print(to_drop)
     df1 = df.drop(to_drop, axis=1)
-    # df1 = df1.assign(response = y)
+
     return df1
 
 def number_select(df, column):
     
     # Selects only rows that have a TYPE NUMBER in specified column
     
     # Input: df = df to search; column = 
     
     df1 = df[pd.to_numeric(df[column], errors='coerce').notnull()]
     
     
     return df1
 
-def match(df1, df2, feature, substrate = True):
+def match(df1, df2, feature, substrate = True, graph = False):
     
     # Iterates through df1: looks at adsorbate, substrate, and site combination
     # Find matches in df2 for adsorbate/substrate/site combination to grab its energy
     
     if feature in list(df1.columns):
         newfeat = feature + ' 2'
+        df1.insert(int(np.where(df1.columns == feature)[0][0])+1, newfeat, np.nan)
     
     else:
         newfeat = feature
+        df1[newfeat] = np.nan
     
-    df1[newfeat] = np.nan
+    if graph:
+        df1[newfeat] = pd.DataFrame(df1[newfeat], dtype = object)
     
-    if not substrate:
-        for count, i in df1.iterrows():
-            comparison_column = (df2[['Adsorbate', 'Site']] == i[['Adsorbate', 'Site']]).all(axis = 1)
-            if any(comparison_column):
-                df1.at[count, newfeat] = df2[feature][comparison_column].to_numpy()
-            
-    else:
-        for count, i in df1.iterrows():
-            comparison_column = (df2[['Adsorbate', 'Site', 'Substrate']] == i[['Adsorbate', 'Site', 'Substrate']]).all(axis = 1)
-            if any(comparison_column):
-                df1.at[count, newfeat] = df2[feature][comparison_column].to_numpy()
+    match_feats=['Adsorbate', 'Site']
+    
+    if substrate:
+       match_feats.append('Substrate') 
+        
+    for count, i in df1.iterrows():
+        comparison_column = (df2[match_feats] == i[match_feats]).all(axis = 1)
+        if any(comparison_column):
+            df1.at[count, newfeat] = df2[feature][comparison_column].iloc[0]
     
     df1 = df1.dropna()
 
     return df1
 
 def plot_parity(x, y, label = None, alp = 0.75):
 
@@ -258,15 +271,15 @@
              hyper_param_tune = None, group = 'Adsorbate'): 
     
     # Make model_fit_data 
    
     keys = ['Model', 'Predictions', 'Hyperparameters','Coefficients', 
             'Scaled Coefficients','Coef Stdevs', 'Errors', 'MAE', 
             'Error Stdev', 'Feat. Imp', 'Alphas', 'Model Select', 'Weights', 
-            'Y scaler', 'X scaler']
+            'Y scaler', 'X scaler', 'Pred_std']
     
     model_fit_data = {k: [] for k in keys}
     
     model_data = [[] for i in model_selects]
 
     data = [copy.deepcopy(model_data) for i in models]
 
@@ -341,14 +354,21 @@
                     m['Predictions'].append(scale_y.inverse_transform(prediction))
                     m['Errors'].append(scale_y.inverse_transform(Y_test) - scale_y.inverse_transform(prediction))
                     
                 else:
                     m['Predictions'].append(prediction)
                     m['Errors'].append(Y_test - prediction)
                     
+                if str(type(model)) == "<class 'sklearn.gaussian_process._gpr.GaussianProcessRegressor'>":
+                    std_pred = fitted_model.predict(X_test, return_std = True)[1]
+                    if scale_y:
+                        m['Pred_std'].append(np.sqrt(np.power(std_pred,2)*scale_y.var_))
+                    else:
+                        m['Pred_std'].append(m['Pred_std'])
+                
                 if str(type(model)) == "<class 'sklearn.linear_model._coordinate_descent.LassoCV'>":
                     m['Alphas'].append(fitted_model.alpha_)
                     
                 if str(type(model)) == "<class 'sklearn.linear_model._ridge.RidgeCV'>":
                     m['Alphas'].append(fitted_model.alpha_)
                     
                 if str(type(model)) == "<class 'sklearn.linear_model._coordinate_descent.ElasticNetCV'>":
@@ -539,89 +559,14 @@
         closest.append(np.argmin(np.linalg.norm(components - i, axis = 1)))
     
     plt.figure()
     plt.scatter(new_pca.components_[0,:], new_pca.components_[1,:], c=cluster_fit.labels_)
     plt.ylim((-0.5,0.5))
     plt.xlim((-0.5,0.5))
     return x_pca, new_pca, cluster_fit,closest
-
-def convert_to_spherical(x):
-    
-    dims = len(x[0])
-    
-    spherical = np.empty(shape = np.shape(x))
-    
-    spherical[:,0] = np.linalg.norm(x, axis = 1)
-    
-    for i in np.arange(dims)[:-2]:
-        
-        numerator = x[:,i]
-        denominator = np.linalg.norm(x[:,i:], axis = 1)
-        
-        inside= np.divide(numerator, denominator)
-        
-        spherical[:,i+1] = np.arccos(inside)
-    
-    
-    numerator = x[:, -2] + np.linalg.norm(x[:, -2:], axis = 1)
-    denominator = x[:, -1]
-    
-    fraction = np.divide(numerator, denominator)
-    
-    arccot = np.arctan(np.reciprocal(fraction))
-    
-    
-    spherical[:, -1] = 2*arccot
-    
-   
-    return spherical
-# def draw_graph(graph):
-#     """
-#     Displays the graph
-#     :param graph: networkx graph object
-#     :return: None
-#     """
-    
-#     Pt = [i for i in graph.nodes() if 'Pt' in graph.nodes[i]['element']]
-#     spaced = np.vstack((np.linspace(-0.95, 0.95, len(Pt)), np.ones(len(Pt))*-1)).T
-#     fixed_positions = {i: tuple(spaced[count]) for count, i in enumerate(Pt)}
-#     for i in graph.nodes:
-#         if graph.nodes[i]['element'] != 'Pt':
-#             fixed_positions[i] = (np.random.uniform(-1, 1), np.random.uniform(0,1))
-            
-    
-#     if bool(fixed_positions):
-#         try:
-#             if graph.graph['bonds_solved'] == "Problem with solver":
-#                 pos = nx.spring_layout(graph, pos = fixed_positions, weight=None)
-#             else:
-#                 pos = nx.spring_layout(graph,weight='weight', pos = fixed_positions)
-#         except:
-#             pos = nx.spring_layout(graph, weight='weight', pos = fixed_positions)
-    
-#     else:
-#         pos = nx.spring_layout(graph,weight='weight')
-    
-#     edge_styles = []
-#     for e1, e2, data in graph.edges(data=True):
-#             if data.get("weight", True) == 0: # Ads-Ads bond
-#                 edge_styles.append("dashed")
-#             else: # Surface-Surface bond
-#                 edge_styles.append("solid")
-
-#     plt.figure(figsize = (5,3), dpi = 300)
-#     nx.draw(graph, with_labels=False, node_size=1500, node_color="skyblue",
-#             node_shape="o", alpha=0.5, linewidths=4, font_size=25,style=edge_styles,
-#             font_color="black", font_weight="bold", width=2, edge_color="grey",
-#             pos=pos)
-#     node_labels = nx.get_node_attributes(graph, 'element')
-#     edge_labels = nx.get_edge_attributes(graph,'weight')
-#     nx.draw_networkx_labels(graph, pos, node_labels)
-#     nx.draw_networkx_edge_labels(graph, pos, edge_labels)
-#     plt.show()
     
 def test_predictions(X, models, y, x_scale = None, y_scale = None):
     
     if x_scale:
         X = x_scale.transform(X)
 
     
@@ -679,9 +624,125 @@
     
     for i in periodics:
         for j in periodics:
             for k in periodics:
                 distances[idx] = np.linalg.norm(np.sum(pos1 + np.array([i,j,k]) * cell.T, axis = 1))
                 idx +=1
     return min(distances)
-    
+
+
+def best_fit_transform(A, B):
+    '''
+    Calculates the least-squares best-fit transform that maps corresponding points A to B in m spatial dimensions
+    Input:
+      A: Nxm numpy array of corresponding points
+      B: Nxm numpy array of corresponding points
+    Returns:
+      T: (m+1)x(m+1) homogeneous transformation matrix that maps A on to B
+      R: mxm rotation matrix
+      t: mx1 translation vector
+    '''
+
+    assert A.shape == B.shape
+
+    # get number of dimensions
+    m = A.shape[1]
+
+    # translate points to their centroids
+    centroid_A = np.mean(A, axis=0)
+    centroid_B = np.mean(B, axis=0)
+    AA = A - centroid_A
+    BB = B - centroid_B
+
+    # rotation matrix
+    H = np.dot(AA.T, BB)
+    U, S, Vt = np.linalg.svd(H)
+    R = np.dot(Vt.T, U.T)
+
+    # special reflection case
+    if np.linalg.det(R) < 0:
+       Vt[m-1,:] *= -1
+       R = np.dot(Vt.T, U.T)
+
+    # translation
+    t = centroid_B.T - np.dot(R,centroid_A.T)
+
+    # homogeneous transformation
+    T = np.identity(m+1)
+    T[:m, :m] = R
+    T[:m, m] = t
+
+    return T, R, t
+
+
+def nearest_neighbor(src, dst):
+    '''
+    Find the nearest (Euclidean) neighbor in dst for each point in src
+    Input:
+        src: Nxm array of points
+        dst: Nxm array of points
+    Output:
+        distances: Euclidean distances of the nearest neighbor
+        indices: dst indices of the nearest neighbor
+    '''
+
+    assert src.shape == dst.shape
+
+    neigh = NearestNeighbors(n_neighbors=1)
+    neigh.fit(dst)
+    distances, indices = neigh.kneighbors(src, return_distance=True)
+    return distances.ravel(), indices.ravel()
+
+
+def icp(A, B, init_pose=None, max_iterations=20, tolerance=0.001):
+    '''
+    The Iterative Closest Point method: finds best-fit transform that maps points A on to points B
+    Input:
+        A: Nxm numpy array of source mD points
+        B: Nxm numpy array of destination mD point
+        init_pose: (m+1)x(m+1) homogeneous transformation
+        max_iterations: exit algorithm after max_iterations
+        tolerance: convergence criteria
+    Output:
+        T: final homogeneous transformation that maps A on to B
+        distances: Euclidean distances (errors) of the nearest neighbor
+        i: number of iterations to converge
+    '''
+
+    assert A.shape == B.shape
+
+    # get number of dimensions
+    m = A.shape[1]
+
+    # make points homogeneous, copy them to maintain the originals
+    src = np.ones((m+1,A.shape[0]))
+    dst = np.ones((m+1,B.shape[0]))
+    src[:m,:] = np.copy(A.T)
+    dst[:m,:] = np.copy(B.T)
+
+    # apply the initial pose estimation
+    if init_pose is not None:
+        src = np.dot(init_pose, src)
+
+    prev_error = 0
+
+    for i in range(max_iterations):
+        # find the nearest neighbors between the current source and destination points
+        distances, indices = nearest_neighbor(src[:m,:].T, dst[:m,:].T)
+
+        # compute the transformation between the current source and nearest destination points
+        T,_,_ = best_fit_transform(src[:m,:].T, dst[:m,indices].T)
+
+        # update the current source
+        src = np.dot(T, src)
+
+        # check error
+        mean_error = np.mean(distances)
+        if np.abs(prev_error - mean_error) < tolerance:
+            break
+        prev_error = mean_error
+
+    # calculate final transformation
+    T,_,_ = best_fit_transform(A, src[:m,:].T)
+
+    return T, distances, i
```

### Comparing `AtomsHelpersUtils-0.0.8/AtomsHelpersUtils.egg-info/PKG-INFO` & `AtomsHelpersUtils-0.0.9/AtomsHelpersUtils.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: AtomsHelpersUtils
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Author: Eric Chen
 Author-email: Eric Chen <ericchen@udel.edu>
 Project-URL: Homepage, https://github.com/ericchen-udel/AtomsHelpersUtils.git
 Project-URL: Bug Tracker, https://github.com/ericchen-udel/AtomsHelpersUtils.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #AtomsHelper
```

### Comparing `AtomsHelpersUtils-0.0.8/LICENSE` & `AtomsHelpersUtils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `AtomsHelpersUtils-0.0.8/PKG-INFO` & `AtomsHelpersUtils-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: AtomsHelpersUtils
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Author: Eric Chen
 Author-email: Eric Chen <ericchen@udel.edu>
 Project-URL: Homepage, https://github.com/ericchen-udel/AtomsHelpersUtils.git
 Project-URL: Bug Tracker, https://github.com/ericchen-udel/AtomsHelpersUtils.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #AtomsHelper
```

### Comparing `AtomsHelpersUtils-0.0.8/pyproject.toml` & `AtomsHelpersUtils-0.0.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "AtomsHelpersUtils"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Eric Chen", email="ericchen@udel.edu" },
 ]
 description = "A small example package"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

