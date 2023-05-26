# Comparing `tmp/jupyter_ai-0.7.2.tar.gz` & `tmp/jupyter_ai-0.7.3.tar.gz`

## Comparing `jupyter_ai-0.7.2.tar` & `jupyter_ai-0.7.3.tar`

### file list

```diff
@@ -1,161 +1,161 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/.eslintignore
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/.eslintrc.js
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/.stylelintrc
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/CHANGELOG.md
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/babel.config.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/conftest.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jest.config.js
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/package.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/project.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/setup.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/tsconfig.json
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter-config/nb-config/jupyter_ai.json
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter-config/server-config/jupyter_ai.json
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/_version.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/engine.py
--rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/extension.py
--rw-r--r--   0        0        0    11067 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/handlers.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/models.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/reply_processor.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/task_manager.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/tasks.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/actors/__init__.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/actors/ask.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/actors/base.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/actors/chat_provider.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/actors/config.py
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/actors/default.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/actors/embeddings_provider.py
--rw-r--r--   0        0        0     9042 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/actors/generate.py
--rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/actors/learn.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/actors/memory.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/actors/providers.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/actors/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/document_loaders/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/document_loaders/directory.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/document_loaders/splitter.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/package.json
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json
--rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf
--rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf
--rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2
--rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf
--rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff
--rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf
--rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf
--rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf
--rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf
--rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js
--rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff
--rw-r--r--   0        0        0    41113 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js.LICENSE.txt
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/342.d3a98882c7231544e992.js
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/365.d20799d043a171f06d37.js
--rw-r--r--   0        0        0   157509 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/380.367f93b5ced659dcbadd.js
--rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf
--rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js.LICENSE.txt
--rw-r--r--   0        0        0  1568438 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js.LICENSE.txt
--rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff
--rw-r--r--   0        0        0    23748 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/639.4b9a03d6277bd8590eb1.js
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/643.d05f12a52798d8475b12.js
--rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/675.e2778aeb06575c94bca0.js
--rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf
--rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2
--rw-r--r--   0        0        0    21811 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/693.2c3da85cc10c904e2289.js
--rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/703.3d0d8b7012529f0dd511.js
--rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf
--rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2
--rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/819.5279f5daf1d1f505f15f.js
--rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff
--rw-r--r--   0        0        0   443772 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js.LICENSE.txt
--rw-r--r--   0        0        0    91736 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/861.f0852a9fe000bee67405.js
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/861.f0852a9fe000bee67405.js.LICENSE.txt
--rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff
--rw-r--r--   0        0        0   272943 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/900.aad7c14c6d8f76011810.js
--rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf
--rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff
--rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2
--rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff
--rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf
--rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff
--rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2
--rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff
--rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf
--rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff
--rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2
--rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff
--rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2
--rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff
--rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf
--rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf
--rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff
--rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf
--rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf
--rw-r--r--   0        0        0    11319 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/remoteEntry.9bfcf8f2600a893d38bf.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/style.js
--rw-r--r--   0        0        0   111460 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/tests/__init__.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/jupyter_ai/tests/test_handlers.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/schema/plugin.json
--rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/chat_handler.ts
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/handler.ts
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/icons.ts
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/index.ts
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/inserter.ts
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/selection-watcher.ts
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/theme-provider.ts
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/utils.ts
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/__tests__/jupyter_gai.spec.ts
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/__tests__/widgets/closable-dialog.spec.tsx
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/components/chat-code-view.tsx
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/components/chat-input.tsx
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/components/chat-messages.tsx
--rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/components/chat-settings.tsx
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/components/chat.tsx
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/components/expandable-text-field.tsx
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/components/jl-theme-provider.tsx
--rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/components/open-task-dialog.tsx
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/components/scroll-container.tsx
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/components/select.tsx
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/contexts/collaborators-context.tsx
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/contexts/selection-context.tsx
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/types/mui.d.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/types/svg.d.ts
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/widgets/chat-error.tsx
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/widgets/chat-sidebar.tsx
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/src/widgets/closable-dialog.tsx
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/style/base.css
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/style/expandable-text-field.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/style/index.js
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/style/react-markdown.css
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/style/icons/chat.svg
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/style/icons/jupyternaut.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/ui-tests/tests/jupyter_ai.spec.ts
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/LICENSE
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/README.md
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 jupyter_ai-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/.eslintignore
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/.eslintrc.js
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/.stylelintrc
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/CHANGELOG.md
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/babel.config.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/conftest.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jest.config.js
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/package.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/project.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/setup.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/tsconfig.json
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter-config/nb-config/jupyter_ai.json
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter-config/server-config/jupyter_ai.json
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/_version.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/engine.py
+-rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/extension.py
+-rw-r--r--   0        0        0    11040 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/handlers.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/models.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/reply_processor.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/task_manager.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/tasks.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/__init__.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/ask.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/base.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/chat_provider.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/config.py
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/default.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/embeddings_provider.py
+-rw-r--r--   0        0        0     9042 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/generate.py
+-rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/learn.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/memory.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/providers.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/document_loaders/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/document_loaders/directory.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/document_loaders/splitter.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/package.json
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json
+-rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf
+-rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf
+-rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2
+-rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf
+-rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff
+-rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf
+-rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf
+-rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf
+-rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf
+-rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js
+-rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff
+-rw-r--r--   0        0        0    41113 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js.LICENSE.txt
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/342.d3a98882c7231544e992.js
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/365.d20799d043a171f06d37.js
+-rw-r--r--   0        0        0   157509 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/380.367f93b5ced659dcbadd.js
+-rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf
+-rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js.LICENSE.txt
+-rw-r--r--   0        0        0  1568438 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js.LICENSE.txt
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff
+-rw-r--r--   0        0        0    23774 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/639.b63fa10cbcf2eccddd7d.js
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/643.d05f12a52798d8475b12.js
+-rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/675.e2778aeb06575c94bca0.js
+-rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2
+-rw-r--r--   0        0        0    21811 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/693.2c3da85cc10c904e2289.js
+-rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/703.3d0d8b7012529f0dd511.js
+-rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf
+-rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/819.5279f5daf1d1f505f15f.js
+-rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff
+-rw-r--r--   0        0        0   443772 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js.LICENSE.txt
+-rw-r--r--   0        0        0    91736 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/861.f0852a9fe000bee67405.js
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/861.f0852a9fe000bee67405.js.LICENSE.txt
+-rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff
+-rw-r--r--   0        0        0   272943 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/900.aad7c14c6d8f76011810.js
+-rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf
+-rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff
+-rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2
+-rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff
+-rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf
+-rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff
+-rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2
+-rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff
+-rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf
+-rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff
+-rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2
+-rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff
+-rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2
+-rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff
+-rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf
+-rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf
+-rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff
+-rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf
+-rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf
+-rw-r--r--   0        0        0    11319 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/remoteEntry.df84a6245b68ae8abd9f.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/style.js
+-rw-r--r--   0        0        0   111460 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/tests/__init__.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/tests/test_handlers.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/schema/plugin.json
+-rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/chat_handler.ts
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/handler.ts
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/icons.ts
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/index.ts
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/inserter.ts
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/selection-watcher.ts
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/theme-provider.ts
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/utils.ts
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/__tests__/jupyter_gai.spec.ts
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/__tests__/widgets/closable-dialog.spec.tsx
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/chat-code-view.tsx
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/chat-input.tsx
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/chat-messages.tsx
+-rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/chat-settings.tsx
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/chat.tsx
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/expandable-text-field.tsx
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/jl-theme-provider.tsx
+-rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/open-task-dialog.tsx
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/scroll-container.tsx
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/select.tsx
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/contexts/collaborators-context.tsx
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/contexts/selection-context.tsx
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/types/mui.d.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/types/svg.d.ts
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/widgets/chat-error.tsx
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/widgets/chat-sidebar.tsx
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/widgets/closable-dialog.tsx
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/style/base.css
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/style/expandable-text-field.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/style/index.js
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/style/react-markdown.css
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/style/icons/chat.svg
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/style/icons/jupyternaut.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/ui-tests/tests/jupyter_ai.spec.ts
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/LICENSE
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/README.md
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     9414 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/PKG-INFO
```

