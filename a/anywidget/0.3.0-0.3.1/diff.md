# Comparing `tmp/anywidget-0.3.0.tar.gz` & `tmp/anywidget-0.3.1.tar.gz`

## Comparing `anywidget-0.3.0.tar` & `anywidget-0.3.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 anywidget-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget.json
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 anywidget-0.3.0/package.json
--rw-r--r--   0        0        0   251374 2020-02-02 00:00:00.000000 anywidget-0.3.0/pnpm-lock.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.3.0/pnpm-workspace.yaml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.3.0/.changeset/config.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/__init__.py
--rw-r--r--   0        0        0    24407 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/_descriptor.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/_file_contents.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/_protocols.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/_util.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/py.typed
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/widget.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/labextension/package.json
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/labextension/static/138.cc3c5434a894a5dab1d2.js
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/labextension/static/326.065deffd433fe1343e66.js
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/labextension/static/remoteEntry.73b94c9a97622529eed7.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/nbextension/extension.js
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 anywidget-0.3.0/anywidget/nbextension/index.js
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/astro.config.mjs
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/package.json
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/tailwind.config.cjs
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/tsconfig.json
--rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/anywidget-overview.png
--rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/banner-dark.png
--rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/banner-light.png
--rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/banner-minimal.png
--rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/client-js-diagram.png
--rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/default-og-image.png
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/favicon.svg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/make-scrollable-code-focusable.js
--rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/public/widget-overview.png
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/scripts/ipynb.mjs
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/scripts/render.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/scripts/utils.mjs
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/consts.ts
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/env.d.ts
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/languages.ts
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/util.ts
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/CodeHero.astro
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/ConfettiButton.astro
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Counter.astro
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/CounterButton.astro
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/HeadCommon.astro
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/HeadSEO.astro
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Hero.astro
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Footer/AvatarList.astro
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Footer/Footer.astro
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/AnyWidgetLogo.astro
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/AstroLogo.astro
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/Header.astro
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/HeaderButton.css
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/LanguageSelect.css
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/LanguageSelect.tsx
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/Search.css
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/Search.tsx
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/SidebarToggle.css
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/SidebarToggle.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/SkipToContent.astro
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/ThemeToggleButton.css
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/Header/ThemeToggleButton.tsx
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/LeftSidebar/LeftSidebar.astro
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/PageContent/PageContent.astro
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/RightSidebar/MoreMenu.astro
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/RightSidebar/RightSidebar.astro
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/RightSidebar/TableOfContents.tsx
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/components/examples/Counter.astro
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/layouts/MainLayout.astro
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/layouts/SplashLayout.astro
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/pages/index.astro
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/pages/blog/anywidget-02.md
--rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/pages/blog/introducing-anywidget.mdx
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/pages/en/bundling.md
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/pages/en/getting-started.mdx
--rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/pages/en/notebooks/counter.ipynb
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/styles/index.css
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.3.0/docs/src/styles/theme.css
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.3.0/examples/Counter.ipynb
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 anywidget-0.3.0/examples/minimal_example.ipynb
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 anywidget-0.3.0/packages/anywidget/CHANGELOG.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.3.0/packages/anywidget/build.mjs
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.3.0/packages/anywidget/package.json
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.3.0/packages/anywidget/src/index.js
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.3.0/packages/anywidget/src/plugin.js
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 anywidget-0.3.0/packages/anywidget/src/widget.js
--rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 anywidget-0.3.0/tests/test_descriptor.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.3.0/tests/test_file_contents.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.3.0/tests/test_protocols.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.3.0/tests/test_utils.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.3.0/tests/test_widget.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.3.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.3.0/LICENSE
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 anywidget-0.3.0/README.md
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 anywidget-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 anywidget-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 anywidget-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget.json
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 anywidget-0.3.1/package.json
+-rw-r--r--   0        0        0   251374 2020-02-02 00:00:00.000000 anywidget-0.3.1/pnpm-lock.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.3.1/pnpm-workspace.yaml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.3.1/.changeset/config.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/__init__.py
+-rw-r--r--   0        0        0    24407 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/_descriptor.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/_file_contents.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/_protocols.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/_util.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/py.typed
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/widget.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/labextension/package.json
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/labextension/static/138.71df560f1970e2814d80.js
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/labextension/static/326.ca449025cbc7a2514a5d.js
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/labextension/static/remoteEntry.2cfd77956dbb25c1a49d.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/nbextension/extension.js
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/nbextension/index.js
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/astro.config.mjs
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/package.json
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/tailwind.config.cjs
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/tsconfig.json
+-rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/anywidget-overview.png
+-rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/banner-dark.png
+-rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/banner-light.png
+-rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/banner-minimal.png
+-rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/client-js-diagram.png
+-rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/default-og-image.png
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/favicon.svg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/make-scrollable-code-focusable.js
+-rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/widget-overview.png
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/scripts/ipynb.mjs
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/scripts/render.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/scripts/utils.mjs
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/consts.ts
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/env.d.ts
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/languages.ts
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/util.ts
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/CodeHero.astro
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/ConfettiButton.astro
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Counter.astro
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/CounterButton.astro
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/HeadCommon.astro
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/HeadSEO.astro
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Hero.astro
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Footer/AvatarList.astro
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Footer/Footer.astro
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/AnyWidgetLogo.astro
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/AstroLogo.astro
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/Header.astro
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/HeaderButton.css
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/LanguageSelect.css
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/LanguageSelect.tsx
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/Search.css
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/Search.tsx
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/SidebarToggle.css
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/SidebarToggle.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/SkipToContent.astro
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/ThemeToggleButton.css
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/ThemeToggleButton.tsx
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/LeftSidebar/LeftSidebar.astro
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/PageContent/PageContent.astro
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/RightSidebar/MoreMenu.astro
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/RightSidebar/RightSidebar.astro
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/RightSidebar/TableOfContents.tsx
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/examples/Counter.astro
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/layouts/MainLayout.astro
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/layouts/SplashLayout.astro
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/pages/index.astro
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/pages/blog/anywidget-02.md
+-rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/pages/blog/introducing-anywidget.mdx
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/pages/en/bundling.md
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/pages/en/getting-started.mdx
+-rw-r--r--   0        0        0    10644 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/pages/en/notebooks/counter.ipynb
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/styles/index.css
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/styles/theme.css
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.3.1/examples/Counter.ipynb
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 anywidget-0.3.1/examples/minimal_example.ipynb
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 anywidget-0.3.1/packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.3.1/packages/anywidget/build.mjs
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.3.1/packages/anywidget/package.json
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.3.1/packages/anywidget/src/index.js
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.3.1/packages/anywidget/src/plugin.js
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 anywidget-0.3.1/packages/anywidget/src/widget.js
+-rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 anywidget-0.3.1/tests/test_descriptor.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.3.1/tests/test_file_contents.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.3.1/tests/test_protocols.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.3.1/tests/test_utils.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.3.1/tests/test_widget.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 anywidget-0.3.1/README.md
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 anywidget-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 anywidget-0.3.1/PKG-INFO
```

### Comparing `anywidget-0.3.0/.pre-commit-config.yaml` & `anywidget-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/package.json` & `anywidget-0.3.1/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/pnpm-lock.yaml` & `anywidget-0.3.1/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/anywidget/_descriptor.py` & `anywidget-0.3.1/anywidget/_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/anywidget/_file_contents.py` & `anywidget-0.3.1/anywidget/_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/anywidget/_protocols.py` & `anywidget-0.3.1/anywidget/_protocols.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/anywidget/_util.py` & `anywidget-0.3.1/anywidget/_util.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/anywidget/widget.py` & `anywidget-0.3.1/anywidget/widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/anywidget/labextension/package.json` & `anywidget-0.3.1/anywidget/labextension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95703125%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.2cfd77956dbb25c1a49d.js'}}",*

 * * "'version'": "'0.3.1'"}*

