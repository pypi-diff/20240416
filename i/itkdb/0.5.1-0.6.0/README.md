# Comparing `tmp/itkdb-0.5.1.tar.gz` & `tmp/itkdb-0.6.0.tar.gz`

## Comparing `itkdb-0.5.1.tar` & `itkdb-0.6.0.tar`

### file list

```diff
@@ -1,182 +1,183 @@
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 itkdb-0.5.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 itkdb-0.5.1/.linkcheckerrc
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 itkdb-0.5.1/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 itkdb-0.5.1/add_attachment.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 itkdb-0.5.1/add_comment.py
--rwxr-xr-x   0        0        0    36494 2020-02-02 00:00:00.000000 itkdb-0.5.1/generatePlots.py
--rwxr-xr-x   0        0        0    27894 2020-02-02 00:00:00.000000 itkdb-0.5.1/getContentSummary.py
--rwxr-xr-x   0        0        0    20487 2020-02-02 00:00:00.000000 itkdb-0.5.1/getInventory.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 itkdb-0.5.1/mkdocs.yml
--rwxr-xr-x   0        0        0    27949 2020-02-02 00:00:00.000000 itkdb-0.5.1/registerComponent.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 itkdb-0.5.1/tbump.toml
--rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 itkdb-0.5.1/ci/pre-commit-update.sh
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/config.md
--rw-r--r--   0        0        0    23763 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/examples.md
--rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/history.md
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/index.md
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/install.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/macros.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/.overrides/main.html
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/.snippets/abbrs.txt
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/.snippets/links.txt
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/assets/css/custom.css
--rw-r--r--   0        0        0    23475 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/assets/images/logo.svg
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/meta/authors.md
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/meta/faq.md
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/reference/gen_ref_nav.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/reference/cli/itkdb.md
--rw-r--r--   0        0        0    21379 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts.css
--rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc-CsTKlA.woff2
--rw-r--r--   0        0        0    12864 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc0CsTKlA.woff2
--rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc1CsTKlA.woff2
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc2CsTKlA.woff2
--rw-r--r--   0        0        0    16700 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc3CsTKlA.woff2
--rw-r--r--   0        0        0     7696 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc5CsTKlA.woff2
--rw-r--r--   0        0        0    17508 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc6CsQ.woff2
--rw-r--r--   0        0        0    10076 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic-CsTKlA.woff2
--rw-r--r--   0        0        0    12620 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic0CsTKlA.woff2
--rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic1CsTKlA.woff2
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic2CsTKlA.woff2
--rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic3CsTKlA.woff2
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic5CsTKlA.woff2
--rw-r--r--   0        0        0    17032 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic6CsQ.woff2
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xEIzIFKw.woff2
--rw-r--r--   0        0        0    16676 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xFIzIFKw.woff2
--rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xGIzIFKw.woff2
--rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xHIzIFKw.woff2
--rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xIIzI.woff2
--rw-r--r--   0        0        0     7700 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xLIzIFKw.woff2
--rw-r--r--   0        0        0    10292 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xMIzIFKw.woff2
--rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fABc4EsA.woff2
--rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBBc4.woff2
--rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBxc4EsA.woff2
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCBc4EsA.woff2
--rw-r--r--   0        0        0    15000 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCRc4EsA.woff2
--rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fChc4EsA.woff2
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCxc4EsA.woff2
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfABc4EsA.woff2
--rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBBc4.woff2
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBxc4EsA.woff2
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCBc4EsA.woff2
--rw-r--r--   0        0        0    14684 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCRc4EsA.woff2
--rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfChc4EsA.woff2
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCxc4EsA.woff2
--rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4WxKOzY.woff2
--rw-r--r--   0        0        0    15744 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4mxK.woff2
--rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu5mxKOzY.woff2
--rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu72xKOzY.woff2
--rw-r--r--   0        0        0    11872 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7GxKOzY.woff2
--rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7WxKOzY.woff2
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7mxKOzY.woff2
--rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSV0mf0h.woff2
--rw-r--r--   0        0        0    15208 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSZ0mf0h.woff2
--rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSd0mf0h.woff2
--rw-r--r--   0        0        0    22168 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSh0mQ.woff2
--rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSt0mf0h.woff2
--rw-r--r--   0        0        0    12668 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSx0mf0h.woff2
--rw-r--r--   0        0        0     7264 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtElOUlYIw.woff2
--rw-r--r--   0        0        0    16292 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEleUlYIw.woff2
--rw-r--r--   0        0        0    25916 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEluUlYIw.woff2
--rw-r--r--   0        0        0    24024 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEm-Ul.woff2
--rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEmOUlYIw.woff2
--rw-r--r--   0        0        0    13924 2020-02-02 00:00:00.000000 itkdb-0.5.1/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEn-UlYIw.woff2
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/_version.py
--rw-r--r--   0        0        0    14226 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/client.py
--rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/commandline.py
--rw-r--r--   0        0        0    13294 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/core.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/eos.py
--rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/py.typed
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/responses.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/typing.py
--rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/utils.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/caching/__init__.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/caching/adapter.py
--rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/caching/controller.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/caching/utils.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/data/1x1.jpg
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/data/1x1.sh
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/data/CERN_chain.pem
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/data/README.md
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/data/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/data/tiny.root
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/models/__init__.py
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/models/component.py
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/models/file.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/models/institution.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/settings/__init__.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 itkdb-0.5.1/src/itkdb/settings/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/conftest.py
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/test_cli.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/test_client.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/test_image.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/test_response.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/test_scripts.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/test_session.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/test_user.py
--rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/test_utils.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/test_attachments.py
--rw-r--r--   0        0        0     8549 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/test_binaryData.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/test_cache.py
--rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/test_components.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/test_institution.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/test_models.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/test_projects.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/test_session.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/test_shipments.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/test_stats.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/test_summary.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/test_testproperties.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/test_tests.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/test_user.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/test_warning.py
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_attachments.test_add_attachment.json
--rw-r--r--   0        0        0    94089 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_attachments.test_list_all_attachments.json
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_binaryData.test_get_empty_file.json
--rw-r--r--   0        0        0     7917 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_binaryData.test_get_image.json
--rw-r--r--   0        0        0    11021 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json
--rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_binaryData.test_get_json.json
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_binaryData.test_get_plainText.json
--rw-r--r--   0        0        0   304955 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_binaryData.test_get_zipfile.json
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_binaryData.test_issue4.json
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_components.test_add_comment.json
--rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0    20819 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_components.test_delete_attachment_image_eos.json
--rw-r--r--   0        0        0    32318 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_components.test_get.json
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_components.test_get_component_bulk.json
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_components.test_get_component_info_code.json
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_components.test_get_component_info_serial.json
--rw-r--r--   0        0        0   112349 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json
--rw-r--r--   0        0        0   108642 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json
--rw-r--r--   0        0        0   245837 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_components.test_list_componentsv1.json
--rw-r--r--   0        0        0   245811 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_components.test_list_componentsv2.json
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_institution.test_get.json
--rw-r--r--   0        0        0   101372 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_institution.test_pagination.json
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_projects.test_list_projects.json
--rw-r--r--   0        0        0    32478 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_scripts.test_getInventory.trashUnassembled.json
--rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_session.test_fake_route.json
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_session.test_invalid_project.json
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_session.test_missing_required.json
--rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_session.test_no_bearer.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_session.test_unauthorized.json
--rw-r--r--   0        0        0    19435 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_stats.test_get.json
--rw-r--r--   0        0        0   509788 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_summary.test_get_summary.json
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_testproperties.test_delete_test_property.json
--rw-r--r--   0        0        0    19982 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_tests.test_list_test_types.json
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_user.test_user_anonymous_login.json
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_user.test_user_bad_login.json
--rw-r--r--   0        0        0    17319 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_user.test_user_good_login.json
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 itkdb-0.5.1/tests/integration/cassettes/test_warnings.test_get_component.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 itkdb-0.5.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 itkdb-0.5.1/COPYING
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 itkdb-0.5.1/LICENSE
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 itkdb-0.5.1/README.md
--rw-r--r--   0        0        0     8113 2020-02-02 00:00:00.000000 itkdb-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 itkdb-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 itkdb-0.6.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 itkdb-0.6.0/.linkcheckerrc
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 itkdb-0.6.0/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 itkdb-0.6.0/add_attachment.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 itkdb-0.6.0/add_comment.py
+-rwxr-xr-x   0        0        0    36494 2020-02-02 00:00:00.000000 itkdb-0.6.0/generatePlots.py
+-rwxr-xr-x   0        0        0    27894 2020-02-02 00:00:00.000000 itkdb-0.6.0/getContentSummary.py
+-rwxr-xr-x   0        0        0    20487 2020-02-02 00:00:00.000000 itkdb-0.6.0/getInventory.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 itkdb-0.6.0/mkdocs.yml
+-rwxr-xr-x   0        0        0    27949 2020-02-02 00:00:00.000000 itkdb-0.6.0/registerComponent.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 itkdb-0.6.0/tbump.toml
+-rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 itkdb-0.6.0/ci/pre-commit-update.sh
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/config.md
+-rw-r--r--   0        0        0    24368 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/examples.md
+-rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/history.md
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/index.md
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/install.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/macros.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/.overrides/main.html
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/.snippets/abbrs.txt
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/.snippets/links.txt
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/assets/css/custom.css
+-rw-r--r--   0        0        0    23475 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/meta/authors.md
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/meta/faq.md
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/reference/gen_ref_nav.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/reference/cli/itkdb.md
+-rw-r--r--   0        0        0    21379 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts.css
+-rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc-CsTKlA.woff2
+-rw-r--r--   0        0        0    12864 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc0CsTKlA.woff2
+-rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc1CsTKlA.woff2
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc2CsTKlA.woff2
+-rw-r--r--   0        0        0    16700 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc3CsTKlA.woff2
+-rw-r--r--   0        0        0     7696 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc5CsTKlA.woff2
+-rw-r--r--   0        0        0    17508 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc6CsQ.woff2
+-rw-r--r--   0        0        0    10076 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic-CsTKlA.woff2
+-rw-r--r--   0        0        0    12620 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic0CsTKlA.woff2
+-rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic1CsTKlA.woff2
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic2CsTKlA.woff2
+-rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic3CsTKlA.woff2
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic5CsTKlA.woff2
+-rw-r--r--   0        0        0    17032 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic6CsQ.woff2
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xEIzIFKw.woff2
+-rw-r--r--   0        0        0    16676 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xFIzIFKw.woff2
+-rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xGIzIFKw.woff2
+-rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xHIzIFKw.woff2
+-rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xIIzI.woff2
+-rw-r--r--   0        0        0     7700 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xLIzIFKw.woff2
+-rw-r--r--   0        0        0    10292 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xMIzIFKw.woff2
+-rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fABc4EsA.woff2
+-rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBBc4.woff2
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBxc4EsA.woff2
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCBc4EsA.woff2
+-rw-r--r--   0        0        0    15000 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCRc4EsA.woff2
+-rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fChc4EsA.woff2
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCxc4EsA.woff2
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfABc4EsA.woff2
+-rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBBc4.woff2
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBxc4EsA.woff2
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCBc4EsA.woff2
+-rw-r--r--   0        0        0    14684 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCRc4EsA.woff2
+-rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfChc4EsA.woff2
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCxc4EsA.woff2
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4WxKOzY.woff2
+-rw-r--r--   0        0        0    15744 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4mxK.woff2
+-rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu5mxKOzY.woff2
+-rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu72xKOzY.woff2
+-rw-r--r--   0        0        0    11872 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7GxKOzY.woff2
+-rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7WxKOzY.woff2
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7mxKOzY.woff2
+-rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSV0mf0h.woff2
+-rw-r--r--   0        0        0    15208 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSZ0mf0h.woff2
+-rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSd0mf0h.woff2
+-rw-r--r--   0        0        0    22168 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSh0mQ.woff2
+-rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSt0mf0h.woff2
+-rw-r--r--   0        0        0    12668 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSx0mf0h.woff2
+-rw-r--r--   0        0        0     7264 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtElOUlYIw.woff2
+-rw-r--r--   0        0        0    16292 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEleUlYIw.woff2
+-rw-r--r--   0        0        0    25916 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEluUlYIw.woff2
+-rw-r--r--   0        0        0    24024 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEm-Ul.woff2
+-rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEmOUlYIw.woff2
+-rw-r--r--   0        0        0    13924 2020-02-02 00:00:00.000000 itkdb-0.6.0/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEn-UlYIw.woff2
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/_version.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/_version.pyi
+-rw-r--r--   0        0        0    14226 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/client.py
+-rw-r--r--   0        0        0     9512 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/commandline.py
+-rw-r--r--   0        0        0    15274 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/core.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/eos.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/py.typed
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/responses.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/typing.py
+-rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/utils.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/caching/__init__.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/caching/adapter.py
+-rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/caching/controller.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/caching/utils.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/data/1x1.jpg
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/data/1x1.sh
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/data/CERN_chain.pem
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/data/README.md
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/data/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/data/tiny.root
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/models/__init__.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/models/component.py
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/models/file.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/models/institution.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/settings/__init__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 itkdb-0.6.0/src/itkdb/settings/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/test_cli.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/test_client.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/test_image.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/test_response.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/test_scripts.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/test_session.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/test_user.py
+-rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/test_attachments.py
+-rw-r--r--   0        0        0     8549 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/test_binaryData.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/test_cache.py
+-rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/test_components.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/test_institution.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/test_models.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/test_projects.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/test_session.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/test_shipments.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/test_stats.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/test_summary.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/test_testproperties.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/test_tests.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/test_user.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/test_warning.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_attachments.test_add_attachment.json
+-rw-r--r--   0        0        0    94089 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_attachments.test_list_all_attachments.json
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_binaryData.test_get_empty_file.json
+-rw-r--r--   0        0        0     7917 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_binaryData.test_get_image.json
+-rw-r--r--   0        0        0    11021 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_binaryData.test_get_json.json
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_binaryData.test_get_plainText.json
+-rw-r--r--   0        0        0   304955 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_binaryData.test_get_zipfile.json
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_binaryData.test_issue4.json
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_components.test_add_comment.json
+-rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json
+-rw-r--r--   0        0        0    20819 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_components.test_delete_attachment_image_eos.json
+-rw-r--r--   0        0        0    32318 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_components.test_get.json
+-rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_components.test_get_component_bulk.json
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_components.test_get_component_info_code.json
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_components.test_get_component_info_serial.json
+-rw-r--r--   0        0        0   112349 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json
+-rw-r--r--   0        0        0   108642 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json
+-rw-r--r--   0        0        0   245837 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_components.test_list_componentsv1.json
+-rw-r--r--   0        0        0   245811 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_components.test_list_componentsv2.json
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_institution.test_get.json
+-rw-r--r--   0        0        0   101372 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_institution.test_pagination.json
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_projects.test_list_projects.json
+-rw-r--r--   0        0        0    32478 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_scripts.test_getInventory.trashUnassembled.json
+-rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_session.test_fake_route.json
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_session.test_invalid_project.json
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_session.test_missing_required.json
+-rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_session.test_no_bearer.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_session.test_unauthorized.json
+-rw-r--r--   0        0        0    19435 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_stats.test_get.json
+-rw-r--r--   0        0        0   509788 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_summary.test_get_summary.json
+-rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_testproperties.test_delete_test_property.json
+-rw-r--r--   0        0        0    19982 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json
+-rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_tests.test_list_test_types.json
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_user.test_user_anonymous_login.json
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_user.test_user_bad_login.json
+-rw-r--r--   0        0        0    17319 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_user.test_user_good_login.json
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 itkdb-0.6.0/tests/integration/cassettes/test_warnings.test_get_component.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 itkdb-0.6.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 itkdb-0.6.0/COPYING
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 itkdb-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 itkdb-0.6.0/README.md
+-rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 itkdb-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     9298 2020-02-02 00:00:00.000000 itkdb-0.6.0/PKG-INFO
```