### Comparing `jupyter_ai-0.7.2/.eslintrc.js` & `jupyter_ai-0.7.3/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/RELEASE.md` & `jupyter_ai-0.7.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jest.config.js` & `jupyter_ai-0.7.3/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/package.json` & `jupyter_ai-0.7.3/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.7.3'"}*

```diff
@@ -121,9 +121,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.7.2"
+    "version": "0.7.3"
 }
```

### Comparing `jupyter_ai-0.7.2/tsconfig.json` & `jupyter_ai-0.7.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/__init__.py` & `jupyter_ai-0.7.3/jupyter_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/engine.py` & `jupyter_ai-0.7.3/jupyter_ai/engine.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/extension.py` & `jupyter_ai-0.7.3/jupyter_ai/extension.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/handlers.py` & `jupyter_ai-0.7.3/jupyter_ai/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,26 +157,26 @@
 
     async def get(self, *args, **kwargs):
         """Get an event socket."""
         self.pre_get()
         res = super().get(*args, **kwargs)
         await res
 
-    def get_current_user(self) -> ChatUser:
+    def get_chat_user(self) -> ChatUser:
         """Retrieves the current user. If collaborative mode is disabled, one
         is synthesized from the login."""
         collaborative = self.config.get("LabApp", {}).get("collaborative", False)
 
         if collaborative:
             return ChatUser(**asdict(self.current_user))
         
         
         login = getpass.getuser()
         return ChatUser(
-            username=self.current_user.username,
+            username=login,
             initials=login[0].capitalize(),
             name=login,
             display_name=login,
             color=None,
             avatar_url=None
         )
 