```diff
@@ -22,15 +22,15 @@
     },
     "files": [
         "dist"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.73b94c9a97622529eed7.js"
+            "load": "static/remoteEntry.2cfd77956dbb25c1a49d.js"
         },
         "extension": "src/plugin",
         "outputDir": "../../anywidget/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -42,9 +42,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `anywidget-0.3.0/anywidget/labextension/static/138.cc3c5434a894a5dab1d2.js` & `anywidget-0.3.1/anywidget/labextension/static/326.ca449025cbc7a2514a5d.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,30 @@
 "use strict";
 (self.webpackChunkanywidget = self.webpackChunkanywidget || []).push([
-    [138], {
-        138: (e, t, i) => {
-            i.r(t), i(203), define(["@jupyter-widgets/base"], create)
+    [326], {
+        326: (e, t, i) => {
+            i.r(t), i.d(t, {
+                default: () => d
+            });
+            var n = i(395),
+                a = i(203),
+                s = i(147);
+            const d = {
+                id: `${s.u2}:plugin`,
+                requires: [n.IJupyterWidgetRegistry],
+                activate: (e, t) => {
+                    let i = (0, a.Z)(n);
+                    t.registerWidget({
+                        name: s.u2,
+                        version: s.i8,
+                        exports: i
+                    })
+                },
+                autoStart: !0
+            }
         },
         203: (e, t, i) => {
             i.d(t, {
                 Z: () => c
             });
             var n = i(147);
 
@@ -61,42 +79,42 @@
                     static view_module_version = n.i8;
                     initialize(...e) {
                         super.initialize(...e), this.on("change:_css", (() => {
                             let e = this.get("_anywidget_id");
                             e && (console.debug(`[anywidget] css hot updated: ${e}`), s(this.get("_css"), e))
                         })), this.on("change:_esm", (async () => {
                             let e = this.get("_anywidget_id");
-                            if (e) {
-                                console.debug(`[anywidget] esm hot updated: ${e}`);
-                                for await (let e of Object.values(this.views ?? {})) {
-                                    let t = await d(this.get("_esm"));
-                                    await e._anywidget_cached_cleanup(), e.$el.empty(), e.stopListening(this);
-                                    let i = await t.render(e);
-                                    i && (this._anywidget_cached_cleanup = i)
-                                }
+                            if (!e) return;
+                            console.debug(`[anywidget] esm hot updated: ${e}`);
+                            let t = Object.values(this.views ?? {});
+                            for await (let e of t) {
+                                let t = await d(this.get("_esm"));
+                                await e._anywidget_cached_cleanup(), e.$el.empty(), e.stopListening(this);
+                                let i = await t.render(e);
+                                e._anywidget_cached_cleanup = i ?? (() => {})
                             }
                         }))
                     }
                 }
                 class i extends e.DOMWidgetView {
                     async render() {
                         await s(this.model.get("_css"), this.model.get("_anywidget_id"));
                         let e = await d(this.model.get("_esm")),
                             t = await e.render(this);
-                        t && (this._anywidget_cached_cleanup = t)
+                        this._anywidget_cached_cleanup = t ?? (() => {})
                     }
-                    async _anywidget_cached_cleanup() {}
+                    _anywidget_cached_cleanup() {}
                     async remove() {
                         return await this._anywidget_cached_cleanup(), super.remove()
                     }
                 }
                 return {
                     AnyModel: t,
                     AnyView: i
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.3.0"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.3.1"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.3.0/anywidget/labextension/static/326.065deffd433fe1343e66.js` & `anywidget-0.3.1/anywidget/labextension/static/138.71df560f1970e2814d80.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,12 @@
 "use strict";
 (self.webpackChunkanywidget = self.webpackChunkanywidget || []).push([
-    [326], {
-        326: (e, t, i) => {
-            i.r(t), i.d(t, {
-                default: () => d
-            });
-            var n = i(395),
-                a = i(203),
-                s = i(147);
-            const d = {
-                id: `${s.u2}:plugin`,
-                requires: [n.IJupyterWidgetRegistry],
-                activate: (e, t) => {
-                    let i = (0, a.Z)(n);
-                    t.registerWidget({
-                        name: s.u2,
-                        version: s.i8,
-                        exports: i
-                    })
-                },
-                autoStart: !0
-            }
+    [138], {
+        138: (e, t, i) => {
+            i.r(t), i(203), define(["@jupyter-widgets/base"], create)
         },
         203: (e, t, i) => {
             i.d(t, {
                 Z: () => c
             });
             var n = i(147);
 
@@ -79,42 +61,42 @@
                     static view_module_version = n.i8;
                     initialize(...e) {
                         super.initialize(...e), this.on("change:_css", (() => {
                             let e = this.get("_anywidget_id");
                             e && (console.debug(`[anywidget] css hot updated: ${e}`), s(this.get("_css"), e))
                         })), this.on("change:_esm", (async () => {
                             let e = this.get("_anywidget_id");
-                            if (e) {
-                                console.debug(`[anywidget] esm hot updated: ${e}`);
-                                for await (let e of Object.values(this.views ?? {})) {
-                                    let t = await d(this.get("_esm"));
-                                    await e._anywidget_cached_cleanup(), e.$el.empty(), e.stopListening(this);
-                                    let i = await t.render(e);
-                                    i && (this._anywidget_cached_cleanup = i)
-                                }
+                            if (!e) return;
+                            console.debug(`[anywidget] esm hot updated: ${e}`);
+                            let t = Object.values(this.views ?? {});
+                            for await (let e of t) {
+                                let t = await d(this.get("_esm"));
+                                await e._anywidget_cached_cleanup(), e.$el.empty(), e.stopListening(this);
+                                let i = await t.render(e);
+                                e._anywidget_cached_cleanup = i ?? (() => {})
                             }
                         }))
                     }
                 }
                 class i extends e.DOMWidgetView {
                     async render() {
                         await s(this.model.get("_css"), this.model.get("_anywidget_id"));
                         let e = await d(this.model.get("_esm")),
                             t = await e.render(this);
-                        t && (this._anywidget_cached_cleanup = t)
+                        this._anywidget_cached_cleanup = t ?? (() => {})
                     }
-                    async _anywidget_cached_cleanup() {}
+                    _anywidget_cached_cleanup() {}
                     async remove() {
                         return await this._anywidget_cached_cleanup(), super.remove()
                     }
                 }
                 return {
                     AnyModel: t,
                     AnyView: i
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.3.0"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.3.1"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.3.0/anywidget/labextension/static/remoteEntry.73b94c9a97622529eed7.js` & `anywidget-0.3.1/anywidget/labextension/static/remoteEntry.2cfd77956dbb25c1a49d.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, v = {
+    var e, r, t, n, o, a, i, u, f, l, s, d, c, p, h, v = {
             408: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(138).then((() => () => t(138))),
                         "./extension": () => t.e(326).then((() => () => t(326)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -41,45 +41,45 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        138: "cc3c5434a894a5dab1d2",
-        326: "065deffd433fe1343e66"
+        138: "71df560f1970e2814d80",
+        326: "ca449025cbc7a2514a5d"
     } [e] + ".js?v=" + {
-        138: "cc3c5434a894a5dab1d2",
-        326: "065deffd433fe1343e66"
+        138: "71df560f1970e2814d80",
+        326: "ca449025cbc7a2514a5d"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", m.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var s = l[f];
+                for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
+                    var s = f[l];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
                         i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -104,15 +104,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => m.e(138).then((() => () => m(138))),
                         from: i,
                         eager: !1
                     })
-                })("anywidget", "0.3.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("anywidget", "0.3.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -147,94 +147,94 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
         for (a = 1; a < e.length; a++) {
             var u = e[a];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
+            i.push(0 === u ? "not(" + f() + ")" : 1 === u ? "(" + f() + " || " + f() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
-        return l();
+        return f();
 
-        function l() {
+        function f() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+            for (var i = 0, u = 1, f = !0;; u++, i++) {
+                var l, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(l = r[i]))[0])) return !f || ("u" == d ? u > n && !o : "" == d != o);
                 if ("u" == s) {
-                    if (!l || "u" != d) return !1
-                } else if (l)
+                    if (!f || "u" != d) return !1
+                } else if (f)
                     if (d == s)
                         if (u <= n) {
-                            if (f != e[u]) return !1
+                            if (l != e[u]) return !1
                         } else {
-                            if (o ? f > e[u] : f < e[u]) return !1;
-                            f != e[u] && (l = !1)
+                            if (o ? l > e[u] : l < e[u]) return !1;
+                            l != e[u] && (f = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
-                    l = !1, u--
+                    f = !1, u--
                 } else {
                     if (u <= n || s < d != o) return !1;
-                    l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                    f = !1
+                } else "s" != d && "n" != d && (f = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, i = (e, r) => {
         var t = m.S[e];
         if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), s(e[t][o])
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(f(e, t, o, n)), s(e[t][o])
     }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
         var a = m.I(r);
         return a && a.then ? a.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), p = {}, c = {
+    })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), c = {}, p = {
         395: () => d("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ])
     }, h = {
         326: [395]
     }, m.f.consumes = (e, r) => {
         m.o(h, e) && h[e].forEach((e => {
-            if (m.o(p, e)) return r.push(p[e]);
+            if (m.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    p[e] = 0, m.m[e] = t => {
+                    c[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete p[e], m.m[e] = t => {
+                    delete c[e], m.m[e] = t => {
                         throw delete m.c[e], r
                     }
                 };
             try {
-                var o = c[e]();
-                o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
+                var o = p[e]();
+                o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             957: 0
@@ -255,20 +255,20 @@
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
-                    l = 0;
+                    f = 0;
                 if (a.some((r => 0 !== e[r]))) {
                     for (n in i) m.o(i, n) && (m.m[n] = i[n]);
                     u && u(m)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); f < a.length; f++) o = a[f], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkanywidget = self.webpackChunkanywidget || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
     var b = m(408);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = b
 })();
```

### Comparing `anywidget-0.3.0/anywidget/nbextension/index.js` & `anywidget-0.3.1/anywidget/nbextension/index.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 // package.json
 var name = "anywidget";
-var version = "0.3.0";
+var version = "0.3.1";
 
 // src/widget.js
 function is_href(str) {
     return str.startsWith("http://") || str.startsWith("https://");
 }
 async function load_css_href(href, anywidget_id) {
     let prev = document.querySelector(`link[id='${anywidget_id}']`);
@@ -93,36 +93,38 @@
                 load_css(this.get("_css"), id);
             });
             this.on("change:_esm", async () => {
                 let id = this.get("_anywidget_id");
                 if (!id)
                     return;
                 console.debug(`[anywidget] esm hot updated: ${id}`);
-                for await (let view of Object.values(this.views ?? {})) {
+                let views = (
+                    /** @type {Promise<AnyView>[]} */
+                    Object.values(this.views ?? {})
+                );
+                for await (let view of views) {
                     let widget = await load_esm(this.get("_esm"));
-                    await /** @type {AnyView} */
-                    view._anywidget_cached_cleanup();
+                    await view._anywidget_cached_cleanup();
                     view.$el.empty();
                     view.stopListening(this);
                     let cleanup = await widget.render(view);
-                    if (cleanup)
-                        this._anywidget_cached_cleanup = cleanup;
+                    view._anywidget_cached_cleanup = cleanup ?? (() => {});
                 }
             });
         }
     }
     class AnyView extends base.DOMWidgetView {
         async render() {
             await load_css(this.model.get("_css"), this.model.get("_anywidget_id"));
             let widget = await load_esm(this.model.get("_esm"));
             let cleanup = await widget.render(this);
-            if (cleanup)
-                this._anywidget_cached_cleanup = cleanup;
+            this._anywidget_cached_cleanup = cleanup ?? (() => {});
         }
-        async _anywidget_cached_cleanup() {}
+        /** @type {() => Promise<void> | void} */
+        _anywidget_cached_cleanup() {}
         async remove() {
             await this._anywidget_cached_cleanup();
             return super.remove();
         }
     }
     return {
         AnyModel,
```

### Comparing `anywidget-0.3.0/docs/README.md` & `anywidget-0.3.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/astro.config.mjs` & `anywidget-0.3.1/docs/astro.config.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/package.json` & `anywidget-0.3.1/docs/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/public/anywidget-overview.png` & `anywidget-0.3.1/docs/public/anywidget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/public/banner-dark.png` & `anywidget-0.3.1/docs/public/banner-dark.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/public/banner-light.png` & `anywidget-0.3.1/docs/public/banner-light.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/public/banner-minimal.png` & `anywidget-0.3.1/docs/public/banner-minimal.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/public/client-js-diagram.png` & `anywidget-0.3.1/docs/public/client-js-diagram.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/public/default-og-image.png` & `anywidget-0.3.1/docs/public/default-og-image.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/public/favicon.svg` & `anywidget-0.3.1/docs/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/public/widget-overview.png` & `anywidget-0.3.1/docs/public/widget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/scripts/ipynb.mjs` & `anywidget-0.3.1/docs/scripts/ipynb.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/scripts/utils.mjs` & `anywidget-0.3.1/docs/scripts/utils.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/consts.ts` & `anywidget-0.3.1/docs/src/consts.ts`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/CodeHero.astro` & `anywidget-0.3.1/docs/src/components/CodeHero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/CounterButton.astro` & `anywidget-0.3.1/docs/src/components/CounterButton.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/HeadCommon.astro` & `anywidget-0.3.1/docs/src/components/HeadCommon.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/HeadSEO.astro` & `anywidget-0.3.1/docs/src/components/HeadSEO.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/Hero.astro` & `anywidget-0.3.1/docs/src/components/Hero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/Footer/AvatarList.astro` & `anywidget-0.3.1/docs/src/components/Footer/AvatarList.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/Header/AnyWidgetLogo.astro` & `anywidget-0.3.1/docs/src/components/Header/AnyWidgetLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/Header/AstroLogo.astro` & `anywidget-0.3.1/docs/src/components/Header/AstroLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/Header/Header.astro` & `anywidget-0.3.1/docs/src/components/Header/Header.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/Header/HeaderButton.css` & `anywidget-0.3.1/docs/src/components/Header/HeaderButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/Header/LanguageSelect.css` & `anywidget-0.3.1/docs/src/components/Header/LanguageSelect.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/Header/LanguageSelect.tsx` & `anywidget-0.3.1/docs/src/components/Header/LanguageSelect.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/Header/Search.css` & `anywidget-0.3.1/docs/src/components/Header/Search.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/Header/Search.tsx` & `anywidget-0.3.1/docs/src/components/Header/Search.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/Header/SidebarToggle.tsx` & `anywidget-0.3.1/docs/src/components/Header/SidebarToggle.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/Header/ThemeToggleButton.css` & `anywidget-0.3.1/docs/src/components/Header/ThemeToggleButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/Header/ThemeToggleButton.tsx` & `anywidget-0.3.1/docs/src/components/Header/ThemeToggleButton.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/LeftSidebar/LeftSidebar.astro` & `anywidget-0.3.1/docs/src/components/LeftSidebar/LeftSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/PageContent/PageContent.astro` & `anywidget-0.3.1/docs/src/components/PageContent/PageContent.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/RightSidebar/MoreMenu.astro` & `anywidget-0.3.1/docs/src/components/RightSidebar/MoreMenu.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/RightSidebar/RightSidebar.astro` & `anywidget-0.3.1/docs/src/components/RightSidebar/RightSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/RightSidebar/TableOfContents.tsx` & `anywidget-0.3.1/docs/src/components/RightSidebar/TableOfContents.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/components/examples/Counter.astro` & `anywidget-0.3.1/docs/src/components/examples/Counter.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/layouts/MainLayout.astro` & `anywidget-0.3.1/docs/src/layouts/MainLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/layouts/SplashLayout.astro` & `anywidget-0.3.1/docs/src/layouts/SplashLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/pages/blog/anywidget-02.md` & `anywidget-0.3.1/docs/src/pages/blog/anywidget-02.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/pages/blog/introducing-anywidget.mdx` & `anywidget-0.3.1/docs/src/pages/blog/introducing-anywidget.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/pages/en/bundling.md` & `anywidget-0.3.1/docs/src/pages/en/bundling.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/pages/en/getting-started.mdx` & `anywidget-0.3.1/docs/src/pages/en/getting-started.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md` & `anywidget-0.3.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 are the easiest and most flexible way to synchronize data between the
 front end and Python. The `sync=True` keyword argument tells the widget
 framework to handle synchronizing that value to the front end. Take the following
 `CustomWidget`:
 
 ```python
 class CustomWidget(anywidget.AnyWidget):
-    _esm = (pathlib.Path(__file__).parent / "index.js").read_text()
+    _esm = pathlib.Path("index.js")
     my_value = traitlets.Int(0).tag(sync=True)
 ```
 
 It defines an Integer `my_value` trait, which is synchronized with the front
 end. The `render` function now has the ability to:
 
 - **get** `my_value`
```

### Comparing `anywidget-0.3.0/docs/src/pages/en/notebooks/counter.ipynb` & `anywidget-0.3.1/docs/src/pages/en/notebooks/counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/styles/index.css` & `anywidget-0.3.1/docs/src/styles/index.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/docs/src/styles/theme.css` & `anywidget-0.3.1/docs/src/styles/theme.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/examples/Counter.ipynb` & `anywidget-0.3.1/examples/Counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/examples/minimal_example.ipynb` & `anywidget-0.3.1/examples/minimal_example.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/packages/anywidget/CHANGELOG.md` & `anywidget-0.3.1/packages/anywidget/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # anywidget
 
+## 0.3.1
+
+### Patch Changes
+
+- fix: properly cache cleanup function for HMR ([#122](https://github.com/manzt/anywidget/pull/122))
+
 ## 0.3.0
 
 ### Minor Changes
 
 - fix: replace deprecated `ipykernel.comm.Comm` with `comm` module ([#119](https://github.com/manzt/anywidget/pull/119))
 
 ### Patch Changes
```

### Comparing `anywidget-0.3.0/packages/anywidget/build.mjs` & `anywidget-0.3.1/packages/anywidget/build.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/packages/anywidget/package.json` & `anywidget-0.3.1/packages/anywidget/package.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.3.1'"}*

```diff
@@ -38,9 +38,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `anywidget-0.3.0/packages/anywidget/src/widget.js` & `anywidget-0.3.1/packages/anywidget/src/widget.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -134,20 +134,23 @@
 
             // Handles ESM updates from anywidget during development.
             this.on("change:_esm", async () => {
                 let id = this.get("_anywidget_id");
                 if (!id) return;
                 console.debug(`[anywidget] esm hot updated: ${id}`);
 
-                for await (let view of Object.values(this.views ?? {})) {
+                let views = ( /** @type {Promise<AnyView>[]} */ (Object.values(this.views ?? {})));
+
+                for await (let view of views) {
+
                     // load updated esm
                     let widget = await load_esm(this.get("_esm"));
 
                     // call any cleanup logic defined by the previous module.
-                    await ( /** @type {AnyView} */ (view))._anywidget_cached_cleanup();
+                    await view._anywidget_cached_cleanup();
 
                     // `view.$el` is a cached jQuery object for the view's element.
                     // This removes all child nodes but avoids deleting the root so
                     // we can rerender.
                     view.$el.empty();
 
                     // Unsubscribe from any handlers registered to `view.listenTo`
@@ -159,29 +162,30 @@
                     // e.g., `model.off(null, null, anywidgetSymbol)`, but that might
                     // be more trouble than it's worth and this is just a feature for
                     // development.
                     view.stopListening(this);
 
                     // render the view with the updated render
                     let cleanup = await widget.render(view);
-                    if (cleanup) this._anywidget_cached_cleanup = cleanup;
+                    view._anywidget_cached_cleanup = cleanup ?? (() => {});
                 }
             });
         }
     }
 
     class AnyView extends base.DOMWidgetView {
         async render() {
             await load_css(this.model.get("_css"), this.model.get("_anywidget_id"));
             let widget = await load_esm(this.model.get("_esm"));
             let cleanup = await widget.render(this);
-            if (cleanup) this._anywidget_cached_cleanup = cleanup;
+            this._anywidget_cached_cleanup = cleanup ?? (() => {});
         }
 
-        async _anywidget_cached_cleanup() {}
+        /** @type {() => Promise<void> | void} */
+        _anywidget_cached_cleanup() {}
 
         async remove() {
             // call any user-defined cleanup logic before this view is completely removed.
             await this._anywidget_cached_cleanup();
             return super.remove();
         }
     }
```

### Comparing `anywidget-0.3.0/tests/test_descriptor.py` & `anywidget-0.3.1/tests/test_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/tests/test_file_contents.py` & `anywidget-0.3.1/tests/test_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/tests/test_utils.py` & `anywidget-0.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/tests/test_widget.py` & `anywidget-0.3.1/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/LICENSE` & `anywidget-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/README.md` & `anywidget-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/pyproject.toml` & `anywidget-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.0/PKG-INFO` & `anywidget-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anywidget
-Version: 0.3.0
+Version: 0.3.1
 Summary: custom jupyter widgets made easy
 Project-URL: homepage, https://github.com/manzt/anywidget
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata; python_version < '3.8'
```

