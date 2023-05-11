# Comparing `tmp/elastic_blast-1.0.0.tar.gz` & `tmp/elastic_blast-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elastic_blast-1.0.0.tar", last modified: Thu Dec  8 21:26:38 2022, max compression
+gzip compressed data, was "elastic_blast-1.1.0.tar", last modified: Thu May 11 14:13:28 2023, max compression
```

## Comparing `elastic_blast-1.0.0.tar` & `elastic_blast-1.1.0.tar`

### file list

```diff
@@ -1,210 +1,211 @@
-drwxr-xr-x   0 boratyng  (5629) blast      (990)        0 2022-12-08 21:26:38.531449 elastic_blast-1.0.0/
--rw-r--r--   0 boratyng  (5629) blast      (990)     1004 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/LICENSE.md
--rw-r--r--   0 boratyng  (5629) blast      (990)    51050 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/Makefile
--rw-r--r--   0 boratyng  (5629) blast      (990)     3554 2022-12-08 21:26:38.531449 elastic_blast-1.0.0/PKG-INFO
--rw-r--r--   0 boratyng  (5629) blast      (990)     3471 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/README.md
-drwxr-xr-x   0 boratyng  (5629) blast      (990)        0 2022-12-08 21:26:38.510449 elastic_blast-1.0.0/bin/
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1958 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/bin/aws-create-elastic-blast-janitor-role.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1278 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/bin/aws-delete-elastic-blast-janitor-role.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)      342 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/bin/aws-describe-elastic-blast-janitor-role.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)      939 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/bin/aws-get-auto-scaling-events.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     3377 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/bin/aws-show-my-undeleted-searches.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     9823 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/bin/blast-tuner.py
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     7310 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/bin/cleanup-stale-gcp-resources.py
--rwxr-xr-x   0 boratyng  (5629) blast      (990)    18724 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/bin/create-blastdb-metadata.py
--rwxr-xr-x   0 boratyng  (5629) blast      (990)    11062 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/bin/elastic-blast
--rwxr-xr-x   0 boratyng  (5629) blast      (990)    11207 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/bin/elb-cost.py
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     6347 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/bin/fasta_split.py
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1375 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/bin/gcp-setup-elastic-blast-janitor.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     3409 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/bin/gcp-show-my-undeleted-searches.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1434 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/bin/gcp_ram_size.py
--rwxr-xr-x   0 boratyng  (5629) blast      (990)      452 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/bin/results2clustername.sh
-drwxr-xr-x   0 boratyng  (5629) blast      (990)        0 2022-12-08 21:26:38.510449 elastic_blast-1.0.0/requirements/
--rw-r--r--   0 boratyng  (5629) blast      (990)      224 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/requirements/base.txt
--rw-r--r--   0 boratyng  (5629) blast      (990)      188 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/requirements/test.txt
--rw-r--r--   0 boratyng  (5629) blast      (990)      205 2022-12-08 21:26:38.532449 elastic_blast-1.0.0/setup.cfg
--rw-r--r--   0 boratyng  (5629) blast      (990)       74 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/setup.py
-drwxr-xr-x   0 boratyng  (5629) blast      (990)        0 2022-12-08 21:26:38.507449 elastic_blast-1.0.0/share/
-drwxr-xr-x   0 boratyng  (5629) blast      (990)        0 2022-12-08 21:26:38.519449 elastic_blast-1.0.0/share/etc/
--rw-r--r--   0 boratyng  (5629) blast      (990)     6215 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elastic-blast-aws-iam-policy.json.template
--rw-r--r--   0 boratyng  (5629) blast      (990)      414 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-chicken-gut-metagenome.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      502 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-corrupted-db.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      406 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-custom-db.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      588 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-multiple-query-files.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      551 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-neg-taxidfiltering.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      556 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-non-default-params.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      365 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-nopal-transcriptome.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      264 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-nt-16-spot-nodes.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      435 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-nt-8-nodes.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      648 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-out-of-memory-db-download.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      645 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-out-of-memory.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      834 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-pdbnt-all-azs-provided.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      520 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-pdbnt-auto-shutdown.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      745 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-pdbnt-s3-query-create-resources-small-instance.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      393 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-pdbnt-s3-query-create-resources.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      482 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-pdbnt.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      487 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-refseq_rna-nvme.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      544 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastn-taxidfiltering.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      426 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastp-dark-matter-nvme-4-jobs.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      464 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastp-dark-matter-nvme.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      455 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastp-dark-matter-optimal-spot.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      574 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastp-dark-matter.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      381 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastp-nopal-transcriptome.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      366 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastp-nr-s3-query-create-resources.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      810 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastp-nr-small-dark-matter.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      282 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastx-jaersn01.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      333 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastx-nopal-transcriptome.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      300 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-blastx-nr-jaers-wgs.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      380 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-contam.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      642 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-megablast-sra-spots.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      584 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-megablast-vht1.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      471 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-rpstblastn-five-example.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      195 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-split-only-ebs-mane.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      197 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-split-only-ebs-vht2.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      174 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-split-only-ebs-viralmeta.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      195 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-split-only-local-ssd-mane.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      197 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-split-only-local-ssd-vht2.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      174 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-split-only-local-ssd-viralmeta.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      827 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-spot-optimal-instance-type-blastn-pdbnt.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      276 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-aws-viralmetagenomes-vs-nr.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      384 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastdb-download-test.template
--rw-r--r--   0 boratyng  (5629) blast      (990)      498 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastn-chicken-gut-metagenome-autoscale.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      420 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastn-custom-db.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      415 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastn-multiple-query-files.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      421 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastn-neg-taxidfiltering.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      440 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastn-nopal-transcriptome.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      449 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastn-nt-coronaviridae.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      362 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastn-nt-eb239.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      377 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastn-nt.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      397 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastn-pdbnt-autoscale.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      367 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastn-pdbnt-k8s-too-many-jobs.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      464 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastn-pdbnt-local-ssd.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      352 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastn-pdbnt.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      430 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastn-taxidfiltering.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      385 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastp-nopal-transcriptome.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      352 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastp-nr-eb239.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      432 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastp-nr-viral-metagenome.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      365 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastp-nr.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      378 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastp-swissprot.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      392 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastx-nopal-transcriptome.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      447 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-blastx-nr-WB4_2_0811.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      339 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-psiblast-nr.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      323 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-psiblast-swissprot.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      325 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-rpsblast-amr.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      313 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-rpsblast-split-cdd.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      353 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-rpstblastn-WB4_2_0811.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      392 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-rpstblastn-cdd.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      547 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-rpstblastn-five-example.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      466 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-slava-blastp-nr.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      322 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-tblastn-nt-viral-metagenome.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      362 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-tblastx-virusrep.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)       16 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-user-taxidlist
--rw-r--r--   0 boratyng  (5629) blast      (990)      421 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/elb-vadims-blastn-nt.ini
--rw-r--r--   0 boratyng  (5629) blast      (990)      196 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/etc/yamllint-config.yaml
-drwxr-xr-x   0 boratyng  (5629) blast      (990)        0 2022-12-08 21:26:38.520449 elastic_blast-1.0.0/share/test/
--rw-r--r--   0 boratyng  (5629) blast      (990)     2106 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/test/Makefile
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1209 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/test/cloud-split-test.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)    11152 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/test/elb-vs-local-blast-regression-test.sh
--rw-r--r--   0 boratyng  (5629) blast      (990)      322 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/test/job-get-blast-version.yaml
--rw-r--r--   0 boratyng  (5629) blast      (990)      782 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/test/job-show-blastdbs.yaml
--rw-r--r--   0 boratyng  (5629) blast      (990)      635 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/test/job-show-queries.yaml
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     2127 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/test/pd-scalability-tests.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1239 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/test/sanity-check-pdbnt-search-local-unsplit-query-vs-elastic-blast.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)      864 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/test/sanity-check-pdbnt-search-local-vs-elastic-blast.sh
--rw-r--r--   0 boratyng  (5629) blast      (990)      341 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/test/show-get-available-blastdb.yaml
-drwxr-xr-x   0 boratyng  (5629) blast      (990)        0 2022-12-08 21:26:38.523449 elastic_blast-1.0.0/share/tools/
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     3188 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/aws-create-instance-with-custom-instance-profile.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)      432 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/aws-delete-instance-with-custom-instance-profile.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     2706 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/aws-elastic-blast-number-of-nodes.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)      387 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/aws-list-az.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1086 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/aws-list-vpc.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)      688 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/aws-policy-create.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)      427 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/aws-policy-delete.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)      744 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/aws-policy-describe.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1718 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/aws-role-create.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)      828 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/aws-role-delete.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)      495 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/aws-role-describe.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1571 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/aws-test-instance-with-custom-instance-profile.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     2892 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/deploy-elastic-blast-docs.sh
--rw-r--r--   0 boratyng  (5629) blast      (990)      250 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/elastic-blast-completion.bash
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     2516 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/gcp-create-svc-acct.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     2090 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/gcp-delete-svc-acct.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1035 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/iam-policy-patcher.py
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1001 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/impersonate-tc.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)      414 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/loc.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1037 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/paper-case-study-submit-blastn-eudicotyledons.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1186 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/paper-case-study-submit-blastn-non-eudicotyledons.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1026 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/paper-case-study-submit-megablast-eudicotyledons.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1030 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/paper-case-study-submit-megablast-non-eudicotyledons.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)      620 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/pin-python-versions-for-release.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1883 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/query-analyzer.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     2336 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/release-to-github.sh
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     6679 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/run-report.py
-drwxr-xr-x   0 boratyng  (5629) blast      (990)        0 2022-12-08 21:26:38.524449 elastic_blast-1.0.0/share/tools/test-gcp-permissions/
--rw-r--r--   0 boratyng  (5629) blast      (990)        5 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/test-gcp-permissions/.gitignore
--rw-r--r--   0 boratyng  (5629) blast      (990)     1940 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/test-gcp-permissions/Makefile
--rw-r--r--   0 boratyng  (5629) blast      (990)      112 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/test-gcp-permissions/requirements.txt
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     3517 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/share/tools/test-gcp-permissions/test-gcp-permissions.py
-drwxr-xr-x   0 boratyng  (5629) blast      (990)        0 2022-12-08 21:26:38.507449 elastic_blast-1.0.0/src/
-drwxr-xr-x   0 boratyng  (5629) blast      (990)        0 2022-12-08 21:26:38.527449 elastic_blast-1.0.0/src/elastic_blast/
--rw-r--r--   0 boratyng  (5629) blast      (990)     1280 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/__init__.py
--rw-r--r--   0 boratyng  (5629) blast      (990)    55287 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/aws.py
--rw-r--r--   0 boratyng  (5629) blast      (990)     6256 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/aws_traits.py
--rw-r--r--   0 boratyng  (5629) blast      (990)    15880 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/base.py
-drwxr-xr-x   0 boratyng  (5629) blast      (990)        0 2022-12-08 21:26:38.528449 elastic_blast-1.0.0/src/elastic_blast/commands/
--rw-r--r--   0 boratyng  (5629) blast      (990)        0 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/commands/__init__.py
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     1733 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/commands/delete.py
--rw-r--r--   0 boratyng  (5629) blast      (990)    26769 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/commands/run_summary.py
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     4599 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/commands/status.py
--rwxr-xr-x   0 boratyng  (5629) blast      (990)    13259 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/commands/submit.py
--rw-r--r--   0 boratyng  (5629) blast      (990)    11321 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/config.py
--rw-r--r--   0 boratyng  (5629) blast      (990)    11886 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/constants.py
--rw-r--r--   0 boratyng  (5629) blast      (990)     3649 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/cost.py
--rw-r--r--   0 boratyng  (5629) blast      (990)     4913 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/db_metadata.py
--rw-r--r--   0 boratyng  (5629) blast      (990)     6352 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/elasticblast.py
--rw-r--r--   0 boratyng  (5629) blast      (990)     1894 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/elasticblast_factory.py
--rw-r--r--   0 boratyng  (5629) blast      (990)    58214 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/elb_config.py
--rw-r--r--   0 boratyng  (5629) blast      (990)    22757 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/filehelper.py
--rw-r--r--   0 boratyng  (5629) blast      (990)    42253 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/gcp.py
--rw-r--r--   0 boratyng  (5629) blast      (990)     3061 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/gcp_traits.py
--rwxr-xr-x   0 boratyng  (5629) blast      (990)     6120 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/janitor.py
--rw-r--r--   0 boratyng  (5629) blast      (990)     4477 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/jobs.py
--rw-r--r--   0 boratyng  (5629) blast      (990)    40328 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/kubernetes.py
--rw-r--r--   0 boratyng  (5629) blast      (990)     4755 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/object_storage_utils.py
-drwxr-xr-x   0 boratyng  (5629) blast      (990)        0 2022-12-08 21:26:38.528449 elastic_blast-1.0.0/src/elastic_blast/resources/
--rw-r--r--   0 boratyng  (5629) blast      (990)        0 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/resources/__init__.py
-drwxr-xr-x   0 boratyng  (5629) blast      (990)        0 2022-12-08 21:26:38.529449 elastic_blast-1.0.0/src/elastic_blast/resources/quotas/
--rw-r--r--   0 boratyng  (5629) blast      (990)        0 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/resources/quotas/__init__.py
--rw-r--r--   0 boratyng  (5629) blast      (990)     4689 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/resources/quotas/quota_aws_batch.py
--rw-r--r--   0 boratyng  (5629) blast      (990)     2458 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/resources/quotas/quota_aws_ec2_cf.py
--rw-r--r--   0 boratyng  (5629) blast      (990)     1529 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/resources/quotas/quota_check.py
--rw-r--r--   0 boratyng  (5629) blast      (990)     4945 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/split.py
--rw-r--r--   0 boratyng  (5629) blast      (990)     1845 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/subst.py
--rw-r--r--   0 boratyng  (5629) blast      (990)     8782 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/taxonomy.py
-drwxr-xr-x   0 boratyng  (5629) blast      (990)        0 2022-12-08 21:26:38.531449 elastic_blast-1.0.0/src/elastic_blast/templates/
--rw-r--r--   0 boratyng  (5629) blast      (990)     3970 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/blast-batch-job-local-ssd.yaml.template
--rw-r--r--   0 boratyng  (5629) blast      (990)     4520 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/blast-batch-job.yaml.template
--rw-r--r--   0 boratyng  (5629) blast      (990)     1200 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/cloudformation-admin-iam.yaml
--rw-r--r--   0 boratyng  (5629) blast      (990)    29404 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/elastic-blast-cf.yaml
--rw-r--r--   0 boratyng  (5629) blast      (990)     9262 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/elastic-blast-janitor-cf.yaml
--rw-r--r--   0 boratyng  (5629) blast      (990)      888 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/elb-janitor-cronjob.yaml.template
--rw-r--r--   0 boratyng  (5629) blast      (990)      270 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/elb-janitor-rbac.yaml
--rw-r--r--   0 boratyng  (5629) blast      (990)      641 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/job-cloud-split-local-ssd.yaml.template
--rw-r--r--   0 boratyng  (5629) blast      (990)     2754 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/job-init-local-ssd.yaml.template
--rw-r--r--   0 boratyng  (5629) blast      (990)     3129 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/job-init-pv.yaml.template
--rw-r--r--   0 boratyng  (5629) blast      (990)     1121 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/job-submit-jobs.yaml.template
--rw-r--r--   0 boratyng  (5629) blast      (990)      309 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/pvc-rom.yaml.template
--rw-r--r--   0 boratyng  (5629) blast      (990)      212 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/pvc-rwo.yaml.template
--rw-r--r--   0 boratyng  (5629) blast      (990)      292 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/storage-gcp-ssd.yaml
--rw-r--r--   0 boratyng  (5629) blast      (990)      293 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/storage-gcp.yaml
--rw-r--r--   0 boratyng  (5629) blast      (990)      160 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/volume-snapshot-class.yaml
--rw-r--r--   0 boratyng  (5629) blast      (990)      213 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/templates/volume-snapshot.yaml
--rw-r--r--   0 boratyng  (5629) blast      (990)    16550 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/tuner.py
--rw-r--r--   0 boratyng  (5629) blast      (990)    23261 2022-12-06 18:39:49.000000 elastic_blast-1.0.0/src/elastic_blast/util.py
-drwxr-xr-x   0 boratyng  (5629) blast      (990)        0 2022-12-08 21:26:38.528449 elastic_blast-1.0.0/src/elastic_blast.egg-info/
--rw-r--r--   0 boratyng  (5629) blast      (990)     3554 2022-12-08 21:26:38.000000 elastic_blast-1.0.0/src/elastic_blast.egg-info/PKG-INFO
--rw-r--r--   0 boratyng  (5629) blast      (990)     7902 2022-12-08 21:26:38.000000 elastic_blast-1.0.0/src/elastic_blast.egg-info/SOURCES.txt
--rw-r--r--   0 boratyng  (5629) blast      (990)        1 2022-12-08 21:26:38.000000 elastic_blast-1.0.0/src/elastic_blast.egg-info/dependency_links.txt
--rw-r--r--   0 boratyng  (5629) blast      (990)        1 2022-12-08 21:26:30.000000 elastic_blast-1.0.0/src/elastic_blast.egg-info/not-zip-safe
--rw-r--r--   0 boratyng  (5629) blast      (990)      224 2022-12-08 21:26:38.000000 elastic_blast-1.0.0/src/elastic_blast.egg-info/requires.txt
--rw-r--r--   0 boratyng  (5629) blast      (990)       14 2022-12-08 21:26:38.000000 elastic_blast-1.0.0/src/elastic_blast.egg-info/top_level.txt
+drwxr-xr-x   0 camacho   (4819) blast      (990)        0 2023-05-11 14:13:28.589128 elastic_blast-1.1.0/
+-rw-r--r--   0 camacho   (4819) blast      (990)     1004 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/LICENSE.md
+-rw-r--r--   0 camacho   (4819) blast      (990)    50980 2023-05-09 12:46:22.000000 elastic_blast-1.1.0/Makefile
+-rw-r--r--   0 camacho   (4819) blast      (990)     4006 2023-05-11 14:13:28.589128 elastic_blast-1.1.0/PKG-INFO
+-rw-r--r--   0 camacho   (4819) blast      (990)     3923 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/README.md
+drwxr-xr-x   0 camacho   (4819) blast      (990)        0 2023-05-11 14:13:28.521128 elastic_blast-1.1.0/bin/
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1958 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/bin/aws-create-elastic-blast-janitor-role.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1278 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/bin/aws-delete-elastic-blast-janitor-role.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)      342 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/bin/aws-describe-elastic-blast-janitor-role.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)      939 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/bin/aws-get-auto-scaling-events.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     3377 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/bin/aws-show-my-undeleted-searches.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     9969 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/bin/blast-tuner.py
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     7310 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/bin/cleanup-stale-gcp-resources.py
+-rwxr-xr-x   0 camacho   (4819) blast      (990)    18724 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/bin/create-blastdb-metadata.py
+-rwxr-xr-x   0 camacho   (4819) blast      (990)    11243 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/bin/elastic-blast
+-rwxr-xr-x   0 camacho   (4819) blast      (990)    11207 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/bin/elb-cost.py
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     6347 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/bin/fasta_split.py
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1375 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/bin/gcp-setup-elastic-blast-janitor.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     3409 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/bin/gcp-show-my-undeleted-searches.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1434 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/bin/gcp_ram_size.py
+-rwxr-xr-x   0 camacho   (4819) blast      (990)      452 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/bin/results2clustername.sh
+drwxr-xr-x   0 camacho   (4819) blast      (990)        0 2023-05-11 14:13:28.521128 elastic_blast-1.1.0/requirements/
+-rw-r--r--   0 camacho   (4819) blast      (990)      226 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/requirements/base.txt
+-rw-r--r--   0 camacho   (4819) blast      (990)      207 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/requirements/test.txt
+-rw-r--r--   0 camacho   (4819) blast      (990)      205 2023-05-11 14:13:28.590128 elastic_blast-1.1.0/setup.cfg
+-rw-r--r--   0 camacho   (4819) blast      (990)       74 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/setup.py
+drwxr-xr-x   0 camacho   (4819) blast      (990)        0 2023-05-11 14:13:28.498128 elastic_blast-1.1.0/share/
+drwxr-xr-x   0 camacho   (4819) blast      (990)        0 2023-05-11 14:13:28.533128 elastic_blast-1.1.0/share/etc/
+-rw-r--r--   0 camacho   (4819) blast      (990)     6215 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elastic-blast-aws-iam-policy.json.template
+-rw-r--r--   0 camacho   (4819) blast      (990)      414 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-chicken-gut-metagenome.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      502 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-corrupted-db.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      406 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-custom-db.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      588 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-multiple-query-files.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      551 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-neg-taxidfiltering.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      556 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-non-default-params.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      365 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-nopal-transcriptome.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      264 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-nt-16-spot-nodes.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      435 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-nt-8-nodes.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      648 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-out-of-memory-db-download.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      645 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-out-of-memory.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      834 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-pdbnt-all-azs-provided.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      520 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-pdbnt-auto-shutdown.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      745 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-pdbnt-s3-query-create-resources-small-instance.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      393 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-pdbnt-s3-query-create-resources.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      482 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-pdbnt.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      487 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-refseq_rna-nvme.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      544 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastn-taxidfiltering.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      426 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastp-dark-matter-nvme-4-jobs.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      464 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastp-dark-matter-nvme.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      455 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastp-dark-matter-optimal-spot.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      574 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastp-dark-matter.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      381 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastp-nopal-transcriptome.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      366 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastp-nr-s3-query-create-resources.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      810 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastp-nr-small-dark-matter.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      282 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastx-jaersn01.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      333 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastx-nopal-transcriptome.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      300 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-blastx-nr-jaers-wgs.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      380 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-contam.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      642 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-megablast-sra-spots.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      584 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-megablast-vht1.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      471 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-rpstblastn-five-example.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      195 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-split-only-ebs-mane.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      197 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-split-only-ebs-vht2.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      174 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-split-only-ebs-viralmeta.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      195 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-split-only-local-ssd-mane.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      197 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-split-only-local-ssd-vht2.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      174 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-split-only-local-ssd-viralmeta.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      827 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-spot-optimal-instance-type-blastn-pdbnt.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      276 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-aws-viralmetagenomes-vs-nr.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      384 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastdb-download-test.template
+-rw-r--r--   0 camacho   (4819) blast      (990)      498 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastn-chicken-gut-metagenome-autoscale.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      420 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastn-custom-db.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      415 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastn-multiple-query-files.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      421 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastn-neg-taxidfiltering.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      440 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastn-nopal-transcriptome.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      449 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastn-nt-coronaviridae.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      362 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastn-nt-eb239.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      377 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastn-nt.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      397 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastn-pdbnt-autoscale.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      367 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastn-pdbnt-k8s-too-many-jobs.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      464 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastn-pdbnt-local-ssd.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      352 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastn-pdbnt.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      430 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastn-taxidfiltering.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      385 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastp-nopal-transcriptome.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      352 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastp-nr-eb239.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      432 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastp-nr-viral-metagenome.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      365 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastp-nr.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      378 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastp-swissprot.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      392 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastx-nopal-transcriptome.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      447 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-blastx-nr-WB4_2_0811.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      339 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-psiblast-nr.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      323 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-psiblast-swissprot.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      325 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-rpsblast-amr.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      313 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-rpsblast-split-cdd.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      353 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-rpstblastn-WB4_2_0811.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      392 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-rpstblastn-cdd.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      547 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-rpstblastn-five-example.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      466 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-slava-blastp-nr.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      322 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-tblastn-nt-viral-metagenome.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      362 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-tblastx-virusrep.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)       16 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-user-taxidlist
+-rw-r--r--   0 camacho   (4819) blast      (990)      421 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/elb-vadims-blastn-nt.ini
+-rw-r--r--   0 camacho   (4819) blast      (990)      196 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/etc/yamllint-config.yaml
+drwxr-xr-x   0 camacho   (4819) blast      (990)        0 2023-05-11 14:13:28.535128 elastic_blast-1.1.0/share/test/
+-rw-r--r--   0 camacho   (4819) blast      (990)     2106 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/test/Makefile
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1209 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/test/cloud-split-test.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)    11152 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/test/elb-vs-local-blast-regression-test.sh
+-rw-r--r--   0 camacho   (4819) blast      (990)      322 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/test/job-get-blast-version.yaml
+-rw-r--r--   0 camacho   (4819) blast      (990)      782 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/test/job-show-blastdbs.yaml
+-rw-r--r--   0 camacho   (4819) blast      (990)      635 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/test/job-show-queries.yaml
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     2127 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/test/pd-scalability-tests.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1239 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/test/sanity-check-pdbnt-search-local-unsplit-query-vs-elastic-blast.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)      864 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/test/sanity-check-pdbnt-search-local-vs-elastic-blast.sh
+-rw-r--r--   0 camacho   (4819) blast      (990)      341 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/test/show-get-available-blastdb.yaml
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1955 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/test/test-k8s-versions.sh
+drwxr-xr-x   0 camacho   (4819) blast      (990)        0 2023-05-11 14:13:28.539128 elastic_blast-1.1.0/share/tools/
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     3188 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/aws-create-instance-with-custom-instance-profile.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)      432 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/aws-delete-instance-with-custom-instance-profile.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     2706 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/aws-elastic-blast-number-of-nodes.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)      387 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/aws-list-az.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1086 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/aws-list-vpc.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)      688 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/aws-policy-create.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)      427 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/aws-policy-delete.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)      744 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/aws-policy-describe.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1718 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/aws-role-create.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)      828 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/aws-role-delete.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)      495 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/aws-role-describe.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1571 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/aws-test-instance-with-custom-instance-profile.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     2892 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/deploy-elastic-blast-docs.sh
+-rw-r--r--   0 camacho   (4819) blast      (990)      250 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/elastic-blast-completion.bash
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     2516 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/gcp-create-svc-acct.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     2090 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/gcp-delete-svc-acct.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1035 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/iam-policy-patcher.py
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1001 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/impersonate-tc.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)      414 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/loc.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1037 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/paper-case-study-submit-blastn-eudicotyledons.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1186 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/paper-case-study-submit-blastn-non-eudicotyledons.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1026 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/paper-case-study-submit-megablast-eudicotyledons.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1030 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/paper-case-study-submit-megablast-non-eudicotyledons.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)      853 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/pin-python-versions-for-release.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1883 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/query-analyzer.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     2336 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/release-to-github.sh
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     6679 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/run-report.py
+drwxr-xr-x   0 camacho   (4819) blast      (990)        0 2023-05-11 14:13:28.539128 elastic_blast-1.1.0/share/tools/test-gcp-permissions/
+-rw-r--r--   0 camacho   (4819) blast      (990)        5 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/test-gcp-permissions/.gitignore
+-rw-r--r--   0 camacho   (4819) blast      (990)     1940 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/test-gcp-permissions/Makefile
+-rw-r--r--   0 camacho   (4819) blast      (990)      112 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/test-gcp-permissions/requirements.txt
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     3517 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/share/tools/test-gcp-permissions/test-gcp-permissions.py
+drwxr-xr-x   0 camacho   (4819) blast      (990)        0 2023-05-11 14:13:28.511128 elastic_blast-1.1.0/src/
+drwxr-xr-x   0 camacho   (4819) blast      (990)        0 2023-05-11 14:13:28.568128 elastic_blast-1.1.0/src/elastic_blast/
+-rw-r--r--   0 camacho   (4819) blast      (990)     1280 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/__init__.py
+-rw-r--r--   0 camacho   (4819) blast      (990)    55798 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/aws.py
+-rw-r--r--   0 camacho   (4819) blast      (990)     6540 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/aws_traits.py
+-rw-r--r--   0 camacho   (4819) blast      (990)    15880 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/base.py
+drwxr-xr-x   0 camacho   (4819) blast      (990)        0 2023-05-11 14:13:28.570128 elastic_blast-1.1.0/src/elastic_blast/commands/
+-rw-r--r--   0 camacho   (4819) blast      (990)        0 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/commands/__init__.py
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     1733 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/commands/delete.py
+-rw-r--r--   0 camacho   (4819) blast      (990)    26769 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/commands/run_summary.py
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     4599 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/commands/status.py
+-rwxr-xr-x   0 camacho   (4819) blast      (990)    13259 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/commands/submit.py
+-rw-r--r--   0 camacho   (4819) blast      (990)    11321 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/config.py
+-rw-r--r--   0 camacho   (4819) blast      (990)    12152 2023-05-09 12:46:22.000000 elastic_blast-1.1.0/src/elastic_blast/constants.py
+-rw-r--r--   0 camacho   (4819) blast      (990)     3649 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/cost.py
+-rw-r--r--   0 camacho   (4819) blast      (990)     4913 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/db_metadata.py
+-rw-r--r--   0 camacho   (4819) blast      (990)     6352 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/elasticblast.py
+-rw-r--r--   0 camacho   (4819) blast      (990)     1894 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/elasticblast_factory.py
+-rw-r--r--   0 camacho   (4819) blast      (990)    58490 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/elb_config.py
+-rw-r--r--   0 camacho   (4819) blast      (990)    22806 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/filehelper.py
+-rw-r--r--   0 camacho   (4819) blast      (990)    42541 2023-05-09 12:46:22.000000 elastic_blast-1.1.0/src/elastic_blast/gcp.py
+-rw-r--r--   0 camacho   (4819) blast      (990)     3061 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/gcp_traits.py
+-rwxr-xr-x   0 camacho   (4819) blast      (990)     6135 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/janitor.py
+-rw-r--r--   0 camacho   (4819) blast      (990)     4477 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/jobs.py
+-rw-r--r--   0 camacho   (4819) blast      (990)    40358 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/kubernetes.py
+-rw-r--r--   0 camacho   (4819) blast      (990)     4755 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/object_storage_utils.py
+drwxr-xr-x   0 camacho   (4819) blast      (990)        0 2023-05-11 14:13:28.570128 elastic_blast-1.1.0/src/elastic_blast/resources/
+-rw-r--r--   0 camacho   (4819) blast      (990)        0 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/resources/__init__.py
+drwxr-xr-x   0 camacho   (4819) blast      (990)        0 2023-05-11 14:13:28.571128 elastic_blast-1.1.0/src/elastic_blast/resources/quotas/
+-rw-r--r--   0 camacho   (4819) blast      (990)        0 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/resources/quotas/__init__.py
+-rw-r--r--   0 camacho   (4819) blast      (990)     4689 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/resources/quotas/quota_aws_batch.py
+-rw-r--r--   0 camacho   (4819) blast      (990)     4925 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/resources/quotas/quota_aws_ec2_cf.py
+-rw-r--r--   0 camacho   (4819) blast      (990)     1534 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/resources/quotas/quota_check.py
+-rw-r--r--   0 camacho   (4819) blast      (990)     4945 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/split.py
+-rw-r--r--   0 camacho   (4819) blast      (990)     1845 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/subst.py
+-rw-r--r--   0 camacho   (4819) blast      (990)     8828 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/taxonomy.py
+drwxr-xr-x   0 camacho   (4819) blast      (990)        0 2023-05-11 14:13:28.589128 elastic_blast-1.1.0/src/elastic_blast/templates/
+-rw-r--r--   0 camacho   (4819) blast      (990)     4044 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/blast-batch-job-local-ssd.yaml.template
+-rw-r--r--   0 camacho   (4819) blast      (990)     4594 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/blast-batch-job.yaml.template
+-rw-r--r--   0 camacho   (4819) blast      (990)     1200 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/cloudformation-admin-iam.yaml
+-rw-r--r--   0 camacho   (4819) blast      (990)    29404 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/elastic-blast-cf.yaml
+-rw-r--r--   0 camacho   (4819) blast      (990)     9262 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/elastic-blast-janitor-cf.yaml
+-rw-r--r--   0 camacho   (4819) blast      (990)      883 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/elb-janitor-cronjob.yaml.template
+-rw-r--r--   0 camacho   (4819) blast      (990)      270 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/elb-janitor-rbac.yaml
+-rw-r--r--   0 camacho   (4819) blast      (990)      641 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/job-cloud-split-local-ssd.yaml.template
+-rw-r--r--   0 camacho   (4819) blast      (990)     2754 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/job-init-local-ssd.yaml.template
+-rw-r--r--   0 camacho   (4819) blast      (990)     3129 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/job-init-pv.yaml.template
+-rw-r--r--   0 camacho   (4819) blast      (990)     1121 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/job-submit-jobs.yaml.template
+-rw-r--r--   0 camacho   (4819) blast      (990)      309 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/pvc-rom.yaml.template
+-rw-r--r--   0 camacho   (4819) blast      (990)      212 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/pvc-rwo.yaml.template
+-rw-r--r--   0 camacho   (4819) blast      (990)      292 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/storage-gcp-ssd.yaml
+-rw-r--r--   0 camacho   (4819) blast      (990)      293 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/storage-gcp.yaml
+-rw-r--r--   0 camacho   (4819) blast      (990)      160 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/volume-snapshot-class.yaml
+-rw-r--r--   0 camacho   (4819) blast      (990)      213 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/templates/volume-snapshot.yaml
+-rw-r--r--   0 camacho   (4819) blast      (990)    16783 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/tuner.py
+-rw-r--r--   0 camacho   (4819) blast      (990)    24383 2023-05-05 19:36:06.000000 elastic_blast-1.1.0/src/elastic_blast/util.py
+drwxr-xr-x   0 camacho   (4819) blast      (990)        0 2023-05-11 14:13:28.569128 elastic_blast-1.1.0/src/elastic_blast.egg-info/
+-rw-r--r--   0 camacho   (4819) blast      (990)     4006 2023-05-11 14:13:28.000000 elastic_blast-1.1.0/src/elastic_blast.egg-info/PKG-INFO
+-rw-r--r--   0 camacho   (4819) blast      (990)     7934 2023-05-11 14:13:28.000000 elastic_blast-1.1.0/src/elastic_blast.egg-info/SOURCES.txt
+-rw-r--r--   0 camacho   (4819) blast      (990)        1 2023-05-11 14:13:28.000000 elastic_blast-1.1.0/src/elastic_blast.egg-info/dependency_links.txt
+-rw-r--r--   0 camacho   (4819) blast      (990)        1 2023-05-11 14:13:19.000000 elastic_blast-1.1.0/src/elastic_blast.egg-info/not-zip-safe
+-rw-r--r--   0 camacho   (4819) blast      (990)      226 2023-05-11 14:13:28.000000 elastic_blast-1.1.0/src/elastic_blast.egg-info/requires.txt
+-rw-r--r--   0 camacho   (4819) blast      (990)       14 2023-05-11 14:13:28.000000 elastic_blast-1.1.0/src/elastic_blast.egg-info/top_level.txt
```

### Comparing `elastic_blast-1.0.0/LICENSE.md` & `elastic_blast-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/Makefile` & `elastic_blast-1.1.0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 ELB_TEST_TIMEOUT_HEPATITIS_VS_NT?=95
 ELB_TEST_TIMEOUT_MANE_VS_PDBNT?=15
 ELB_TEST_TIMEOUT_MANE_VS_PDBNT_OPTIMAL_INSTANCE_TYPE?=30
 ELB_TEST_TIMEOUT_COALA_VS_NR?=120
 ELB_TEST_TIMEOUT_BLASTP_VIRAL_METAGENOME_VS_NR?=130
 ELB_TEST_TIMEOUT_BLASTX_WB4_2_0811_VS_NR=180
 ELB_TEST_TIMEOUT_TBLASTN_VIRAL_META_VS_NT=90