@@ -185,15 +185,15 @@
         """Generates a client ID to identify the current WS connection."""
         return uuid.uuid4().hex
 
     def open(self):
         """Handles opening of a WebSocket connection. Client ID can be retrieved
         from `self.client_id`."""
 
-        current_user = self.get_current_user().dict()
+        current_user = self.get_chat_user().dict()
         client_id = self.generate_client_id()
 
         self.chat_handlers[client_id] = self
         self.chat_clients[client_id] = ChatClient(**current_user, id=client_id)
         self.client_id = client_id
         self.write_message(ConnectionMessage(client_id=client_id).dict())
```

### Comparing `jupyter_ai-0.7.2/jupyter_ai/models.py` & `jupyter_ai-0.7.3/jupyter_ai/models.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/reply_processor.py` & `jupyter_ai-0.7.3/jupyter_ai/reply_processor.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/task_manager.py` & `jupyter_ai-0.7.3/jupyter_ai/task_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/tasks.py` & `jupyter_ai-0.7.3/jupyter_ai/tasks.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/actors/ask.py` & `jupyter_ai-0.7.3/jupyter_ai/actors/ask.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/actors/base.py` & `jupyter_ai-0.7.3/jupyter_ai/actors/base.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/actors/chat_provider.py` & `jupyter_ai-0.7.3/jupyter_ai/actors/chat_provider.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/actors/config.py` & `jupyter_ai-0.7.3/jupyter_ai/actors/config.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/actors/default.py` & `jupyter_ai-0.7.3/jupyter_ai/actors/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,26 +49,26 @@
             llm=llm,
             prompt=prompt_template,
             verbose=True,
             memory=self.memory
         )
     
     def clear_memory(self):
-        if not self.memory:
-            return
         
         # clear chain memory
-        self.memory.clear()
+        if self.memory:
+            self.memory.clear()
 
         # clear transcript for existing chat clients
         reply_message = ClearMessage()
         self.reply_queue.put(reply_message)
 
         # clear transcript for new chat clients
-        self.chat_history.clear()
+        if self.chat_history:
+            self.chat_history.clear()
 
     def _process_message(self, message: HumanChatMessage):
         self.get_llm_chain()
         response = self.llm_chain.predict(
             input=message.body,
             stop=["\nHuman:"]
         )