### Comparing `itkdb-0.5.1/.gitlab-ci.yml` & `itkdb-0.6.0/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,14 @@
   image: $IMAGE
   rules:
     - if: $CI_PIPELINE_SOURCE == "push"
   script:
     - pipx run hatch run +py=${PYTHON_VERSION} dev:test
   parallel:
     matrix:
-      - IMAGE: "python:3.7-buster"
-        PYTHON_VERSION: "3.7"
       - IMAGE: "python:3.8-buster"
         PYTHON_VERSION: "3.8"
       - IMAGE: "python:3.9-buster"
         PYTHON_VERSION: "3.9"
       - IMAGE: "python:3.10-buster"
         PYTHON_VERSION: "3.10"
       - IMAGE: "python:3.11-buster"
```

### Comparing `itkdb-0.5.1/.pre-commit-config.yaml` & `itkdb-0.6.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     getInventory.py|
     registerComponent.py|
     tests/integration/cassettes/.*.json
   )$
 
 repos:
   - repo: https://github.com/psf/black-pre-commit-mirror
-    rev: "24.3.0"
+    rev: "24.4.0"
     hooks:
       - id: black-jupyter
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.5.0"
+    rev: "v4.6.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
         exclude: mkdocs.yml
@@ -58,15 +58,15 @@
   - repo: https://github.com/adamchainz/blacken-docs
     rev: "1.16.0"
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==22.8.0]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.4
+    rev: v0.3.7
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: "v1.9.0"
     hooks:
