# Comparing `tmp/jupyter_ai-0.6.1.tar.gz` & `tmp/jupyter_ai-0.7.0.tar.gz`

## Comparing `jupyter_ai-0.6.1.tar` & `jupyter_ai-0.7.0.tar`

### file list

```diff
@@ -1,157 +1,163 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/.eslintignore
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/.eslintrc.js
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/.stylelintrc
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/CHANGELOG.md
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/babel.config.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/conftest.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jest.config.js
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/package.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/project.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/setup.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/tsconfig.json
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter-config/nb-config/jupyter_ai.json
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter-config/server-config/jupyter_ai.json
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/_version.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/engine.py
--rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/extension.py
--rw-r--r--   0        0        0     8094 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/handlers.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/models.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/reply_processor.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/task_manager.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/tasks.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/actors/__init__.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/actors/ask.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/actors/base.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/actors/default.py
--rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/actors/generate.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/actors/learn.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/actors/memory.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/actors/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/document_loaders/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/document_loaders/directory.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/document_loaders/splitter.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/package.json
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json
--rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf
--rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf
--rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2
--rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf
--rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff
--rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf
--rw-r--r--   0        0        0    79896 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/165.9dda3cd58dc434a135e2.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/165.9dda3cd58dc434a135e2.js.LICENSE.txt
--rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf
--rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf
--rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf
--rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/296.bda9232f6e5ca4db8f1c.js
--rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff
--rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf
--rw-r--r--   0        0        0     7566 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/465.d994a7f1c5808a09fbe5.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/465.d994a7f1c5808a09fbe5.js.LICENSE.txt
--rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/560.2fa7b4ae7a0d43e8eb1f.js
--rw-r--r--   0        0        0   468858 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/586.d8af1e48008aba81c9a4.js
--rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff
--rw-r--r--   0        0        0   460651 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/641.55df6eadf8891e5a1bbe.js
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/641.55df6eadf8891e5a1bbe.js.LICENSE.txt
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/643.3e00b12acf02dce55cc2.js
--rw-r--r--   0        0        0   157416 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/673.68e7ac52ccd7076d341f.js
--rw-r--r--   0        0        0    40847 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/675.73a31f502181054c8492.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/675.73a31f502181054c8492.js.LICENSE.txt
--rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf
--rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2
--rw-r--r--   0        0        0    34117 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/698.db0bf7bc349a78b068d5.js
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/698.db0bf7bc349a78b068d5.js.LICENSE.txt
--rw-r--r--   0        0        0     9714 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/703.d52ed379ae2e07ba3d54.js
--rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/710.92355af1c50cee7b836f.js
--rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/785.89e5ffc932d4302b02fa.js
--rw-r--r--   0        0        0    15490 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/787.7f6980b88a058f8d58c8.js
--rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2
--rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff
--rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff
--rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf
--rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff
--rw-r--r--   0        0        0    11076 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/92.8c406c1018e3357f19d8.js
--rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf
--rw-r--r--   0        0        0   157436 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/964.1d210ce1e570332cead5.js
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2
--rw-r--r--   0        0        0  1568187 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/990.ef9212deeffc976b3352.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/990.ef9212deeffc976b3352.js.LICENSE.txt
--rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff
--rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf
--rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff
--rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2
--rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff
--rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf
--rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff
--rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2
--rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff
--rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2
--rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff
--rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf
--rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf
--rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff
--rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf
--rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf
--rw-r--r--   0        0        0    11544 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/remoteEntry.585abad92d66f32304a2.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/style.js
--rw-r--r--   0        0        0   114416 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/tests/__init__.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/tests/test_handlers.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/schema/plugin.json
--rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/chat_handler.ts
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/handler.ts
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/icons.ts
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/index.ts
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/inserter.ts
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/selection-watcher.ts
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/theme-provider.ts
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/utils.ts
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/__tests__/jupyter_gai.spec.ts
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/__tests__/widgets/closable-dialog.spec.tsx
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/components/chat-code-view.tsx
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/components/chat-input.tsx
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/components/chat-messages.tsx
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/components/chat.tsx
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/components/expandable-text-field.tsx
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/components/jl-theme-provider.tsx
--rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/components/open-task-dialog.tsx
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/components/scroll-container.tsx
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/contexts/collaborators-context.tsx
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/contexts/selection-context.tsx
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/types/mui.d.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/types/svg.d.ts
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/widgets/chat-error.tsx
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/widgets/chat-sidebar.tsx
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/widgets/closable-dialog.tsx
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/style/base.css
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/style/expandable-text-field.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/style/index.js
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/style/react-markdown.css
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/style/icons/chat.svg
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/style/icons/psychology.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/ui-tests/tests/jupyter_ai.spec.ts
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/LICENSE
--rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/README.md
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     8337 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/.eslintignore
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/.eslintrc.js
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/.stylelintrc
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/babel.config.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/conftest.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jest.config.js
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/package.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/project.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/setup.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/tsconfig.json
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter-config/nb-config/jupyter_ai.json
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter-config/server-config/jupyter_ai.json
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/_version.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/engine.py
+-rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/extension.py
+-rw-r--r--   0        0        0    11067 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/handlers.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/models.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/reply_processor.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/task_manager.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/tasks.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/actors/__init__.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/actors/ask.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/actors/base.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/actors/chat_provider.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/actors/config.py
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/actors/default.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/actors/embeddings_provider.py
+-rw-r--r--   0        0        0     9042 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/actors/generate.py
+-rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/actors/learn.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/actors/memory.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/actors/providers.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/actors/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/document_loaders/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/document_loaders/directory.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/document_loaders/splitter.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/package.json
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json
+-rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf
+-rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf
+-rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2
+-rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf
+-rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff
+-rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf
+-rw-r--r--   0        0        0    79896 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/165.9dda3cd58dc434a135e2.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/165.9dda3cd58dc434a135e2.js.LICENSE.txt
+-rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf
+-rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf
+-rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf
+-rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/296.bda9232f6e5ca4db8f1c.js
+-rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff
+-rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf
+-rw-r--r--   0        0        0   157511 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/460.1a227a7f70bb8e160091.js
+-rw-r--r--   0        0        0     7566 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/465.d994a7f1c5808a09fbe5.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/465.d994a7f1c5808a09fbe5.js.LICENSE.txt
+-rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/560.2fa7b4ae7a0d43e8eb1f.js
+-rw-r--r--   0        0        0   468858 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/586.d8af1e48008aba81c9a4.js
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff
+-rw-r--r--   0        0        0    22475 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/639.ba44eea9c8de7134d76e.js
+-rw-r--r--   0        0        0   460651 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/641.55df6eadf8891e5a1bbe.js
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/641.55df6eadf8891e5a1bbe.js.LICENSE.txt
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/643.d05f12a52798d8475b12.js
+-rw-r--r--   0        0        0    40847 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/675.73a31f502181054c8492.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/675.73a31f502181054c8492.js.LICENSE.txt
+-rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2
+-rw-r--r--   0        0        0    34117 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/698.db0bf7bc349a78b068d5.js
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/698.db0bf7bc349a78b068d5.js.LICENSE.txt
+-rw-r--r--   0        0        0     9714 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/703.d52ed379ae2e07ba3d54.js
+-rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/710.92355af1c50cee7b836f.js
+-rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/785.89e5ffc932d4302b02fa.js
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2
+-rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff
+-rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff
+-rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf
+-rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff
+-rw-r--r--   0        0        0    11076 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/92.8c406c1018e3357f19d8.js
+-rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf
+-rw-r--r--   0        0        0   157436 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/964.1d210ce1e570332cead5.js
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2
+-rw-r--r--   0        0        0  1568187 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/990.ef9212deeffc976b3352.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/990.ef9212deeffc976b3352.js.LICENSE.txt
+-rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff
+-rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf
+-rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff
+-rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2
+-rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff
+-rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf
+-rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff
+-rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2
+-rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff
+-rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2
+-rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff
+-rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf
+-rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf
+-rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff
+-rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf
+-rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf
+-rw-r--r--   0        0        0    11544 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/remoteEntry.a041aa160809d9fa05d2.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/style.js
+-rw-r--r--   0        0        0   114416 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/tests/__init__.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/jupyter_ai/tests/test_handlers.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/schema/plugin.json
+-rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/chat_handler.ts
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/handler.ts
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/icons.ts
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/index.ts
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/inserter.ts
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/selection-watcher.ts
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/theme-provider.ts
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/utils.ts
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/__tests__/jupyter_gai.spec.ts
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/__tests__/widgets/closable-dialog.spec.tsx
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/components/chat-code-view.tsx
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/components/chat-input.tsx
+-rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/components/chat-messages.tsx
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/components/chat-settings.tsx
+-rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/components/chat.tsx
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/components/expandable-text-field.tsx
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/components/jl-theme-provider.tsx
+-rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/components/open-task-dialog.tsx
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/components/scroll-container.tsx
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/components/select.tsx
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/contexts/collaborators-context.tsx
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/contexts/selection-context.tsx
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/types/mui.d.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/types/svg.d.ts
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/widgets/chat-error.tsx
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/widgets/chat-sidebar.tsx
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/src/widgets/closable-dialog.tsx
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/style/base.css
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/style/expandable-text-field.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/style/index.js
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/style/react-markdown.css
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/style/icons/chat.svg
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/style/icons/jupyternaut.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/ui-tests/tests/jupyter_ai.spec.ts
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/README.md
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     9421 2020-02-02 00:00:00.000000 jupyter_ai-0.7.0/PKG-INFO
```

### Comparing `jupyter_ai-0.6.1/.eslintrc.js` & `jupyter_ai-0.7.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/RELEASE.md` & `jupyter_ai-0.7.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jest.config.js` & `jupyter_ai-0.7.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/package.json` & `jupyter_ai-0.7.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.7.0'"}*

```diff
@@ -122,9 +122,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.6.1"
+    "version": "0.7.0"
 }
```

### Comparing `jupyter_ai-0.6.1/tsconfig.json` & `jupyter_ai-0.7.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/__init__.py` & `jupyter_ai-0.7.0/jupyter_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/engine.py` & `jupyter_ai-0.7.0/jupyter_ai/engine.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/extension.py` & `jupyter_ai-0.7.0/jupyter_ai/extension.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,57 @@
 import asyncio
-import os
-import queue
+
+from jupyter_ai.actors.chat_provider import ChatProviderActor
+from jupyter_ai.actors.config import ConfigActor
+from jupyter_ai.actors.embeddings_provider import EmbeddingsProviderActor
+from jupyter_ai.actors.providers import ProvidersActor
+
+from jupyter_ai_magics.utils import load_providers
+
 from langchain.memory import ConversationBufferWindowMemory
 from jupyter_ai.actors.default import DefaultActor 
 from jupyter_ai.actors.ask import AskActor 
 from jupyter_ai.actors.learn import LearnActor
 from jupyter_ai.actors.router import Router
 from jupyter_ai.actors.memory import MemoryActor
 from jupyter_ai.actors.generate import GenerateActor
 from jupyter_ai.actors.base import ACTOR_TYPE
 from jupyter_ai.reply_processor import ReplyProcessor
 from jupyter_server.extension.application import ExtensionApp
-from .handlers import ChatHandler, ChatHistoryHandler, PromptAPIHandler, TaskAPIHandler
+
+from .handlers import (
+    ChatHandler, 
+    ChatHistoryHandler, 
+    EmbeddingsModelProviderHandler, 
+    ModelProviderHandler, 
+    PromptAPIHandler, 
+    TaskAPIHandler,
+    GlobalConfigHandler
+)
+
 from importlib_metadata import entry_points
 import inspect
 from .engine import BaseModelEngine
-from jupyter_ai_magics.providers import ChatOpenAINewProvider, ChatOpenAIProvider
 
 import ray
 from ray.util.queue import Queue
+from jupyter_ai_magics.utils import load_providers
 
 
 class AiExtension(ExtensionApp):
     name = "jupyter_ai"
     handlers = [
+        ("api/ai/config", GlobalConfigHandler),
         ("api/ai/prompt", PromptAPIHandler),
         (r"api/ai/tasks/?", TaskAPIHandler),
         (r"api/ai/tasks/([\w\-:]*)", TaskAPIHandler),
         (r"api/ai/chats/?", ChatHandler),
         (r"api/ai/chats/history?", ChatHistoryHandler),
+        (r"api/ai/providers?", ModelProviderHandler),
+        (r"api/ai/providers/embeddings?", EmbeddingsModelProviderHandler),
     ]
 
     @property
     def ai_engines(self): 
         if "ai_engines" not in self.settings:
             self.settings["ai_engines"] = {}
 
@@ -87,64 +106,79 @@
                 continue
             
             default_tasks += module_default_tasks
 
         self.settings["ai_default_tasks"] = default_tasks
         self.log.info("Registered all default tasks.")
 
-        if ChatOpenAINewProvider.auth_strategy.name not in os.environ:
-            raise EnvironmentError(f"`{ChatOpenAINewProvider.auth_strategy.name}` value not set in environment. For chat to work, this value should be provided.")
-
-        ## load OpenAI provider
-        self.settings["openai_chat"] = ChatOpenAIProvider(model_id="gpt-3.5-turbo")
+        providers = load_providers(log=self.log)
+        self.settings["chat_providers"] = providers
+        self.log.info("Registered providers.")
 
         self.log.info(f"Registered {self.name} server extension")
 
-        # Add a message queue to the settings to be used by the chat handler
-        self.settings["chat_message_queue"] = queue.Queue()
-
         # Store chat clients in a dictionary
         self.settings["chat_clients"] = {}
         self.settings["chat_handlers"] = {}
         
         # store chat messages in memory for now
+        # this is only used to render the UI, and is not the conversational
+        # memory object used by the LM chain.
         self.settings["chat_history"] = []
 
 
         reply_queue = Queue()
         self.settings["reply_queue"] = reply_queue
 