```

### Comparing `jupyter_ai-0.7.2/jupyter_ai/actors/embeddings_provider.py` & `jupyter_ai-0.7.3/jupyter_ai/actors/embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/actors/generate.py` & `jupyter_ai-0.7.3/jupyter_ai/actors/generate.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/actors/learn.py` & `jupyter_ai-0.7.3/jupyter_ai/actors/learn.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/actors/memory.py` & `jupyter_ai-0.7.3/jupyter_ai/actors/memory.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/actors/providers.py` & `jupyter_ai-0.7.3/jupyter_ai/actors/providers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/actors/router.py` & `jupyter_ai-0.7.3/jupyter_ai/actors/router.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/document_loaders/directory.py` & `jupyter_ai-0.7.3/jupyter_ai/document_loaders/directory.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/document_loaders/splitter.py` & `jupyter_ai-0.7.3/jupyter_ai/document_loaders/splitter.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/package.json` & `jupyter_ai-0.7.3/jupyter_ai/labextension/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745833333333334%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.df84a6245b68ae8abd9f.js'}}",*

 * * "'version'": "'0.7.3'"}*

```diff
@@ -59,15 +59,15 @@
         "schema/*.json",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter-ai",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.9bfcf8f2600a893d38bf.js",
+            "load": "static/remoteEntry.df84a6245b68ae8abd9f.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_ai"
                 },
@@ -126,9 +126,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.7.2"
+    "version": "0.7.3"
 }
```

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig` & `jupyter_ai-0.7.3/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.7.3'"}*