```

### Comparing `itkdb-0.5.1/generatePlots.py` & `itkdb-0.6.0/generatePlots.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/getContentSummary.py` & `itkdb-0.6.0/getContentSummary.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/getInventory.py` & `itkdb-0.6.0/getInventory.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/mkdocs.yml` & `itkdb-0.6.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/registerComponent.py` & `itkdb-0.6.0/registerComponent.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tbump.toml` & `itkdb-0.6.0/tbump.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2230 2e35 2e31 220a 0a23 2045  t = "0.5.1"..# E
+00000010: 7420 3d20 2230 2e36 2e30 220a 0a23 2045  t = "0.6.0"..# E
 00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
 00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
 00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
 00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
 00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
 00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
 00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
@@ -14,16 +14,16 @@
 000000d0: 6361 6e64 6964 6174 653e 5c64 2b29 0a20  candidate>\d+). 
 000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
 000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
 00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
 00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
 00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
 00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
-00000140: 6d70 2076 6572 7369 6f6e 3a20 302e 352e  mp version: 0.5.
-00000150: 3120 e286 9220 7b6e 6577 5f76 6572 7369  1 ... {new_versi
+00000140: 6d70 2076 6572 7369 6f6e 3a20 302e 362e  mp version: 0.6.
+00000150: 3020 e286 9220 7b6e 6577 5f76 6572 7369  0 ... {new_versi
 00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
 00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
 00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
 00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
 000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
 000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
 000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
```

### Comparing `itkdb-0.5.1/ci/pre-commit-update.sh` & `itkdb-0.6.0/ci/pre-commit-update.sh`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/config.md` & `itkdb-0.6.0/docs/config.md`

 * *Files 11% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 environment variables for this package are prefixed with `ITKDB_`. As of now,
 there are:
 
 | Variable                   | Default                                                                                  | Description                                                                                                                |
 | -------------------------- | ---------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
 | ITKDB_ACCESS_CODE1         | `""`                                                                                     | First access code                                                                                                          |
 | ITKDB_ACCESS_CODE2         | `""`                                                                                     | Second access code                                                                                                         |
+| ITKDB_AUDREYTWO_API_KEY    | `""`                                                                                     | API key for Audrey II                                                                                                      |
 | ITKDB_ACCESS_SCOPE         | `"openid https://itkpd-test.unicorncollege.cz"`                                          | OIDC scope for the API                                                                                                     |
 | ITKDB_ACCESS_AUDIENCE      | `"https://itkpd-test.unicorncollege.cz"`                                                 | OIDC aucience for the API                                                                                                  |
 | ITKDB_AUTH_URL             | `"https://uuidentity.plus4u.net/uu-oidc-maing02/bb977a99f4cc4c37a2afce3fd599d0a7/oidc/"` | OIDC Authentication url for the API                                                                                        |
-| ITKDB_SITE_URL             | `"https://itkpd-test.unicorncollege.cz/"`                                                | Base url for the API                                                                                                       |
+| ITKDB_API_URL              | `"https://itkpd-test.unicorncollege.cz/"`                                                | Base url for the API                                                                                                       |
 | ITKDB_CASSETTE_LIBRARY_DIR | `"tests/integration/cassettes"`                                                          | Local path for storing recorded requests for playback (developer setting)                                                  |
 | ITKDB_LEEWAY               | 2                                                                                        | Default amount of time (in seconds) for leeway when checking local machine time against server response for authentication |
 
 !!! note "Added in version 0.4.0"
 
     - `ITKDB_ACCESS_SCOPE`
     - `ITKDB_ACCESS_AUDIENCE`
@@ -35,9 +36,10 @@
 load environment variables from a file called `.env` in the current directory
 you're running `itkdb` from. This allows you to dynamically inject environment
 variables in while running, but without the need to export in `.bash_profile` or
 similar. You can create a `.env` file with contents like
 
 ```bash title=".env"
 ITKDB_ACCESS_CODE1=abcdef
-ITKDB_ACCESS_CODE2=123456"
+ITKDB_ACCESS_CODE2=123456
+ITKDB_AUDREYTWO_API_KEY=mytoken
 ```
```

### Comparing `itkdb-0.5.1/docs/examples.md` & `itkdb-0.6.0/docs/examples.md`

 * *Files 2% similar despite different names*

```diff
@@ -635,7 +635,21 @@
         "userIdentity",
         "code",
         "contentType",
         "filename",
         "url",
     ]
     ```
+
+## Using a bearer token for your requests
+
+`itkdb` supports a [itkdb.typing.UserLike][] object which allows one to change the method of authentication (or create your own `User` type that is used by [itkdb.core.Client][]. In this example, we will demonstrate how to switch to [itkdb.core.UserBearer][].
+
+```py
+import itkdb
+
+user = itkdb.core.UserBearer(bearer="mybearertoken")  # (1)!
+client = itkdb.Client(user=user)  # (2)!
+```
+
+1. Create your [itkdb.core.UserBearer][] user.
+2. Tell the [itkdb.Client][] to use your user. Then, the `client` will make requests to the API using the configured API url.
```

### Comparing `itkdb-0.5.1/docs/history.md` & `itkdb-0.6.0/docs/history.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,33 @@
 
 **_Changed:_**
 
 **_Added:_**
 
 **_Fixed:_**
 
+## [0.6.0](https://gitlab.cern.ch/atlas-itk/sw/db/itkdb/-/tags/v0.6.0) - 2024-04-16 ## {: #itkdb-v0.6.0 }
+
+**_Added:_**
+
+- Support for simple bearer authentication via [itkdb.core.UserBearer][]
+
+**_Changed:_**
+
+- Dropped support for python 3.7
+- Renamed `ITKDB_SITE_URL` to `ITKDB_API_URL`
+
+
+## [0.5.1](https://gitlab.cern.ch/atlas-itk/sw/db/itkdb/-/tags/v0.5.1) - 2024-04-05 ## {: #itkdb-v0.5.1 }
+
+**_Fixed:_**
+
+- Pagination of requests without a body are fixed, such as `client.get('listComponents')`.
+
+
 ## [0.5.0](https://gitlab.cern.ch/atlas-itk/sw/db/itkdb/-/tags/v0.5.0) - 2024-03-11 ## {: #itkdb-v0.5.0 }
 
 **_Added:_**
 
 - Command-line interfaces for [`itkdb eos upload`](../reference/cli/itkdb#itkdb-eos-upload) and [`itkdb eos delete`](../reference/cli/itkdb#itkdb-eos-upload)
 
 **_Changed:_**
```

### Comparing `itkdb-0.5.1/docs/index.md` & `itkdb-0.6.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/install.md` & `itkdb-0.6.0/docs/install.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/assets/css/custom.css` & `itkdb-0.6.0/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/assets/images/logo.svg` & `itkdb-0.6.0/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/meta/faq.md` & `itkdb-0.6.0/docs/meta/faq.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/reference/gen_ref_nav.py` & `itkdb-0.6.0/docs/reference/gen_ref_nav.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts.css` & `itkdb-0.6.0/docs/stylesheets/fonts.css`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc-CsTKlA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc-CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc0CsTKlA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc0CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc1CsTKlA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc1CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc2CsTKlA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc2CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc3CsTKlA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc3CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc5CsTKlA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc5CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc6CsQ.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc6CsQ.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic-CsTKlA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic-CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic0CsTKlA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic0CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic1CsTKlA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic1CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic2CsTKlA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic2CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic3CsTKlA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic3CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic5CsTKlA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic5CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic6CsQ.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic6CsQ.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xEIzIFKw.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xEIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xFIzIFKw.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xFIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xGIzIFKw.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xGIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xHIzIFKw.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xHIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xIIzI.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xIIzI.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xLIzIFKw.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xLIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xMIzIFKw.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xMIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fABc4EsA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fABc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBBc4.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBBc4.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBxc4EsA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBxc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCBc4EsA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCBc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCRc4EsA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCRc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fChc4EsA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fChc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCxc4EsA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCxc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfABc4EsA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfABc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBBc4.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBBc4.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBxc4EsA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBxc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCBc4EsA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCBc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCRc4EsA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCRc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfChc4EsA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfChc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCxc4EsA.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCxc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4WxKOzY.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4WxKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4mxK.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4mxK.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu5mxKOzY.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu5mxKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu72xKOzY.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu72xKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7GxKOzY.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7GxKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7WxKOzY.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7WxKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7mxKOzY.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7mxKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSV0mf0h.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSV0mf0h.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSZ0mf0h.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSZ0mf0h.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSd0mf0h.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSd0mf0h.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSh0mQ.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSh0mQ.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSt0mf0h.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSt0mf0h.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSx0mf0h.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSx0mf0h.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtElOUlYIw.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtElOUlYIw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEleUlYIw.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEleUlYIw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEluUlYIw.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEluUlYIw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEm-Ul.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEm-Ul.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEmOUlYIw.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEmOUlYIw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEn-UlYIw.woff2` & `itkdb-0.6.0/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEn-UlYIw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/src/itkdb/client.py` & `itkdb-0.6.0/src/itkdb/client.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/src/itkdb/commandline.py` & `itkdb-0.6.0/src/itkdb/commandline.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 @click.option(
     "--access-code2",
     prompt=not (bool(settings.ITKDB_ACCESS_CODE2)),
     default=settings.ITKDB_ACCESS_CODE2,
     show_default=True,
 )
 @click.option("--auth-url", default=settings.ITKDB_AUTH_URL, show_default=True)
-@click.option("--site-url", default=settings.ITKDB_SITE_URL, show_default=True)
+@click.option("--site-url", default=settings.ITKDB_API_URL, show_default=True)
 @click.option(
     "--save-auth",
     help="Filename to save authenticated user to for persistence between requests",
     default=".auth",
     type=click.Path(path_type=Path, exists=False, writable=True, resolve_path=True),
 )
 def entrypoint(access_code1, access_code2, auth_url, site_url, save_auth):
```

### Comparing `itkdb-0.5.1/src/itkdb/core.py` & `itkdb-0.6.0/src/itkdb/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,69 @@
 from __future__ import annotations
 
 import logging
 import pickle  # nosec
 import time
 from pathlib import Path
-from typing import ClassVar
+from typing import Any, Callable, ClassVar, cast
 
 import cachecontrol.caches.file_cache
 import requests
 from cachecontrol.heuristics import ExpiresAfter
 from jose import jwt
 from requests.status_codes import codes
 
 from itkdb import exceptions
 from itkdb._version import __version__
 from itkdb.caching import CacheControlAdapter, CacheController
 from itkdb.settings import settings
+from itkdb.typing import UserLike
 
 log = logging.getLogger(__name__)
 
 
-class User:
+class UserBearer(UserLike):
+    """
+    Class for managing bearer tokens.
+
+    Args:
+        bearer (str): Bearer token
+        prefix_url (str): The prefix for all non-absolute URIs
+
+    !!! note "Added in version 0.6.0"
+    """
+
+    def __init__(
+        self,
+        bearer: str = settings.ITKDB_AUDREYTWO_API_KEY,
+    ):
+        # session handling (for injection in tests)
+        self._session = requests.Session()
+        self._session.headers.update({"User-Agent": f"itkdb/{__version__}"})
+        # store last call to authenticate
+        self._response: requests.Response | None = None
+        self._status_code: int | None = None
+        # initialization configuration
+        self._bearer: str = bearer
+
+    def authenticate(self) -> bool:
+        return True
+
+    @property
+    def bearer(self) -> str:
+        """
+        The bearer token.
+        """
+        return self._bearer
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__:s}(bearer={self.bearer})"
+
+
+class User(UserLike):
     """
     Class for managing user tokens and authentication flow.
 
     Args:
         access_code1 (str): ITkPD Access Code 1
         access_code2 (str): ITkPD Access Code 2
         audience (str): ITkPD OIDC Audience
@@ -39,50 +78,50 @@
     !!! note "Added in version 0.4.7"
         - `auth_expiry_threshold` to force reauthentication sooner
 
     """
 
     def __init__(
         self,
-        access_code1=settings.ITKDB_ACCESS_CODE1,
-        access_code2=settings.ITKDB_ACCESS_CODE2,
-        audience=settings.ITKDB_ACCESS_AUDIENCE,
-        prefix_url=settings.ITKDB_AUTH_URL,
-        jwt_options=None,
+        access_code1: str = settings.ITKDB_ACCESS_CODE1,
+        access_code2: str = settings.ITKDB_ACCESS_CODE2,
+        audience: str = settings.ITKDB_ACCESS_AUDIENCE,
+        prefix_url: str = settings.ITKDB_AUTH_URL,
+        jwt_options: dict[str, Any] | None = None,
         save_auth: Path | str | None = None,
         auth_expiry_threshold: int = 15,
     ):
         # session handling (for injection in tests)
         self._session = requests.Session()
         self._session.headers.update({"User-Agent": f"itkdb/{__version__}"})
         # store last call to authenticate
-        self._response = None
-        self._status_code = None
+        self._response: requests.Response | None = None
+        self._status_code: int | None = None
         # store jwks for validation/verification
-        self._jwks = None
+        self._jwks: dict[str, Any] | None = None
         # store information after authorization occurs
-        self._access_token = None
-        self._raw_id_token = None
-        self._id_token = None
+        self._access_token: str | None = None
+        self._raw_id_token: str | None = None
+        self._id_token: dict[str, Any] | None = None
         # initialization configuration
-        self._access_code1 = access_code1
-        self._access_code2 = access_code2
-        self._audience = audience
-        self._prefix_url = prefix_url
+        self._access_code1: str = access_code1
+        self._access_code2: str = access_code2
+        self._audience: str = audience
+        self._prefix_url: str = prefix_url
         # update jwt_options if provided
-        self._jwt_options = {
+        self._jwt_options: dict[str, Any] = {
             "leeway": int(settings.ITKDB_LEEWAY)
         }  # **jwt_options, python3 only
         self._jwt_options.update(jwt_options or {})
         # serialization/persistence
         self._save_auth: Path | None = Path(save_auth) if save_auth else None
-        self.auth_expiry_threshold = auth_expiry_threshold
+        self.auth_expiry_threshold: int = auth_expiry_threshold
         self._load()
 
-    def _load(self):
+    def _load(self) -> bool:
         if self._save_auth and self._save_auth.is_file():
             try:
                 with self._save_auth.open("rb") as _pickle_file:
                     saved_user = pickle.load(_pickle_file)  # nosec
                 if saved_user.is_expired():
                     log.warning(
                         "Saved user session is expired in %s. Creating a new one.",
@@ -106,23 +145,24 @@
                     pickle.dump(self, fpointer, pickle.HIGHEST_PROTOCOL)
                     return True
                 except (pickle.PicklingError, AttributeError, TypeError):
                     log.warning("Unable to save user session to %s.", self._save_auth)
             return False
         return False
 
-    def _load_jwks(self, force=False):
+    def _load_jwks(self, force: bool = False) -> None:
         if self._jwks is None or force:
             self._jwks = self._session.get(
                 "https://uuidentity.plus4u.net/uu-oidc-maing02/bb977a99f4cc4c37a2afce3fd599d0a7/oidc/listKeys"
             ).json()
 
-    def _parse_id_token(self):
+    def _parse_id_token(self) -> None:
         if self._raw_id_token:
             self._load_jwks()
+            assert self._jwks
             self._id_token = jwt.decode(
                 self._raw_id_token,
                 self._jwks,
                 algorithms="RS256",
                 audience=self._audience,
                 options=self._jwt_options,
             )
@@ -175,15 +215,15 @@
     def access_code2(self) -> str:
         """
         The second access code.
         """
         return self._access_code2
 
     @property
-    def access_token(self) -> str:
+    def access_token(self) -> str | None:
         """
         The opaque access token for the user.
         """
         return self._access_token
 
     @property
     def id_token(self) -> dict[str, str | list[str] | int]:
@@ -193,37 +233,37 @@
         return self._id_token if self._id_token else {}
 
     @property
     def name(self) -> str:
         """
         The name for the user.
         """
-        return self.id_token.get("name", "")
+        return cast(str, self.id_token.get("name", ""))
 
     @property
     def expires_at(self) -> int:
         """
         The Epoch Unix Timestamp that the user session expires at.
         """
-        return self.id_token.get("exp", 0)
+        return cast(int, self.id_token.get("exp", 0))
 
     @property
     def expires_in(self) -> int:
         """
         The time until expiration in seconds.
         """
-        expires_in = self.expires_at - time.time()
+        expires_in: float = self.expires_at - time.time()
         return 0 if expires_in < 0 else int(expires_in)
 
     @property
     def identity(self) -> str:
         """
         The identity for the user in the ITk Production Database.
         """
-        return self.id_token.get("uuidentity", "")
+        return cast(str, self.id_token.get("uuidentity", ""))
 
     @property
     def bearer(self) -> str:
         """
         The bearer token for the user.
         """
         return self._raw_id_token if self._raw_id_token else ""
@@ -240,15 +280,15 @@
 
     def is_expired(self) -> bool:
         """
         Whether current user session is expired given the expiration threshold.
         """
         return not self.expires_in > self.auth_expiry_threshold
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.__class__.__name__:s}(name={self.name:s}, expires_in={self.expires_in:d}s)"
 
 
 class Session(requests.Session):
     """
     Lightweight wrapper around `requests.Session` with basic error-handling, auto-(re)authentication, and URI prefixing.
 
@@ -270,15 +310,15 @@
         auth_expiry_threshold (int): Number of seconds until token expiration to do a reauthentication (see itkdb.core.User)
 
     !!! note "Added in version 0.4.7"
         - `auth_expiry_threshold` to force reauthentication sooner
 
     """
 
-    STATUS_EXCEPTIONS: ClassVar[dict[int, exceptions.ITkDBException]] = {
+    STATUS_EXCEPTIONS: ClassVar[dict[int, type[exceptions.ITkDBException]]] = {
         codes["bad_gateway"]: exceptions.ServerError,
         codes["bad_request"]: exceptions.BadRequest,
         codes["conflict"]: exceptions.Conflict,
         codes["found"]: exceptions.Redirect,
         codes["forbidden"]: exceptions.Forbidden,
         codes["gateway_timeout"]: exceptions.ServerError,
         codes["internal_server_error"]: exceptions.ServerError,
@@ -290,31 +330,33 @@
         codes["unavailable_for_legal_reasons"]: exceptions.UnavailableForLegalReasons,
     }
     SUCCESS_STATUSES: ClassVar[set[int]] = {codes["created"], codes["ok"]}
 
     def __init__(
         self,
         user: User | None = None,
-        prefix_url=settings.ITKDB_SITE_URL,
+        prefix_url: str = settings.ITKDB_API_URL,
         save_auth: Path | str | None = None,
-        cache: bool = True,
-        expires_after=None,
-        auth_expiry_threshold=15,
+        cache: bool | object = True,
+        expires_after: dict[str, int] | None = None,
+        auth_expiry_threshold: int = 15,
     ):
         super().__init__()
         self.headers.update({"User-Agent": f"itkdb/{__version__}"})
-        self.user = (
+        self.user: UserLike = (
             user
             if user
             else User(save_auth=save_auth, auth_expiry_threshold=auth_expiry_threshold)
         )
-        self.auth = self.authorize
-        self.prefix_url = prefix_url
+        self.auth: Callable[[requests.PreparedRequest], requests.PreparedRequest] = (
+            self.authorize
+        )
+        self.prefix_url: str = prefix_url
         # store last call
-        self._response = None
+        self._response: requests.Response | None = None
 
         cache_options = {}
         if cache:
             cache = (
                 cachecontrol.caches.file_cache.FileCache(".webcache")
                 if cache is True
                 else cache
@@ -328,52 +370,57 @@
         if cache_options:
             # add caching
             super().mount(
                 self.prefix_url,
                 CacheControlAdapter(controller_class=CacheController, **cache_options),
             )
 
-    def authorize(self, req):
+    def authorize(self, req: requests.PreparedRequest) -> requests.PreparedRequest:
         """
         Add authentication information to the request by updating the headers.
         """
-        if req.url.startswith(settings.ITKDB_SITE_URL):
+        if req.url.startswith(settings.ITKDB_API_URL):  # type: ignore[union-attr]
             self.user.authenticate()
             req.headers.update({"Authorization": f"Bearer {self.user.bearer:s}"})
         return req
 
-    def _normalize_url(self, url):
-        return requests.compat.urljoin(self.prefix_url, url)
+    def _normalize_url(self, url: str | bytes) -> str:
+        url_str = url.decode("utf-8") if isinstance(url, bytes) else url
+        return requests.compat.urljoin(self.prefix_url, url_str)
 
-    def _check_response(self, response):
+    def _check_response(self, response: requests.Response) -> None:
         if response.status_code in self.STATUS_EXCEPTIONS:
             raise self.STATUS_EXCEPTIONS[response.status_code](response)
 
         try:
             response.raise_for_status()
         except BaseException as err:
             raise exceptions.UnhandledResponse(response) from err
 
-    def prepare_request(self, request):
+    def prepare_request(self, request: requests.Request) -> requests.PreparedRequest:
         request.url = self._normalize_url(request.url)
         return super().prepare_request(request)
 
-    def send(self, request, **kwargs):
+    def send(
+        self, request: requests.PreparedRequest, **kwargs: Any
+    ) -> requests.Response:
         response = super().send(request, **kwargs)
         self._response = response
         log.debug(
             "Response: %s (%s bytes)",
             response.status_code,
             response.headers.get("content-length"),
         )
         self._check_response(response)
         return response
 
-    def request(self, method, url, *args, **kwargs):
+    def request(
+        self, method: str | bytes, url: str | bytes, *args: Any, **kwargs: Any
+    ) -> requests.Response:
         url = self._normalize_url(url)
         return super().request(method, url, *args, **kwargs)
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args: Any, **kwargs: Any) -> requests.Response:
         if len(args) == 1:
             return self.send(self.prepare_request(*args), **kwargs)
 
         return self.request(*args, **kwargs)
```

### Comparing `itkdb-0.5.1/src/itkdb/eos.py` & `itkdb-0.6.0/src/itkdb/eos.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from itkdb.data import path as itkdb_data
 
 try:
     import pycurl
 except ModuleNotFoundError:
     HAS_PYCURL = False
 except ImportError as imp_err:
-    imp_err_msg = "There is an error importing pycurl. Please see the documentation for some hints.\n\n  https://itkdb.docs.cern.ch/0.5/meta/faq/"  # pylint: disable=invalid-name
+    imp_err_msg = "There is an error importing pycurl. Please see the documentation for some hints.\n\n  https://itkdb.docs.cern.ch/0.6/meta/faq/"  # pylint: disable=invalid-name
     raise ImportError(imp_err_msg) from imp_err
 else:
     HAS_PYCURL = True
 
 log = logging.getLogger(__name__)
```

### Comparing `itkdb-0.5.1/src/itkdb/exceptions.py` & `itkdb-0.6.0/src/itkdb/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from __future__ import annotations
 
 import json
 from contextlib import suppress
 from urllib.parse import urlparse
 
+import requests
+
 from .utils import pretty_print
 
 try:
     from json.decoder import JSONDecodeError
 except ImportError:
     JSONDecodeError = ValueError
 
@@ -31,19 +33,21 @@
 class InvalidInvocation(ITkDBException):
     """Indicate that the code to execute cannot be completed."""
 
 
 class ResponseException(ITkDBException):
     """Indicate that there was an error with the completed HTTP request."""
 
-    def __init__(self, response, additional_message=None):
+    def __init__(
+        self, response: requests.Response, additional_message: str | None = None
+    ):
         """Initialize a ResponseException instance.
         :param response: A requests.response instance.
         """
-        self.response = response
+        self.response: requests.Response = response
         message = f"received {response.status_code} HTTP response for following request\n{pretty_print(response.request)}"
 
         try:
             if additional_message is None:
                 additional_message = json.dumps(response.json(), indent=2)
 
         except JSONDecodeError:
```

### Comparing `itkdb-0.5.1/src/itkdb/responses.py` & `itkdb-0.6.0/src/itkdb/responses.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/src/itkdb/utils.py` & `itkdb-0.6.0/src/itkdb/utils.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/src/itkdb/caching/adapter.py` & `itkdb-0.6.0/src/itkdb/caching/adapter.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/src/itkdb/caching/controller.py` & `itkdb-0.6.0/src/itkdb/caching/controller.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/src/itkdb/caching/utils.py` & `itkdb-0.6.0/src/itkdb/caching/utils.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/src/itkdb/data/1x1.sh` & `itkdb-0.6.0/src/itkdb/data/1x1.sh`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/src/itkdb/data/CERN_chain.pem` & `itkdb-0.6.0/src/itkdb/data/CERN_chain.pem`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/src/itkdb/data/README.md` & `itkdb-0.6.0/src/itkdb/data/README.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/src/itkdb/models/component.py` & `itkdb-0.6.0/src/itkdb/models/component.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     @property
     def serial_number(self) -> str:
         """serial number of component"""
         return self._data.get("serialNumber", "") or ""
 
     @property
-    def id(self) -> str:
+    def id(self) -> str:  # pylint: disable=invalid-name
         """unique identifier of component"""
         return str(self._data["id"])
 
     @property
     def children(self) -> list[Any]:
         """children of component"""
         return self._children or self._data.get("children", []) or []
```

### Comparing `itkdb-0.5.1/src/itkdb/models/file.py` & `itkdb-0.6.0/src/itkdb/models/file.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/src/itkdb/models/institution.py` & `itkdb-0.6.0/src/itkdb/models/institution.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/conftest.py` & `itkdb-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/test_cli.py` & `itkdb-0.6.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/test_client.py` & `itkdb-0.6.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/test_image.py` & `itkdb-0.6.0/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/test_response.py` & `itkdb-0.6.0/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/test_scripts.py` & `itkdb-0.6.0/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/test_session.py` & `itkdb-0.6.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/test_user.py` & `itkdb-0.6.0/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/test_utils.py` & `itkdb-0.6.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/test_attachments.py` & `itkdb-0.6.0/tests/integration/test_attachments.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/test_binaryData.py` & `itkdb-0.6.0/tests/integration/test_binaryData.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/test_cache.py` & `itkdb-0.6.0/tests/integration/test_cache.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/test_components.py` & `itkdb-0.6.0/tests/integration/test_components.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/test_institution.py` & `itkdb-0.6.0/tests/integration/test_institution.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/test_session.py` & `itkdb-0.6.0/tests/integration/test_session.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/test_shipments.py` & `itkdb-0.6.0/tests/integration/test_shipments.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/test_summary.py` & `itkdb-0.6.0/tests/integration/test_summary.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/test_testproperties.py` & `itkdb-0.6.0/tests/integration/test_testproperties.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/test_tests.py` & `itkdb-0.6.0/tests/integration/test_tests.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/test_user.py` & `itkdb-0.6.0/tests/integration/test_user.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/test_warning.py` & `itkdb-0.6.0/tests/integration/test_warning.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_attachments.test_add_attachment.json` & `itkdb-0.6.0/tests/integration/cassettes/test_attachments.test_add_attachment.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_attachments.test_list_all_attachments.json` & `itkdb-0.6.0/tests/integration/cassettes/test_attachments.test_list_all_attachments.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_binaryData.test_get_empty_file.json` & `itkdb-0.6.0/tests/integration/cassettes/test_binaryData.test_get_empty_file.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_binaryData.test_get_image.json` & `itkdb-0.6.0/tests/integration/cassettes/test_binaryData.test_get_image.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json` & `itkdb-0.6.0/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_binaryData.test_get_json.json` & `itkdb-0.6.0/tests/integration/cassettes/test_binaryData.test_get_json.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_binaryData.test_get_plainText.json` & `itkdb-0.6.0/tests/integration/cassettes/test_binaryData.test_get_plainText.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_binaryData.test_get_zipfile.json` & `itkdb-0.6.0/tests/integration/cassettes/test_binaryData.test_get_zipfile.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_binaryData.test_issue4.json` & `itkdb-0.6.0/tests/integration/cassettes/test_binaryData.test_issue4.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_components.test_add_comment.json` & `itkdb-0.6.0/tests/integration/cassettes/test_components.test_add_comment.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json` & `itkdb-0.6.0/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_components.test_delete_attachment_image_eos.json` & `itkdb-0.6.0/tests/integration/cassettes/test_components.test_delete_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_components.test_get.json` & `itkdb-0.6.0/tests/integration/cassettes/test_components.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_components.test_get_component_bulk.json` & `itkdb-0.6.0/tests/integration/cassettes/test_components.test_get_component_bulk.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_components.test_get_component_info_code.json` & `itkdb-0.6.0/tests/integration/cassettes/test_components.test_get_component_info_code.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_components.test_get_component_info_serial.json` & `itkdb-0.6.0/tests/integration/cassettes/test_components.test_get_component_info_serial.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json` & `itkdb-0.6.0/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json` & `itkdb-0.6.0/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_components.test_list_componentsv1.json` & `itkdb-0.6.0/tests/integration/cassettes/test_components.test_list_componentsv1.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_components.test_list_componentsv2.json` & `itkdb-0.6.0/tests/integration/cassettes/test_components.test_list_componentsv2.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_institution.test_get.json` & `itkdb-0.6.0/tests/integration/cassettes/test_institution.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_institution.test_pagination.json` & `itkdb-0.6.0/tests/integration/cassettes/test_institution.test_pagination.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_projects.test_list_projects.json` & `itkdb-0.6.0/tests/integration/cassettes/test_projects.test_list_projects.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json` & `itkdb-0.6.0/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json` & `itkdb-0.6.0/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json` & `itkdb-0.6.0/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_session.test_fake_route.json` & `itkdb-0.6.0/tests/integration/cassettes/test_session.test_fake_route.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_session.test_invalid_project.json` & `itkdb-0.6.0/tests/integration/cassettes/test_session.test_invalid_project.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_session.test_missing_required.json` & `itkdb-0.6.0/tests/integration/cassettes/test_session.test_missing_required.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_session.test_no_bearer.json` & `itkdb-0.6.0/tests/integration/cassettes/test_session.test_no_bearer.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json` & `itkdb-0.6.0/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_stats.test_get.json` & `itkdb-0.6.0/tests/integration/cassettes/test_stats.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_summary.test_get_summary.json` & `itkdb-0.6.0/tests/integration/cassettes/test_summary.test_get_summary.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_testproperties.test_delete_test_property.json` & `itkdb-0.6.0/tests/integration/cassettes/test_testproperties.test_delete_test_property.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json` & `itkdb-0.6.0/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_tests.test_list_test_types.json` & `itkdb-0.6.0/tests/integration/cassettes/test_tests.test_list_test_types.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_user.test_user_anonymous_login.json` & `itkdb-0.6.0/tests/integration/cassettes/test_user.test_user_anonymous_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_user.test_user_bad_login.json` & `itkdb-0.6.0/tests/integration/cassettes/test_user.test_user_bad_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_user.test_user_good_login.json` & `itkdb-0.6.0/tests/integration/cassettes/test_user.test_user_good_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/tests/integration/cassettes/test_warnings.test_get_component.json` & `itkdb-0.6.0/tests/integration/cassettes/test_warnings.test_get_component.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/.gitignore` & `itkdb-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/COPYING` & `itkdb-0.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/LICENSE` & `itkdb-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `itkdb-0.5.1/README.md` & `itkdb-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ITk DB v0.5.1
+# ITk DB v0.6.0
 
 Python wrapper around the ITk Production Database API.
 
 ---
 
 <!-- sync the following div with docs/index.md -->
 <div align="center">
```

### Comparing `itkdb-0.5.1/pyproject.toml` & `itkdb-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,27 @@
 maintainers = [
     { name = "Giordon Stark", email = "kratsg@gmail.com" },
 ]
 
 description = "Python wrapper to interface with ITk DB."
 readme = "README.md"
 
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Topic :: Scientific/Engineering",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Development Status :: 1 - Planning",
 ]
@@ -60,15 +59,15 @@
     "pycurl", # for EOS uploads
 ]
 contrib = [
   "html2text"
 ]
 
 [project.urls]
-Documentation = "https://itkdb.docs.cern.ch/0.5/"
+Documentation = "https://itkdb.docs.cern.ch/0.6/"
 Homepage = "https://gitlab.cern.ch/atlas-itk/sw/db/itkdb"
 "Bug Tracker" = "https://gitlab.cern.ch/atlas-itk/sw/db/itkdb/issues"
 Source = "https://gitlab.cern.ch/atlas-itk/sw/db/itkdb"
 
 [project.scripts]
 itkdb = "itkdb.commandline:entrypoint"
 
@@ -126,15 +125,15 @@
 platform.macos.set-pre-install-commands = ["python -m pip install --no-cache-dir --compile --ignore-installed --install-option='--with-openssl' pycurl"]
 
 [tool.hatch.envs.dev.scripts]
 test = "pytest -ra {args}"
 doctest = "test -k 'itkdb or test_true'"
 
 [[tool.hatch.envs.dev.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11", "pypy3.8"]
+python = ["3.8", "3.9", "3.10", "3.11", "pypy3.8"]
 
 [tool.hatch.envs.docs]
 template = "docs"
 dependencies = [
     "mkdocs>=1.4.0",
     "mkdocs-material>=8.5.6",
     # Plugins
@@ -189,40 +188,40 @@
 testpaths = [
   "tests",
   "src",
 ]
 
 [tool.mypy]
 files = "src"
-python_version = "3.7"
+python_version = "3.8"
 warn_unused_configs = true
 strict = true
 hide_error_codes = false
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 
 [[tool.mypy.overrides]]
 module = [
   'simple_settings.*',
   'magic.*',
   'pylibmagic.*',
+  'cachecontrol.*',
 ]
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = [
   'itkdb',
   'itkdb.models',
   'itkdb.models.institution',
   'itkdb.models.file',
   'itkdb.responses',
   'itkdb.caching.*',
   'itkdb.utils',
   'itkdb.exceptions',
-  'itkdb.core',
   'itkdb.client',
   'itkdb.commandline',
   'itkdb.eos',
 ]
 ignore_errors = true
 
 [tool.ruff]
@@ -254,15 +253,15 @@
 ]
 ignore = ["PLR", "E501"]
 typing-modules = ["itkdb.typing"]
 unfixable = ["T20", "F841"]
 isort.required-imports = ["from __future__ import annotations"]
 
 [tool.pylint]
-py-version = "3.7"
+py-version = "3.8"
 ignore-paths= ["src/itkdb/_version.py"]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 messages_control.disable = [
   "design",
   "fixme",
   "line-too-long",
```

### Comparing `itkdb-0.5.1/PKG-INFO` & `itkdb-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.3
 Name: itkdb
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python wrapper to interface with ITk DB.
-Project-URL: Documentation, https://itkdb.docs.cern.ch/0.5/
+Project-URL: Documentation, https://itkdb.docs.cern.ch/0.6/
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itkdb
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itkdb/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/sw/db/itkdb
 Author-email: Giordon Stark <kratsg@gmail.com>
 Maintainer-email: Giordon Stark <kratsg@gmail.com>
 License-File: COPYING
 License-File: LICENSE
@@ -15,21 +15,20 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: attrs
 Requires-Dist: cachecontrol[filecache]
 Requires-Dist: certifi
 Requires-Dist: click>=6.0
 Requires-Dist: importlib-resources; python_version < '3.9'
 Requires-Dist: pylibmagic; platform_system != 'Windows'
 Requires-Dist: python-dotenv
@@ -43,15 +42,15 @@
 Requires-Dist: urllib3>=1.26.11
 Provides-Extra: contrib
 Requires-Dist: html2text; extra == 'contrib'
 Provides-Extra: eos
 Requires-Dist: pycurl; extra == 'eos'
 Description-Content-Type: text/markdown
 
-# ITk DB v0.5.1
+# ITk DB v0.6.0
 
 Python wrapper around the ITk Production Database API.
 
 ---
 
 <!-- sync the following div with docs/index.md -->
 <div align="center">
```