-ELB_TEST_TIMEOUT_TBLASTX_BDQE01=30
+ELB_TEST_TIMEOUT_TBLASTX_BDQE01=45
 ELB_TEST_TIMEOUT_RPSBLAST_AMR=40
 ELB_TEST_TIMEOUT_RPSTBLASTN_WB4_2_0811=30
 ELB_TEST_TIMEOUT_VIRAL_METAGENOMES_VS_SWISSPROT?=40
 ELB_TEST_TIMEOUT_ALGAE_BACTERIUM_VS_NR?=6000
 ELB_TEST_TIMEOUT_CORONAVIRUS_VS_ITSELF?=20
 ELB_TEST_TIMEOUT_DB_DOWNLOAD?=60
 ELB_TEST_TIMEOUT_JAERS_VS_NR?=300
@@ -914,35 +914,35 @@
 creds.sh:
 	[ -f ~/.aws/credentials ] && mv ~/.aws/credentials ~/.aws/credentials~ || true
 	source setenv.sh && env -u AWS_PROFILE ${GET_SAML_CREDS_TOOL} | tee $@
 	-aws sts get-caller-identity
 
 # Use to generate an AWS credentials file for the jump account. 
 # Pre-requisite, the ROLEARN and PRINCIPLEARN environment variables are set in setenv.sh