```diff
@@ -121,9 +121,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.7.2"
+    "version": "0.7.3"
 }
```

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json` & `jupyter_ai-0.7.3/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/342.d3a98882c7231544e992.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/342.d3a98882c7231544e992.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/365.d20799d043a171f06d37.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/365.d20799d043a171f06d37.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/380.367f93b5ced659dcbadd.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/380.367f93b5ced659dcbadd.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/639.4b9a03d6277bd8590eb1.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/639.b63fa10cbcf2eccddd7d.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,16 @@
                 const [t, n] = (0, l.useState)((0, m.Z)());
                 return (0, l.useEffect)((() => {
                     !async function() {
                         n(await async function() {
                             await async function() {
                                 for (; !document.body.hasAttribute("data-jp-theme-light");) await new Promise((e => setTimeout(e, 100)))
                             }();
-                            const e = document.body.getAttribute("data-jp-theme-light");
+                            const e = document.body.getAttribute("data-jp-theme-light"),
+                                t = p("--jp-ui-font-color1");
                             return (0, m.Z)({
                                 spacing: 4,
                                 components: {
                                     MuiButton: {
                                         defaultProps: {
                                             size: "small"
                                         }
@@ -125,28 +126,31 @@
                                     },
                                     success: {
                                         main: p("--jp-success-color1"),
                                         light: p("--jp-success-color2"),
                                         dark: p("--jp-success-color0")
                                     },
                                     text: {
-                                        primary: p("--jp-ui-font-color1"),
+                                        primary: t,
                                         secondary: p("--jp-ui-font-color2"),
                                         disabled: p("--jp-ui-font-color3")
                                     }
                                 },
                                 shape: {
                                     borderRadius: 2
                                 },
                                 typography: {
                                     fontFamily: p("--jp-ui-font-family"),
                                     fontSize: 12,
                                     htmlFontSize: 16,
                                     button: {
                                         textTransform: "capitalize"
+                                    },
+                                    allVariants: {
+                                        color: t
                                     }
                                 }
                             })
                         }())
                     }()
                 }), []), i().createElement(h.Z, {
                     theme: t
```

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/643.d05f12a52798d8475b12.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/643.d05f12a52798d8475b12.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/675.e2778aeb06575c94bca0.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/675.e2778aeb06575c94bca0.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/693.2c3da85cc10c904e2289.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/693.2c3da85cc10c904e2289.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/703.3d0d8b7012529f0dd511.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/703.3d0d8b7012529f0dd511.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/819.5279f5daf1d1f505f15f.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/819.5279f5daf1d1f505f15f.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/861.f0852a9fe000bee67405.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/861.f0852a9fe000bee67405.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/900.aad7c14c6d8f76011810.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/900.aad7c14c6d8f76011810.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/remoteEntry.9bfcf8f2600a893d38bf.js` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/remoteEntry.df84a6245b68ae8abd9f.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, o, n, i, f, l, d, c, u, s, p, h, b, m, v, y, g, j, P, w, k, _, O, S = {
+    var e, r, t, a, o, n, i, f, l, c, d, u, s, p, h, b, m, v, y, g, j, P, w, k, _, O, S = {
             22399: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(341), t.e(380), t.e(271), t.e(963), t.e(639)]).then((() => () => t(11639))),
                         "./extension": () => Promise.all([t.e(341), t.e(380), t.e(271), t.e(963), t.e(639)]).then((() => () => t(11639))),
                         "./style": () => t.e(643).then((() => () => t(76643)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -67,15 +67,15 @@
         365: "d20799d043a171f06d37",
         380: "367f93b5ced659dcbadd",
         407: "6b1f897f3ceb4355d6ac",
         456: "3766abc0ca49db318bcd",
         527: "96409770f04a31a6ae7e",
         564: "43eaeac5fe02580e918d",
         598: "168be006d4b42d34521a",
-        639: "4b9a03d6277bd8590eb1",
+        639: "b63fa10cbcf2eccddd7d",
         643: "d05f12a52798d8475b12",
         675: "e2778aeb06575c94bca0",
         693: "2c3da85cc10c904e2289",
         703: "3d0d8b7012529f0dd511",
         819: "5279f5daf1d1f505f15f",
         860: "03421bb262ea8bfa0af1",
         861: "f0852a9fe000bee67405",
@@ -89,15 +89,15 @@
         365: "d20799d043a171f06d37",
         380: "367f93b5ced659dcbadd",
         407: "6b1f897f3ceb4355d6ac",
         456: "3766abc0ca49db318bcd",
         527: "96409770f04a31a6ae7e",
         564: "43eaeac5fe02580e918d",
         598: "168be006d4b42d34521a",
-        639: "4b9a03d6277bd8590eb1",
+        639: "b63fa10cbcf2eccddd7d",
         643: "d05f12a52798d8475b12",
         675: "e2778aeb06575c94bca0",
         693: "2c3da85cc10c904e2289",
         703: "3d0d8b7012529f0dd511",
         819: "5279f5daf1d1f505f15f",
         860: "03421bb262ea8bfa0af1",
         861: "f0852a9fe000bee67405",
@@ -111,18 +111,18 @@
             if ("object" == typeof window) return window
         }
     }(), x.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), t = {}, a = "@jupyter-ai/core:", x.l = (e, r, o, n) => {
         if (t[e]) t[e].push(r);
         else {
             var i, f;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
-                    var c = l[d];
-                    if (c.getAttribute("src") == e || c.getAttribute("data-webpack") == a + o) {
-                        i = c;
+                for (var l = document.getElementsByTagName("script"), c = 0; c < l.length; c++) {
+                    var d = l[c];
+                    if (d.getAttribute("src") == e || d.getAttribute("data-webpack") == a + o) {
+                        i = d;
                         break
                     }
                 }
             i || (f = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, x.nc && i.setAttribute("nonce", x.nc), i.setAttribute("data-webpack", a + o), i.src = e), t[e] = [r];
             var u = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(s);
                     var o = t[e];
@@ -158,15 +158,15 @@
                         (!f || !f.loaded && (!a != !f.eager ? a : i > f.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (f("@emotion/react", "11.11.0", (() => Promise.all([x.e(296), x.e(527), x.e(271), x.e(342)]).then((() => () => x(26527))))), f("@emotion/styled", "11.11.0", (() => Promise.all([x.e(675), x.e(271), x.e(564), x.e(407)]).then((() => () => x(52675))))), f("@jupyter-ai/core", "0.7.2", (() => Promise.all([x.e(341), x.e(380), x.e(271), x.e(963), x.e(639)]).then((() => () => x(11639))))), f("@mui/material", "5.13.1", (() => Promise.all([x.e(296), x.e(860), x.e(341), x.e(271), x.e(564), x.e(963), x.e(456)]).then((() => () => x(30860))))), f("react-markdown", "8.0.7", (() => Promise.all([x.e(693), x.e(861), x.e(271)]).then((() => () => x(81861))))), f("react-syntax-highlighter", "15.5.0", (() => Promise.all([x.e(598), x.e(271)]).then((() => () => x(95598))))), f("rehype-katex", "6.0.3", (() => Promise.all([x.e(693), x.e(900)]).then((() => () => x(94900))))), f("remark-math", "5.1.1", (() => x.e(703).then((() => () => x(7703)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (f("@emotion/react", "11.11.0", (() => Promise.all([x.e(296), x.e(527), x.e(271), x.e(342)]).then((() => () => x(26527))))), f("@emotion/styled", "11.11.0", (() => Promise.all([x.e(675), x.e(271), x.e(564), x.e(407)]).then((() => () => x(52675))))), f("@jupyter-ai/core", "0.7.3", (() => Promise.all([x.e(341), x.e(380), x.e(271), x.e(963), x.e(639)]).then((() => () => x(11639))))), f("@mui/material", "5.13.1", (() => Promise.all([x.e(296), x.e(860), x.e(341), x.e(271), x.e(564), x.e(963), x.e(456)]).then((() => () => x(30860))))), f("react-markdown", "8.0.7", (() => Promise.all([x.e(693), x.e(861), x.e(271)]).then((() => () => x(81861))))), f("react-syntax-highlighter", "15.5.0", (() => Promise.all([x.e(598), x.e(271)]).then((() => () => x(95598))))), f("rehype-katex", "6.0.3", (() => Promise.all([x.e(693), x.e(900)]).then((() => () => x(94900))))), f("remark-math", "5.1.1", (() => x.e(703).then((() => () => x(7703)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         x.g.importScripts && (e = x.g.location + "");
         var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -216,31 +216,31 @@
     }, f = (e, r) => {
         if (0 in e) {
             r = o(r);
             var t = e[0],
                 a = t < 0;
             a && (t = -t - 1);
             for (var n = 0, i = 1, l = !0;; i++, n++) {
-                var d, c, u = i < e.length ? (typeof e[i])[0] : "";
-                if (n >= r.length || "o" == (c = (typeof(d = r[n]))[0])) return !l || ("u" == u ? i > t && !a : "" == u != a);
-                if ("u" == c) {
+                var c, d, u = i < e.length ? (typeof e[i])[0] : "";
+                if (n >= r.length || "o" == (d = (typeof(c = r[n]))[0])) return !l || ("u" == u ? i > t && !a : "" == u != a);
+                if ("u" == d) {
                     if (!l || "u" != u) return !1
                 } else if (l)
-                    if (u == c)
+                    if (u == d)
                         if (i <= t) {
-                            if (d != e[i]) return !1
+                            if (c != e[i]) return !1
                         } else {
-                            if (a ? d > e[i] : d < e[i]) return !1;
-                            d != e[i] && (l = !1)
+                            if (a ? c > e[i] : c < e[i]) return !1;
+                            c != e[i] && (l = !1)
                         }
                 else if ("s" != u && "n" != u) {
                     if (a || i <= t) return !1;
                     l = !1, i--
                 } else {
-                    if (i <= t || c < u != a) return !1;
+                    if (i <= t || d < u != a) return !1;
                     l = !1
                 } else "s" != u && "n" != u && (l = !1, i--)
             }
         }
         var s = [],
             p = s.pop.bind(s);
         for (n = 1; n < e.length; n++) {
@@ -248,37 +248,37 @@
             s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? f(h, r) : !p())
         }
         return !!p()
     }, l = (e, r) => {
         var t = x.S[e];
         if (!t || !x.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, d = (e, r) => {
+    }, c = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
-    }, c = (e, r) => {
+    }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(a) + ")", s = (e, r, t, a) => {
-        var o = c(e, t);
+        var o = d(e, t);
         return f(a, o) || b(u(e, t, o, a)), v(e[t][o])
     }, p = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !f(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
     }, h = (e, r, t, a) => {
         var o = e[t];
         return "No satisfying version (" + i(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
     }, b = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, m = (e, r, t, a) => {
         b(h(e, r, t, a))
     }, v = e => (e.loaded = 1, e.get()), g = (y = e => function(r, t, a, o) {
         var n = x.I(r);
         return n && n.then ? n.then(e.bind(e, r, x.S[r], t, a, o)) : e(r, x.S[r], t, a, o)
-    })(((e, r, t, a) => r && x.o(r, t) ? v(d(r, t)) : a())), j = y(((e, r, t, a) => (l(e, t), v(p(r, t, a) || m(r, e, t, a) || d(r, t))))), P = y(((e, r, t, a) => (l(e, t), s(r, 0, t, a)))), w = y(((e, r, t, a, o) => {
+    })(((e, r, t, a) => r && x.o(r, t) ? v(c(r, t)) : a())), j = y(((e, r, t, a) => (l(e, t), v(p(r, t, a) || m(r, e, t, a) || c(r, t))))), P = y(((e, r, t, a) => (l(e, t), s(r, 0, t, a)))), w = y(((e, r, t, a, o) => {
         var n = r && x.o(r, t) && p(r, t, a);
         return n ? v(n) : o()
     })), k = {}, _ = {
         56271: () => P("default", "react", [1, 17, 0, 1]),
         79510: () => w("default", "@emotion/react", [1, 11, 4, 1], (() => Promise.all([x.e(296), x.e(527), x.e(365)]).then((() => () => x(26527))))),
         92764: () => w("default", "@emotion/styled", [1, 11, 3, 0], (() => Promise.all([x.e(675), x.e(564), x.e(407)]).then((() => () => x(52675))))),
         22502: () => P("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
```

### Comparing `jupyter_ai-0.7.2/jupyter_ai/labextension/static/third-party-licenses.json` & `jupyter_ai-0.7.3/jupyter_ai/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/schema/plugin.json` & `jupyter_ai-0.7.3/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/chat_handler.ts` & `jupyter_ai-0.7.3/src/chat_handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/handler.ts` & `jupyter_ai-0.7.3/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/icons.ts` & `jupyter_ai-0.7.3/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/index.ts` & `jupyter_ai-0.7.3/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/inserter.ts` & `jupyter_ai-0.7.3/src/inserter.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/selection-watcher.ts` & `jupyter_ai-0.7.3/src/selection-watcher.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/theme-provider.ts` & `jupyter_ai-0.7.3/src/theme-provider.ts`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     await new Promise(resolve => setTimeout(resolve, 100)); // Wait 100ms
   }
 }
 
 export async function getJupyterLabTheme(): Promise<Theme> {
   await pollUntilReady();
   const light = document.body.getAttribute('data-jp-theme-light');
+  const primaryFontColor = getCSSVariable('--jp-ui-font-color1');
   return createTheme({
     spacing: 4,
     components: {
       MuiButton: {
         defaultProps: {
           size: 'small'
         }
@@ -108,25 +109,30 @@
       },
       success: {
         main: getCSSVariable('--jp-success-color1'),
         light: getCSSVariable('--jp-success-color2'),
         dark: getCSSVariable('--jp-success-color0')
       },
       text: {
-        primary: getCSSVariable('--jp-ui-font-color1'),
+        primary: primaryFontColor,
         secondary: getCSSVariable('--jp-ui-font-color2'),
         disabled: getCSSVariable('--jp-ui-font-color3')
       }
     },
     shape: {
       borderRadius: 2
     },
     typography: {
       fontFamily: getCSSVariable('--jp-ui-font-family'),
       fontSize: 12,
       htmlFontSize: 16,
       button: {
         textTransform: 'capitalize'
+      },
+      // this is undocumented as of the time of writing.
+      // https://stackoverflow.com/a/62950304/12548458
+      allVariants: {
+        color: primaryFontColor
       }
     }
   });
 }
```

### Comparing `jupyter_ai-0.7.2/src/utils.ts` & `jupyter_ai-0.7.3/src/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/__tests__/widgets/closable-dialog.spec.tsx` & `jupyter_ai-0.7.3/src/__tests__/widgets/closable-dialog.spec.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/components/chat-code-view.tsx` & `jupyter_ai-0.7.3/src/components/chat-code-view.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/components/chat-input.tsx` & `jupyter_ai-0.7.3/src/components/chat-input.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/components/chat-messages.tsx` & `jupyter_ai-0.7.3/src/components/chat-messages.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/components/chat-settings.tsx` & `jupyter_ai-0.7.3/src/components/chat-settings.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/components/chat.tsx` & `jupyter_ai-0.7.3/src/components/chat.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/components/expandable-text-field.tsx` & `jupyter_ai-0.7.3/src/components/expandable-text-field.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/components/jl-theme-provider.tsx` & `jupyter_ai-0.7.3/src/components/jl-theme-provider.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/components/open-task-dialog.tsx` & `jupyter_ai-0.7.3/src/components/open-task-dialog.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/components/scroll-container.tsx` & `jupyter_ai-0.7.3/src/components/scroll-container.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/components/select.tsx` & `jupyter_ai-0.7.3/src/components/select.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/contexts/collaborators-context.tsx` & `jupyter_ai-0.7.3/src/contexts/collaborators-context.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/contexts/selection-context.tsx` & `jupyter_ai-0.7.3/src/contexts/selection-context.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/widgets/chat-error.tsx` & `jupyter_ai-0.7.3/src/widgets/chat-error.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/widgets/chat-sidebar.tsx` & `jupyter_ai-0.7.3/src/widgets/chat-sidebar.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/src/widgets/closable-dialog.tsx` & `jupyter_ai-0.7.3/src/widgets/closable-dialog.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/style/icons/jupyternaut.svg` & `jupyter_ai-0.7.3/style/icons/jupyternaut.svg`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/ui-tests/README.md` & `jupyter_ai-0.7.3/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/ui-tests/jupyter_server_test_config.py` & `jupyter_ai-0.7.3/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/ui-tests/tests/jupyter_ai.spec.ts` & `jupyter_ai-0.7.3/ui-tests/tests/jupyter_ai.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/.gitignore` & `jupyter_ai-0.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/LICENSE` & `jupyter_ai-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/README.md` & `jupyter_ai-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.2/pyproject.toml` & `jupyter_ai-0.7.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,42 +2,41 @@
 requires = ["hatchling>=1.4.0", "jupyterlab>=3.4.7,<4.0.0", "hatch-nodejs-version"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyter_ai"
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.7,<3.11"
+requires-python = ">=3.8,<3.11"
 classifiers = [
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
     "Framework :: Jupyter :: JupyterLab :: 3",
     "Framework :: Jupyter :: JupyterLab :: Extensions",
     "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "jupyter_server>=1.6,<3",
     "jupyterlab>=3.5,<4",
     "pydantic",
     "openai~=0.26",
     "aiosqlite~=0.18",
     "importlib_metadata~=5.2.0",
-    "langchain==0.0.158",
+    "langchain==0.0.159",
     "tiktoken", # required for OpenAIEmbeddings
     "jupyter_ai_magics",
     "ray~=2.4.0", # Requires grpcio installation from conda
     "faiss-cpu", # Not distributed by official repo
-    "wcmatch",
+    "typing_extensions==4.5.0"
 ]
 
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.entry-points."jupyter_ai.model_engine_classes"]
 gpt3 = "jupyter_ai:GPT3ModelEngine"
```

### Comparing `jupyter_ai-0.7.2/PKG-INFO` & `jupyter_ai-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai
-Version: 0.7.2
+Version: 0.7.3
 Summary: A generative AI extension for JupyterLab
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -40,31 +40,30 @@
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.11,>=3.8
 Requires-Dist: aiosqlite~=0.18
 Requires-Dist: faiss-cpu
 Requires-Dist: importlib-metadata~=5.2.0
 Requires-Dist: jupyter-ai-magics
 Requires-Dist: jupyter-server<3,>=1.6
 Requires-Dist: jupyterlab<4,>=3.5
-Requires-Dist: langchain==0.0.158
+Requires-Dist: langchain==0.0.159
 Requires-Dist: openai~=0.26
 Requires-Dist: pydantic
 Requires-Dist: ray~=2.4.0
 Requires-Dist: tiktoken
-Requires-Dist: wcmatch
+Requires-Dist: typing-extensions==4.5.0
 Provides-Extra: all
 Requires-Dist: ai21; extra == 'all'
 Requires-Dist: anthropic; extra == 'all'
 Requires-Dist: boto3; extra == 'all'
 Requires-Dist: cohere; extra == 'all'
 Requires-Dist: huggingface-hub; extra == 'all'
 Requires-Dist: ipywidgets; extra == 'all'
```