-        router = Router.options(name="router").remote(
+        router = Router.options(name=ACTOR_TYPE.ROUTER).remote(
             reply_queue=reply_queue,
-            log=self.log
+            log=self.log,
         )
         default_actor = DefaultActor.options(name=ACTOR_TYPE.DEFAULT.value).remote(
             reply_queue=reply_queue, 
-            log=self.log
+            log=self.log,
+            chat_history=self.settings["chat_history"]
+        )
+
+        providers_actor = ProvidersActor.options(name=ACTOR_TYPE.PROVIDERS.value).remote(
+            log=self.log,
+        )
+        config_actor = ConfigActor.options(name=ACTOR_TYPE.CONFIG.value).remote(
+            log=self.log,
+        )
+        chat_provider_actor = ChatProviderActor.options(name=ACTOR_TYPE.CHAT_PROVIDER.value).remote(
+            log=self.log,
+        )
+        embeddings_provider_actor = EmbeddingsProviderActor.options(name=ACTOR_TYPE.EMBEDDINGS_PROVIDER.value).remote(
+            log=self.log,
         )
         learn_actor = LearnActor.options(name=ACTOR_TYPE.LEARN.value).remote(
             reply_queue=reply_queue,
             log=self.log,
             root_dir=self.serverapp.root_dir,
         )
         ask_actor = AskActor.options(name=ACTOR_TYPE.ASK.value).remote(
             reply_queue=reply_queue, 
-            log=self.log
+            log=self.log,
         )
         memory_actor = MemoryActor.options(name=ACTOR_TYPE.MEMORY.value).remote(
             log=self.log,
-            memory=ConversationBufferWindowMemory(return_messages=True, k=2)
+            memory=ConversationBufferWindowMemory(return_messages=True, k=2),
         )
         generate_actor = GenerateActor.options(name=ACTOR_TYPE.GENERATE.value).remote(
             reply_queue=reply_queue, 
             log=self.log,
-            root_dir=self.settings['server_root_dir']
+            root_dir=self.settings['server_root_dir'],
         )
      
         self.settings['router'] = router
+        self.settings['providers_actor'] = providers_actor
+        self.settings['config_actor'] = config_actor
+        self.settings['chat_provider_actor'] = chat_provider_actor
+        self.settings['embeddings_provider_actor'] = embeddings_provider_actor
         self.settings["default_actor"] = default_actor
         self.settings["learn_actor"] = learn_actor
         self.settings["ask_actor"] = ask_actor
         self.settings["memory_actor"] = memory_actor
         self.settings["generate_actor"] = generate_actor
 
         reply_processor = ReplyProcessor(self.settings['chat_handlers'], reply_queue, log=self.log)
```

### Comparing `jupyter_ai-0.6.1/jupyter_ai/models.py` & `jupyter_ai-0.7.0/jupyter_ai/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,36 @@
+from jupyter_ai_magics.providers import AuthStrategy
+
 from pydantic import BaseModel 
 from typing import Dict, List, Union, Literal, Optional
 
 class PromptRequest(BaseModel):
     task_id: str
     engine_id: str
     prompt_variables: Dict[str, str]
 
 # the type of message used to chat with the agent
 class ChatRequest(BaseModel):
     prompt: str
 
-class ChatClient(BaseModel):
-    # Client ID assigned by us. Necessary because different JupyterLab clients
-    # on the same device (i.e. running on multiple tabs/windows) may have the
-    # same user ID assigned to them by IdentityProvider.
-    id: str
+class ChatUser(BaseModel):
     # User ID assigned by IdentityProvider.
     username: str
     initials: str
     name: str
     display_name: str
     color: Optional[str]
     avatar_url: Optional[str]
 
+class ChatClient(ChatUser):
+    # A unique client ID assigned to identify different JupyterLab clients on
+    # the same device (i.e. running on multiple tabs/windows), which may have
+    # the same username assigned to them by the IdentityProvider.
+    id: str
+
 class AgentChatMessage(BaseModel):
     type: Literal["agent"] = "agent"
     id: str
     time: float
     body: str
     # message ID of the HumanChatMessage it is replying to
     reply_to: str
@@ -74,7 +78,32 @@
     insertion_mode: str
     prompt_template: str
     engines: List[ListEnginesEntry]
 
 class ChatHistory(BaseModel):
     """History of chat messages"""
     messages: List[ChatMessage]
+
+
+class ListProvidersEntry(BaseModel):
+    """Model provider with supported models
+    and provider's authentication strategy
+    """
+    id: str
+    name: str
+    models: List[str]
+    auth_strategy: AuthStrategy
+
+
+class ListProvidersResponse(BaseModel):
+    providers: List[ListProvidersEntry]
+
+class IndexedDir(BaseModel):
+    path: str
+
+class IndexMetadata(BaseModel):
+    dirs: List[IndexedDir]
+
+class GlobalConfig(BaseModel):
+    model_provider_id: Optional[str] = None
+    embeddings_provider_id: Optional[str] = None
+    api_keys: Dict[str, str] = {}
```

### Comparing `jupyter_ai-0.6.1/jupyter_ai/reply_processor.py` & `jupyter_ai-0.7.0/jupyter_ai/reply_processor.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/task_manager.py` & `jupyter_ai-0.7.0/jupyter_ai/task_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/tasks.py` & `jupyter_ai-0.7.0/jupyter_ai/tasks.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/actors/ask.py` & `jupyter_ai-0.7.0/jupyter_ai/actors/ask.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import argparse
+from typing import Dict, List, Type
+from jupyter_ai_magics.providers import BaseProvider
 
 import ray
 from ray.util.queue import Queue
 
-from langchain import OpenAI
 from langchain.chains import ConversationalRetrievalChain
+from langchain.schema import BaseRetriever, Document
 
 from jupyter_ai.models import HumanChatMessage
 from jupyter_ai.actors.base import ACTOR_TYPE, BaseActor, Logger
 
 
 @ray.remote
 class AskActor(BaseActor):
@@ -17,42 +19,60 @@
     follows the Retrieval and Generation (RAG) tehnique to
     query the documents from the index, and sends this context
     to the LLM to generate the final reply.
     """
 
     def __init__(self, reply_queue: Queue, log: Logger):
         super().__init__(reply_queue=reply_queue, log=log)
-        index_actor = ray.get_actor(ACTOR_TYPE.LEARN.value)
-        handle = index_actor.get_index.remote()
-        vectorstore = ray.get(handle)
-        if not vectorstore:
-            return
-
-        self.chat_history = []
-        self.chat_provider = ConversationalRetrievalChain.from_llm(
-            OpenAI(temperature=0, verbose=True),
-            vectorstore.as_retriever()
-        )
 
         self.parser.prog = '/ask'
         self.parser.add_argument('query', nargs=argparse.REMAINDER)
 
+    def create_llm_chain(self, provider: Type[BaseProvider], provider_params: Dict[str, str]):
+        retriever = Retriever()
+        self.llm = provider(**provider_params)
+        self.chat_history = []
+        self.llm_chain = ConversationalRetrievalChain.from_llm(
+            self.llm,
+            retriever
+        )
 
     def _process_message(self, message: HumanChatMessage):
         args = self.parse_args(message)
         if args is None:
             return
         query = ' '.join(args.query)
         if not query:
             self.reply(f"{self.parser.format_usage()}", message)
             return
         
+        self.get_llm_chain()
+
+        try:
+            result = self.llm_chain({"question": query, "chat_history": self.chat_history})
+            response = result['answer']
+            self.chat_history.append((query, response))
+            self.reply(response, message)
+        except AssertionError as e:
+            self.log.error(e)
+            response = """Sorry, an error occurred while reading the from the learned documents. 
+            If you have changed the embedding provider, try deleting the existing index by running 
+            `/learn -d` command and then re-submitting the `learn <directory>` to learn the documents,
+            and then asking the question again.
+            """
+            self.reply(response, message)
+
+
+class Retriever(BaseRetriever):
+    """Wrapper retriever class to get relevant docs
+    from the vector store, this is important because
+    of inconsistent de-serialization of index when it's
+    accessed directly from the ask actor.
+    """
+    
+    def get_relevant_documents(self, question: str):
         index_actor = ray.get_actor(ACTOR_TYPE.LEARN.value)
-        handle = index_actor.get_index.remote()
-        vectorstore = ray.get(handle)
-        # Have to reference the latest index
-        self.chat_provider.retriever = vectorstore.as_retriever()
-        
-        result = self.chat_provider({"question": query, "chat_history": self.chat_history})
-        response = result['answer']
-        self.chat_history.append((query, response))
-        self.reply(response, message)
+        docs = ray.get(index_actor.get_relevant_documents.remote(question))
+        return docs
+    
+    async def aget_relevant_documents(self, query: str) -> List[Document]:
+        return await super().aget_relevant_documents(query)
```

### Comparing `jupyter_ai-0.6.1/jupyter_ai/actors/generate.py` & `jupyter_ai-0.7.0/jupyter_ai/actors/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import json
 import os
-import time
-from uuid import uuid4
+from typing import Dict, Type
 
 import ray
 from ray.util.queue import Queue
 
 from langchain.llms import BaseLLM
-from langchain.chat_models import ChatOpenAI
 from langchain.prompts import PromptTemplate
 from langchain.llms import BaseLLM
 from langchain.chains import LLMChain
 
 import nbformat
 
-from jupyter_ai.models import AgentChatMessage, HumanChatMessage
+from jupyter_ai.models import HumanChatMessage
 from jupyter_ai.actors.base import BaseActor, Logger
-from jupyter_ai_magics.providers import ChatOpenAINewProvider
+from jupyter_ai_magics.providers import BaseProvider, ChatOpenAINewProvider
 
 schema = """{
   "$schema": "http://json-schema.org/draft-07/schema#",
   "type": "object",
   "properties": {
     "description": {
       "type": "string"
@@ -63,16 +61,14 @@
                 "schema"
             ],
         )
         return cls(prompt=prompt, llm=llm, verbose=verbose)
 
 def generate_outline(description, llm=None, verbose=False):
     """Generate an outline of sections given a description of a notebook."""
-    if llm is None:
-        llm = ChatOpenAINewProvider(model_id='gpt-3.5-turbo')
     chain = NotebookOutlineChain.from_llm(llm=llm, verbose=verbose)
     outline = chain.predict(description=description, schema=schema)
     return json.loads(outline)
 
 class CodeImproverChain(LLMChain):
     """Chain to improve source code."""
 
@@ -121,16 +117,14 @@
                 "code_so_far"
             ],
         )
         return cls(prompt=prompt, llm=llm, verbose=verbose)
 
 def generate_code(outline, llm=None, verbose=False):
     """Generate source code for a section given a description of the notebook and section."""
-    if llm is None:
-        llm = ChatOpenAINewProvider(model_id='gpt-3.5-turbo')
     chain = NotebookSectionCodeChain.from_llm(llm=llm, verbose=verbose)
     code_so_far = []
     for section in outline['sections']:
         code = chain.predict(
             description=outline['description'],
             title=section['title'],
             content=section['content'],
@@ -173,16 +167,14 @@
                 "content",
             ],
         )
         return cls(prompt=prompt, llm=llm, verbose=verbose)
 
 def generate_title_and_summary(outline, llm=None, verbose=False):
     """Generate a title and summary of a notebook outline using an LLM."""
-    if llm is None:
-        llm = ChatOpenAINewProvider(model_id='gpt-3.5-turbo')
     summary_chain = NotebookSummaryChain.from_llm(llm=llm, verbose=verbose)
     title_chain = NotebookTitleChain.from_llm(llm=llm, verbose=verbose)
     summary = summary_chain.predict(content=outline)
     title = title_chain.predict(content=outline)
     outline['summary'] = summary
     outline['title'] = title.strip('"')
     return outline
@@ -206,17 +198,24 @@
 @ray.remote
 class GenerateActor(BaseActor):
     """A Ray actor to generate a Jupyter notebook given a description."""
 
     def __init__(self, reply_queue: Queue, root_dir: str, log: Logger):
         super().__init__(log=log, reply_queue=reply_queue)
         self.root_dir = os.path.abspath(os.path.expanduser(root_dir))
-        self.llm = ChatOpenAINewProvider(model_id='gpt-3.5-turbo')
+        self.llm = None
+
+    def create_llm_chain(self, provider: Type[BaseProvider], provider_params: Dict[str, str]):
+        llm = provider(**provider_params)
+        self.llm = llm
+        return llm
   
     def _process_message(self, message: HumanChatMessage):
+        self.get_llm_chain()
+        
         response = "👍 Great, I will get started on your notebook. It may take a few minutes, but I will reply here when the notebook is ready. In the meantime, you can continue to ask me other questions."
         self.reply(response, message)
 
         prompt = message.body
         outline = generate_outline(prompt, llm=self.llm, verbose=True)
         # Save the user input prompt, the description property is now LLM generated.
         outline['prompt'] = prompt
```

### Comparing `jupyter_ai-0.6.1/jupyter_ai/actors/memory.py` & `jupyter_ai-0.7.0/jupyter_ai/actors/memory.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/actors/router.py` & `jupyter_ai-0.7.0/jupyter_ai/actors/router.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import ray
 from ray.util.queue import Queue
 
 from jupyter_ai.actors.base import ACTOR_TYPE, COMMANDS, Logger, BaseActor