+AWS_PROF=$(shell source setenv.sh && printenv ROLEARN | awk -F / '{print $$NF}')
 aws-credentials: export DURATION=28800
 aws-credentials:
 	@source setenv.sh && env -u AWS_PROFILE ${GET_SAML_CREDS_TOOL} ${USER} | \
 		sed 's/export AWS_ACCESS_KEY_ID/aws_access_key_id/;s/export AWS_SECRET_ACCESS_KEY/aws_secret_access_key/;s/export AWS_SESSION_TOKEN/aws_session_token/;s/export AWS_DEFAULT_REGION/region/;s/"//g;1a[default]' | \
 		egrep -v AWS_ACCT\|AWS_CRED_TIME | tee $@
-	@source setenv.sh && printenv ROLEARN | awk -F / '{print "["$$NF"]"}' | tee -a $@
-	#@echo role_arn = arn:aws:iam::823214259253:role/AWS-RESEARCH-BLAST | tee -a $@
-	@echo role_arn = arn:aws:iam::414262389673:role/AWS-RESEARCH-BLAST | tee -a $@
+	@printf "\n[${AWS_PROF}]\n" | tee -a $@
+	@echo role_arn = arn:aws:iam::414262389673:role/${AWS_PROF} | tee -a $@
 	@echo source_profile = default | tee -a $@
 	@grep ^region $@ | tee -a $@
 	cp -pv --backup=numbered $@ ~/.aws/credentials