-from jupyter_ai.models import ClearMessage
 
 @ray.remote
 class Router(BaseActor):
     def __init__(self, reply_queue: Queue, log: Logger):
         """Routes messages to the correct actor.
         
         To register new actors, add the actor type in the `ACTOR_TYPE` enum and 
@@ -21,11 +20,11 @@
 
         if message.body.startswith("/"):
             command = message.body.split(' ', 1)[0]
             if command in COMMANDS.keys():
                 actor = ray.get_actor(COMMANDS[command].value)
                 actor.process_message.remote(message)
             if command == '/clear':
-                reply_message = ClearMessage()
-                self.reply_queue.put(reply_message)
+                actor = ray.get_actor(ACTOR_TYPE.DEFAULT)
+                actor.clear_memory.remote()
         else:
             default.process_message.remote(message)
```

### Comparing `jupyter_ai-0.6.1/jupyter_ai/document_loaders/directory.py` & `jupyter_ai-0.7.0/jupyter_ai/document_loaders/directory.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/document_loaders/splitter.py` & `jupyter_ai-0.7.0/jupyter_ai/document_loaders/splitter.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/package.json` & `jupyter_ai-0.7.0/jupyter_ai/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745833333333334%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.a041aa160809d9fa05d2.js'}}",*

 * * "'version'": "'0.7.0'"}*

```diff
@@ -60,15 +60,15 @@
         "schema/*.json",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter-ai",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.585abad92d66f32304a2.js",
+            "load": "static/remoteEntry.a041aa160809d9fa05d2.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_ai"
                 },
@@ -127,9 +127,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.6.1"
+    "version": "0.7.0"
 }
```

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig` & `jupyter_ai-0.7.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.7.0'"}*

```diff
@@ -122,9 +122,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.6.1"
+    "version": "0.7.0"
 }
```

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json` & `jupyter_ai-0.7.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'jupyter.lab.setting-icon'": "'jupyter-ai::chat'"}*

```diff
@@ -26,15 +26,15 @@
                 "command": "ai:generate-from-editor-selection",
                 "name": "ai:generate-from-editor-selection",
                 "rank": 520,
                 "selector": ".jp-FileEditor"
             }
         ]
     },
-    "jupyter.lab.setting-icon": "jupyter-ai::psychology",
+    "jupyter.lab.setting-icon": "jupyter-ai::chat",
     "jupyter.lab.setting-icon-label": "Jupyter AI Chat",
     "jupyter.lab.toolbars": {
         "Cell": [
             {
                 "command": "ai:explain-or-codify-cell",
                 "name": "ai:explain-or-codify-cell",
                 "rank": 10
```

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/165.9dda3cd58dc434a135e2.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/165.9dda3cd58dc434a135e2.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/296.bda9232f6e5ca4db8f1c.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/296.bda9232f6e5ca4db8f1c.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/465.d994a7f1c5808a09fbe5.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/465.d994a7f1c5808a09fbe5.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/586.d8af1e48008aba81c9a4.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/586.d8af1e48008aba81c9a4.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/641.55df6eadf8891e5a1bbe.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/641.55df6eadf8891e5a1bbe.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/643.3e00b12acf02dce55cc2.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/643.d05f12a52798d8475b12.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -2,203 +2,203 @@
 (self.webpackChunk_jupyter_ai_core = self.webpackChunk_jupyter_ai_core || []).push([
     [643], {
         61246: (e, n, t) => {
             t.d(n, {
                 Z: () => s
             });
             var r = t(82609),
-                a = t.n(r),
-                i = t(83055),
-                o = t(98814),
-                c = a()((function(e) {
+                i = t.n(r),
+                o = t(83055),
+                a = t(98814),
+                c = i()((function(e) {
                     return e[1]
                 }));
-            c.i(i.Z), c.i(o.Z), c.push([e.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/", ""]);
+            c.i(o.Z), c.i(a.Z), c.push([e.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/", ""]);
             const s = c
         },
         83055: (e, n, t) => {
             t.d(n, {
-                Z: () => i
+                Z: () => o
             });
             var r = t(82609),
-                a = t.n(r)()((function(e) {
+                i = t.n(r)()((function(e) {
                     return e[1]
                 }));
-            a.push([e.id, ".jp-ai-ExpandableTextField-label {\n  font-size: var(--jp-ui-font-size0);\n}\n\n.jp-ai-ExpandableTextField-value {\n  font-size: var(--jp-ui-font-size1);\n}\n\n.jp-ai-ExpandableTextField-value-collapsed {\n  white-space: nowrap;\n  text-overflow: ellipsis;\n  width: 100%;\n  display: block;\n  overflow: hidden;\n}\n\n.jp-ai-ExpandableTextField-value-expanded {\n  text-overflow: none;\n  overflow: visible;\n  height: auto;\n}\n", ""]);
-            const i = a
+            i.push([e.id, ".jp-ai-ExpandableTextField-label {\n  font-size: var(--jp-ui-font-size0);\n}\n\n.jp-ai-ExpandableTextField-value {\n  font-size: var(--jp-ui-font-size1);\n}\n\n.jp-ai-ExpandableTextField-value-collapsed {\n  white-space: nowrap;\n  text-overflow: ellipsis;\n  width: 100%;\n  display: block;\n  overflow: hidden;\n}\n\n.jp-ai-ExpandableTextField-value-expanded {\n  text-overflow: none;\n  overflow: visible;\n  height: auto;\n}\n", ""]);
+            const o = i
         },
         98814: (e, n, t) => {
             t.d(n, {
-                Z: () => i
+                Z: () => o
             });
             var r = t(82609),
-                a = t.n(r)()((function(e) {
+                i = t.n(r)()((function(e) {
                     return e[1]
                 }));
-            a.push([e.id, ".jp-RenderedHTMLCommon.jp-ai-react-markdown > pre {\n    margin: 0px;\n}\n\n.jp-RenderedHTMLCommon.jp-ai-react-markdown {\n    padding: 0px;\n}", ""]);
-            const i = a
+            i.push([e.id, ".jp-RenderedHTMLCommon.jp-ai-react-markdown > pre {\n  margin: 0;\n}\n\n.jp-RenderedHTMLCommon.jp-ai-react-markdown {\n  padding: 0;\n}\n\n/* !important specifier required to override inline styles from Prism */\n.jp-ai-code {\n  font-family: var(--jp-code-font-family) !important;\n  font-size: var(--jp-code-font-size) !important;\n  line-height: var(--jp-code-line-height) !important;\n}\n", ""]);
+            const o = i
         },
         82609: e => {
             e.exports = function(e) {
                 var n = [];
                 return n.toString = function() {
                     return this.map((function(n) {
                         var t = e(n);
                         return n[2] ? "@media ".concat(n[2], " {").concat(t, "}") : t
                     })).join("")
                 }, n.i = function(e, t, r) {
                     "string" == typeof e && (e = [
                         [null, e, ""]
                     ]);
-                    var a = {};
+                    var i = {};
                     if (r)
-                        for (var i = 0; i < this.length; i++) {
-                            var o = this[i][0];
-                            null != o && (a[o] = !0)
+                        for (var o = 0; o < this.length; o++) {
+                            var a = this[o][0];
+                            null != a && (i[a] = !0)
                         }
                     for (var c = 0; c < e.length; c++) {
                         var s = [].concat(e[c]);
-                        r && a[s[0]] || (t && (s[2] ? s[2] = "".concat(t, " and ").concat(s[2]) : s[2] = t), n.push(s))
+                        r && i[s[0]] || (t && (s[2] ? s[2] = "".concat(t, " and ").concat(s[2]) : s[2] = t), n.push(s))
                     }
                 }, n
             }
         },
         46062: (e, n, t) => {
-            var r, a = function() {
+            var r, i = function() {
                     var e = {};
                     return function(n) {
                         if (void 0 === e[n]) {
                             var t = document.querySelector(n);
                             if (window.HTMLIFrameElement && t instanceof window.HTMLIFrameElement) try {
                                 t = t.contentDocument.head
                             } catch (e) {
                                 t = null
                             }
                             e[n] = t
                         }
                         return e[n]
                     }
                 }(),
-                i = [];
+                o = [];
 
-            function o(e) {
-                for (var n = -1, t = 0; t < i.length; t++)
-                    if (i[t].identifier === e) {
+            function a(e) {
+                for (var n = -1, t = 0; t < o.length; t++)
+                    if (o[t].identifier === e) {
                         n = t;
                         break
                     } return n
             }
 
             function c(e, n) {
-                for (var t = {}, r = [], a = 0; a < e.length; a++) {
-                    var c = e[a],
+                for (var t = {}, r = [], i = 0; i < e.length; i++) {
+                    var c = e[i],
                         s = n.base ? c[0] + n.base : c[0],
                         l = t[s] || 0,
-                        u = "".concat(s, " ").concat(l);
+                        d = "".concat(s, " ").concat(l);
                     t[s] = l + 1;
-                    var d = o(u),
+                    var u = a(d),
                         f = {
                             css: c[1],
                             media: c[2],
                             sourceMap: c[3]
-                        }; - 1 !== d ? (i[d].references++, i[d].updater(f)) : i.push({
-                        identifier: u,
+                        }; - 1 !== u ? (o[u].references++, o[u].updater(f)) : o.push({
+                        identifier: d,
                         updater: h(f, n),
                         references: 1
-                    }), r.push(u)
+                    }), r.push(d)
                 }
                 return r
             }
 
             function s(e) {
                 var n = document.createElement("style"),
                     r = e.attributes || {};
                 if (void 0 === r.nonce) {
-                    var i = t.nc;
-                    i && (r.nonce = i)
+                    var o = t.nc;
+                    o && (r.nonce = o)
                 }
                 if (Object.keys(r).forEach((function(e) {
                         n.setAttribute(e, r[e])
                     })), "function" == typeof e.insert) e.insert(n);
                 else {
-                    var o = a(e.insert || "head");
-                    if (!o) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
-                    o.appendChild(n)
+                    var a = i(e.insert || "head");
+                    if (!a) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
+                    a.appendChild(n)
                 }
                 return n
             }
-            var l, u = (l = [], function(e, n) {
+            var l, d = (l = [], function(e, n) {
                 return l[e] = n, l.filter(Boolean).join("\n")
             });
 
-            function d(e, n, t, r) {
-                var a = t ? "" : r.media ? "@media ".concat(r.media, " {").concat(r.css, "}") : r.css;
-                if (e.styleSheet) e.styleSheet.cssText = u(n, a);
+            function u(e, n, t, r) {
+                var i = t ? "" : r.media ? "@media ".concat(r.media, " {").concat(r.css, "}") : r.css;
+                if (e.styleSheet) e.styleSheet.cssText = d(n, i);
                 else {
-                    var i = document.createTextNode(a),
-                        o = e.childNodes;
-                    o[n] && e.removeChild(o[n]), o.length ? e.insertBefore(i, o[n]) : e.appendChild(i)
+                    var o = document.createTextNode(i),
+                        a = e.childNodes;
+                    a[n] && e.removeChild(a[n]), a.length ? e.insertBefore(o, a[n]) : e.appendChild(o)
                 }
             }
 
             function f(e, n, t) {
                 var r = t.css,
-                    a = t.media,
-                    i = t.sourceMap;
-                if (a ? e.setAttribute("media", a) : e.removeAttribute("media"), i && "undefined" != typeof btoa && (r += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(i)))), " */")), e.styleSheet) e.styleSheet.cssText = r;
+                    i = t.media,
+                    o = t.sourceMap;
+                if (i ? e.setAttribute("media", i) : e.removeAttribute("media"), o && "undefined" != typeof btoa && (r += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(o)))), " */")), e.styleSheet) e.styleSheet.cssText = r;
                 else {
                     for (; e.firstChild;) e.removeChild(e.firstChild);
                     e.appendChild(document.createTextNode(r))
                 }
             }
             var p = null,
                 v = 0;
 
             function h(e, n) {
-                var t, r, a;
+                var t, r, i;
                 if (n.singleton) {
-                    var i = v++;
-                    t = p || (p = s(n)), r = d.bind(null, t, i, !1), a = d.bind(null, t, i, !0)
-                } else t = s(n), r = f.bind(null, t, n), a = function() {
+                    var o = v++;
+                    t = p || (p = s(n)), r = u.bind(null, t, o, !1), i = u.bind(null, t, o, !0)
+                } else t = s(n), r = f.bind(null, t, n), i = function() {
                     ! function(e) {
                         if (null === e.parentNode) return !1;
                         e.parentNode.removeChild(e)
                     }(t)
                 };
                 return r(e),
                     function(n) {
                         if (n) {
                             if (n.css === e.css && n.media === e.media && n.sourceMap === e.sourceMap) return;
                             r(e = n)
-                        } else a()
+                        } else i()
                     }
             }
             e.exports = function(e, n) {
                 (n = n || {}).singleton || "boolean" == typeof n.singleton || (n.singleton = (void 0 === r && (r = Boolean(window && document && document.all && !window.atob)), r));
                 var t = c(e = e || [], n);
                 return function(e) {
                     if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
                         for (var r = 0; r < t.length; r++) {
-                            var a = o(t[r]);
-                            i[a].references--
+                            var i = a(t[r]);
+                            o[i].references--
                         }
                         for (var s = c(e, n), l = 0; l < t.length; l++) {
-                            var u = o(t[l]);
-                            0 === i[u].references && (i[u].updater(), i.splice(u, 1))
+                            var d = a(t[l]);
+                            0 === o[d].references && (o[d].updater(), o.splice(d, 1))
                         }
                         t = s
                     }
                 }
             }
         },
         76643: (e, n, t) => {
             t.r(n);
             var r = t(46062),
-                a = t.n(r),
-                i = t(61246);
-            a()(i.Z, {
+                i = t.n(r),
+                o = t(61246);
+            i()(o.Z, {
                 insert: "head",
                 singleton: !1
-            }), i.Z.locals
+            }), o.Z.locals
         }
     }
 ]);
```

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/673.68e7ac52ccd7076d341f.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/460.1a227a7f70bb8e160091.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
 (self.webpackChunk_jupyter_ai_core = self.webpackChunk_jupyter_ai_core || []).push([
-    [673], {
+    [460], {
         14859: A => {
             A.exports = function(A) {
                 return A && A.__esModule ? A : {
                     default: A
                 }
             }, A.exports.__esModule = !0, A.exports.default = A.exports
         },
@@ -729,38 +729,47 @@
         53868: (A, e, s) => {
             "use strict";
             s.d(e, {
                 Z: () => t
             });
             const t = s.p + "f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf"
         },
-        45275: (A, e, s) => {
+        21023: (A, e, s) => {
             "use strict";
             var t = s(14859);
             e.Z = void 0;
             var i = t(s(64938)),
                 a = s(85893),
-                o = (0, i.default)([(0, a.jsx)("path", {
-                    d: "M13 8.57c-.79 0-1.43.64-1.43 1.43s.64 1.43 1.43 1.43 1.43-.64 1.43-1.43-.64-1.43-1.43-1.43z"
-                }, "0"), (0, a.jsx)("path", {
-                    d: "M13 3C9.25 3 6.2 5.94 6.02 9.64L4.1 12.2c-.25.33-.01.8.4.8H6v3c0 1.1.9 2 2 2h1v3h7v-4.68c2.36-1.12 4-3.53 4-6.32 0-3.87-3.13-7-7-7zm3 7c0 .13-.01.26-.02.39l.83.66c.08.06.1.16.05.25l-.8 1.39c-.05.09-.16.12-.24.09l-.99-.4c-.21.16-.43.29-.67.39L14 13.83c-.01.1-.1.17-.2.17h-1.6c-.1 0-.18-.07-.2-.17l-.15-1.06c-.25-.1-.47-.23-.68-.39l-.99.4c-.09.03-.2 0-.25-.09l-.8-1.39c-.05-.08-.03-.19.05-.25l.84-.66c-.01-.13-.02-.26-.02-.39s.02-.27.04-.39l-.85-.66c-.08-.06-.1-.16-.05-.26l.8-1.38c.05-.09.15-.12.24-.09l1 .4c.2-.15.43-.29.67-.39L12 6.17c.02-.1.1-.17.2-.17h1.6c.1 0 .18.07.2.17l.15 1.06c.24.1.46.23.67.39l1-.4c.09-.03.2 0 .24.09l.8 1.38c.05.09.03.2-.05.26l-.85.66c.03.12.04.25.04.39z"
-                }, "1")], "Psychology");
+                o = (0, i.default)((0, a.jsx)("path", {
+                    d: "M20 11H7.83l5.59-5.59L12 4l-8 8 8 8 1.41-1.41L7.83 13H20v-2z"
+                }), "ArrowBack");
             e.Z = o
         },
         26307: (A, e, s) => {
             "use strict";
             var t = s(14859);
             e.Z = void 0;
             var i = t(s(64938)),
                 a = s(85893),
                 o = (0, i.default)((0, a.jsx)("path", {
                     d: "M2.01 21 23 12 2.01 3 2 10l15 2-15 2z"
                 }), "Send");
             e.Z = o
         },
+        94229: (A, e, s) => {
+            "use strict";
+            var t = s(14859);
+            e.Z = void 0;
+            var i = t(s(64938)),
+                a = s(85893),
+                o = (0, i.default)((0, a.jsx)("path", {
+                    d: "M19.14 12.94c.04-.3.06-.61.06-.94 0-.32-.02-.64-.07-.94l2.03-1.58c.18-.14.23-.41.12-.61l-1.92-3.32c-.12-.22-.37-.29-.59-.22l-2.39.96c-.5-.38-1.03-.7-1.62-.94l-.36-2.54c-.04-.24-.24-.41-.48-.41h-3.84c-.24 0-.43.17-.47.41l-.36 2.54c-.59.24-1.13.57-1.62.94l-2.39-.96c-.22-.08-.47 0-.59.22L2.74 8.87c-.12.21-.08.47.12.61l2.03 1.58c-.05.3-.09.63-.09.94s.02.64.07.94l-2.03 1.58c-.18.14-.23.41-.12.61l1.92 3.32c.12.22.37.29.59.22l2.39-.96c.5.38 1.03.7 1.62.94l.36 2.54c.05.24.24.41.48.41h3.84c.24 0 .44-.17.47-.41l.36-2.54c.59-.24 1.13-.56 1.62-.94l2.39.96c.22.08.47 0 .59-.22l1.92-3.32c.12-.22.07-.47-.12-.61l-2.01-1.58zM12 15.6c-1.98 0-3.6-1.62-3.6-3.6s1.62-3.6 3.6-3.6 3.6 1.62 3.6 3.6-1.62 3.6-3.6 3.6z"
+                }), "Settings");
+            e.Z = o
+        },
         64938: (A, e, s) => {
             "use strict";
             Object.defineProperty(e, "__esModule", {
                 value: !0
             }), Object.defineProperty(e, "default", {
                 enumerable: !0,
                 get: function() {
```

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/675.73a31f502181054c8492.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/675.73a31f502181054c8492.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/698.db0bf7bc349a78b068d5.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/698.db0bf7bc349a78b068d5.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/703.d52ed379ae2e07ba3d54.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/703.d52ed379ae2e07ba3d54.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/710.92355af1c50cee7b836f.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/710.92355af1c50cee7b836f.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/785.89e5ffc932d4302b02fa.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/785.89e5ffc932d4302b02fa.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/787.7f6980b88a058f8d58c8.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/639.ba44eea9c8de7134d76e.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -1,37 +1,40 @@
 "use strict";
 (self.webpackChunk_jupyter_ai_core = self.webpackChunk_jupyter_ai_core || []).push([
-    [787], {
-        65787: (e, t, n) => {
+    [639], {
+        11639: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => te
+                default: () => ce
             });
-            var o = n(45687),
-                r = n(35059),
-                s = n(56271),
-                i = n.n(s),
-                l = n(73033),
-                a = n(18377),
-                c = n(71893),
-                u = n(10492);
+            var r = n(45687),
+                o = n(35059),
+                i = n(56271),
+                l = n.n(i),
+                a = n(73033),
+                s = n(18377),
+                c = n(13191),
+                u = n(94229),
+                d = n(21023),
+                m = n(71893),
+                p = n(10492);
 
-            function d(e) {
+            function h(e) {
                 return getComputedStyle(document.body).getPropertyValue(e).trim()
             }
 
-            function p(e) {
-                const [t, n] = (0, s.useState)((0, c.Z)());
-                return (0, s.useEffect)((() => {
+            function g(e) {
+                const [t, n] = (0, i.useState)((0, m.Z)());
+                return (0, i.useEffect)((() => {
                     !async function() {
                         n(await async function() {
                             await async function() {
                                 for (; !document.body.hasAttribute("data-jp-theme-light");) await new Promise((e => setTimeout(e, 100)))
                             }();
                             const e = document.body.getAttribute("data-jp-theme-light");
-                            return (0, c.Z)({
+                            return (0, m.Z)({
                                 spacing: 4,
                                 components: {
                                     MuiButton: {
                                         defaultProps: {
                                             size: "small"
                                         }
                                     },
@@ -97,588 +100,796 @@
                                         defaultProps: {
                                             variant: "dense"
                                         }
                                     }
                                 },
                                 palette: {
                                     background: {
-                                        paper: d("--jp-layout-color1"),
-                                        default: d("--jp-layout-color1")
+                                        paper: h("--jp-layout-color1"),
+                                        default: h("--jp-layout-color1")
                                     },
                                     mode: "true" === e ? "light" : "dark",
                                     primary: {
-                                        main: d("--jp-brand-color1"),
-                                        light: d("--jp-brand-color2"),
-                                        dark: d("--jp-brand-color0")
+                                        main: h("--jp-brand-color1"),
+                                        light: h("--jp-brand-color2"),
+                                        dark: h("--jp-brand-color0")
                                     },
                                     error: {
-                                        main: d("--jp-error-color1"),
-                                        light: d("--jp-error-color2"),
-                                        dark: d("--jp-error-color0")
+                                        main: h("--jp-error-color1"),
+                                        light: h("--jp-error-color2"),
+                                        dark: h("--jp-error-color0")
                                     },
                                     warning: {
-                                        main: d("--jp-warn-color1"),
-                                        light: d("--jp-warn-color2"),
-                                        dark: d("--jp-warn-color0")
+                                        main: h("--jp-warn-color1"),
+                                        light: h("--jp-warn-color2"),
+                                        dark: h("--jp-warn-color0")
                                     },
                                     success: {
-                                        main: d("--jp-success-color1"),
-                                        light: d("--jp-success-color2"),
-                                        dark: d("--jp-success-color0")
+                                        main: h("--jp-success-color1"),
+                                        light: h("--jp-success-color2"),
+                                        dark: h("--jp-success-color0")
                                     },
                                     text: {
-                                        primary: d("--jp-ui-font-color1"),
-                                        secondary: d("--jp-ui-font-color2"),
-                                        disabled: d("--jp-ui-font-color3")
+                                        primary: h("--jp-ui-font-color1"),
+                                        secondary: h("--jp-ui-font-color2"),
+                                        disabled: h("--jp-ui-font-color3")
                                     }
                                 },
                                 shape: {
                                     borderRadius: 2
                                 },
                                 typography: {
-                                    fontFamily: d("--jp-ui-font-family"),
+                                    fontFamily: h("--jp-ui-font-family"),
                                     fontSize: 12,
                                     htmlFontSize: 16,
                                     button: {
                                         textTransform: "capitalize"
                                     }
                                 }
                             })
                         }())
                     }()
-                }), []), i().createElement(u.Z, {
+                }), []), l().createElement(p.Z, {
                     theme: t
                 }, e.children)
             }
-            var h, m = n(13191),
-                g = n(45275),
-                f = n(77986),
+            var f = n(77986),
                 v = n(48942),
                 y = n.n(v),
                 x = n(96707),
-                b = n.n(x),
-                w = n(40532),
-                E = n.n(w),
+                E = n.n(x),
+                b = n(40532),
+                C = n.n(b),
                 S = (n(38662), n(72647)),
-                C = n(93528);
+                _ = n(93528),
+                w = n(6277);
+            const k = "jp-ai-code";
 
             function j({
                 className: e,
                 children: t,
                 ...n
             }) {
-                return i().createElement("code", Object.assign({}, n, {
-                    className: e
+                return l().createElement("code", Object.assign({}, n, {
+                    className: (0, w.Z)(k, e)
                 }), t)
-            }! function(e) {
+            }
+            var I;
+            ! function(e) {
                 e[e.None = 0] = "None", e[e.Copying = 1] = "Copying", e[e.Copied = 2] = "Copied"
-            }(h || (h = {}));
-            const _ = {
-                [h.None]: "Copy to clipboard",
-                [h.Copying]: "Copying...",
-                [h.Copied]: "Copied!"
+            }(I || (I = {}));
+            const P = {
+                [I.None]: "Copy to clipboard",
+                [I.Copying]: "Copying...",
+                [I.Copied]: "Copied!"
             };
 
-            function k({
+            function M({
                 language: e,
                 children: t,
                 ...n
             }) {
-                const o = (0, s.useMemo)((() => String(t).replace(/\n$/, "")), [t]),
-                    [r, l] = (0, s.useState)(h.None);
-                return i().createElement(m.Box, {
+                const r = (0, i.useMemo)((() => String(t).replace(/\n$/, "")), [t]),
+                    [o, a] = (0, i.useState)(I.None);
+                return l().createElement(c.Box, {
                     sx: {
                         display: "flex",
                         flexDirection: "column"
                     }
-                }, i().createElement(S.Prism, Object.assign({}, n, {
-                    children: o,
-                    style: C.Z,
+                }, l().createElement(S.Prism, Object.assign({}, n, {
+                    className: (0, w.Z)(n.className, k),
+                    children: r,
+                    style: _.Z,
                     language: e,
                     PreTag: "div"
-                })), i().createElement(m.Button, {
+                })), l().createElement(c.Button, {
                     onClick: async () => {
-                        l(h.Copying);
+                        a(I.Copying);
                         try {
-                            await navigator.clipboard.writeText(o)
+                            await navigator.clipboard.writeText(r)
                         } catch (e) {
-                            return console.error(e), void l(h.None)
+                            return console.error(e), void a(I.None)
                         }
-                        l(h.Copied), setTimeout((() => l(h.None)), 1e3)
+                        a(I.Copied), setTimeout((() => a(I.None)), 1e3)
                     },
-                    disabled: r !== h.None,
+                    disabled: o !== I.None,
                     sx: {
                         alignSelf: "flex-end"
                     }
-                }, _[r]))
+                }, P[o]))
             }
 
-            function I({
+            function L({
                 inline: e,
                 className: t,
                 ...n
             }) {
-                const o = /language-(\w+)/.exec(t || "");
-                return e ? i().createElement(j, Object.assign({}, n)) : i().createElement(k, Object.assign({}, n, {
-                    language: o ? o[1] : void 0
+                const r = /language-(\w+)/.exec(t || "");
+                return e ? l().createElement(j, Object.assign({}, n)) : l().createElement(M, Object.assign({}, n, {
+                    language: r ? r[1] : void 0
                 }))
             }
-            const P = i().createContext({});
+            const A = l().createContext({});
 
-            function M({
+            function T({
                 globalAwareness: e,
                 children: t
             }) {
-                const [n, o] = (0, s.useState)({});
-                return (0, s.useEffect)((() => {
+                const [n, r] = (0, i.useState)({});
+                return (0, i.useEffect)((() => {
                     function t() {
                         var t;
                         const n = null !== (t = null == e ? void 0 : e.getStates()) && void 0 !== t ? t : new Map,
-                            r = {};
+                            o = {};
                         n.forEach((e => {
-                            r[e.user.username] = e.user
-                        })), o(r)
+                            o[e.user.username] = e.user
+                        })), r(o)
                     }
                     return null == e || e.on("change", t), () => {
                         null == e || e.off("change", t)
                     }
-                }), [e]), e ? i().createElement(P.Provider, {
+                }), [e]), e ? l().createElement(A.Provider, {
                     value: n
                 }, t) : t
             }
+            var B = n(22502);
+            const F = new B.LabIcon({
+                    name: "jupyter-ai::chat",
+                    svgstr: '<svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M0 0h24v24H0V0z" fill="none"/>\n    <path d="M15 4v7H5.17L4 12.17V4h11m1-2H3c-.55 0-1 .45-1 1v14l4-4h10c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm5 4h-2v9H6v2c0 .55.45 1 1 1h11l4 4V7c0-.55-.45-1-1-1z"/>\n  </g>\n</svg>\n'
+                }),
+                N = new B.LabIcon({
+                    name: "jupyter-ai::jupyternaut",
+                    svgstr: '<svg viewBox="0 0 38 38" fill="none"\n    xmlns="http://www.w3.org/2000/svg">\n    <g clip-path="url(#clip0_0_2356)">\n        <rect width="38" height="38" fill="white" />\n        <circle cx="19" cy="19" r="19" fill="#F37726" />\n        <path fill-rule="evenodd" clip-rule="evenodd"\n            d="M19.9483 6.83653C20.5827 6.6205 21.0391 6.0196 21.0391 5.31212C21.0391 4.42296 20.3183 3.70215 19.4291 3.70215C18.5399 3.70215 17.8191 4.42296 17.8191 5.31212C17.8191 6.01951 18.2753 6.62033 18.9096 6.83644V8.00387H18.3702C12.0844 8.00387 6.97151 13.1171 6.97151 19.4026C6.97151 25.6885 12.0848 30.8013 18.3702 30.8013H19.7682C26.0541 30.8013 31.167 25.6881 31.167 19.4026C31.167 13.1773 26.1511 8.10183 19.9483 8.00527V6.83653ZM18.3702 29H19.7682C25.1351 29 29.4985 24.0213 29.4985 20.6545C29.4985 15.2876 25.1351 10.9242 19.7682 10.9242H18.3702C13.0034 10.9242 8.64 15.2876 8.64 20.6545C8.64 24.0213 13.0034 29 18.3702 29ZM32.8926 23.997C33.6267 23.997 33.6301 23.4847 33.6348 22.7562V22.7562V22.7562V22.7561C33.636 22.5714 33.6373 22.3728 33.6506 22.1651C33.7079 21.3027 33.7245 20.4643 33.7079 19.6759L33.7046 19.5569C33.6673 18.2251 33.661 17.999 32.3999 17.7511L32.252 17.7265L32.2535 17.776C32.2611 18.0225 32.2686 18.269 32.2686 18.515C32.2686 20.3168 31.9974 22.0628 31.4956 23.704C31.3593 24.1499 31.8389 24.5669 32.249 24.3451L32.8926 23.997ZM5.28037 23.997C4.54628 23.997 4.54296 23.4847 4.53822 22.7563C4.53702 22.5715 4.53573 22.3729 4.52241 22.1651C4.46511 21.3027 4.44849 20.4644 4.4651 19.6759L4.46846 19.557C4.50567 18.2251 4.51198 17.9991 5.77316 17.7512L5.921 17.7265L5.91949 17.776L5.91949 17.776C5.91193 18.0225 5.90438 18.269 5.90438 18.515C5.90438 20.3169 6.17557 22.0628 6.67738 23.704C6.81372 24.1499 6.33412 24.5669 5.92398 24.3451L5.28037 23.997ZM19.5225 11.9922C14.8928 11.9922 11.0449 14.9283 10.0641 18.7499C9.93031 19.2711 10.6154 19.4434 10.9411 19.0152C12.324 17.1972 14.0829 16.8622 15.6479 16.5641C17.7622 16.1614 19.5225 15.8262 19.5225 11.9922Z"\n            fill="white" />\n    </g>\n    <defs>\n        <clipPath id="clip0_0_2356">\n            <rect width="38" height="38" fill="white" />\n        </clipPath>\n    </defs>\n</svg>'
+                }).react;
 
-            function A(e) {
+            function R(e) {
                 var t;
-                const n = (0, s.useContext)(P),
-                    o = {
+                const n = (0, i.useContext)(A),
+                    r = {
                         height: "24px",
                         width: "24px"
                     };
-                let r;
+                let o;
                 if ("human" === e.message.type) {
-                    const s = null === (t = null == n ? void 0 : n[e.message.client.username]) || void 0 === t ? void 0 : t.color;
-                    r = i().createElement(m.Avatar, {
+                    const i = null === (t = null == n ? void 0 : n[e.message.client.username]) || void 0 === t ? void 0 : t.color;
+                    o = l().createElement(c.Avatar, {
                         sx: {
-                            ...o,
-                            ...s && {
-                                bgcolor: s
+                            ...r,
+                            ...i && {
+                                bgcolor: i
                             }
                         }
-                    }, i().createElement(m.Typography, {
+                    }, l().createElement(c.Typography, {
                         sx: {
                             fontSize: "var(--jp-ui-font-size1)",
                             color: "var(--jp-ui-inverse-font-color1)"
                         }
                     }, e.message.client.initials))
-                } else r = i().createElement(m.Avatar, {
+                } else o = l().createElement(c.Avatar, {
                     sx: {
-                        ...o,
+                        ...r,
                         bgcolor: "var(--jp-jupyter-icon-color)"
                     }
-                }, i().createElement(g.Z, null));
-                const l = "human" === e.message.type ? e.message.client.display_name : "Jupyter AI";
-                return i().createElement(m.Box, {
+                }, l().createElement(N, {
+                    display: "block",
+                    height: "100%",
+                    width: "100%"
+                }));
+                const a = "human" === e.message.type ? e.message.client.display_name : "Jupyternaut";
+                return l().createElement(c.Box, {
                     sx: {
                         display: "flex",
                         alignItems: "center",
                         "& > :not(:last-child)": {
                             marginRight: 3
                         },
                         ...e.sx
                     }
-                }, r, i().createElement(m.Box, {
+                }, o, l().createElement(c.Box, {
                     sx: {
                         display: "flex",
                         flexGrow: 1,
                         flexWrap: "wrap",
                         justifyContent: "space-between",
                         alignItems: "center"
                     }
-                }, i().createElement(m.Typography, {
+                }, l().createElement(c.Typography, {
                     sx: {
                         fontWeight: 700,
                         color: "var(--jp-ui-font-color1)"
                     }
-                }, l), i().createElement(m.Typography, {
+                }, a), l().createElement(c.Typography, {
                     sx: {
                         fontSize: "0.8em",
                         color: "var(--jp-ui-font-color2)",
                         fontWeight: 300
                     }
                 }, e.timestamp)))
             }
 
             function z(e) {
-                const [t, n] = (0, s.useState)({});
-                return (0, s.useEffect)((() => {
+                const [t, n] = (0, i.useState)({});
+                return (0, i.useEffect)((() => {
                     function t() {
                         const t = {};
                         for (const n of e.messages) t[n.id] = (0, f.formatDistanceToNowStrict)((0, f.fromUnixTime)(n.time)) + " ago";
                         n(t)
                     }
                     t();
-                    const o = setInterval(t, 5e3);
+                    const r = setInterval(t, 5e3);
                     return () => {
-                        clearInterval(o)
+                        clearInterval(r)
                     }
-                }), [e.messages]), i().createElement(m.Box, {
+                }), [e.messages]), l().createElement(c.Box, {
                     sx: {
                         "& > :not(:last-child)": {
                             borderBottom: "1px solid var(--jp-border-color2)"
                         }
                     }
-                }, e.messages.map(((e, n) => i().createElement(m.Box, {
+                }, e.messages.map(((e, n) => l().createElement(c.Box, {
                     key: n,
                     sx: {
                         padding: 4
                     }
-                }, i().createElement(A, {
+                }, l().createElement(R, {
                     message: e,
                     timestamp: t[e.id],
                     sx: {
                         marginBottom: 3
                     }
-                }), i().createElement(y(), {
+                }), l().createElement(y(), {
                     className: "jp-RenderedHTMLCommon jp-ai-react-markdown",
                     components: {
-                        code: I
+                        code: L
                     },
-                    remarkPlugins: [b()],
-                    rehypePlugins: [E()]
+                    remarkPlugins: [E()],
+                    rehypePlugins: [C()]
                 }, e.body)))))
             }
-            var L = n(26307);
+            var H = n(26307);
 
-            function B(e) {
-                return i().createElement(m.Box, {
+            function Z(e) {
+                return l().createElement(c.Box, {
                     sx: e.sx
-                }, i().createElement(m.Box, {
+                }, l().createElement(c.Box, {
                     sx: {
                         display: "flex"
                     }
-                }, i().createElement(m.TextField, {
+                }, l().createElement(c.TextField, {
                     value: e.value,
                     onChange: t => e.onChange(t.target.value),
                     fullWidth: !0,
                     variant: "outlined",
                     multiline: !0,
                     onKeyDown: function(t) {
                         "Enter" === t.key && t.shiftKey && (e.onSend(), t.stopPropagation(), t.preventDefault())
                     },
                     InputProps: {
-                        endAdornment: i().createElement(m.InputAdornment, {
+                        endAdornment: l().createElement(c.InputAdornment, {
                             position: "end"
-                        }, i().createElement(m.IconButton, {
+                        }, l().createElement(c.IconButton, {
                             size: "small",
                             color: "primary",
                             onClick: e.onSend,
                             disabled: !e.value.trim().length
-                        }, i().createElement(L.Z, null)))
-                    }
-                })), e.hasSelection && i().createElement(m.FormGroup, {
+                        }, l().createElement(H.Z, null)))
+                    },
+                    FormHelperTextProps: {
+                        sx: {
+                            marginLeft: "auto",
+                            marginRight: 0
+                        }
+                    },
+                    helperText: e.value.length > 2 ? e.helperText : " "
+                })), e.hasSelection && l().createElement(c.FormGroup, {
                     sx: {
                         display: "flex",
                         flexDirection: "row"
                     }
-                }, i().createElement(m.FormControlLabel, {
-                    control: i().createElement(m.Checkbox, {
+                }, l().createElement(c.FormControlLabel, {
+                    control: l().createElement(c.Checkbox, {
                         checked: e.includeSelection,
                         onChange: e.toggleIncludeSelection
                     }),
                     label: "Include selection"
-                }), i().createElement(m.FormControlLabel, {
-                    control: i().createElement(m.Checkbox, {
+                }), l().createElement(c.FormControlLabel, {
+                    control: l().createElement(c.Checkbox, {
                         checked: e.replaceSelection,
                         onChange: e.toggleReplaceSelection
                     }),
                     label: "Replace selection"
                 })))
             }
-            const R = i().createContext([null, () => {}]);
 
-            function T({
+            function D(e) {
+                return l().createElement(c.FormControl, {
+                    fullWidth: !0
+                }, l().createElement(c.InputLabel, null, e.label), l().createElement(c.Select, Object.assign({}, e, {
+                    value: null === e.value ? "null" : e.value,
+                    label: e.label,
+                    onChange: (t, n) => {
+                        var r;
+                        "null" === t.target.value && (t.target.value = null), null === (r = e.onChange) || void 0 === r || r.call(e, t, n)
+                    },
+                    MenuProps: {
+                        sx: {
+                            maxHeight: "50%",
+                            minHeight: 400
+                        }
+                    }
+                }), e.children))
+            }
+            var O, W, V = n(28142),
+                J = n(48820);
+            async function $(e = "", t = {}) {
+                const n = J.ServerConnection.makeSettings(),
+                    r = V.URLExt.join(n.baseUrl, "api/ai", e);
+                let o;
+                try {
+                    o = await J.ServerConnection.makeRequest(r, t, n)
+                } catch (e) {
+                    throw new J.ServerConnection.NetworkError(e)
+                }
+                let i = await o.text();
+                if (i.length > 0) try {
+                    i = JSON.parse(i)
+                } catch (e) {
+                    console.log("Not a JSON response body.", o)
+                }
+                if (!o.ok) throw new J.ServerConnection.ResponseError(o, i.message || i);
+                return i
+            }
+
+            function G() {
+                const [e, t] = (0, i.useState)(W.Loading), [n, r] = (0, i.useState)(), [o, a] = (0, i.useState)(), [u, d] = (0, i.useState)(), [m, p] = (0, i.useState)(), [h, g] = (0, i.useState)({
+                    model_provider_id: null,
+                    embeddings_provider_id: null,
+                    api_keys: {}
+                }), [f, v] = (0, i.useState)(!1), [y, x] = (0, i.useState)();
+                return (0, i.useEffect)((() => {
+                    !async function() {
+                        try {
+                            const [e, n, r] = await Promise.all([O.getConfig(), O.listLmProviders(), O.listEmProviders()]);
+                            a(e), g(e), d(n), p(r), t(W.Ready)
+                        } catch (e) {
+                            console.error(e), e instanceof Error && r(e.message), t(W.FetchError)
+                        }
+                    }()
+                }), []), (0, i.useEffect)((() => {
+                    var e, t;
+                    const n = null === (e = h.model_provider_id) || void 0 === e ? void 0 : e.split(":")[0],
+                        r = null === (t = h.embeddings_provider_id) || void 0 === t ? void 0 : t.split(":")[0],
+                        i = null == u ? void 0 : u.providers.find((e => e.id === n)),
+                        l = null == m ? void 0 : m.providers.find((e => e.id === r)),
+                        a = {};
+                    (null == i ? void 0 : i.auth_strategy) && "env" === i.auth_strategy.type && (a[i.auth_strategy.name] = (null == o ? void 0 : o.api_keys[i.auth_strategy.name]) || ""), (null == l ? void 0 : l.auth_strategy) && "env" === l.auth_strategy.type && (a[l.auth_strategy.name] = (null == o ? void 0 : o.api_keys[l.auth_strategy.name]) || ""), g((e => ({
+                        ...e,
+                        api_keys: {
+                            ...null == o ? void 0 : o.api_keys,
+                            ...a
+                        }
+                    })))
+                }), [h.model_provider_id, h.embeddings_provider_id]), e === W.Loading ? l().createElement(s.Z, {
+                    sx: {
+                        width: "100%",
+                        height: "100%",
+                        boxSizing: "border-box",
+                        display: "flex",
+                        alignItems: "center",
+                        justifyContent: "space-around"
+                    }
+                }, l().createElement(c.CircularProgress, null)) : e !== W.FetchError && u && m && o ? l().createElement(s.Z, {
+                    sx: {
+                        padding: 4,
+                        boxSizing: "border-box",
+                        "& > .MuiAlert-root": {
+                            marginBottom: 2
+                        }
+                    }
+                }, e === W.SubmitError && l().createElement(c.Alert, {
+                    severity: "error"
+                }, y ? `An error occurred. Error details:\n\n${y}` : "An unknown error occurred. Check the console for more details."), e === W.Success && l().createElement(c.Alert, {
+                    severity: "success"
+                }, "Settings saved successfully."), l().createElement(D, {
+                    value: h.model_provider_id,
+                    label: "Language model",
+                    onChange: e => g((t => ({
+                        ...t,
+                        model_provider_id: e.target.value
+                    }))),
+                    MenuProps: {
+                        sx: {
+                            maxHeight: "50%",
+                            minHeight: 400
+                        }
+                    }
+                }, l().createElement(c.MenuItem, {
+                    value: "null"
+                }, "None"), u.providers.map((e => e.models.filter((e => "*" !== e)).map((t => l().createElement(c.MenuItem, {
+                    value: `${e.id}:${t}`
+                }, e.name, " :: ", t)))))), l().createElement(D, {
+                    value: h.embeddings_provider_id,
+                    label: "Embedding model",
+                    onChange: e => g((t => ({
+                        ...t,
+                        embeddings_provider_id: e.target.value
+                    }))),
+                    MenuProps: {
+                        sx: {
+                            maxHeight: "50%",
+                            minHeight: 400
+                        }
+                    }
+                }, l().createElement(c.MenuItem, {
+                    value: "null"
+                }, "None"), m.providers.map((e => e.models.filter((e => "*" !== e)).map((t => l().createElement(c.MenuItem, {
+                    value: `${e.id}:${t}`
+                }, e.name, " :: ", t)))))), Object.entries(h.api_keys).map((([e, t], n) => l().createElement(c.TextField, {
+                    key: n,
+                    label: e,
+                    value: t,
+                    fullWidth: !0,
+                    type: "password",
+                    onChange: t => g((n => ({
+                        ...n,
+                        api_keys: {
+                            ...n.api_keys,
+                            [e]: t.target.value
+                        }
+                    })))
+                }))), l().createElement(s.Z, {
+                    sx: {
+                        display: "flex",
+                        justifyContent: "flex-end"
+                    }
+                }, l().createElement(c.Button, {
+                    variant: "contained",
+                    onClick: async () => {
+                        const e = {
+                            ...h,
+                            api_keys: {
+                                ...h.api_keys
+                            }
+                        };
+                        for (const t in e.api_keys) "" === e.api_keys[t] && delete e.api_keys[t];
+                        v(!0);
+                        try {
+                            await O.updateConfig(e)
+                        } catch (e) {
+                            console.error(e), e instanceof Error && x(e.message), t(W.SubmitError)
+                        }
+                        t(W.Success), v(!1)
+                    },
+                    disabled: f
+                }, f ? "Saving..." : "Save changes"))) : l().createElement(s.Z, {
+                    sx: {
+                        width: "100%",
+                        height: "100%",
+                        padding: 4,
+                        boxSizing: "border-box"
+                    }
+                }, l().createElement(c.Alert, {
+                    severity: "error"
+                }, n ? `An error occurred. Error details:\n\n${n}` : "An unknown error occurred. Check the console for more details."))
+            }! function(e) {
+                e.sendPrompt = async function(e) {
+                    let t;
+                    try {
+                        t = await $("prompt", {
+                            method: "POST",
+                            body: JSON.stringify(e)
+                        })
+                    } catch (e) {
+                        return Promise.reject(e)
+                    }
+                    return t
+                }, e.listTasks = async function() {
+                    return $("tasks")
+                }, e.describeTask = async function(e) {
+                    return $(`tasks/${e}`)
+                }, e.getConfig = async function() {
+                    return $("config")
+                }, e.listLmProviders = async function() {
+                    return $("providers")
+                }, e.listEmProviders = async function() {
+                    return $("providers/embeddings")
+                }, e.updateConfig = async function(e) {
+                    return $("config", {
+                        method: "POST",
+                        body: JSON.stringify(e)
+                    })
+                }
+            }(O || (O = {})),
+            function(e) {
+                e[e.Loading = 0] = "Loading", e[e.Ready = 1] = "Ready", e[e.FetchError = 2] = "FetchError", e[e.SubmitError = 3] = "SubmitError", e[e.Success = 4] = "Success"
+            }(W || (W = {}));
+            const U = l().createContext([null, () => {}]);
+
+            function Q({
                 selectionWatcher: e,
                 children: t
             }) {
-                const [n, o] = (0, s.useState)(null);
-                (0, s.useEffect)((() => {
+                const [n, r] = (0, i.useState)(null);
+                (0, i.useEffect)((() => {
                     e.selectionChanged.connect(((e, t) => {
-                        o(t)
+                        r(t)
                     }))
                 }), []);
-                const r = (0, s.useCallback)((t => {
+                const o = (0, i.useCallback)((t => {
                     e.replaceSelection(t)
                 }), [e]);
-                return i().createElement(R.Provider, {
-                    value: [n, r]
+                return l().createElement(U.Provider, {
+                    value: [n, o]
                 }, t)
             }
 
-            function D(e) {
-                const t = (0, s.useMemo)((() => "jupyter-ai-scroll-container-" + Date.now().toString()), []);
-                return (0, s.useEffect)((() => {
+            function q(e) {
+                const t = (0, i.useMemo)((() => "jupyter-ai-scroll-container-" + Date.now().toString()), []);
+                return (0, i.useEffect)((() => {
                     const e = document.querySelector(`#${t}`);
                     if (!e) return;
                     const n = new IntersectionObserver((t => {
                         t.forEach((t => {
                             t.isIntersecting && e.scroll({
                                 top: 999999999
                             })
                         }))
                     }), {
                         threshold: 1
                     });
                     return n.observe(e), () => n.disconnect()
-                }), []), i().createElement(m.Box, {
+                }), []), l().createElement(c.Box, {
                     id: t,
                     sx: {
                         overflowY: "scroll",
                         "& *": {
                             overflowAnchor: "none"
                         },
                         ...e.sx
                     }
-                }, i().createElement(m.Box, {
+                }, l().createElement(c.Box, {
                     sx: {
                         minHeight: "100.01%"
                     }
-                }, e.children), i().createElement(m.Box, {
+                }, e.children), l().createElement(c.Box, {
                     sx: {
                         overflowAnchor: "auto",
                         height: "1px"
                     }
                 }))
             }
 
-            function N({
-                chatHandler: e
+            function K({
+                chatHandler: e,
+                setChatView: t
             }) {
-                const [t, n] = (0, s.useState)([]), [o, r] = (0, s.useState)(!0), [l, c] = (0, s.useState)(!1), [u, d] = (0, s.useState)(""), [p, h] = (0, s.useContext)(R);
-                return (0, s.useEffect)((() => {
+                const [n, r] = (0, i.useState)([]), [o, a] = (0, i.useState)(!1), [d, m] = (0, i.useState)(!0), [p, h] = (0, i.useState)(!1), [g, f] = (0, i.useState)(""), [v, y] = (0, i.useContext)(U);
+                return (0, i.useEffect)((() => {
                     !async function() {
                         try {
-                            const t = await e.getHistory();
-                            n(t.messages)
-                        } catch (e) {}
+                            const [t, n] = await Promise.all([e.getHistory(), O.getConfig()]);
+                            r(t.messages), n.model_provider_id || a(!0)
+                        } catch (e) {
+                            console.error(e)
+                        }
                     }()
-                }), [e]), (0, s.useEffect)((() => {
+                }), [e]), (0, i.useEffect)((() => {
                     function t(e) {
-                        "connection" !== e.type && ("clear" !== e.type ? n((t => [...t, e])) : n([]))
+                        "connection" !== e.type && ("clear" !== e.type ? r((t => [...t, e])) : r([]))
                     }
                     return e.addListener(t),
                         function() {
                             e.removeListener(t)
                         }
-                }), [e]), i().createElement(a.Z, {
+                }), [e]), o ? l().createElement(s.Z, {
                     sx: {
-                        width: "100%",
-                        height: "100%",
-                        boxSizing: "border-box",
-                        background: "var(--jp-layout-color0)",
+                        padding: 4,
                         display: "flex",
-                        flexDirection: "column"
+                        flexGrow: 1,
+                        alignItems: "top",
+                        justifyContent: "space-around"
                     }
-                }, i().createElement(D, {
+                }, l().createElement(c.Stack, {
+                    spacing: 4
+                }, l().createElement("p", null, "Welcome to Jupyter AI! To get started, please select a language model to chat with from the settings panel. You will also likely need to provide API credentials, so be sure to have those handy."), l().createElement(c.Button, {
+                    variant: "contained",
+                    startIcon: l().createElement(u.Z, null),
+                    size: "large",
+                    onClick: () => (a(!1), void t(Y.Settings))
+                }, "Start Here"))) : l().createElement(l().Fragment, null, l().createElement(q, {
                     sx: {
                         flexGrow: 1
                     }
-                }, i().createElement(z, {
-                    messages: t
-                }), i().createElement(a.Z, {
-                    sx: {
-                        overflowAnchor: "auto",
-                        height: "1px"
-                    }
-                })), i().createElement(B, {
-                    value: u,
-                    onChange: d,
+                }, l().createElement(z, {
+                    messages: n
+                })), l().createElement(Z, {
+                    value: g,
+                    onChange: f,
                     onSend: async () => {
-                        d("");
-                        const t = u + (o && (null == p ? void 0 : p.text) ? "\n\n```\n" + p.text + "```" : ""),
+                        f("");
+                        const t = g + (d && (null == v ? void 0 : v.text) ? "\n\n```\n" + v.text + "\n```" : ""),
                             n = await e.sendMessage({
                                 prompt: t
                             }),
                             r = await e.replyFor(n);
-                        if (l && p) {
+                        if (p && v) {
                             const {
                                 cellId: e,
                                 ...t
-                            } = p;
-                            h({
+                            } = v;
+                            y({
                                 ...t,
                                 ...e && {
                                     cellId: e
                                 },
                                 text: r.body
                             })
                         }
                     },
-                    hasSelection: !!(null == p ? void 0 : p.text),
-                    includeSelection: o,
-                    toggleIncludeSelection: () => r((e => !e)),
-                    replaceSelection: l,
-                    toggleReplaceSelection: () => c((e => !e)),
+                    hasSelection: !!(null == v ? void 0 : v.text),
+                    includeSelection: d,
+                    toggleIncludeSelection: () => m((e => !e)),
+                    replaceSelection: p,
+                    toggleReplaceSelection: () => h((e => !e)),
                     sx: {
                         paddingLeft: 4,
                         paddingRight: 4,
-                        paddingTop: 2,
-                        paddingBottom: 2,
+                        paddingTop: 3.5,
+                        paddingBottom: 0,
                         borderTop: "1px solid var(--jp-border-color1)"
-                    }
+                    },
+                    helperText: l().createElement("span", null, "Press ", l().createElement("b", null, "Shift"), " + ", l().createElement("b", null, "Enter"), " to submit message")
                 }))
             }
+            var Y;
 
-            function F(e) {
-                return i().createElement(p, null, i().createElement(T, {
+            function X(e) {
+                const [t, n] = (0, i.useState)(e.chatView || Y.Chat);
+                return l().createElement(g, null, l().createElement(Q, {
                     selectionWatcher: e.selectionWatcher
-                }, i().createElement(M, {
+                }, l().createElement(T, {
                     globalAwareness: e.globalAwareness
-                }, i().createElement(N, {
-                    chatHandler: e.chatHandler
-                }))))
-            }
-            var O = n(22502);
-            new O.LabIcon({
-                name: "jupyter-ai::psychology",
-                svgstr: '<svg xmlns="http://www.w3.org/2000/svg" class="css-10cscxr" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="PsychologyIcon">\n    <path d="M13 8.57c-.79 0-1.43.64-1.43 1.43s.64 1.43 1.43 1.43 1.43-.64 1.43-1.43-.64-1.43-1.43-1.43z"></path><path d="M13 3C9.25 3 6.2 5.94 6.02 9.64L4.1 12.2c-.25.33-.01.8.4.8H6v3c0 1.1.9 2 2 2h1v3h7v-4.68c2.36-1.12 4-3.53 4-6.32 0-3.87-3.13-7-7-7zm3 7c0 .13-.01.26-.02.39l.83.66c.08.06.1.16.05.25l-.8 1.39c-.05.09-.16.12-.24.09l-.99-.4c-.21.16-.43.29-.67.39L14 13.83c-.01.1-.1.17-.2.17h-1.6c-.1 0-.18-.07-.2-.17l-.15-1.06c-.25-.1-.47-.23-.68-.39l-.99.4c-.09.03-.2 0-.25-.09l-.8-1.39c-.05-.08-.03-.19.05-.25l.84-.66c-.01-.13-.02-.26-.02-.39s.02-.27.04-.39l-.85-.66c-.08-.06-.1-.16-.05-.26l.8-1.38c.05-.09.15-.12.24-.09l1 .4c.2-.15.43-.29.67-.39L12 6.17c.02-.1.1-.17.2-.17h1.6c.1 0 .18.07.2.17l.15 1.06c.24.1.46.23.67.39l1-.4c.09-.03.2 0 .24.09l.8 1.38c.05.09.03.2-.05.26l-.85.66c.03.12.04.25.04.39z">\n    </path>\n</svg>'
-            });
-            const W = new O.LabIcon({
-                name: "jupyter-ai::chat",
-                svgstr: '<svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M0 0h24v24H0V0z" fill="none"/>\n    <path d="M15 4v7H5.17L4 12.17V4h11m1-2H3c-.55 0-1 .45-1 1v14l4-4h10c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm5 4h-2v9H6v2c0 .55.45 1 1 1h11l4 4V7c0-.55-.45-1-1-1z"/>\n  </g>\n</svg>\n'
-            });
-            var H = n(80819),
-                J = n(26413),
-                Z = n(51473),
-                U = n(41123),
-                V = n(78918),
-                G = n(71840);
+                }, l().createElement(s.Z, {
+                    sx: {
+                        width: "100%",
+                        height: "100%",
+                        boxSizing: "border-box",
+                        background: "var(--jp-layout-color0)",
+                        display: "flex",
+                        flexDirection: "column"
+                    }
+                }, l().createElement(s.Z, {
+                    sx: {
+                        display: "flex",
+                        justifyContent: "space-between"
+                    }
+                }, t !== Y.Chat ? l().createElement(c.IconButton, {
+                    onClick: () => n(Y.Chat)
+                }, l().createElement(d.Z, null)) : l().createElement(s.Z, null), t === Y.Chat ? l().createElement(c.IconButton, {
+                    onClick: () => n(Y.Settings)
+                }, l().createElement(u.Z, null)) : l().createElement(s.Z, null)), t === Y.Chat && l().createElement(K, {
+                    chatHandler: e.chatHandler,
+                    setChatView: n
+                }), t === Y.Settings && l().createElement(G, null)))))
+            }! function(e) {
+                e[e.Chat = 0] = "Chat", e[e.Settings = 1] = "Settings"
+            }(Y || (Y = {}));
+            var ee = n(80819),
+                te = n(26413),
+                ne = n(51473),
+                re = n(41123),
+                oe = n(78918),
+                ie = n(71840);
 
-            function $(e) {
+            function le(e) {
                 var t;
-                if (!(e instanceof H.DocumentWidget)) return null;
+                if (!(e instanceof ee.DocumentWidget)) return null;
                 let n;
                 const {
-                    content: o
+                    content: r
                 } = e;
-                return o instanceof Z.FileEditor ? n = o.editor : o instanceof U.Notebook && (n = null === (t = o.activeCell) || void 0 === t ? void 0 : t.editor), n instanceof J.CodeMirrorEditor ? n : void 0
+                return r instanceof ne.FileEditor ? n = r.editor : r instanceof re.Notebook && (n = null === (t = r.activeCell) || void 0 === t ? void 0 : t.editor), n instanceof te.CodeMirrorEditor ? n : void 0
             }
-            class Q {
+            class ae {
                 constructor(e) {
-                    if (this._mainAreaWidget = null, this._selection = null, this._selectionChanged = new G.Signal(this), !(e instanceof o.LabShell)) throw "Shell is not an instance of LabShell. Jupyter AI does not currently support custom shells.";
+                    if (this._mainAreaWidget = null, this._selection = null, this._selectionChanged = new ie.Signal(this), !(e instanceof r.LabShell)) throw "Shell is not an instance of LabShell. Jupyter AI does not currently support custom shells.";
                     this._shell = e, this._shell.currentChanged.connect(((e, t) => {
                         this._mainAreaWidget = t.newValue
                     })), setInterval(this._poll.bind(this), 200)
                 }
                 get selectionChanged() {
                     return this._selectionChanged
                 }
                 replaceSelection(e) {
-                    const t = (0, V.find)(this._shell.widgets(), (t => t.id === e.widgetId));
-                    if (!(t instanceof H.DocumentWidget)) return;
-                    if (this._shell.activateById(e.widgetId), t.content instanceof U.Notebook && e.cellId) {
+                    const t = (0, oe.find)(this._shell.widgets(), (t => t.id === e.widgetId));
+                    if (!(t instanceof ee.DocumentWidget)) return;
+                    if (this._shell.activateById(e.widgetId), t.content instanceof re.Notebook && e.cellId) {
                         const n = function(e, t) {
                             var n;
-                            const o = null === (n = e.model) || void 0 === n ? void 0 : n.sharedModel.cells.findIndex((e => e.getId() === t));
-                            return void 0 === o ? -1 : o
+                            const r = null === (n = e.model) || void 0 === n ? void 0 : n.sharedModel.cells.findIndex((e => e.getId() === t));
+                            return void 0 === r ? -1 : r
                         }(t.content, e.cellId); - 1 !== n && (t.content.activeCellIndex = n)
                     }
-                    const n = $(t);
+                    const n = le(t);
                     if (!n) return;
                     n.model.sharedModel.updateSource(n.getOffsetAt(e.start), n.getOffsetAt(e.end), e.text);
-                    const o = n.getPositionAt(n.getOffsetAt(e.start) + e.text.length);
+                    const r = n.getPositionAt(n.getOffsetAt(e.start) + e.text.length);
                     n.setSelection({
-                        start: o,
-                        end: o
+                        start: r,
+                        end: r
                     })
                 }
                 _poll() {
                     const e = this._selection,
                         t = function(e) {
                             var t;
-                            const n = $(e);
-                            if (!(n && e instanceof H.DocumentWidget)) return null;
-                            let o;
-                            e.content instanceof U.Notebook && (o = null === (t = e.content.activeCell) || void 0 === t ? void 0 : t.model.id);
+                            const n = le(e);
+                            if (!(n && e instanceof ee.DocumentWidget)) return null;
+                            let r;
+                            e.content instanceof re.Notebook && (r = null === (t = e.content.activeCell) || void 0 === t ? void 0 : t.model.id);
                             let {
-                                start: r,
-                                end: s,
-                                ...i
+                                start: o,
+                                end: i,
+                                ...l
                             } = n.getSelection();
-                            const l = n.getOffsetAt(r),
-                                a = n.getOffsetAt(s),
-                                c = n.model.sharedModel.getSource().substring(l, a);
-                            return l > a && ([r, s] = [s, r]), {
-                                ...i,
-                                start: r,
-                                end: s,
+                            const a = n.getOffsetAt(o),
+                                s = n.getOffsetAt(i),
+                                c = n.model.sharedModel.getSource().substring(a, s);
+                            return a > s && ([o, i] = [i, o]), {
+                                ...l,
+                                start: o,
+                                end: i,
                                 text: c,
                                 widgetId: e.id,
-                                ...o && {
-                                    cellId: o
+                                ...r && {
+                                    cellId: r
                                 }
                             }
                         }(this._mainAreaWidget);
                     (null == e ? void 0 : e.text) !== (null == t ? void 0 : t.text) && (this._selection = t, this._selectionChanged.emit(t))
                 }
             }
-            var q, K = n(48820),
-                Y = n(28142);
-            async function X(e = "", t = {}) {
-                const n = K.ServerConnection.makeSettings(),
-                    o = Y.URLExt.join(n.baseUrl, "api/ai", e);
-                let r;
-                try {
-                    r = await K.ServerConnection.makeRequest(o, t, n)
-                } catch (e) {
-                    throw new K.ServerConnection.NetworkError(e)
-                }
-                let s = await r.text();
-                if (s.length > 0) try {
-                    s = JSON.parse(s)
-                } catch (e) {
-                    console.log("Not a JSON response body.", r)
-                }
-                if (!r.ok) throw new K.ServerConnection.ResponseError(r, s.message || s);
-                return s
-            }! function(e) {
-                e.sendPrompt = async function(e) {
-                    let t;
-                    try {
-                        t = await X("prompt", {
-                            method: "POST",
-                            body: JSON.stringify(e)
-                        })
-                    } catch (e) {
-                        return Promise.reject(e)
-                    }
-                    return t
-                }, e.listTasks = async function() {
-                    return X("tasks")
-                }, e.describeTask = async function(e) {
-                    return X(`tasks/${e}`)
-                }
-            }(q || (q = {}));
-            class ee {
+            class se {
                 constructor(e = {}) {
                     var t;
-                    this.id = "", this._sendResolverQueue = [], this._replyForResolverDict = {}, this._isDisposed = !1, this._socket = null, this._listeners = [], this.serverSettings = null !== (t = e.serverSettings) && void 0 !== t ? t : K.ServerConnection.makeSettings()
+                    this.id = "", this._sendResolverQueue = [], this._replyForResolverDict = {}, this._isDisposed = !1, this._socket = null, this._listeners = [], this.serverSettings = null !== (t = e.serverSettings) && void 0 !== t ? t : J.ServerConnection.makeSettings()
                 }
                 initialize() {
                     return new Promise(((e, t) => {
                         if (this.isDisposed) return;
                         const {
                             token: n,
-                            WebSocket: o,
-                            wsUrl: r
-                        } = this.serverSettings, s = Y.URLExt.join(r, "api/ai/chats") + (n ? `?token=${encodeURIComponent(n)}` : ""), i = this._socket = new o(s);
-                        i.onerror = e => t(e), i.onmessage = e => e.data && this._onMessage(JSON.parse(e.data));
-                        const l = t => {
-                            "connection" === t.type && (this.id = t.client_id, e(), this.removeListener(l))
+                            WebSocket: r,
+                            wsUrl: o
+                        } = this.serverSettings, i = V.URLExt.join(o, "api/ai/chats") + (n ? `?token=${encodeURIComponent(n)}` : ""), l = this._socket = new r(i);
+                        l.onerror = e => t(e), l.onmessage = e => e.data && this._onMessage(JSON.parse(e.data));
+                        const a = t => {
+                            "connection" === t.type && (this.id = t.client_id, e(), this.removeListener(a))
                         };
-                        this.addListener(l)
+                        this.addListener(a)
                     }))
                 }
                 sendMessage(e) {
                     return new Promise((t => {
                         var n;
                         null === (n = this._socket) || void 0 === n || n.send(JSON.stringify(e)), this._sendResolverQueue.push(t)
                     }))
@@ -696,15 +907,15 @@
                     t > -1 && this._listeners.splice(t, 1)
                 }
                 async getHistory() {
                     let e = {
                         messages: []
                     };
                     try {
-                        e = await X("chats/history", {
+                        e = await $("chats/history", {
                             method: "GET"
                         })
                     } catch (e) {
                         return Promise.reject(e)
                     }
                     return e
                 }
@@ -718,53 +929,53 @@
                     e && (this._socket = null, e.onopen = () => {}, e.onerror = () => {}, e.onmessage = () => {}, e.onclose = () => {}, e.close())
                 }
                 _onMessage(e) {
                     var t;
                     "human" === e.type && e.client.id === this.id && (null === (t = this._sendResolverQueue.shift()) || void 0 === t || t(e.id)), "agent" === e.type && e.reply_to in this._replyForResolverDict && (this._replyForResolverDict[e.reply_to](e), delete this._replyForResolverDict[e.reply_to]), this._listeners.forEach((t => t(e)))
                 }
             }
-            const te = {
+            const ce = {
                 id: "jupyter_ai:plugin",
                 autoStart: !0,
-                optional: [r.IGlobalAwareness, o.ILayoutRestorer],
+                optional: [o.IGlobalAwareness, r.ILayoutRestorer],
                 activate: async (e, t, n) => {
-                    const o = new Q(e.shell),
-                        r = new ee;
-                    let s = null;
+                    const r = new ae(e.shell),
+                        o = new se;
+                    let i = null;
                     try {
-                        await r.initialize(), s = function(e, t, n) {
-                            const o = l.ReactWidget.create(i().createElement(F, {
+                        await o.initialize(), i = function(e, t, n) {
+                            const r = a.ReactWidget.create(l().createElement(X, {
                                 selectionWatcher: e,
                                 chatHandler: t,
                                 globalAwareness: n
                             }));
-                            return o.id = "jupyter-ai::chat", o.title.icon = W, o.title.caption = "Jupyter AI Chat", o
-                        }(o, r, t)
+                            return r.id = "jupyter-ai::chat", r.title.icon = F, r.title.caption = "Jupyter AI Chat", r
+                        }(r, o, t)
                     } catch (e) {
-                        s = function() {
-                            const e = l.ReactWidget.create(i().createElement(p, null, i().createElement(m.Box, {
+                        i = function() {
+                            const e = a.ReactWidget.create(l().createElement(g, null, l().createElement(c.Box, {
                                 sx: {
                                     width: "100%",
                                     height: "100%",
                                     boxSizing: "border-box",
                                     background: "var(--jp-layout-color0)",
                                     display: "flex",
                                     flexDirection: "column"
                                 }
-                            }, i().createElement(m.Box, {
+                            }, l().createElement(c.Box, {
                                 sx: {
                                     padding: 4
                                 }
-                            }, i().createElement(m.Alert, {
+                            }, l().createElement(c.Alert, {
                                 severity: "error"
                             }, "There seems to be a problem with the Chat backend, please look at the JupyterLab server logs or contact your administrator to correct this problem.")))));
-                            return e.id = "jupyter-ai::chat", e.title.icon = W, e.title.caption = "Jupyter AI Chat", e
+                            return e.id = "jupyter-ai::chat", e.title.icon = F, e.title.caption = "Jupyter AI Chat", e
                         }()
                     }
-                    e.shell.add(s, "left", {
+                    e.shell.add(i, "left", {
                         rank: 2e3
-                    }), n && n.add(s, "jupyter-ai-chat")
+                    }), n && n.add(i, "jupyter-ai-chat")
                 }
             }
         }
     }
 ]);
```

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/92.8c406c1018e3357f19d8.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/92.8c406c1018e3357f19d8.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/964.1d210ce1e570332cead5.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/964.1d210ce1e570332cead5.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/990.ef9212deeffc976b3352.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/990.ef9212deeffc976b3352.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/remoteEntry.585abad92d66f32304a2.js` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/remoteEntry.a041aa160809d9fa05d2.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, o, n, i, f, l, d, c, u, s, p, h, b, m, v, y, g, j, P, w, k, _, O = {
+    var e, r, t, a, o, n, i, l, f, d, c, u, s, p, h, b, m, v, y, g, j, P, w, k, _, O = {
             22399: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(675), t.e(673), t.e(271), t.e(222), t.e(787)]).then((() => () => t(65787))),
-                        "./extension": () => Promise.all([t.e(675), t.e(673), t.e(271), t.e(222), t.e(787)]).then((() => () => t(65787))),
+                        "./index": () => Promise.all([t.e(675), t.e(460), t.e(271), t.e(222), t.e(639)]).then((() => () => t(11639))),
+                        "./extension": () => Promise.all([t.e(675), t.e(460), t.e(271), t.e(222), t.e(639)]).then((() => () => t(11639))),
                         "./style": () => t.e(643).then((() => () => t(76643)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     n = (e, r) => {
                         if (t.S) {
@@ -63,82 +63,82 @@
         92: "8c406c1018e3357f19d8",
         165: "9dda3cd58dc434a135e2",
         211: "07dc02de739c8581fa0e",
         222: "17df77bb621ad2efa277",
         271: "fef2c73c25d43d569231",
         296: "bda9232f6e5ca4db8f1c",
         456: "3fad6902bcadafa972d3",
+        460: "1a227a7f70bb8e160091",
         465: "d994a7f1c5808a09fbe5",
         560: "2fa7b4ae7a0d43e8eb1f",
         586: "d8af1e48008aba81c9a4",
+        639: "ba44eea9c8de7134d76e",
         641: "55df6eadf8891e5a1bbe",
-        643: "3e00b12acf02dce55cc2",
-        673: "68e7ac52ccd7076d341f",
+        643: "d05f12a52798d8475b12",
         675: "73a31f502181054c8492",
         698: "db0bf7bc349a78b068d5",
         703: "d52ed379ae2e07ba3d54",
         710: "92355af1c50cee7b836f",
         785: "89e5ffc932d4302b02fa",
-        787: "7f6980b88a058f8d58c8",
         799: "b2bec652471d9e2c00d9",
         964: "1d210ce1e570332cead5",
         990: "ef9212deeffc976b3352"
     } [e] + ".js?v=" + {
         92: "8c406c1018e3357f19d8",
         165: "9dda3cd58dc434a135e2",
         211: "07dc02de739c8581fa0e",
         222: "17df77bb621ad2efa277",
         271: "fef2c73c25d43d569231",
         296: "bda9232f6e5ca4db8f1c",
         456: "3fad6902bcadafa972d3",
+        460: "1a227a7f70bb8e160091",
         465: "d994a7f1c5808a09fbe5",
         560: "2fa7b4ae7a0d43e8eb1f",
         586: "d8af1e48008aba81c9a4",
+        639: "ba44eea9c8de7134d76e",
         641: "55df6eadf8891e5a1bbe",
-        643: "3e00b12acf02dce55cc2",
-        673: "68e7ac52ccd7076d341f",
+        643: "d05f12a52798d8475b12",
         675: "73a31f502181054c8492",
         698: "db0bf7bc349a78b068d5",
         703: "d52ed379ae2e07ba3d54",
         710: "92355af1c50cee7b836f",
         785: "89e5ffc932d4302b02fa",
-        787: "7f6980b88a058f8d58c8",
         799: "b2bec652471d9e2c00d9",
         964: "1d210ce1e570332cead5",
         990: "ef9212deeffc976b3352"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), t = {}, a = "@jupyter-ai/core:", E.l = (e, r, o, n) => {
         if (t[e]) t[e].push(r);
         else {
-            var i, f;
+            var i, l;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
-                    var c = l[d];
+                for (var f = document.getElementsByTagName("script"), d = 0; d < f.length; d++) {
+                    var c = f[d];
                     if (c.getAttribute("src") == e || c.getAttribute("data-webpack") == a + o) {
                         i = c;
                         break
                     }
                 }
-            i || (f = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", a + o), i.src = e), t[e] = [r];
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", a + o), i.src = e), t[e] = [r];
             var u = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(s);
                     var o = t[e];
                     if (delete t[e], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(a))), r) return r(a)
                 },
                 s = setTimeout(u.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = u.bind(null, i.onerror), i.onload = u.bind(null, i.onload), f && document.head.appendChild(i)
+            i.onerror = u.bind(null, i.onerror), i.onload = u.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -150,25 +150,25 @@
             a || (a = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(a.indexOf(o) >= 0)) {
                 if (a.push(o), e[t]) return e[t];
                 E.o(E.S, t) || (E.S[t] = {});
                 var n = E.S[t],
                     i = "@jupyter-ai/core",
-                    f = (e, r, t, a) => {
+                    l = (e, r, t, a) => {
                         var o = n[e] = n[e] || {},
-                            f = o[r];
-                        (!f || !f.loaded && (!a != !f.eager ? a : i > f.from)) && (o[r] = {
+                            l = o[r];
+                        (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
-                    l = [];
-                return "default" === t && (f("@emotion/react", "11.10.5", (() => Promise.all([E.e(296), E.e(465), E.e(271), E.e(785)]).then((() => () => E(51465))))), f("@emotion/styled", "11.10.5", (() => Promise.all([E.e(92), E.e(271), E.e(211), E.e(799), E.e(560)]).then((() => () => E(43092))))), f("@jupyter-ai/core", "0.6.1", (() => Promise.all([E.e(675), E.e(673), E.e(271), E.e(222), E.e(787)]).then((() => () => E(65787))))), f("@mui/material", "5.11.8", (() => Promise.all([E.e(296), E.e(641), E.e(675), E.e(271), E.e(211), E.e(222), E.e(456)]).then((() => () => E(98641))))), f("date-fns", "2.29.3", (() => E.e(964).then((() => () => E(8964))))), f("react-markdown", "8.0.6", (() => Promise.all([E.e(698), E.e(165), E.e(271)]).then((() => () => E(4165))))), f("react-syntax-highlighter", "15.5.0", (() => Promise.all([E.e(990), E.e(271)]).then((() => () => E(67990))))), f("rehype-katex", "6.0.2", (() => Promise.all([E.e(698), E.e(586)]).then((() => () => E(66586))))), f("remark-math", "5.1.1", (() => E.e(703).then((() => () => E(7703)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                    f = [];
+                return "default" === t && (l("@emotion/react", "11.10.5", (() => Promise.all([E.e(296), E.e(465), E.e(271), E.e(785)]).then((() => () => E(51465))))), l("@emotion/styled", "11.10.5", (() => Promise.all([E.e(92), E.e(271), E.e(211), E.e(799), E.e(560)]).then((() => () => E(43092))))), l("@jupyter-ai/core", "0.7.0", (() => Promise.all([E.e(675), E.e(460), E.e(271), E.e(222), E.e(639)]).then((() => () => E(11639))))), l("@mui/material", "5.11.8", (() => Promise.all([E.e(296), E.e(641), E.e(675), E.e(271), E.e(211), E.e(222), E.e(456)]).then((() => () => E(98641))))), l("date-fns", "2.29.3", (() => E.e(964).then((() => () => E(8964))))), l("react-markdown", "8.0.6", (() => Promise.all([E.e(698), E.e(165), E.e(271)]).then((() => () => E(4165))))), l("react-syntax-highlighter", "15.5.0", (() => Promise.all([E.e(990), E.e(271)]).then((() => () => E(67990))))), l("rehype-katex", "6.0.2", (() => Promise.all([E.e(698), E.e(586)]).then((() => () => E(66586))))), l("remark-math", "5.1.1", (() => E.e(703).then((() => () => E(7703)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -186,98 +186,98 @@
         e = o(e), r = o(r);
         for (var t = 0;;) {
             if (t >= e.length) return t < r.length && "u" != (typeof r[t])[0];
             var a = e[t],
                 n = (typeof a)[0];
             if (t >= r.length) return "u" == n;
             var i = r[t],
-                f = (typeof i)[0];
-            if (n != f) return "o" == n && "n" == f || "s" == f || "u" == n;
+                l = (typeof i)[0];
+            if (n != l) return "o" == n && "n" == l || "s" == l || "u" == n;
             if ("o" != n && "u" != n && a != i) return a < i;
             t++
         }
     }, i = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(f = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, f);
+            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
             return t
         }
         var n = [];
         for (o = 1; o < e.length; o++) {
-            var f = e[o];
-            n.push(0 === f ? "not(" + l() + ")" : 1 === f ? "(" + l() + " || " + l() + ")" : 2 === f ? n.pop() + " " + n.pop() : i(f))
+            var l = e[o];
+            n.push(0 === l ? "not(" + f() + ")" : 1 === l ? "(" + f() + " || " + f() + ")" : 2 === l ? n.pop() + " " + n.pop() : i(l))
         }
-        return l();
+        return f();
 
-        function l() {
+        function f() {
             return n.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, f = (e, r) => {
+    }, l = (e, r) => {
         if (0 in e) {
             r = o(r);
             var t = e[0],
                 a = t < 0;
             a && (t = -t - 1);
-            for (var n = 0, i = 1, l = !0;; i++, n++) {
+            for (var n = 0, i = 1, f = !0;; i++, n++) {
                 var d, c, u = i < e.length ? (typeof e[i])[0] : "";
-                if (n >= r.length || "o" == (c = (typeof(d = r[n]))[0])) return !l || ("u" == u ? i > t && !a : "" == u != a);
+                if (n >= r.length || "o" == (c = (typeof(d = r[n]))[0])) return !f || ("u" == u ? i > t && !a : "" == u != a);
                 if ("u" == c) {
-                    if (!l || "u" != u) return !1
-                } else if (l)
+                    if (!f || "u" != u) return !1
+                } else if (f)
                     if (u == c)
                         if (i <= t) {
                             if (d != e[i]) return !1
                         } else {
                             if (a ? d > e[i] : d < e[i]) return !1;
-                            d != e[i] && (l = !1)
+                            d != e[i] && (f = !1)
                         }
                 else if ("s" != u && "n" != u) {
                     if (a || i <= t) return !1;
-                    l = !1, i--
+                    f = !1, i--
                 } else {
                     if (i <= t || c < u != a) return !1;
-                    l = !1
-                } else "s" != u && "n" != u && (l = !1, i--)
+                    f = !1
+                } else "s" != u && "n" != u && (f = !1, i--)
             }
         }
         var s = [],
             p = s.pop.bind(s);
         for (n = 1; n < e.length; n++) {
             var h = e[n];
-            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? f(h, r) : !p())
+            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? l(h, r) : !p())
         }
         return !!p()
-    }, l = (e, r) => {
+    }, f = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, c = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(a) + ")", s = (e, r, t, a) => {
         var o = c(e, t);
-        return f(a, o) || "undefined" != typeof console && console.warn && console.warn(u(e, t, o, a)), m(e[t][o])
+        return l(a, o) || "undefined" != typeof console && console.warn && console.warn(u(e, t, o, a)), m(e[t][o])
     }, p = (e, r, t) => {
         var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !f(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
+        return (r = Object.keys(a).reduce(((e, r) => !l(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
     }, h = (e, r, t, a) => {
         var o = e[t];
         return "No satisfying version (" + i(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
     }, b = (e, r, t, a) => {
         "undefined" != typeof console && console.warn && console.warn(h(e, r, t, a))
     }, m = e => (e.loaded = 1, e.get()), y = (v = e => function(r, t, a, o) {
         var n = E.I(r);
         return n && n.then ? n.then(e.bind(e, r, E.S[r], t, a, o)) : e(r, E.S[r], t, a, o)
-    })(((e, r, t, a) => r && E.o(r, t) ? m(d(r, t)) : a())), g = v(((e, r, t, a) => (l(e, t), m(p(r, t, a) || b(r, e, t, a) || d(r, t))))), j = v(((e, r, t, a) => (l(e, t), s(r, 0, t, a)))), P = v(((e, r, t, a, o) => {
+    })(((e, r, t, a) => r && E.o(r, t) ? m(d(r, t)) : a())), g = v(((e, r, t, a) => (f(e, t), m(p(r, t, a) || b(r, e, t, a) || d(r, t))))), j = v(((e, r, t, a) => (f(e, t), s(r, 0, t, a)))), P = v(((e, r, t, a, o) => {
         var n = r && E.o(r, t) && p(r, t, a);
         return n ? m(n) : o()
     })), w = {}, k = {
         56271: () => j("default", "react", [1, 17, 0, 1]),
         28800: () => P("default", "@emotion/styled", [1, 11, 3, 0], (() => Promise.all([E.e(92), E.e(211), E.e(799)]).then((() => () => E(43092))))),
         62148: () => P("default", "@emotion/react", [1, 11, 4, 1], (() => Promise.all([E.e(296), E.e(465), E.e(710)]).then((() => () => E(51465))))),
         13191: () => P("default", "@mui/material", [1, 5, 11, 0], (() => Promise.all([E.e(296), E.e(641), E.e(211), E.e(456)]).then((() => () => E(98641))))),
@@ -302,15 +302,15 @@
         40799: () => P("default", "@emotion/react", [1, 11, 0, 0, , "rc", 0], (() => Promise.all([E.e(296), E.e(465)]).then((() => () => E(51465))))),
         14456: () => j("default", "react-dom", [1, 17, 0, 1])
     }, _ = {
         211: [85211],
         222: [28800, 62148],
         271: [56271],
         456: [14456],
-        787: [13191, 22502, 26413, 28142, 35059, 40532, 41123, 45687, 48820, 48942, 51473, 71840, 72647, 73033, 77986, 78918, 80819, 96707],
+        639: [13191, 22502, 26413, 28142, 35059, 40532, 41123, 45687, 48820, 48942, 51473, 71840, 72647, 73033, 77986, 78918, 80819, 96707],
         799: [40799]
     }, E.f.consumes = (e, r) => {
         E.o(_, e) && _[e].forEach((e => {
             if (E.o(w, e)) return r.push(w[e]);
             var t = r => {
                     w[e] = 0, E.m[e] = t => {
                         delete E.c[e], t.exports = r()
@@ -348,21 +348,21 @@
                             n = t && t.target && t.target.src;
                         i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", i.name = "ChunkLoadError", i.type = o, i.request = n, a[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var a, o, [n, i, f] = t,
-                    l = 0;
+                var a, o, [n, i, l] = t,
+                    f = 0;
                 if (n.some((r => 0 !== e[r]))) {
                     for (a in i) E.o(i, a) && (E.m[a] = i[a]);
-                    f && f(E)
+                    l && l(E)
                 }
-                for (r && r(t); l < n.length; l++) o = n[l], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); f < n.length; f++) o = n[f], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_jupyter_ai_core = self.webpackChunk_jupyter_ai_core || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), E.nc = void 0;
     var x = E(22399);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyter-ai/core"] = x
 })();
```

### Comparing `jupyter_ai-0.6.1/jupyter_ai/labextension/static/third-party-licenses.json` & `jupyter_ai-0.7.0/jupyter_ai/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/schema/plugin.json` & `jupyter_ai-0.7.0/schema/plugin.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'jupyter.lab.setting-icon'": "'jupyter-ai::chat'"}*

```diff
@@ -26,15 +26,15 @@
                 "command": "ai:generate-from-editor-selection",
                 "name": "ai:generate-from-editor-selection",
                 "rank": 520,
                 "selector": ".jp-FileEditor"
             }
         ]
     },
-    "jupyter.lab.setting-icon": "jupyter-ai::psychology",
+    "jupyter.lab.setting-icon": "jupyter-ai::chat",
     "jupyter.lab.setting-icon-label": "Jupyter AI Chat",
     "jupyter.lab.toolbars": {
         "Cell": [
             {
                 "command": "ai:explain-or-codify-cell",
                 "name": "ai:explain-or-codify-cell",
                 "rank": 10
```

### Comparing `jupyter_ai-0.6.1/src/chat_handler.ts` & `jupyter_ai-0.7.0/src/chat_handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/src/index.ts` & `jupyter_ai-0.7.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/src/inserter.ts` & `jupyter_ai-0.7.0/src/inserter.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/src/selection-watcher.ts` & `jupyter_ai-0.7.0/src/selection-watcher.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/src/theme-provider.ts` & `jupyter_ai-0.7.0/src/theme-provider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/src/utils.ts` & `jupyter_ai-0.7.0/src/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/src/__tests__/widgets/closable-dialog.spec.tsx` & `jupyter_ai-0.7.0/src/__tests__/widgets/closable-dialog.spec.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/src/components/chat-code-view.tsx` & `jupyter_ai-0.7.0/src/components/chat-code-view.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import React, { useState, useMemo } from 'react';
 
 import type { CodeProps } from 'react-markdown/lib/ast-to-react';
 import { Prism as SyntaxHighlighter } from 'react-syntax-highlighter';
 import { duotoneLight } from 'react-syntax-highlighter/dist/esm/styles/prism';
 import { Box, Button } from '@mui/material';
+import cx from 'clsx';
 
 type ChatCodeViewProps = CodeProps;
 
 type ChatCodeInlineProps = ChatCodeViewProps;
 
 type ChatCodeBlockProps = ChatCodeViewProps & {
   language?: string;
 };
 
+const JPAI_CODE_CLASS = 'jp-ai-code';
+
 function ChatCodeInline({
   className,
   children,
   ...props
 }: ChatCodeInlineProps) {
   return (
-    <code {...props} className={className}>
+    <code {...props} className={cx(JPAI_CODE_CLASS, className)}>
       {children}
     </code>
   );
 }
 
 enum CopyStatus {
   None,
@@ -55,14 +58,15 @@
     setTimeout(() => setCopyStatus(CopyStatus.None), 1000);
   };
 
   return (
     <Box sx={{ display: 'flex', flexDirection: 'column' }}>
       <SyntaxHighlighter
         {...props}
+        className={cx(props.className, JPAI_CODE_CLASS)}
         children={value}
         style={duotoneLight}
         language={language}
         PreTag="div"
       />
       <Button
         onClick={copy}
```

### Comparing `jupyter_ai-0.6.1/src/components/chat-input.tsx` & `jupyter_ai-0.7.0/src/components/chat-input.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -18,44 +18,50 @@
   onChange: (newValue: string) => unknown;
   onSend: () => unknown;
   hasSelection: boolean;
   includeSelection: boolean;
   toggleIncludeSelection: () => unknown;
   replaceSelection: boolean;
   toggleReplaceSelection: () => unknown;
+  helperText: JSX.Element
   sx?: SxProps<Theme>;
 };
 
 export function ChatInput(props: ChatInputProps): JSX.Element {
+  
   function handleKeyDown(event: React.KeyboardEvent<HTMLInputElement>) {
     if (event.key === 'Enter' && event.shiftKey) {
       props.onSend();
       event.stopPropagation();
       event.preventDefault();
     }
   }
   return (
     <Box sx={props.sx}>
-      <Box sx={{ display: 'flex' }}>
+      <Box sx={{ display: 'flex'}}>
         <TextField
           value={props.value}
           onChange={e => props.onChange(e.target.value)}
           fullWidth
           variant="outlined"
           multiline
           onKeyDown={handleKeyDown}
           InputProps={{
             endAdornment: (
                <InputAdornment position="end">
                   <IconButton size="small" color="primary" onClick={props.onSend} disabled={!props.value.trim().length}>
                      <SendIcon />
                   </IconButton>
                </InputAdornment>
-            ),
+            )
          }}
+         FormHelperTextProps={{
+          sx: {marginLeft: 'auto', marginRight: 0}
+         }}
+         helperText={props.value.length > 2 ? props.helperText : ' '}
         />
       </Box>
       {props.hasSelection && (
         <FormGroup sx={{ display: 'flex', flexDirection: 'row' }}>
           <FormControlLabel
             control={
               <Checkbox
```

### Comparing `jupyter_ai-0.6.1/src/components/chat-messages.tsx` & `jupyter_ai-0.7.0/src/components/chat-messages.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import React, { useState, useEffect } from 'react';
 
 import { Avatar, Box, Typography } from '@mui/material';
 import type { SxProps, Theme } from '@mui/material';
-import PsychologyIcon from '@mui/icons-material/Psychology';
 import { formatDistanceToNowStrict, fromUnixTime } from 'date-fns';
 import ReactMarkdown from 'react-markdown';
 import remarkMath from 'remark-math';
 import rehypeKatex from 'rehype-katex';
 import 'katex/dist/katex.min.css';
 
 import { ChatCodeView } from './chat-code-view';
 import { AiService } from '../handler';
 import { useCollaboratorsContext } from '../contexts/collaborators-context';
+import { Jupyternaut } from '../icons';
 
 type ChatMessagesProps = {
   messages: AiService.ChatMessage[];
 };
 
 type ChatMessageHeaderProps = {
   message: AiService.ChatMessage;
@@ -50,23 +50,23 @@
           {props.message.client.initials}
         </Typography>
       </Avatar>
     );
   } else {
     avatar = (
       <Avatar sx={{ ...sharedStyles, bgcolor: 'var(--jp-jupyter-icon-color)' }}>
-        <PsychologyIcon />
+        <Jupyternaut display="block" height="100%" width="100%" />
       </Avatar>
     );
   }
 
   const name =
     props.message.type === 'human'
       ? props.message.client.display_name
-      : 'Jupyter AI';
+      : 'Jupyternaut';
 
   return (
     <Box
       sx={{
         display: 'flex',
         alignItems: 'center',
         '& > :not(:last-child)': {
@@ -81,16 +81,24 @@
           display: 'flex',
           flexGrow: 1,
           flexWrap: 'wrap',
           justifyContent: 'space-between',
           alignItems: 'center'
         }}
       >
-        <Typography sx={{ fontWeight: 700, color: 'var(--jp-ui-font-color1)' }}>{name}</Typography>
-        <Typography sx={{ fontSize: '0.8em', color: 'var(--jp-ui-font-color2)', fontWeight: 300 }}>
+        <Typography sx={{ fontWeight: 700, color: 'var(--jp-ui-font-color1)' }}>
+          {name}
+        </Typography>
+        <Typography
+          sx={{
+            fontSize: '0.8em',
+            color: 'var(--jp-ui-font-color2)',
+            fontWeight: 300
+          }}
+        >
           {props.timestamp}
         </Typography>
       </Box>
     </Box>
   );
 }
 
@@ -116,15 +124,19 @@
     return () => {
       clearInterval(intervalId);
     };
   }, [props.messages]);
 
   return (
     <Box
-      sx={{ '& > :not(:last-child)': { borderBottom: '1px solid var(--jp-border-color2)' } }}
+      sx={{
+        '& > :not(:last-child)': {
+          borderBottom: '1px solid var(--jp-border-color2)'
+        }
+      }}
     >
       {props.messages.map((message, i) => (
         // extra div needed to ensure each bubble is on a new line
         <Box key={i} sx={{ padding: 4 }}>
           <ChatMessageHeader
             message={message}
             timestamp={timestamps[message.id]}
```

### Comparing `jupyter_ai-0.6.1/src/components/chat.tsx` & `jupyter_ai-0.7.0/src/components/chat.tsx`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,58 @@
 import React, { useState, useEffect } from 'react';
 import { Box } from '@mui/system';
+import { Button, IconButton, Stack } from '@mui/material';
+import SettingsIcon from '@mui/icons-material/Settings';
+import ArrowBackIcon from '@mui/icons-material/ArrowBack';
 import type { Awareness } from 'y-protocols/awareness';
 
 import { JlThemeProvider } from './jl-theme-provider';
 import { ChatMessages } from './chat-messages';
 import { ChatInput } from './chat-input';
+import { ChatSettings } from './chat-settings';
 import { AiService } from '../handler';
 import {
   SelectionContextProvider,
   useSelectionContext
 } from '../contexts/selection-context';
 import { SelectionWatcher } from '../selection-watcher';
 import { ChatHandler } from '../chat_handler';
 import { CollaboratorsContextProvider } from '../contexts/collaborators-context';
 import { ScrollContainer } from './scroll-container';
 
 type ChatBodyProps = {
   chatHandler: ChatHandler;
+  setChatView: (view: ChatView) => void
 };
 
-function ChatBody({ chatHandler }: ChatBodyProps): JSX.Element {
+function ChatBody({ chatHandler, setChatView: chatViewHandler }: ChatBodyProps): JSX.Element {
   const [messages, setMessages] = useState<AiService.ChatMessage[]>([]);
+  const [showWelcomeMessage, setShowWelcomeMessage] = useState<boolean>(false);
   const [includeSelection, setIncludeSelection] = useState(true);
   const [replaceSelection, setReplaceSelection] = useState(false);
   const [input, setInput] = useState('');
   const [selection, replaceSelectionFn] = useSelectionContext();
 
   /**
    * Effect: fetch history on initial render
    */
   useEffect(() => {
     async function fetchHistory() {
       try {
-        const history = await chatHandler.getHistory();
+        const [history, config] = await Promise.all([
+          chatHandler.getHistory(),
+          AiService.getConfig()
+        ]);
         setMessages(history.messages);
+        if (!config.model_provider_id) {
+          setShowWelcomeMessage(true);
+        }
       } catch (e) {
-        
+        console.error(e);
       }
-      
     }
 
     fetchHistory();
   }, [chatHandler]);
 
   /**
    * Effect: listen to chat messages
@@ -67,15 +78,17 @@
   // no need to append to messageGroups imperatively here. all of that is
   // handled by the listeners registered in the effect hooks above.
   const onSend = async () => {
     setInput('');
 
     const prompt =
       input +
-      (includeSelection && selection?.text ? '\n\n```\n' + selection.text + '```': '');
+      (includeSelection && selection?.text
+        ? '\n\n```\n' + selection.text + '\n```'
+        : '');
 
     // send message to backend
     const messageId = await chatHandler.sendMessage({ prompt });
 
     // await reply from agent
     // no need to append to messageGroups state variable, since that's already
     // handled in the effect hooks.
@@ -86,31 +99,53 @@
         ...selectionProps,
         ...(cellId && { cellId }),
         text: reply.body
       });
     }
   };
 
+  const openSettingsView = () => {
+    setShowWelcomeMessage(false)
+    chatViewHandler(ChatView.Settings)
+  }
+
+  if (showWelcomeMessage) {
+    return (
+      <Box
+        sx={{
+          padding: 4,
+          display: 'flex',
+          flexGrow: 1,
+          alignItems: 'top',
+          justifyContent: 'space-around'
+        }}
+      >
+        <Stack spacing={4}>
+          <p>
+            Welcome to Jupyter AI! To get started, please select a language
+            model to chat with from the settings panel. You will also likely
+            need to provide API credentials, so be sure to have those handy.
+          </p>
+          <Button 
+            variant="contained" 
+            startIcon={<SettingsIcon />} 
+            size={'large'}
+            onClick={() => openSettingsView()}
+            >
+              Start Here
+          </Button>
+        </Stack>
+      </Box>
+    );
+  }
+
   return (
-    <Box
-      // root box should not include padding as it offsets the vertical
-      // scrollbar to the left
-      sx={{
-        width: '100%',
-        height: '100%',
-        boxSizing: 'border-box',
-        background: 'var(--jp-layout-color0)',
-        display: 'flex',
-        flexDirection: 'column'
-      }}
-    >
+    <>
       <ScrollContainer sx={{ flexGrow: 1 }}>
         <ChatMessages messages={messages} />
-        {/* https://css-tricks.com/books/greatest-css-tricks/pin-scrolling-to-bottom/ */}
-        <Box sx={{ overflowAnchor: 'auto', height: '1px' }} />
       </ScrollContainer>
       <ChatInput
         value={input}
         onChange={setInput}
         onSend={onSend}
         hasSelection={!!selection?.text}
         includeSelection={includeSelection}
@@ -120,33 +155,80 @@
         replaceSelection={replaceSelection}
         toggleReplaceSelection={() =>
           setReplaceSelection(replaceSelection => !replaceSelection)
         }
         sx={{
           paddingLeft: 4,
           paddingRight: 4,
-          paddingTop: 2,
-          paddingBottom: 2,
+          paddingTop: 3.5,
+          paddingBottom: 0,
           borderTop: '1px solid var(--jp-border-color1)'
         }}
+        helperText={
+          <span>
+            Press <b>Shift</b> + <b>Enter</b> to submit message
+          </span>
+        }
       />
-    </Box>
+    </>
   );
 }
 
 export type ChatProps = {
   selectionWatcher: SelectionWatcher;
   chatHandler: ChatHandler;
   globalAwareness: Awareness | null;
+  chatView?: ChatView
 };
 
+enum ChatView {
+  Chat,
+  Settings
+}
+
 export function Chat(props: ChatProps) {
+  const [view, setView] = useState<ChatView>(props.chatView || ChatView.Chat);
+
   return (
     <JlThemeProvider>
       <SelectionContextProvider selectionWatcher={props.selectionWatcher}>
         <CollaboratorsContextProvider globalAwareness={props.globalAwareness}>
-          <ChatBody chatHandler={props.chatHandler} />
+          <Box
+            // root box should not include padding as it offsets the vertical
+            // scrollbar to the left
+            sx={{
+              width: '100%',
+              height: '100%',
+              boxSizing: 'border-box',
+              background: 'var(--jp-layout-color0)',
+              display: 'flex',
+              flexDirection: 'column'
+            }}
+          >
+            {/* top bar */}
+            <Box sx={{ display: 'flex', justifyContent: 'space-between' }}>
+              {view !== ChatView.Chat ? (
+                <IconButton onClick={() => setView(ChatView.Chat)}>
+                  <ArrowBackIcon />
+                </IconButton>
+              ) : (
+                <Box />
+              )}
+              {view === ChatView.Chat ? (
+                <IconButton onClick={() => setView(ChatView.Settings)}>
+                  <SettingsIcon />
+                </IconButton>
+              ) : (
+                <Box />
+              )}
+            </Box>
+            {/* body */}
+            {view === ChatView.Chat && (
+              <ChatBody chatHandler={props.chatHandler} setChatView={setView}/>
+            )}
+            {view === ChatView.Settings && <ChatSettings />}
+          </Box>
         </CollaboratorsContextProvider>
       </SelectionContextProvider>
     </JlThemeProvider>
   );
 }
```

### Comparing `jupyter_ai-0.6.1/src/components/expandable-text-field.tsx` & `jupyter_ai-0.7.0/src/components/expandable-text-field.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/src/components/jl-theme-provider.tsx` & `jupyter_ai-0.7.0/src/components/jl-theme-provider.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/src/components/open-task-dialog.tsx` & `jupyter_ai-0.7.0/src/components/open-task-dialog.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/src/components/scroll-container.tsx` & `jupyter_ai-0.7.0/src/components/scroll-container.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/src/contexts/collaborators-context.tsx` & `jupyter_ai-0.7.0/src/contexts/collaborators-context.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/src/contexts/selection-context.tsx` & `jupyter_ai-0.7.0/src/contexts/selection-context.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/src/widgets/chat-error.tsx` & `jupyter_ai-0.7.0/src/widgets/chat-error.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/src/widgets/chat-sidebar.tsx` & `jupyter_ai-0.7.0/src/widgets/chat-sidebar.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/src/widgets/closable-dialog.tsx` & `jupyter_ai-0.7.0/src/widgets/closable-dialog.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/ui-tests/README.md` & `jupyter_ai-0.7.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/ui-tests/jupyter_server_test_config.py` & `jupyter_ai-0.7.0/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/ui-tests/tests/jupyter_ai.spec.ts` & `jupyter_ai-0.7.0/ui-tests/tests/jupyter_ai.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/.gitignore` & `jupyter_ai-0.7.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -115,15 +115,12 @@
 .pyre/
 
 # End of https://www.gitignore.io/api/python
 
 # OSX files
 .DS_Store
 
-# local config storing authn credentials
-config.py
-
 # vscode
 .vscode
 
 # Coverage reports
 coverage/*
```

### Comparing `jupyter_ai-0.6.1/LICENSE` & `jupyter_ai-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.1/README.md` & `jupyter_ai-0.7.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -7,29 +7,43 @@
 for the server extension and a NPM package named `jupyter_ai`
 for the frontend extension.
 
 ## Requirements
 
 - JupyterLab >= 3.5 (not JupyterLab 4)
 
-## Install
+## Installation
 
-To install the extension, execute:
+You can use `conda` or `pip` to install Jupyter AI. If you're using macOS on an Apple Silicon-based Mac (M1, M1 Pro, M2, etc.), we strongly recommend using `conda`.
 
-```bash
-pip install jupyter_ai
-```
+Because of Ray's incompatibility with Python 3.11, you must use Python 3.9, or 3.10 with Jupyter AI. The instructions below presume that you are using Python 3.10.
+
+Before you can use Jupyter AI, you will need to install any packages and set environment variables with API keys for the model providers that you will use. See [our documentation](https://jupyter-ai.readthedocs.io/en/latest/users/index.html) for details about what you'll need.
+
+### With pip
+
+    $ pip install jupyter_ai
+
+### With conda
+
+First, install [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) and create an environment that uses Python 3.10:
+
+    $ conda create -n jupyter-ai python=3.10
+    $ conda activate jupyter-ai
+    $ pip install jupyter_ai
+
+If you are using an Apple Silicon-based Mac (M1, M1 Pro, M2, etc.), you need to uninstall the `pip` provided version of `grpcio` and install the version provided by `conda` instead.
+
+    $ pip uninstall grpcio; conda install grpcio 
 
 ## Uninstall
 
 To remove the extension, execute:
 
-```bash
-pip uninstall jupyter_ai
-```
+    $ pip uninstall jupyter_ai
 
 ## Usage with GPT-3
 
 To use the `GPT3ModelEngine` in `jupyter_ai`, you will need an OpenAI API key.
 Copy the API key and then create a Jupyter config file locally at `config.py` to
 store the API key.
```

### Comparing `jupyter_ai-0.6.1/pyproject.toml` & `jupyter_ai-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 dependencies = [
     "jupyter_server>=1.6,<3",
     "jupyterlab>=3.5,<4",
     "pydantic",
     "openai~=0.26",
     "aiosqlite~=0.18",
     "importlib_metadata~=5.2.0",
-    "langchain==0.0.153",
+    "langchain==0.0.158",
     "tiktoken", # required for OpenAIEmbeddings
     "jupyter_ai_magics",
-    "ray==2.2.0", # latest ray version 2.3.0 requires grpcio installation from conda
+    "ray~=2.4.0", # Requires grpcio installation from conda
     "faiss-cpu", # Not distributed by official repo
     "wcmatch",
 ]
 
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.entry-points."jupyter_ai.model_engine_classes"]
```

### Comparing `jupyter_ai-0.6.1/PKG-INFO` & `jupyter_ai-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai
-Version: 0.6.1
+Version: 0.7.0
 Summary: A generative AI extension for JupyterLab
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -51,18 +51,18 @@
 Requires-Python: <3.11,>=3.7
 Requires-Dist: aiosqlite~=0.18
 Requires-Dist: faiss-cpu
 Requires-Dist: importlib-metadata~=5.2.0
 Requires-Dist: jupyter-ai-magics
 Requires-Dist: jupyter-server<3,>=1.6
 Requires-Dist: jupyterlab<4,>=3.5
-Requires-Dist: langchain==0.0.153
+Requires-Dist: langchain==0.0.158
 Requires-Dist: openai~=0.26
 Requires-Dist: pydantic
-Requires-Dist: ray==2.2.0
+Requires-Dist: ray~=2.4.0
 Requires-Dist: tiktoken
 Requires-Dist: wcmatch
 Provides-Extra: all
 Requires-Dist: ai21; extra == 'all'
 Requires-Dist: anthropic; extra == 'all'
 Requires-Dist: boto3; extra == 'all'
 Requires-Dist: cohere; extra == 'all'
@@ -87,29 +87,43 @@
 for the server extension and a NPM package named `jupyter_ai`
 for the frontend extension.
 
 ## Requirements
 
 - JupyterLab >= 3.5 (not JupyterLab 4)
 
-## Install
+## Installation
 
-To install the extension, execute:
+You can use `conda` or `pip` to install Jupyter AI. If you're using macOS on an Apple Silicon-based Mac (M1, M1 Pro, M2, etc.), we strongly recommend using `conda`.
 
-```bash
-pip install jupyter_ai
-```
+Because of Ray's incompatibility with Python 3.11, you must use Python 3.9, or 3.10 with Jupyter AI. The instructions below presume that you are using Python 3.10.
+
+Before you can use Jupyter AI, you will need to install any packages and set environment variables with API keys for the model providers that you will use. See [our documentation](https://jupyter-ai.readthedocs.io/en/latest/users/index.html) for details about what you'll need.
+
+### With pip
+
+    $ pip install jupyter_ai
+
+### With conda
+
+First, install [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) and create an environment that uses Python 3.10:
+
+    $ conda create -n jupyter-ai python=3.10
+    $ conda activate jupyter-ai
+    $ pip install jupyter_ai
+
+If you are using an Apple Silicon-based Mac (M1, M1 Pro, M2, etc.), you need to uninstall the `pip` provided version of `grpcio` and install the version provided by `conda` instead.
+
+    $ pip uninstall grpcio; conda install grpcio 
 
 ## Uninstall
 
 To remove the extension, execute:
 
-```bash
-pip uninstall jupyter_ai
-```
+    $ pip uninstall jupyter_ai
 
 ## Usage with GPT-3
 
 To use the `GPT3ModelEngine` in `jupyter_ai`, you will need an OpenAI API key.
 Copy the API key and then create a Jupyter config file locally at `config.py` to
 store the API key.
```