-	@echo "export AWS_PROFILE=AWS-RESEARCH-BLAST"
+	@echo "export AWS_PROFILE=${AWS_PROF}"
 	@echo "unset AWS_CRED_TIME AWS_ACCT AWS_SESSION_TOKEN AWS_DEFAULT_REGION AWS_SECRET_ACCESS_KEY AWS_ACCESS_KEY_ID"
 	-aws --profile default sts get-caller-identity
-	-aws --profile AWS-RESEARCH-BLAST sts get-caller-identity
+	-aws --profile ${AWS_PROF} sts get-caller-identity
 
 .PHONY: aws-whoami
 aws-whoami:
 	-aws sts get-caller-identity
 	-aws --profile default sts get-caller-identity
-	-aws --profile AWS-RESEARCH-BLAST sts get-caller-identity
+	-aws --profile ${AWS_PROF} sts get-caller-identity
 
 .PHONY: eks-credentials
 eks-credentials:
 	aws eks update-kubeconfig --region ${ELB_AWS_REGION} --name ${ELB_CLUSTER_NAME}
 
 .PHONY: aws-limits
 aws-limits: ${VENV} creds.sh
```

### Comparing `elastic_blast-1.0.0/PKG-INFO` & `elastic_blast-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elastic_blast
-Version: 1.0.0
+Version: 1.1.0
 License-File: LICENSE.md
 
 ElasticBLAST
 ============
 
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/elastic-blast/badges/version.svg)](https://anaconda.org/bioconda/elastic-blast)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/elastic-blast/badges/latest_release_date.svg)](https://anaconda.org/bioconda/elastic-blast)
@@ -48,14 +48,21 @@
 most suitable to you:
 
 * [Installation from PyPI.org][1]
 * [Installation from BioConda][2]
 * [Installation for the AWS Cloud Shell][3]
 * [Installation for the GCP Cloud Shell][4]
 
+
+Publication:
+------------
+
+Camacho C, Boratyn GM, Joukov V, Vera Alvarez R, Madden TL. ElasticBLAST: accelerating sequence search via cloud computing. BMC Bioinformatics. 2023 Mar 26;24(1):117. doi: [10.1186/s12859-023-05245-9](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-023-05245-9). PMID: [36967390](https://pubmed.ncbi.nlm.nih.gov/36967390/); PMCID: [PMC10040096](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10040096/).
+
+
 Developer information
 ---------------------
 
 ### How to build ElasticBLAST
 
     make elastic-blast
```

### Comparing `elastic_blast-1.0.0/README.md` & `elastic_blast-1.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -43,14 +43,21 @@
 most suitable to you:
 
 * [Installation from PyPI.org][1]
 * [Installation from BioConda][2]
 * [Installation for the AWS Cloud Shell][3]
 * [Installation for the GCP Cloud Shell][4]
 
+
+Publication:
+------------
+
+Camacho C, Boratyn GM, Joukov V, Vera Alvarez R, Madden TL. ElasticBLAST: accelerating sequence search via cloud computing. BMC Bioinformatics. 2023 Mar 26;24(1):117. doi: [10.1186/s12859-023-05245-9](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-023-05245-9). PMID: [36967390](https://pubmed.ncbi.nlm.nih.gov/36967390/); PMCID: [PMC10040096](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10040096/).
+
+
 Developer information
 ---------------------
 
 ### How to build ElasticBLAST
 
     make elastic-blast
```

### Comparing `elastic_blast-1.0.0/bin/aws-create-elastic-blast-janitor-role.sh` & `elastic_blast-1.1.0/bin/aws-create-elastic-blast-janitor-role.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/bin/aws-delete-elastic-blast-janitor-role.sh` & `elastic_blast-1.1.0/bin/aws-delete-elastic-blast-janitor-role.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/bin/aws-get-auto-scaling-events.sh` & `elastic_blast-1.1.0/bin/aws-get-auto-scaling-events.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/bin/aws-show-my-undeleted-searches.sh` & `elastic_blast-1.1.0/bin/aws-show-my-undeleted-searches.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/bin/blast-tuner.py` & `elastic_blast-1.1.0/bin/blast-tuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,16 +102,18 @@
         options += f' {mt_mode}'
 
         num_cpus = get_num_cpus(cloud_provider = cloud_provider,
                                 program = args.program,
                                 mt_mode = mt_mode,
                                 query = query_data)
         conf[CFG_BLAST][CFG_BLAST_PROGRAM] = args.program
+        task = ElbSupportedPrograms().get_task(args.program, args.options)
         conf[CFG_BLAST][CFG_BLAST_BATCH_LEN] = str(get_batch_length(cloud_provider = cloud_provider,
                                                           program = args.program,
+                                                          task = task,
                                                           mt_mode = mt_mode,
                                                           num_cpus = num_cpus))
 
         if len(options) > 1:
            conf[CFG_BLAST][CFG_BLAST_OPTIONS] = options
 
         conf[CFG_CLUSTER][CFG_CLUSTER_NUM_CPUS] = str(num_cpus)
```

### Comparing `elastic_blast-1.0.0/bin/cleanup-stale-gcp-resources.py` & `elastic_blast-1.1.0/bin/cleanup-stale-gcp-resources.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/bin/create-blastdb-metadata.py` & `elastic_blast-1.1.0/bin/create-blastdb-metadata.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/bin/elastic-blast` & `elastic_blast-1.1.0/bin/elastic-blast`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from elastic_blast.commands.status import create_arg_parser as create_status_arg_parser
 from elastic_blast.commands.delete import delete as elb_delete
 from elastic_blast.commands.run_summary import create_arg_parser as create_run_summary_arg_parser
 from elastic_blast.util import validate_installation, check_positive_int, config_logging, UserReportError, SafeExecError
 from elastic_blast.util import ElbSupportedPrograms, clean_up
 from elastic_blast import constants
 from elastic_blast.gcp import check_prerequisites
+from elastic_blast.aws import check_auxiliary_versions
 from elastic_blast.config import configure
 from elastic_blast.elb_config import ElasticBlastConfig
 from elastic_blast.constants import ElbCommand
 from elastic_blast.constants import ELB_DFLT_LOGLEVEL, ELB_DFLT_LOGFILE
 from elastic_blast.constants import CFG_CLOUD_PROVIDER, CFG_CP_GCP_PROJECT
 
 DESC = r"""This application facilitates running BLAST on large amounts of query sequence data
@@ -69,16 +70,19 @@
         if not args.subcommand:
             # report missing command line task
             raise UserReportError(returncode=constants.INPUT_ERROR,
                                   message=NO_TASK_MSG)
         config_logging(args)
         cfg = configure(args)
         logging.info(f"ElasticBLAST {args.subcommand} {VERSION}")
+        logging.info(f'python version: {":".join(sys.version.split())}')
         if CFG_CP_GCP_PROJECT in cfg[CFG_CLOUD_PROVIDER]:
             check_prerequisites()
+        else:
+            check_auxiliary_versions()
         task = ElbCommand(args.subcommand.lower())
         cfg = ElasticBlastConfig(cfg, args.dry_run, task=task)
         logging.debug(pformat(cfg.asdict()))
         #TODO: use cfg only when args.wait, args.sync, and args.run_label are replicated in cfg
         return args.func(args, cfg, clean_up_stack)
     except (SafeExecError, UserReportError) as e:
         logging.error(e.message)
```

### Comparing `elastic_blast-1.0.0/bin/elb-cost.py` & `elastic_blast-1.1.0/bin/elb-cost.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/bin/fasta_split.py` & `elastic_blast-1.1.0/bin/fasta_split.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/bin/gcp-setup-elastic-blast-janitor.sh` & `elastic_blast-1.1.0/bin/gcp-setup-elastic-blast-janitor.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/bin/gcp-show-my-undeleted-searches.sh` & `elastic_blast-1.1.0/bin/gcp-show-my-undeleted-searches.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/bin/gcp_ram_size.py` & `elastic_blast-1.1.0/bin/gcp_ram_size.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/etc/elastic-blast-aws-iam-policy.json.template` & `elastic_blast-1.1.0/share/etc/elastic-blast-aws-iam-policy.json.template`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/etc/elb-aws-blastn-multiple-query-files.ini` & `elastic_blast-1.1.0/share/etc/elb-aws-blastn-multiple-query-files.ini`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/etc/elb-aws-blastn-neg-taxidfiltering.ini` & `elastic_blast-1.1.0/share/etc/elb-aws-blastn-neg-taxidfiltering.ini`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/etc/elb-aws-blastn-non-default-params.ini` & `elastic_blast-1.1.0/share/etc/elb-aws-blastn-non-default-params.ini`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/etc/elb-aws-blastn-out-of-memory-db-download.ini` & `elastic_blast-1.1.0/share/etc/elb-aws-blastn-out-of-memory-db-download.ini`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/etc/elb-aws-blastn-out-of-memory.ini` & `elastic_blast-1.1.0/share/etc/elb-aws-blastn-out-of-memory.ini`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/etc/elb-aws-blastn-pdbnt-all-azs-provided.ini` & `elastic_blast-1.1.0/share/etc/elb-aws-blastn-pdbnt-all-azs-provided.ini`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/etc/elb-aws-blastn-pdbnt-auto-shutdown.ini` & `elastic_blast-1.1.0/share/etc/elb-aws-blastn-pdbnt-auto-shutdown.ini`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/etc/elb-aws-blastn-pdbnt-s3-query-create-resources-small-instance.ini` & `elastic_blast-1.1.0/share/etc/elb-aws-blastn-pdbnt-s3-query-create-resources-small-instance.ini`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/etc/elb-aws-blastn-taxidfiltering.ini` & `elastic_blast-1.1.0/share/etc/elb-aws-blastn-taxidfiltering.ini`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/etc/elb-aws-blastp-dark-matter.ini` & `elastic_blast-1.1.0/share/etc/elb-aws-blastp-dark-matter.ini`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/etc/elb-aws-blastp-nr-small-dark-matter.ini` & `elastic_blast-1.1.0/share/etc/elb-aws-blastp-nr-small-dark-matter.ini`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/etc/elb-aws-megablast-sra-spots.ini` & `elastic_blast-1.1.0/share/etc/elb-aws-megablast-sra-spots.ini`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/etc/elb-aws-megablast-vht1.ini` & `elastic_blast-1.1.0/share/etc/elb-aws-megablast-vht1.ini`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/etc/elb-aws-spot-optimal-instance-type-blastn-pdbnt.ini` & `elastic_blast-1.1.0/share/etc/elb-aws-spot-optimal-instance-type-blastn-pdbnt.ini`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/etc/elb-rpstblastn-five-example.ini` & `elastic_blast-1.1.0/share/etc/elb-rpstblastn-five-example.ini`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/test/Makefile` & `elastic_blast-1.1.0/share/test/Makefile`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/test/cloud-split-test.sh` & `elastic_blast-1.1.0/share/test/cloud-split-test.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/test/elb-vs-local-blast-regression-test.sh` & `elastic_blast-1.1.0/share/test/elb-vs-local-blast-regression-test.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/test/job-show-blastdbs.yaml` & `elastic_blast-1.1.0/share/test/job-show-blastdbs.yaml`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/test/job-show-queries.yaml` & `elastic_blast-1.1.0/share/test/job-show-queries.yaml`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/test/pd-scalability-tests.sh` & `elastic_blast-1.1.0/share/test/pd-scalability-tests.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/test/sanity-check-pdbnt-search-local-unsplit-query-vs-elastic-blast.sh` & `elastic_blast-1.1.0/share/test/sanity-check-pdbnt-search-local-unsplit-query-vs-elastic-blast.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/test/sanity-check-pdbnt-search-local-vs-elastic-blast.sh` & `elastic_blast-1.1.0/share/test/sanity-check-pdbnt-search-local-vs-elastic-blast.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/aws-create-instance-with-custom-instance-profile.sh` & `elastic_blast-1.1.0/share/tools/aws-create-instance-with-custom-instance-profile.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/aws-elastic-blast-number-of-nodes.sh` & `elastic_blast-1.1.0/share/tools/aws-elastic-blast-number-of-nodes.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/aws-list-vpc.sh` & `elastic_blast-1.1.0/share/tools/aws-list-vpc.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/aws-policy-create.sh` & `elastic_blast-1.1.0/share/tools/aws-policy-create.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/aws-policy-describe.sh` & `elastic_blast-1.1.0/share/tools/aws-policy-describe.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/aws-role-create.sh` & `elastic_blast-1.1.0/share/tools/aws-role-create.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/aws-role-delete.sh` & `elastic_blast-1.1.0/share/tools/aws-role-delete.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/aws-test-instance-with-custom-instance-profile.sh` & `elastic_blast-1.1.0/share/tools/aws-test-instance-with-custom-instance-profile.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/deploy-elastic-blast-docs.sh` & `elastic_blast-1.1.0/share/tools/deploy-elastic-blast-docs.sh`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     exit 1
 fi
 [ -f $DBALIASTEST ] || { echo FATAL ERROR: cannot find $DBALIASTEST; exit 1; }
 [ -f $SDRELEASE ] || { echo FATAL ERROR: cannot find $SDRELEASE; exit 1; }
 
 #  Hosts information should be obtained from *MachineTasking confluence page
 TEST_HOSTS="testblast142,testblast143"  
-BETH_PROD_HOSTS="blast339,blast349,blast359"
+BETH_PROD_HOSTS="blast339,blast349,blast520"
 COLO_PROD_HOSTS="blast3416.st-va,blast3420.st-va"
 HOSTS=$TEST_HOSTS
 if [[ "$deployment_target" == "prod" ]] ; then
     HOSTS=$BETH_PROD_HOSTS
 fi
 
 # Per Yan's suggestion
```

### Comparing `elastic_blast-1.0.0/share/tools/gcp-create-svc-acct.sh` & `elastic_blast-1.1.0/share/tools/gcp-create-svc-acct.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/gcp-delete-svc-acct.sh` & `elastic_blast-1.1.0/share/tools/gcp-delete-svc-acct.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/iam-policy-patcher.py` & `elastic_blast-1.1.0/share/tools/iam-policy-patcher.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/impersonate-tc.sh` & `elastic_blast-1.1.0/share/tools/impersonate-tc.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/paper-case-study-submit-blastn-eudicotyledons.sh` & `elastic_blast-1.1.0/share/tools/paper-case-study-submit-blastn-eudicotyledons.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/paper-case-study-submit-blastn-non-eudicotyledons.sh` & `elastic_blast-1.1.0/share/tools/paper-case-study-submit-blastn-non-eudicotyledons.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/paper-case-study-submit-megablast-eudicotyledons.sh` & `elastic_blast-1.1.0/share/tools/paper-case-study-submit-megablast-eudicotyledons.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/paper-case-study-submit-megablast-non-eudicotyledons.sh` & `elastic_blast-1.1.0/share/tools/paper-case-study-submit-megablast-non-eudicotyledons.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/query-analyzer.sh` & `elastic_blast-1.1.0/share/tools/query-analyzer.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/release-to-github.sh` & `elastic_blast-1.1.0/share/tools/release-to-github.sh`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/run-report.py` & `elastic_blast-1.1.0/share/tools/run-report.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/test-gcp-permissions/Makefile` & `elastic_blast-1.1.0/share/tools/test-gcp-permissions/Makefile`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/share/tools/test-gcp-permissions/test-gcp-permissions.py` & `elastic_blast-1.1.0/share/tools/test-gcp-permissions/test-gcp-permissions.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/__init__.py` & `elastic_blast-1.1.0/src/elastic_blast/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/aws.py` & `elastic_blast-1.1.0/src/elastic_blast/aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 from dataclasses_json import dataclass_json
 from dataclasses import dataclass, field
 from copy import deepcopy
 
 from .util import convert_labels_to_aws_tags, convert_disk_size_to_gb
 from .util import convert_memory_to_mb, UserReportError
 from .util import ElbSupportedPrograms, get_usage_reporting, sanitize_aws_batch_job_name
-from .util import get_resubmission_error_msg
+from .util import get_resubmission_error_msg, safe_exec
 from .constants import BLASTDB_ERROR, CLUSTER_ERROR, ELB_QUERY_LENGTH, PERMISSIONS_ERROR
 from .constants import ELB_QUERY_BATCH_DIR, ELB_METADATA_DIR
 from .constants import ELB_DOCKER_IMAGE_AWS, INPUT_ERROR, ELB_QS_DOCKER_IMAGE_AWS
 from .constants import DEPENDENCY_ERROR, TIMEOUT_ERROR
 from .constants import ELB_AWS_JOB_IDS, ELB_S3_PREFIX, ELB_GCS_PREFIX
 from .constants import ELB_DFLT_NUM_BATCHES_FOR_TESTING, ELB_UNKNOWN_NUMBER_OF_QUERY_SPLITS
 from .constants import ElbStatus, ELB_CJS_DOCKER_IMAGE_AWS
@@ -66,14 +66,15 @@
 from .constants import STATUS_MESSAGE_ERROR, STATUS_MESSAGE_VERBOSE
 from .filehelper import parse_bucket_name_key
 from .aws_traits import get_machine_properties, create_aws_config, get_availability_zones_for
 from .object_storage_utils import write_to_s3
 from .base import DBSource
 from .elb_config import ElasticBlastConfig, sanitize_aws_tag
 from .elasticblast import ElasticBlast
+from . import VERSION
 
 
 CF_TEMPLATE = os.path.join(os.path.dirname(__file__), 'templates', 'elastic-blast-cf.yaml')
 # the order of job states reflects state transitions and is important for
 # ElasticBlastAws.get_job_ids method
 AWS_BATCH_JOB_STATES = ['SUBMITTED', 'PENDING', 'RUNNABLE', 'STARTING', 'RUNNING', 'SUCCEEDED', 'FAILED']
 SECONDS2SLEEP = 10
@@ -142,14 +143,25 @@
         if self.query_splitting:
             id_list.append(self.query_splitting)
         if self.job_submission:
             id_list.append(self.job_submission)
         return id_list
 
 
+def check_auxiliary_versions():
+    """Check version of auxiliary tools: awscli. No errors will be reported
+    if the tools are not accessible."""
+    try:
+        p = safe_exec('aws --version')
+    except:
+        logging.debug('Could not check awscli version')
+    else:
+        logging.debug(f'{":".join(p.stdout.decode().split())}')
+
+
 class ElasticBlastAws(ElasticBlast):
     """ Implementation of core ElasticBLAST functionality in AWS.
     Uses a CloudFormation template and AWS Batch for its main operation.
     Uses a nested CloudFormation template and lambda to clean up after itself
     (janitor module)
     """
 
@@ -848,15 +860,17 @@
             # and pass BLAST_USAGE_REPORT environment var to container
             if usage_reporting:
                 overrides['environment'] = [{'name': 'BLAST_ELB_JOB_ID',
                                              'value': elb_job_id},
                                             {'name': 'BLAST_USAGE_REPORT',
                                              'value': 'true'},
                                             {'name': 'BLAST_ELB_BATCH_NUM',
-                                             'value': str(i)}]
+                                             'value': str(i)},
+                                            {'name': 'BLAST_ELB_VERSION',
+                                             'value': VERSION}]
             else:
                 overrides['environment'] = [{'name': 'BLAST_USAGE_REPORT',
                                              'value': 'false'}]
             if not self.dry_run:
                 submit_job_args = {
                     "jobQueue": self.job_queue_name,
                     "jobDefinition": self.blast_job_definition_name,
```

### Comparing `elastic_blast-1.0.0/src/elastic_blast/aws_traits.py` & `elastic_blast-1.1.0/src/elastic_blast/aws_traits.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 import boto3 # type: ignore
 from botocore.exceptions import ClientError, NoCredentialsError # type: ignore
 import logging
 from typing import Optional, List, Any
 from .util import UserReportError, check_aws_region_for_invalid_characters
 from .base import InstanceProperties, PositiveInteger, MemoryStr
 from .constants import ELB_DFLT_AWS_REGION, INPUT_ERROR, PERMISSIONS_ERROR
+from .constants import DEPENDENCY_ERROR
 
 
 def create_aws_config(region: Optional[str] = None) -> Config:
     """Create boto3 config object using application config parameters"""
     retval = None
     if region:
         retval = Config(region_name=region)
@@ -86,28 +87,32 @@
         logging.debug(err)
         raise UserReportError(returncode=PERMISSIONS_ERROR, message=str(err))
     return InstanceProperties(ncpus, nram)
 
 
 def get_instance_type_offerings(region: str) -> List[str]:
     """Get a list of instance types offered in an AWS region"""
-    ec2 = boto3.client('ec2')
+    boto_cfg = create_aws_config(region)
+    ec2 = boto3.client('ec2', config=boto_cfg)
     try:
         current = ec2.describe_instance_type_offerings(LocationType='region', Filters=[{'Name': 'location', 'Values': [region]}])
         instance_types = current['InstanceTypeOfferings']
         while 'NextToken' in current:
-            current = ec2.describe_instance_type_offerings(LocationType='regioon', Filters=[{'Name': 'location', 'Values': [region]}], NextToken=current['NextToken'])
+            current = ec2.describe_instance_type_offerings(LocationType='region', Filters=[{'Name': 'location', 'Values': [region]}], NextToken=current['NextToken'])
             instance_types += current['InstanceTypeOfferings']
     except ClientError as err:
         logging.debug(err)
         raise UserReportError(returncode=INPUT_ERROR, message=f'Invalid AWS region "{region}"')
     except NoCredentialsError as err:
         logging.debug(err)
         raise UserReportError(returncode=PERMISSIONS_ERROR, message=str(err))
 
+    if not instance_types:
+        raise UserReportError(returncode=DEPENDENCY_ERROR,
+                              message=f'Could not get instance types available in region: {region}')
     return [it['InstanceType'] for it in instance_types]
 
 
 def get_suitable_instance_types(min_memory: MemoryStr,
                                 min_cpus: PositiveInteger,
                                 instance_types: Optional[List[str]] = None) -> List[Any]:
     """Get a list of instance type descriptions with at least min_memory and
```

### Comparing `elastic_blast-1.0.0/src/elastic_blast/base.py` & `elastic_blast-1.1.0/src/elastic_blast/base.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/commands/delete.py` & `elastic_blast-1.1.0/src/elastic_blast/commands/delete.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/commands/run_summary.py` & `elastic_blast-1.1.0/src/elastic_blast/commands/run_summary.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/commands/status.py` & `elastic_blast-1.1.0/src/elastic_blast/commands/status.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/commands/submit.py` & `elastic_blast-1.1.0/src/elastic_blast/commands/submit.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/config.py` & `elastic_blast-1.1.0/src/elastic_blast/config.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/constants.py` & `elastic_blast-1.1.0/src/elastic_blast/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,15 +200,15 @@
 
 
 ELB_DFLT_GCP_REGION = 'us-east4'
 ELB_DFLT_GCP_ZONE = 'us-east4-b'
 ELB_DFLT_AWS_REGION = 'us-east-1'
 ELB_UNKNOWN_GCP_PROJECT = 'elb-unknown-gcp-project'
 
-ELB_DOCKER_VERSION = '1.1.3'
+ELB_DOCKER_VERSION = '1.2.0'    # ElasticBLAST 1.1.0 uses BLAST+ 2.14.0
 ELB_QS_DOCKER_VERSION = '0.1.4'
 ELB_JANITOR_DOCKER_VERSION = '0.3.0'
 ELB_JOB_SUBMIT_DOCKER_VERSION = '3.0.0'
 
 ELB_DOCKER_IMAGE_GCP = f'gcr.io/ncbi-sandbox-blast/ncbi/elb:{ELB_DOCKER_VERSION}'
 ELB_DOCKER_IMAGE_AWS = f'public.ecr.aws/ncbi-elasticblast/elasticblast-elb:{ELB_DOCKER_VERSION}'
 
@@ -222,28 +222,33 @@
 
 ELB_DFLT_AWS_DISK_TYPE = 'gp3'
 ELB_DFLT_AWS_PD_SIZE = '1000G'
 # Only relevant if the disk-type is set to io2
 ELB_DFLT_AWS_PROVISIONED_IOPS = '2000'
 ELB_DFLT_AWS_SPOT_BID_PERCENTAGE = '100'
 
+# This value is assigned to gke_version. It should be set to None to use the
+# default k8s version in GKE, otherwise it should be set to a specific version
+# supported by GKE (e.g.: 1.25)
+ELB_DFLT_GCP_K8S_VERSION = '1.25'
+
 # Config sections
 CFG_CLOUD_PROVIDER = 'cloud-provider'
 CFG_CLUSTER = 'cluster'
 CFG_BLAST = 'blast'
 CFG_TIMEOUTS = 'timeouts'
 # Config keys
 # Cloud provider
 CFG_CP_NAME = 'name'
 CFG_CP_GCP_PROJECT = 'gcp-project'
 CFG_CP_GCP_REGION = 'gcp-region'
 CFG_CP_GCP_ZONE = 'gcp-zone'
 CFG_CP_GCP_NETWORK = 'gcp-network'
 CFG_CP_GCP_SUBNETWORK = 'gcp-subnetwork'
-CFG_CP_GCP_GKE_VERSION = 'gke-version'
+CFG_CP_GCP_K8S_VERSION = 'gke-version'
 CFG_CP_AWS_REGION = 'aws-region'
 CFG_CP_AWS_KEY_PAIR = 'aws-key-pair'
 CFG_CP_AWS_VPC = 'aws-vpc'
 CFG_CP_AWS_SUBNET = 'aws-subnet'
 CFG_CP_AWS_SECURITY_GROUP = 'aws-security-group'
 CFG_CP_AWS_JOB_ROLE = 'aws-job-role'
 CFG_CP_AWS_INSTANCE_ROLE = 'aws-instance-role'
```

### Comparing `elastic_blast-1.0.0/src/elastic_blast/cost.py` & `elastic_blast-1.1.0/src/elastic_blast/cost.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/db_metadata.py` & `elastic_blast-1.1.0/src/elastic_blast/db_metadata.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/elasticblast.py` & `elastic_blast-1.1.0/src/elastic_blast/elasticblast.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/elasticblast_factory.py` & `elastic_blast-1.1.0/src/elastic_blast/elasticblast_factory.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/elb_config.py` & `elastic_blast-1.1.0/src/elastic_blast/elb_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 from .constants import ELB_DFLT_INIT_PV_TIMEOUT, ELB_DFLT_BLAST_K8S_TIMEOUT
 from .constants import ELB_DFLT_AWS_SPOT_BID_PERCENTAGE
 from .constants import ELB_DFLT_AWS_DISK_TYPE, ELB_DFLT_OUTFMT
 from .constants import ELB_BLASTDB_MEMORY_MARGIN
 from .constants import CFG_CLOUD_PROVIDER
 from .constants import CFG_CP_GCP_PROJECT, CFG_CP_GCP_REGION, CFG_CP_GCP_ZONE
 from .constants import CFG_CP_GCP_NETWORK, CFG_CP_GCP_SUBNETWORK
-from .constants import CFG_CP_GCP_GKE_VERSION
+from .constants import CFG_CP_GCP_K8S_VERSION
 from .constants import CFG_CP_AWS_REGION, CFG_CP_AWS_VPC, CFG_CP_AWS_SUBNET
 from .constants import CFG_CP_AWS_JOB_ROLE, CFG_CP_AWS_BATCH_SERVICE_ROLE
 from .constants import CFG_CP_AWS_INSTANCE_ROLE, CFG_CP_AWS_SPOT_FLEET_ROLE
 from .constants import CFG_CP_AWS_SECURITY_GROUP, CFG_CP_AWS_KEY_PAIR
 from .constants import CFG_BLAST, CFG_BLAST_PROGRAM, CFG_BLAST_DB
 from .constants import CFG_BLAST_DB_SRC, CFG_BLAST_RESULTS, CFG_BLAST_QUERY
 from .constants import CFG_BLAST_OPTIONS, CFG_BLAST_BATCH_LEN
@@ -82,14 +82,15 @@
 from .constants import SYSTEM_MEMORY_RESERVE, ELB_AWS_ARM_INSTANCE_TYPE_REGEX
 from .constants import ELB_DFLT_AWS_NUM_CPUS, ELB_DFLT_GCP_NUM_CPUS
 from .constants import ELB_S3_PREFIX, ELB_GCS_PREFIX, ELB_UNKNOWN_MAX_NUMBER_OF_CONCURRENT_JOBS
 from .constants import AWS_ROLE_PREFIX, CFG_CP_AWS_AUTO_SHUTDOWN_ROLE
 from .constants import BLASTDB_ERROR, ELB_UNKNOWN, ELB_JANITOR_SCHEDULE
 from .constants import ELB_DFLT_GCP_REGION, ELB_DFLT_GCP_ZONE
 from .constants import ELB_DFLT_AWS_REGION, ELB_UNKNOWN_GCP_PROJECT
+from .constants import ELB_DFLT_GCP_K8S_VERSION
 from .util import validate_gcp_string, check_aws_region_for_invalid_characters
 from .util import validate_gke_cluster_name, ElbSupportedPrograms
 from .util import get_query_batch_size, get_gcp_project
 from .util import UserReportError, safe_exec
 from .util import gcp_get_regions, sanitize_for_k8s
 from .gcp_traits import get_machine_properties as gcp_get_machine_properties
 from .gcp_traits import enable_gcp_api
@@ -221,30 +222,29 @@
     """GCP config for ElasticBLAST"""
     region: GCPString = GCPString(ELB_DFLT_GCP_REGION)
     project: GCPString = GCPString(ELB_UNKNOWN_GCP_PROJECT)
     zone: GCPString = GCPString(ELB_DFLT_GCP_ZONE)
     network: Optional[str] = None
     subnet: Optional[str] = None
     user: Optional[str] = None
-    # gke_version should be set to None to use the default GKE, otherwise use a specific version supported by GKE (e.g.: 1.25)
-    gke_version: Optional[str] = None
+    gke_version: Optional[str] = ELB_DFLT_GCP_K8S_VERSION
     # if True, GCP project will be passed to gsutil calls that download files
     # from GCS and users will be charged for the downloads.
     requester_pays: bool = False
 
     # mapping to class attributes to ConfigParser parameters so that objects
     # can be initialized from ConfigParser objects
     mapping = {'project': ParamInfo(CFG_CLOUD_PROVIDER, CFG_CP_GCP_PROJECT),
                'region': ParamInfo(CFG_CLOUD_PROVIDER, CFG_CP_GCP_REGION),
                'zone': ParamInfo(CFG_CLOUD_PROVIDER, CFG_CP_GCP_ZONE),
                'cloud': None,
                'user': None,
                'network': ParamInfo(CFG_CLOUD_PROVIDER, CFG_CP_GCP_NETWORK),
                'subnet': ParamInfo(CFG_CLOUD_PROVIDER, CFG_CP_GCP_SUBNETWORK),
-               'gke_version': ParamInfo(CFG_CLOUD_PROVIDER, CFG_CP_GCP_GKE_VERSION),
+               'gke_version': ParamInfo(CFG_CLOUD_PROVIDER, CFG_CP_GCP_K8S_VERSION),
                'requester_pays': None}
  
     def __post_init__(self):
         self.cloud = CSP.GCP
         self.user = ELB_UNKNOWN
 
         # FIXME: need to pass dry-run to this method
@@ -719,16 +719,19 @@
                                                    self.cluster.machine_type,
                                                    self.cluster.num_cpus,
                                                    cloud_region=self.cloud_provider.region)
 
         # set batch length
         if self.blast and not self.cluster.dry_run:
             if self.blast.batch_len == ELB_NOT_INITIALIZED_NUM:
+                blast_task = ElbSupportedPrograms().get_task(self.blast.program,
+                                                             self.blast.options)
                 self.blast.batch_len = get_batch_length(self.cloud_provider.cloud,
                                                         self.blast.program,
+                                                        blast_task,
                                                         mt_mode,
                                                         self.cluster.num_cpus,
                                                         self.blast.db_metadata)
             else:
                 logging.debug(f'User provided batch length {self.blast.batch_len}')
                 self.blast.user_provided_batch_len = True
 
@@ -802,14 +805,15 @@
                               aws_region: Optional[str] = None,
                               gcp_project: Optional[str] = None,
                               gcp_region: Optional[str] = None,
                               gcp_zone: Optional[str] = None,
                               program: Optional[str] = None,
                               db: Optional[str] = None,
                               queries: Optional[str] = None,
+                              options: str = '',
                               dry_run: Optional[bool] = None,
                               cluster_name: Optional[str] = None,
                               machine_type: str = ''):
         """Initialize config object from required parameters"""
         if aws_region and (gcp_project or gcp_region or gcp_zone):
             raise ValueError('Cloud provider config contains entries for more than one cloud provider. Only one cloud provider can be used')
 
@@ -838,15 +842,16 @@
                 raise ValueError('BLAST program is missing')
             if not db:
                 raise ValueError('BLAST db is missing')
             if not queries:
                 raise ValueError('BLAST queries are missing')
             self.blast = BlastConfig(program = BLASTProgram(program),
                                      db = db,
-                                     queries_arg = queries)
+                                     queries_arg = queries,
+                                     options = options)
 
             self.timeouts = TimeoutsConfig()
             self.appstate = AppState()
 
 
     def _validate_config_parser(self, parser: configparser.ConfigParser) -> None:
         """Ensure that each config parser key is mapped to an attribute.
```

### Comparing `elastic_blast-1.0.0/src/elastic_blast/filehelper.py` & `elastic_blast-1.1.0/src/elastic_blast/filehelper.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   write to local, GS, and S3
   read gzip, tar/tgz/tar.gz/tar.bz2 (all files in archive merged into one)
 
 Author: Victor Joukov joukovv@ncbi.nlm.nih.gov
 """
 
 import subprocess, os, io, gzip, tarfile, re, tempfile, shutil, sys
-import logging
+import logging, shlex
 import urllib.request
 from string import digits
 from random import sample
 from timeit import default_timer as timer
 from contextlib import contextmanager
 from tenacity import retry, stop_after_attempt, wait_exponential
 from typing import Dict, IO, Tuple, Iterable, Generator, TextIO, List, Optional
@@ -79,20 +79,20 @@
         with open_for_read(qlen_file, gcp_project) as ql:
             qlen = int(ql.read())
         qbatch_list_file = os.path.join(bucket_name, ELB_METADATA_DIR, ELB_GCP_BATCH_LIST)
         with open_for_read(qbatch_list_file, gcp_project) as qlist:
             for line in qlist:
                 query_batches.append(line.strip())
     else:
-        raise NotImplementedError(f'Harvesting query splitting results from {bucket} not supported')
+        raise NotImplementedError(f'Harvesting query splitting results from {bucket_name} not supported')
 
     return QuerySplittingResults(query_length=qlen, query_batches=query_batches)
 
 
-@retry(reraise=True, stop=stop_after_attempt(3), wait=wait_exponential(multiplier=1, min=2, max=10))
+@retry(reraise=True, stop=stop_after_attempt(3), wait=wait_exponential(multiplier=1, min=2, max=10))    # type: ignore
 def upload_file_to_gcs(filename: str, gcs_location: str, dry_run: bool = False) -> None:
     """ Function to copy the filename provided to GCS """
     cmd = f'gsutil -qm cp {filename} {gcs_location}'
     if dry_run:
         logging.info(cmd)
     else:
         safe_exec(cmd)
@@ -480,16 +480,16 @@
     global error_report_funcs
     gzipped = fname[-3:] == ".gz"
     tarred = re.match(r'^.*\.(tar(|\.gz|\.bz2)|tgz)$', fname) is not None
     binary = gzipped or tarred
     mode = 'rb' if binary else 'rt'
     if fname.startswith(ELB_GCS_PREFIX):
         prj = f'-u {gcp_prj}' if gcp_prj else ''
-        cmd = f'gsutil {prj} cat {fname}'
-        proc = subprocess.Popen(cmd.split(),
+        cmd = f'gsutil {prj} cat ' + shlex.quote(fname)
+        proc = subprocess.Popen(shlex.split(cmd),
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             universal_newlines=not binary)
         fileobj = unpack_stream(proc.stdout, gzipped, tarred)
         if proc.stderr:
             error_report_funcs[fileobj] = proc.stderr.read
         return fileobj
```

### Comparing `elastic_blast-1.0.0/src/elastic_blast/gcp.py` & `elastic_blast-1.1.0/src/elastic_blast/gcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 from .constants import GKE_CLUSTER_STATUS_PROVISIONING, GKE_CLUSTER_STATUS_RECONCILING
 from .constants import GKE_CLUSTER_STATUS_RUNNING, GKE_CLUSTER_STATUS_RUNNING_WITH_ERROR
 from .constants import GKE_CLUSTER_STATUS_STOPPING, GKE_CLUSTER_STATUS_ERROR
 from .constants import STATUS_MESSAGE_ERROR
 from .elb_config import ElasticBlastConfig
 from .elasticblast import ElasticBlast
 from .gcp_traits import enable_gcp_api
+from . import VERSION
 
 class ElasticBlastGcp(ElasticBlast):
     """ Implementation of core ElasticBLAST functionality in GCP. """
     def __init__(self, cfg: ElasticBlastConfig, create=False, cleanup_stack: Optional[List[Any]]=None):
         super().__init__(cfg, create, cleanup_stack)
         self.query_files: List[str] = []
         self.cluster_initialized = False
@@ -418,14 +419,15 @@
             'ELB_BLAST_TIMEOUT': str(cfg.timeouts.blast_k8s * 60),
             'ELB_RESULTS': cfg.cluster.results,
             'ELB_NUM_CPUS': str(cfg.cluster.num_cpus),
             'ELB_DB_MOL_TYPE': str(ElbSupportedPrograms().get_db_mol_type(blast_program)),
             'ELB_DOCKER_IMAGE': ELB_DOCKER_IMAGE_GCP,
             'ELB_TIMEFMT': '%s%N',  # timestamp in nanoseconds
             'BLAST_ELB_JOB_ID': uuid.uuid4().hex,
+            'BLAST_ELB_VERSION': VERSION,
             'BLAST_USAGE_REPORT': str(usage_reporting).lower(),
             'K8S_JOB_GET_BLASTDB' : K8S_JOB_GET_BLASTDB,
             'K8S_JOB_LOAD_BLASTDB_INTO_RAM' : K8S_JOB_LOAD_BLASTDB_INTO_RAM,
             'K8S_JOB_IMPORT_QUERY_BATCHES' : K8S_JOB_IMPORT_QUERY_BATCHES,
             'K8S_JOB_SUBMIT_JOBS' : K8S_JOB_SUBMIT_JOBS,
             'K8S_JOB_BLAST' : K8S_JOB_BLAST,
             'K8S_JOB_RESULTS_EXPORT' : K8S_JOB_RESULTS_EXPORT
@@ -543,15 +545,15 @@
         raise ValueError('No disk name provided')
     if not cfg:
         raise ValueError('No application config provided')
     cmd = f'gcloud compute disks delete -q {name} --project {cfg.gcp.project}  --zone {cfg.gcp.zone}'
     safe_exec(cmd)
 
 
-@retry(reraise=True, stop=stop_after_attempt(3), wait=wait_exponential(multiplier=1, min=2, max=10))
+@retry(reraise=True, stop=stop_after_attempt(3), wait=wait_exponential(multiplier=1, min=2, max=10)) # type: ignore
 def _get_pd_id(cfg: ElasticBlastConfig) -> List[str]:
     """ Try to get the GCP persistent disk ID from elastic-blast records"""
     retval = list()
     if cfg.appstate.disk_ids:
         retval = cfg.appstate.disk_ids
         logging.debug(f'GCP disk ID {retval}')
         # no need to get disk id from GS if we already have it
@@ -596,15 +598,15 @@
     Arguments:
         cfg: Config parameters"""
 
     dry_run = cfg.cluster.dry_run
     try_kubernetes = True
     pds = []
     try:
-        pds = _get_pd_id(cfg)
+        pds = _get_pd_id(cfg) # type: ignore
     except Exception as e:
         logging.error(f'Unable to read disk id from GS: {e}')
     else:
         logging.debug(f'PD id {" ".join(pds)}')
 
     # determine the course of action based on cluster status
     while True:
@@ -911,30 +913,35 @@
 
 def check_prerequisites() -> None:
     """ Check that necessary tools, gcloud, gsutil, and kubectl
     are available if necessary.
     If execution of one of these tools is unsuccessful
     it will throw UserReportError exception."""
     try:
-        safe_exec('gcloud --version')
+        p = safe_exec('gcloud --version')
     except SafeExecError as e:
         message = f"Required pre-requisite 'gcloud' doesn't work, check installation of GCP SDK.\nDetails: {e.message}"
         raise UserReportError(DEPENDENCY_ERROR, message)
+    logging.debug(f'{":".join(p.stdout.decode().split())}')
+
     try:
         # client=true prevents kubectl from addressing server which can be down at the moment
-        safe_exec('kubectl version --client=true')
+        p = safe_exec('kubectl version --client=true')
     except SafeExecError as e:
         message = f"Required pre-requisite 'kubectl' doesn't work, check Kubernetes installation.\nDetails: {e.message}"
         raise UserReportError(DEPENDENCY_ERROR, message)
+    logging.debug(f'{":".join(p.stdout.decode().split())}')
+
     # Check we have gsutil available
     try:
-        safe_exec('gsutil --version')
+        p = safe_exec('gsutil --version')
     except SafeExecError as e:
         message = f"Required pre-requisite 'gsutil' doesn't work, check installation of GCP SDK.\nDetails: {e.message}\nNote: this is because your query is located on GS, you may try another location"
         raise UserReportError(DEPENDENCY_ERROR, message)
+    logging.debug(f'{":".join(p.stdout.decode().split())}')
 
 
 def remove_split_query(cfg: ElasticBlastConfig) -> None:
     """ Remove split query from user's results bucket """
     _remove_ancillary_data(cfg, ELB_QUERY_BATCH_DIR)
```

### Comparing `elastic_blast-1.0.0/src/elastic_blast/gcp_traits.py` & `elastic_blast-1.1.0/src/elastic_blast/gcp_traits.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/janitor.py` & `elastic_blast-1.1.0/src/elastic_blast/janitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     """ Wrapper function to copy a file to cloud object storage """
     try:
         check_for_read(bucket)
     except FileNotFoundError:
         if bucket.startswith(ELB_S3_PREFIX):
             copy_file_to_s3(bucket, Path(filename))
         else:
-            upload_file_to_gcs(filename, bucket)
+            upload_file_to_gcs(filename, bucket) # type: ignore
 
 
 def janitor(elb: ElasticBlast) -> None:
     """ ElasticBLAST Janitor function: cleans up ElasticBLAST resources """
     st, _, _ = elb.check_status()
     results = elb.cfg.cluster.results
     cluster_name = elb.cfg.cluster.name
```

### Comparing `elastic_blast-1.0.0/src/elastic_blast/jobs.py` & `elastic_blast-1.1.0/src/elastic_blast/jobs.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/kubernetes.py` & `elastic_blast-1.1.0/src/elastic_blast/kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         p = safe_exec(cmd)
         if p.stdout:
             pds = json.loads(p.stdout.decode())
             return [i['spec']['csi']['volumeHandle'].split('/')[-1] for i in pds['items']]
     return list()
 
 
-@retry( stop=(stop_after_delay(ELB_K8S_JOB_SUBMISSION_TIMEOUT) | stop_after_attempt(ELB_K8S_JOB_SUBMISSION_MAX_RETRIES)), wait=wait_random(min=ELB_K8S_JOB_SUBMISSION_MIN_WAIT, max=ELB_K8S_JOB_SUBMISSION_MAX_WAIT))
+@retry( stop=(stop_after_delay(ELB_K8S_JOB_SUBMISSION_TIMEOUT) | stop_after_attempt(ELB_K8S_JOB_SUBMISSION_MAX_RETRIES)), wait=wait_random(min=ELB_K8S_JOB_SUBMISSION_MIN_WAIT, max=ELB_K8S_JOB_SUBMISSION_MAX_WAIT)) # type: ignore
 def submit_jobs_with_retries(k8s_ctx: str, path: pathlib.Path, dry_run=False) -> List[str]:
     """ Retry kubernetes job submissions with the parameters specified in the decorator """
     return submit_jobs(k8s_ctx, path, dry_run)
 
 
 def submit_jobs(k8s_ctx: str, path: pathlib.Path, dry_run=False) -> List[str]:
     """Submit kubernetes jobs using yaml files in the provided path.
@@ -142,15 +142,15 @@
     if path.is_dir():
         num_files = len(os.listdir(str(path)))
         if num_files == 0 and not dry_run:
             raise RuntimeError(f'Job directory {str(path)} is empty')
         elif num_files > K8S_MAX_JOBS_PER_DIR:
             files = os.listdir(str(path))
             for i, f in enumerate(sorted(files, key=lambda x: int(os.path.splitext(x)[0].split('_')[1]))):
-                retval += submit_jobs_with_retries(k8s_ctx, pathlib.Path(os.path.join(path, f)), dry_run)
+                retval += submit_jobs_with_retries(k8s_ctx, pathlib.Path(os.path.join(path, f)), dry_run) # type: ignore
                 perc_done = i / num_files * 100.
                 if i % 50 == 0:
                     logging.debug(f'Submitted job file # {i} of {num_files} {perc_done:.2f}% done')
             return retval
 
     cmd = f'kubectl --context={k8s_ctx} apply -f {path} -o json'
     if dry_run:
```

### Comparing `elastic_blast-1.0.0/src/elastic_blast/object_storage_utils.py` & `elastic_blast-1.1.0/src/elastic_blast/object_storage_utils.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/resources/quotas/quota_aws_batch.py` & `elastic_blast-1.1.0/src/elastic_blast/resources/quotas/quota_aws_batch.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/resources/quotas/quota_check.py` & `elastic_blast-1.1.0/src/elastic_blast/resources/quotas/quota_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,13 +24,13 @@
     requested can be met, the function will return, otherwise an exception will
     be raised.
     """
     if cfg.cluster.dry_run:
         return
     if cfg.cloud_provider.cloud == elastic_blast.config.CSP.AWS:
         boto_cfg = create_aws_config(cfg.aws.region)
-        ResourceCheckAwsEc2CloudFormation(boto_cfg)()
+        ResourceCheckAwsEc2CloudFormation(cfg, boto_cfg)()
         ResourceCheckAwsBatch(boto_cfg)()
     elif cfg.cloud_provider.cloud == elastic_blast.config.CSP.GCP:
         raise NotImplementedError('Resource check for GCP is not implemented yet')
     else:
         raise NotImplementedError('Resource check for unknown cloud vendor')
```

### Comparing `elastic_blast-1.0.0/src/elastic_blast/split.py` & `elastic_blast-1.1.0/src/elastic_blast/split.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/subst.py` & `elastic_blast-1.1.0/src/elastic_blast/subst.py`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/taxonomy.py` & `elastic_blast-1.1.0/src/elastic_blast/taxonomy.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from .util import UserReportError
 from .elb_config import ElasticBlastConfig 
 
 from typing import List, Dict
 
 
 # retry function up to 3 times if utllib.errors.HTTPError occurs
-@retry(retry=retry_if_exception_type(HTTPError), reraise=True, stop=stop_after_attempt(3), wait=wait_exponential(multiplier=1, min=2, max=10))
+@retry(retry=retry_if_exception_type(HTTPError), reraise=True, stop=stop_after_attempt(3), wait=wait_exponential(multiplier=1, min=2, max=10))  # type: ignore
 def entrez_query(tool: str, query: Dict[str, str]) -> str:
     """Run NCBI entrez query using e-utils.
 
     Arguments:
         tool: E-utils tool (esearch, efetch, esummary, etc.)
         query: Entrez query as a dictionary of key-value pairs
 
@@ -76,15 +76,15 @@
     for taxid in user_taxids:
 
         logging.debug(f'Getting species level taxids for {taxid}')
 
         # esearch
         result = entrez_query('esearch', {'db': 'taxonomy',
                                           'term': f'txid{taxid}[orgn]',
-                                          'usehistory': 'y'})
+                                          'usehistory': 'y'}) # type: ignore
 
         # report an error if taxid is invalid
         if 'PhraseNotFound' in result:
             raise UserReportError(returncode=INPUT_ERROR,
                                   message=f'"{taxid}" is not a valid taxonomy id')
 
         webenvs = re.findall(r'<WebEnv>(\S+)</WebEnv>', result)
@@ -95,15 +95,15 @@
         webenv = webenvs[0]
         query_key = query_keys[0]
 
         # efetch
         result = entrez_query('efetch', {'db': 'taxonomy',
                                          'WebEnv': webenv,
                                          'query_key': query_key,
-                                         'format': 'uid'})
+                                         'format': 'uid'}) # type: ignore
 
         species_taxids += [int(num) for num in re.findall(r'(\d+)', result)]
         # E-utils allows up to 3 requests per second
         if len(user_taxids) > 1:
             time.sleep(1)
 
     return sorted(species_taxids)
```

### Comparing `elastic_blast-1.0.0/src/elastic_blast/templates/blast-batch-job-local-ssd.yaml.template` & `elastic_blast-1.1.0/src/elastic_blast/templates/blast-batch-job-local-ssd.yaml.template`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
         env:
         - name: BLAST_USAGE_REPORT
           value: "${BLAST_USAGE_REPORT}"
         - name: BLAST_ELB_JOB_ID
           value: "${BLAST_ELB_JOB_ID}"
         - name: BLAST_ELB_BATCH_NUM
           value: "${BLAST_ELB_BATCH_NUM}"
+        - name: BLAST_ELB_VERSION
+          value: "${BLAST_ELB_VERSION}"
         command: ["/bin/bash", "-c"]
         args:
         - echo "BASH version ${BASH_VERSION}";
           BLAST_RUNTIME=`mktemp`;
           ERROR_FILE=`mktemp`;
           DATE_NOW=`date -u +${ELB_TIMEFMT}`;
           blastdbcmd -info -db ${ELB_DB} | awk '/total/ {print $3}' | tr -d , > /shared/results/BLASTDB_LENGTH.out;
```

### Comparing `elastic_blast-1.0.0/src/elastic_blast/templates/blast-batch-job.yaml.template` & `elastic_blast-1.1.0/src/elastic_blast/templates/blast-batch-job.yaml.template`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,16 @@
         env:
         - name: BLAST_USAGE_REPORT
           value: "${BLAST_USAGE_REPORT}"
         - name: BLAST_ELB_JOB_ID
           value: "${BLAST_ELB_JOB_ID}"
         - name: BLAST_ELB_BATCH_NUM
           value: "${BLAST_ELB_BATCH_NUM}"
+        - name: BLAST_ELB_VERSION
+          value: "${BLAST_ELB_VERSION}"
         command: ["/bin/bash", "-c"]
         args:
         - echo "BASH version ${BASH_VERSION}";
           BLAST_RUNTIME=`mktemp`;
           ERROR_FILE=`mktemp`;
           DATE_NOW=`date -u +${ELB_TIMEFMT}`;
           blastdbcmd -info -db ${ELB_DB} | awk '/total/ {print $3}' | tr -d , > /blast/results/BLASTDB_LENGTH.out;
```

### Comparing `elastic_blast-1.0.0/src/elastic_blast/templates/cloudformation-admin-iam.yaml` & `elastic_blast-1.1.0/src/elastic_blast/templates/cloudformation-admin-iam.yaml`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/templates/elastic-blast-cf.yaml` & `elastic_blast-1.1.0/src/elastic_blast/templates/elastic-blast-cf.yaml`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/templates/elastic-blast-janitor-cf.yaml` & `elastic_blast-1.1.0/src/elastic_blast/templates/elastic-blast-janitor-cf.yaml`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/templates/elb-janitor-cronjob.yaml.template` & `elastic_blast-1.1.0/src/elastic_blast/templates/elb-janitor-cronjob.yaml.template`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-apiVersion: batch/v1beta1
+apiVersion: batch/v1
 kind: CronJob
 metadata:
   # This cannot exceed 52 characters
   name: elb-janitor
   labels:
     app: janitor
 spec:
```

### Comparing `elastic_blast-1.0.0/src/elastic_blast/templates/job-cloud-split-local-ssd.yaml.template` & `elastic_blast-1.1.0/src/elastic_blast/templates/job-cloud-split-local-ssd.yaml.template`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/templates/job-init-local-ssd.yaml.template` & `elastic_blast-1.1.0/src/elastic_blast/templates/job-init-local-ssd.yaml.template`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/templates/job-init-pv.yaml.template` & `elastic_blast-1.1.0/src/elastic_blast/templates/job-init-pv.yaml.template`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/templates/job-submit-jobs.yaml.template` & `elastic_blast-1.1.0/src/elastic_blast/templates/job-submit-jobs.yaml.template`

 * *Files identical despite different names*

### Comparing `elastic_blast-1.0.0/src/elastic_blast/tuner.py` & `elastic_blast-1.1.0/src/elastic_blast/tuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,22 +160,24 @@
             num_cpus += 1
         if cloud_provider == CSP.AWS:
             return min([num_cpus, MAX_NUM_THREADS_AWS])
         else:
             return min([num_cpus, MAX_NUM_THREADS_GCP])
 
 
-def get_batch_length(cloud_provider: CSP, program: str, mt_mode: MTMode,
-                     num_cpus: int, db_metadata: Optional[DbMetadata] = None) -> int:
+def get_batch_length(cloud_provider: CSP, program: str, task: Optional[str],
+                     mt_mode: MTMode, num_cpus: int,
+                     db_metadata: Optional[DbMetadata] = None) -> int:
     """
     Get batch length for BLAST batch search
 
     Arguments:
         cloud_provider: Cloud provider
         program: BLAST program
+        task: BLAST task command line parameter value
         mt_mode: BLAST MT mode
         num_cpus: Number of threads/CPUs to use
         db_metadata: BLAST database metadata
     """
     batch_len = get_query_batch_size(program)
     if batch_len is None:
         raise UserReportError(returncode=INPUT_ERROR,
@@ -188,14 +190,18 @@
                                   message=f"Invalid BLAST program '{program}'")
         max_num_cpus = MAX_NUM_THREADS_AWS if cloud_provider == CSP.AWS else MAX_NUM_THREADS_GCP
         batch_len *= min((num_cpus, max_num_cpus))
         if program.lower() == 'rpsblast' or program.lower() == 'blastp':
             batch_len *= 2
     else:
         # MTMode.ZERO
+        if program.lower() == 'blastn':
+            if task and task in ['blastn', 'dc-megablast']:
+                batch_len = 1000000
+
         if db_metadata:
             if program.lower() == 'blastp':
                 batch_len = 20000
                 if db_metadata.number_of_letters < 2e10:
                     batch_len = 40000
             elif program.lower() == 'blastx':
                 if db_metadata.number_of_letters < 2e10:
```

### Comparing `elastic_blast-1.0.0/src/elastic_blast/util.py` & `elastic_blast-1.1.0/src/elastic_blast/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from functools import reduce
 from pkg_resources import resource_exists
 from typing import List, Union, Callable, Optional
 from .constants import MolType, GCS_DFLT_BUCKET
 from .constants import DEPENDENCY_ERROR, AWS_MAX_TAG_LENGTH, GCP_MAX_LABEL_LENGTH
 from .constants import AWS_MAX_JOBNAME_LENGTH, CSP, ELB_GCS_PREFIX
 from .constants import ELB_DFLT_LOGLEVEL, ELB_DFLT_LOGFILE
+from .constants import INPUT_ERROR
 from .base import DBSource
 
 RESOURCES = [
     'job-cloud-split-local-ssd.yaml.template',
     'job-init-local-ssd.yaml.template',
     'storage-gcp-ssd.yaml',
     'pvc-rwo.yaml.template',
@@ -84,14 +85,20 @@
         'psiblast',
         'rpsblast',
         'rpstblastn',
         'tblastn',
         'tblastx'
     ]
 
+    _tasks = {'blastp': ['blastp', 'blastp-fast', 'blastp-short'],
+              'blastn': ['blastn', 'blastn-short', 'dc-megablast', 'megablast'],
+              'blastx': ['blastx', 'blastx-fast'],
+              'tblastn': ['tblastn', 'tblastn-fast']}
+              
+
     def get(self):
         return self._programs
 
     def check(self, program):
         if program not in self._programs:
             raise ValueError(f"{program} is not a supported BLAST program")
 
@@ -126,14 +133,29 @@
         elif p in ['blastp', 'tblastn', 'psiblast', 'rpsblast']:
             retval = MolType.PROTEIN
         else:
             raise NotImplementedError(f'Invalid BLAST program "{program}"')
         return retval
 
 
+    def get_task(self, program: str, options: str) -> Optional[str]:
+        """Parse blast command line options and return task or None if the
+        task was not specified in the command line. Raise UserReportError for
+        inapropriate tasks."""
+        m = re.search(r'-task ([\w-]+)', options)
+        if not m:
+            return None
+        task = m.group(1)
+        if program.lower() not in self._tasks.keys():
+            raise UserReportError(INPUT_ERROR, f'Incorrect -task option in "{options}". {program} does not support the task command line parameter.')
+        if task.lower() not in self._tasks[program.lower()]:
+            raise UserReportError(INPUT_ERROR, f'Incorrect -task option in "{options}". Allowed task values for {program} are {self._tasks[program]}.')
+        return task.lower()
+
+
 def get_query_batch_size(program: str) -> int:
     """ Return the query batch size for use in ElasticBLAST
 
     program: BLAST program name
     returns: integer or -1 in case of invalid/unrecognized input
 
     """
```

### Comparing `elastic_blast-1.0.0/src/elastic_blast.egg-info/PKG-INFO` & `elastic_blast-1.1.0/src/elastic_blast.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elastic-blast
-Version: 1.0.0
+Version: 1.1.0
 License-File: LICENSE.md
 
 ElasticBLAST
 ============
 
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/elastic-blast/badges/version.svg)](https://anaconda.org/bioconda/elastic-blast)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/elastic-blast/badges/latest_release_date.svg)](https://anaconda.org/bioconda/elastic-blast)
@@ -48,14 +48,21 @@
 most suitable to you:
 
 * [Installation from PyPI.org][1]
 * [Installation from BioConda][2]
 * [Installation for the AWS Cloud Shell][3]
 * [Installation for the GCP Cloud Shell][4]
 
+
+Publication:
+------------
+
+Camacho C, Boratyn GM, Joukov V, Vera Alvarez R, Madden TL. ElasticBLAST: accelerating sequence search via cloud computing. BMC Bioinformatics. 2023 Mar 26;24(1):117. doi: [10.1186/s12859-023-05245-9](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-023-05245-9). PMID: [36967390](https://pubmed.ncbi.nlm.nih.gov/36967390/); PMCID: [PMC10040096](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10040096/).
+
+
 Developer information
 ---------------------
 
 ### How to build ElasticBLAST
 
     make elastic-blast
```

### Comparing `elastic_blast-1.0.0/src/elastic_blast.egg-info/SOURCES.txt` & `elastic_blast-1.1.0/src/elastic_blast.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 share/test/job-get-blast-version.yaml
 share/test/job-show-blastdbs.yaml
 share/test/job-show-queries.yaml
 share/test/pd-scalability-tests.sh
 share/test/sanity-check-pdbnt-search-local-unsplit-query-vs-elastic-blast.sh
 share/test/sanity-check-pdbnt-search-local-vs-elastic-blast.sh
 share/test/show-get-available-blastdb.yaml
+share/test/test-k8s-versions.sh
 share/tools/aws-create-instance-with-custom-instance-profile.sh
 share/tools/aws-delete-instance-with-custom-instance-profile.sh
 share/tools/aws-elastic-blast-number-of-nodes.sh
 share/tools/aws-list-az.sh
 share/tools/aws-list-vpc.sh
 share/tools/aws-policy-create.sh
 share/tools/aws-policy-delete.sh
```

