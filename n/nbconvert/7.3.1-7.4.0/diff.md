# Comparing `tmp/nbconvert-7.3.1.tar.gz` & `tmp/nbconvert-7.4.0.tar.gz`

## Comparing `nbconvert-7.3.1.tar` & `nbconvert-7.4.0.tar`

### file list

```diff
@@ -1,276 +1,277 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.git-blame-ignore-revs
--rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.mailmap
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.prettierignore
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.readthedocs.yaml
--rw-r--r--   0        0        0    70125 2020-02-02 00:00:00.000000 nbconvert-7.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 nbconvert-7.3.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 nbconvert-7.3.1/RELEASE.md
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 nbconvert-7.3.1/check_requirements.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nbconvert-7.3.1/codecov.yml
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/dependabot.yml
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/Makefile
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/README.md
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/autogen_config.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/make.bat
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/api_examples/template_path/make_html.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/api_examples/template_path/quiz_notebook.py
--rw-r--r--   0        0        0    36829 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/api_examples/template_path/media/image1.png
--rw-r--r--   0        0        0   176383 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/api_examples/template_path/media/image2.png
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/conf.json
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2
--rw-r--r--   0        0        0   266255 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css
--rw-r--r--   0        0        0     8651 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/architecture.rst
--rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/conf.py
--rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/customizing.rst
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/dejavu.rst
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/development_release.rst
--rw-r--r--   0        0        0     7875 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/execute_api.rst
--rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/external_exporters.rst
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/highlighting.rst
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/index.rst
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/install.rst
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/latex_citations.rst
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/nbconvert_library.ipynb
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/need_help.rst
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/removing_cells.rst
--rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/usage.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/_static/empty.txt
--rw-r--r--   0        0        0    36971 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/_static/exporter_inheritance.png
--rw-r--r--   0        0        0    65726 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/_static/preprocessor_inheritance.png
--rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/_static/writer_inheritance.png
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/api/exporters.rst
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/api/filters.rst
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/api/index.rst
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/api/nbconvertapp.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/api/postprocessors.rst
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/api/preprocessors.rst
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/api/writers.rst
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/__main__.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/_version.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/conftest.py
--rwxr-xr-x   0        0        0    24764 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/nbconvertapp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/py.typed
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/__init__.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/asciidoc.py
--rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/base.py
--rw-r--r--   0        0        0    12643 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/exporter.py
--rw-r--r--   0        0        0    11185 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/html.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/latex.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/markdown.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/notebook.py
--rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/pdf.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/python.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/qt_exporter.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/qt_screenshot.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/qtpdf.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/qtpng.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/rst.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/script.py
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/slides.py
--rw-r--r--   0        0        0    26957 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/templateexporter.py
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/webpdf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/__init__.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/base.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/cheese.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_asciidoc.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_export.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_exporter.py
--rw-r--r--   0        0        0     7891 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_html.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_latex.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_markdown.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_notebook.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_pdf.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_python.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_qtpdf.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_qtpng.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_rst.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_script.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_slides.py
--rw-r--r--   0        0        0    27769 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_templateexporter.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_webpdf.py
--rw-r--r--   0        0        0    45585 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/attachment.ipynb
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/lablike.html.j2
--rw-r--r--   0        0        0    10437 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/notebook2.ipynb
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/notebook3.ipynb
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/notebook_inject.ipynb
--rw-r--r--   0        0        0    16782 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/pngmetadata.ipynb
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/prompt_numbers.ipynb
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/rawtest.ipynb
--rw-r--r--   0        0        0    19943 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/svg.ipynb
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/__init__.py
--rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/ansi.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/citation.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/datatypefilter.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/filter_links.py
--rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/highlight.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/latex.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/markdown.py
--rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/markdown_mistune.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/metadata.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/pandoc.py
--rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/strings.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/svg_constants.py
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/widgetsdatatypefilter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/__init__.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/test_ansi.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/test_citation.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/test_datatypefilter.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/test_highlight.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/test_latex.py
--rw-r--r--   0        0        0     8534 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/test_markdown.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/test_metadata.py
--rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/test_strings.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/postprocessors/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/postprocessors/base.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/postprocessors/serve.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/postprocessors/tests/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/postprocessors/tests/test_serve.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/__init__.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/base.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/clearmetadata.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/clearoutput.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/coalescestreams.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/convertfigures.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/csshtmlheader.py
--rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/execute.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/extractoutput.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/highlightmagics.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/latex.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/regexremove.py
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/sanitize.py
--rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/svg2pdf.py
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tagremove.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/__init__.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/base.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/fake_kernelmanager.py
--rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_clearmetadata.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_clearoutput.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_coalescestreams.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_csshtmlheader.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_execute.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_extractoutput.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_highlightmagics.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_latex.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_regexremove.py
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_sanitize.py
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_svg2pdf.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_tagremove.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/files/HelloWorld.ipynb
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/resources/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/templates/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/templates/skeleton/Makefile
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/templates/skeleton/README.md
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/__init__.py
--rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/base.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/fake_exporters.py
--rw-r--r--   0        0        0    28677 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/test_nbconvertapp.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/utils.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/exporter_entrypoint/eptest.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/exporter_entrypoint/eptest-0.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/Unexecuted_widget.ipynb
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/Unexecuted_widget_2.ipynb
--rw-r--r--   0        0        0    96479 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/Widget_List.ipynb
--rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/containerized_deployments.jpeg
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/hello.py
--rw-r--r--   0        0        0    18524 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/issue1849_svg.ipynb
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/jupyter_nbconvert_config.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/latex-linked-image.ipynb
--rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/markdown_display_priority.ipynb
--rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/notebook1.ipynb
--rw-r--r--   0        0        0   125459 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/notebook2.ipynb
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/notebook3_with_errors.ipynb
--rw-r--r--   0        0        0    18657 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/notebook4_jpeg.ipynb
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/notebook5_embed_images.ipynb
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/notebook_jl.ipynb
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/notebook_tags.ipynb
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/override.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/testimage.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/_contextlib_chdir.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/base.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/exceptions.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/io.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/lexers.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/pandoc.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/text.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/tests/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/tests/test_io.py
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/tests/test_pandoc.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/tests/test_version.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/__init__.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/base.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/debug.py
--rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/files.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/stdout.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/tests/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/tests/test_debug.py
--rw-r--r--   0        0        0    10268 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/tests/test_files.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/tests/test_stdout.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/asciidoc/conf.json
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/asciidoc/index.asciidoc.j2
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/base/cell_id_anchor.j2
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/base/celltags.j2
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/base/display_priority.j2
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/base/jupyter_widgets.html.j2
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/base/mathjax.html.j2
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/base/null.j2
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/basic/conf.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/basic/index.html.j2
--rw-r--r--   0        0        0     8261 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/classic/base.html.j2
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/classic/conf.json
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/classic/index.html.j2
--rw-r--r--   0        0        0   265101 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/classic/static/style.css
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/compatibility/display_priority.tpl
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/compatibility/full.tpl
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/lab/base.html.j2
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/lab/conf.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/lab/index.html.j2
--rw-r--r--   0        0        0   581722 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/lab/static/index.css
--rw-r--r--   0        0        0    16733 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/lab/static/theme-dark.css
--rw-r--r--   0        0        0    15637 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/lab/static/theme-light.css
--rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/base.tex.j2
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/conf.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/display_priority.j2
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/document_contents.tex.j2
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/index.tex.j2
--rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/null.j2
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/report.tex.j2
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/style_bw_ipython.tex.j2
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/style_bw_python.tex.j2
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/style_ipython.tex.j2
--rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/style_jupyter.tex.j2
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/style_python.tex.j2
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/markdown/conf.json
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/markdown/index.md.j2
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/python/conf.json
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/python/index.py.j2
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/reveal/base.html.j2
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/reveal/cellslidedata.j2
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/reveal/conf.json
--rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/reveal/index.html.j2
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/reveal/static/custom_reveal.css
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/rst/conf.json
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/rst/index.rst.j2
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/script/conf.json
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/script/script.j2
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/webpdf/conf.json
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/webpdf/index.pdf.j2
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.gitignore
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 nbconvert-7.3.1/LICENSE
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 nbconvert-7.3.1/README.md
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 nbconvert-7.3.1/hatch_build.py
--rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 nbconvert-7.3.1/pyproject.toml
--rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 nbconvert-7.3.1/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.mailmap
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.prettierignore
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.readthedocs.yaml
+-rw-r--r--   0        0        0    72042 2020-02-02 00:00:00.000000 nbconvert-7.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 nbconvert-7.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 nbconvert-7.4.0/RELEASE.md
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 nbconvert-7.4.0/check_requirements.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/Makefile
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/README.md
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/autogen_config.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/make.bat
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/api_examples/template_path/make_html.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/api_examples/template_path/quiz_notebook.py
+-rw-r--r--   0        0        0    36829 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/api_examples/template_path/media/image1.png
+-rw-r--r--   0        0        0   176383 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/api_examples/template_path/media/image2.png
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/conf.json
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2
+-rw-r--r--   0        0        0   266255 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css
+-rw-r--r--   0        0        0     8651 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/architecture.rst
+-rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/conf.py
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/customizing.rst
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/dejavu.rst
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/development_release.rst
+-rw-r--r--   0        0        0     7875 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/execute_api.rst
+-rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/external_exporters.rst
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/highlighting.rst
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/index.rst
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/install.rst
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/latex_citations.rst
+-rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/nbconvert_library.ipynb
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/need_help.rst
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/removing_cells.rst
+-rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/usage.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/_static/empty.txt
+-rw-r--r--   0        0        0    36971 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/_static/exporter_inheritance.png
+-rw-r--r--   0        0        0    65726 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/_static/preprocessor_inheritance.png
+-rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/_static/writer_inheritance.png
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/api/exporters.rst
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/api/filters.rst
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/api/index.rst
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/api/nbconvertapp.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/api/postprocessors.rst
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/api/preprocessors.rst
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/api/writers.rst
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/__main__.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/_version.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/conftest.py
+-rwxr-xr-x   0        0        0    24129 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/nbconvertapp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/py.typed
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/__init__.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/asciidoc.py
+-rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/base.py
+-rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/exporter.py
+-rw-r--r--   0        0        0    11270 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/html.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/latex.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/markdown.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/notebook.py
+-rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/pdf.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/python.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/qt_exporter.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/qt_screenshot.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/qtpdf.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/qtpng.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/rst.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/script.py
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/slides.py
+-rw-r--r--   0        0        0    26970 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/templateexporter.py
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/webpdf.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/__init__.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/base.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/cheese.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_asciidoc.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_export.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_exporter.py
+-rw-r--r--   0        0        0     7891 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_html.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_latex.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_markdown.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_notebook.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_pdf.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_python.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_qtpdf.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_qtpng.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_rst.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_script.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_slides.py
+-rw-r--r--   0        0        0    27769 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_templateexporter.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_webpdf.py
+-rw-r--r--   0        0        0    45585 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/attachment.ipynb
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/lablike.html.j2
+-rw-r--r--   0        0        0    10437 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/notebook2.ipynb
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/notebook3.ipynb
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/notebook_inject.ipynb
+-rw-r--r--   0        0        0    16782 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/pngmetadata.ipynb
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/prompt_numbers.ipynb
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/rawtest.ipynb
+-rw-r--r--   0        0        0    19943 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/svg.ipynb
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/__init__.py
+-rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/ansi.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/citation.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/datatypefilter.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/filter_links.py
+-rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/highlight.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/latex.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/markdown.py
+-rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/markdown_mistune.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/metadata.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/pandoc.py
+-rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/strings.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/svg_constants.py
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/widgetsdatatypefilter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/__init__.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/test_ansi.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/test_citation.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/test_datatypefilter.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/test_highlight.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/test_latex.py
+-rw-r--r--   0        0        0     8534 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/test_markdown.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/test_metadata.py
+-rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/test_strings.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/postprocessors/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/postprocessors/base.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/postprocessors/serve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/postprocessors/tests/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/postprocessors/tests/test_serve.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/__init__.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/base.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/clearmetadata.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/clearoutput.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/coalescestreams.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/convertfigures.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/csshtmlheader.py
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/execute.py
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/extractattachments.py
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/extractoutput.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/highlightmagics.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/latex.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/regexremove.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/sanitize.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/svg2pdf.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tagremove.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/__init__.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/base.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/fake_kernelmanager.py
+-rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_clearmetadata.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_clearoutput.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_coalescestreams.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_csshtmlheader.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_execute.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_extractattachments.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_extractoutput.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_highlightmagics.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_latex.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_regexremove.py
+-rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_sanitize.py
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_svg2pdf.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_tagremove.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/files/HelloWorld.ipynb
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/resources/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/templates/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/templates/skeleton/Makefile
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/templates/skeleton/README.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/__init__.py
+-rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/base.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/fake_exporters.py
+-rw-r--r--   0        0        0    29353 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/test_nbconvertapp.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/utils.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/exporter_entrypoint/eptest.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/exporter_entrypoint/eptest-0.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/Unexecuted_widget.ipynb
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/Unexecuted_widget_2.ipynb
+-rw-r--r--   0        0        0    96479 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/Widget_List.ipynb
+-rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/containerized_deployments.jpeg
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/hello.py
+-rw-r--r--   0        0        0    18524 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/issue1849_svg.ipynb
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/jupyter_nbconvert_config.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/latex-linked-image.ipynb
+-rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/markdown_display_priority.ipynb
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/notebook1.ipynb
+-rw-r--r--   0        0        0   125459 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/notebook2.ipynb
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/notebook3_with_errors.ipynb
+-rw-r--r--   0        0        0    18657 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/notebook4_jpeg.ipynb
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/notebook5_embed_images.ipynb
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/notebook_jl.ipynb
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/notebook_tags.ipynb
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/override.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/testimage.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/_contextlib_chdir.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/base.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/exceptions.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/io.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/lexers.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/pandoc.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/text.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/tests/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/tests/test_io.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/tests/test_pandoc.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/tests/test_version.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/__init__.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/base.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/debug.py
+-rw-r--r--   0        0        0     6017 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/files.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/stdout.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/tests/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/tests/test_debug.py
+-rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/tests/test_files.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/tests/test_stdout.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/asciidoc/conf.json
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/asciidoc/index.asciidoc.j2
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/base/cell_id_anchor.j2
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/base/celltags.j2
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/base/display_priority.j2
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/base/jupyter_widgets.html.j2
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/base/mathjax.html.j2
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/base/null.j2
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/basic/conf.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/basic/index.html.j2
+-rw-r--r--   0        0        0     8261 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/classic/base.html.j2
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/classic/conf.json
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/classic/index.html.j2
+-rw-r--r--   0        0        0   265101 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/classic/static/style.css
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/compatibility/display_priority.tpl
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/compatibility/full.tpl
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/lab/base.html.j2
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/lab/conf.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/lab/index.html.j2
+-rw-r--r--   0        0        0   581722 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/lab/static/index.css
+-rw-r--r--   0        0        0    16733 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/lab/static/theme-dark.css
+-rw-r--r--   0        0        0    15637 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/lab/static/theme-light.css
+-rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/base.tex.j2
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/conf.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/display_priority.j2
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/document_contents.tex.j2
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/index.tex.j2
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/null.j2
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/report.tex.j2
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/style_bw_ipython.tex.j2
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/style_bw_python.tex.j2
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/style_ipython.tex.j2
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/style_jupyter.tex.j2
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/style_python.tex.j2
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/markdown/conf.json
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/markdown/index.md.j2
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/python/conf.json
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/python/index.py.j2
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/reveal/base.html.j2
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/reveal/cellslidedata.j2
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/reveal/conf.json
+-rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/reveal/index.html.j2
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/reveal/static/custom_reveal.css
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/rst/conf.json
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/rst/index.rst.j2
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/script/conf.json
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/script/script.j2
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/webpdf/conf.json
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/webpdf/index.pdf.j2
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.gitignore
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 nbconvert-7.4.0/LICENSE
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 nbconvert-7.4.0/README.md
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 nbconvert-7.4.0/hatch_build.py
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 nbconvert-7.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7925 2020-02-02 00:00:00.000000 nbconvert-7.4.0/PKG-INFO
```

### Comparing `nbconvert-7.3.1/.mailmap` & `nbconvert-7.4.0/.mailmap`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/.pre-commit-config.yaml` & `nbconvert-7.4.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -32,11 +32,11 @@
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.260
+    rev: v0.0.263
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `nbconvert-7.3.1/CHANGELOG.md` & `nbconvert-7.4.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,39 @@
 # Changes in nbconvert
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 7.4.0
+
+([Full Changelog](https://github.com/jupyter/nbconvert/compare/v7.3.1...32fcf7b26462f5d51d577f8beda9d49cd3a0f441))
+
+### Enhancements made
+
+- Add ExtractAttachmentsPreprocessor [#1978](https://github.com/jupyter/nbconvert/pull/1978) ([@tuncbkose](https://github.com/tuncbkose))
+
+### Bugs fixed
+
+- Moved ensure_dir_exists to FilesWriter [#1987](https://github.com/jupyter/nbconvert/pull/1987) ([@tuncbkose](https://github.com/tuncbkose))
+- Tweak exporter default_config merging behavior [#1981](https://github.com/jupyter/nbconvert/pull/1981) ([@tuncbkose](https://github.com/tuncbkose))
+- Revert unintended effects of #1966 [#1974](https://github.com/jupyter/nbconvert/pull/1974) ([@tuncbkose](https://github.com/tuncbkose))
+
+### Maintenance and upkeep improvements
+
+- Fix test_errors_print_traceback test [#1985](https://github.com/jupyter/nbconvert/pull/1985) ([@blink1073](https://github.com/blink1073))
+- Ensure toml support in coverage reporting [#1984](https://github.com/jupyter/nbconvert/pull/1984) ([@blink1073](https://github.com/blink1073))
+- Use local coverage [#1976](https://github.com/jupyter/nbconvert/pull/1976) ([@blink1073](https://github.com/blink1073))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter/nbconvert/graphs/contributors?from=2023-04-10&to=2023-05-08&type=c))
+
+[@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Ablink1073+updated%3A2023-04-10..2023-05-08&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Akrassowski+updated%3A2023-04-10..2023-05-08&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Apre-commit-ci+updated%3A2023-04-10..2023-05-08&type=Issues) | [@tuncbkose](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Atuncbkose+updated%3A2023-04-10..2023-05-08&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 7.3.1
 
 ([Full Changelog](https://github.com/jupyter/nbconvert/compare/v7.3.0...3860152ecea3d9833540eebe279ff603b3d47cea))
 
 ### Bugs fixed
 
 - Remove overwriting of default KernelManager [#1972](https://github.com/jupyter/nbconvert/pull/1972) ([@tuncbkose](https://github.com/tuncbkose))
@@ -14,16 +42,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter/nbconvert/graphs/contributors?from=2023-04-03&to=2023-04-10&type=c))
 
 [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Apre-commit-ci+updated%3A2023-04-03..2023-04-10&type=Issues) | [@tuncbkose](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Atuncbkose+updated%3A2023-04-03..2023-04-10&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 7.3.0
 
 ([Full Changelog](https://github.com/jupyter/nbconvert/compare/v7.2.10...056dc4ecc8f9f3e9249f0dbddf1221c65228b961))
 
 ### Enhancements made
 
 - Allow pattern in output_base [#1967](https://github.com/jupyter/nbconvert/pull/1967) ([@JeppeKlitgaard](https://github.com/JeppeKlitgaard))
```

### Comparing `nbconvert-7.3.1/CONTRIBUTING.md` & `nbconvert-7.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/RELEASE.md` & `nbconvert-7.4.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/check_requirements.py` & `nbconvert-7.4.0/check_requirements.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/.github/workflows/docs.yml` & `nbconvert-7.4.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/.github/workflows/prep-release.yml` & `nbconvert-7.4.0/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/.github/workflows/publish-release.yml` & `nbconvert-7.4.0/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/.github/workflows/tests.yml` & `nbconvert-7.4.0/.github/workflows/tests.yml`

 * *Files 7% similar despite different names*

```diff
@@ -50,18 +50,23 @@
           xvfb-run --auto-servernum hatch run cov:test
 
       - name: Run tests on other platforms
         if: ${{ !startsWith(runner.os, 'linux')  }}
         run: |
           hatch run cov:test
 
-      - name: Code coverage
-        run: |
-          pip install codecov coverage[toml]
-          codecov
+      - uses: jupyterlab/maintainer-tools/.github/actions/upload-coverage@v1
+
+  coverage:
+    runs-on: ubuntu-latest
+    needs:
+      - run-tests
+    steps:
+      - uses: actions/checkout@v3
+      - uses: jupyterlab/maintainer-tools/.github/actions/report-coverage@v1
 
   test_lint:
     name: Test Lint
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
@@ -141,15 +146,15 @@
     steps:
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
       - uses: jupyterlab/maintainer-tools/.github/actions/test-sdist@v1
 
   tests_check: # This job does nothing and is only used for the branch protection
     if: always()
     needs:
-      - run-tests
+      - coverage
       - test_lint
       - test_minimum_versions
       - test_prereleases
       - check_links
       - check_release
       - test_sdist
     runs-on: ubuntu-latest
```

### Comparing `nbconvert-7.3.1/docs/Makefile` & `nbconvert-7.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/README.md` & `nbconvert-7.4.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/autogen_config.py` & `nbconvert-7.4.0/docs/autogen_config.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/make.bat` & `nbconvert-7.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/api_examples/template_path/make_html.py` & `nbconvert-7.4.0/docs/api_examples/template_path/make_html.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/api_examples/template_path/quiz_notebook.py` & `nbconvert-7.4.0/docs/api_examples/template_path/quiz_notebook.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/api_examples/template_path/media/image1.png` & `nbconvert-7.4.0/docs/api_examples/template_path/media/image1.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/api_examples/template_path/media/image2.png` & `nbconvert-7.4.0/docs/api_examples/template_path/media/image2.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2` & `nbconvert-7.4.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css` & `nbconvert-7.4.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/architecture.rst` & `nbconvert-7.4.0/docs/source/architecture.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/conf.py` & `nbconvert-7.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/customizing.rst` & `nbconvert-7.4.0/docs/source/customizing.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/dejavu.rst` & `nbconvert-7.4.0/docs/source/dejavu.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/development_release.rst` & `nbconvert-7.4.0/docs/source/development_release.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/execute_api.rst` & `nbconvert-7.4.0/docs/source/execute_api.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/external_exporters.rst` & `nbconvert-7.4.0/docs/source/external_exporters.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/highlighting.rst` & `nbconvert-7.4.0/docs/source/highlighting.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/index.rst` & `nbconvert-7.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/install.rst` & `nbconvert-7.4.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/latex_citations.rst` & `nbconvert-7.4.0/docs/source/latex_citations.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/nbconvert_library.ipynb` & `nbconvert-7.4.0/docs/source/nbconvert_library.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/need_help.rst` & `nbconvert-7.4.0/docs/source/need_help.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/removing_cells.rst` & `nbconvert-7.4.0/docs/source/removing_cells.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/usage.rst` & `nbconvert-7.4.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/_static/exporter_inheritance.png` & `nbconvert-7.4.0/docs/source/_static/exporter_inheritance.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/_static/preprocessor_inheritance.png` & `nbconvert-7.4.0/docs/source/_static/preprocessor_inheritance.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/_static/writer_inheritance.png` & `nbconvert-7.4.0/docs/source/_static/writer_inheritance.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/api/exporters.rst` & `nbconvert-7.4.0/docs/source/api/exporters.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/api/filters.rst` & `nbconvert-7.4.0/docs/source/api/filters.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/docs/source/api/preprocessors.rst` & `nbconvert-7.4.0/docs/source/api/preprocessors.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/nbconvertapp.py` & `nbconvert-7.4.0/nbconvert/nbconvertapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
 
         WARNING: THE COMMANDLINE INTERFACE MAY CHANGE IN FUTURE RELEASES."""
     )
 
     output_base = Unicode(
         "{notebook_name}",
         help="""Overwrite base name use for output files.
-            Supports pattern replacements '{notebook_name}' and '{notebook_filename}'.
+            Supports pattern replacements '{notebook_name}'.
             """,
     ).tag(config=True)
 
     use_output_suffix = Bool(
         True,
         help="""Whether to apply a suffix prior to the extension (only relevant
             when converting to notebook format). The suffix is determined by
@@ -416,17 +416,15 @@
     def _notebook_filename_to_name(self, notebook_filename):
         """
         Returns the notebook name from the notebook filename by
         applying `output_base` pattern and stripping extension
         """
         basename = os.path.basename(notebook_filename)
         notebook_name = basename[: basename.rfind(".")]
-        notebook_name = self.output_base.format(
-            notebook_name=notebook_name, notebook_filename=notebook_filename
-        )
+        notebook_name = self.output_base.format(notebook_name=notebook_name)
 
         return notebook_name
 
     def init_single_notebook_resources(self, notebook_filename):
         """Step 1: Initialize resources
 
         This initializes the resources dictionary for a single notebook.
@@ -509,15 +507,15 @@
         """
 
         if "unique_key" not in resources:
             msg = "unique_key MUST be specified in the resources, but it is not"
             raise KeyError(msg)
 
         notebook_name = resources["unique_key"]
-        if self.use_output_suffix:
+        if self.use_output_suffix and self.output_base == "{notebook_name}":
             notebook_name += resources.get("output_suffix", "")
 
         write_results = self.writer.write(output, resources, notebook_name=notebook_name)
         return write_results
 
     def postprocess_single_notebook(self, write_results):
         """Step 4: Post-process the written file
@@ -581,26 +579,14 @@
 
         # strip duplicate extension from output_base, to avoid Basename.ext.ext
         if getattr(self.exporter, "file_extension", False):
             base, ext = os.path.splitext(self.output_base)
             if ext == self.exporter.file_extension:
                 self.output_base = base
 
-        # Validate that output_base does not cause us to overwrite already generated
-        # files
-        notebook_names = [self._notebook_filename_to_name(fn) for fn in self.notebooks]
-        if len(notebook_names) != len(set(notebook_names)):
-            msg = (
-                "Conversion would override an already generated output. "
-                "This is probably due to --output or output_base configuration "
-                "leading to non-unique output names. "
-                f"Output notebook names were: {notebook_names}"
-            )
-            raise ValueError(msg)
-
         # convert each notebook
         if not self.from_stdin:
             for notebook_filename in self.notebooks:
                 self.convert_single_notebook(notebook_filename)
         else:
             input_buffer = unicode_stdin_stream()
             # default name when conversion from stdin
```

### Comparing `nbconvert-7.3.1/nbconvert/exporters/__init__.py` & `nbconvert-7.4.0/nbconvert/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/asciidoc.py` & `nbconvert-7.4.0/nbconvert/exporters/asciidoc.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,9 +44,12 @@
                         "text/latex",
                     ]
                 },
                 "ExtractOutputPreprocessor": {"enabled": True},
                 "HighlightMagicsPreprocessor": {"enabled": True},
             }
         )
-        c.merge(super().default_config)
+        if super().default_config:
+            c2 = super().default_config.copy()
+            c2.merge(c)
+            c = c2
         return c
```

### Comparing `nbconvert-7.3.1/nbconvert/exporters/base.py` & `nbconvert-7.4.0/nbconvert/exporters/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/exporter.py` & `nbconvert-7.4.0/nbconvert/exporters/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
             "nbconvert.preprocessors.ClearOutputPreprocessor",
             "nbconvert.preprocessors.ExecutePreprocessor",
             "nbconvert.preprocessors.coalesce_streams",
             "nbconvert.preprocessors.SVG2PDFPreprocessor",
             "nbconvert.preprocessors.LatexPreprocessor",
             "nbconvert.preprocessors.HighlightMagicsPreprocessor",
             "nbconvert.preprocessors.ExtractOutputPreprocessor",
+            "nbconvert.preprocessors.ExtractAttachmentsPreprocessor",
             "nbconvert.preprocessors.ClearMetadataPreprocessor",
         ],
         help="""List of preprocessors available by default, by name, namespace,
         instance, or type.""",
     ).tag(config=True)
 
     def __init__(self, config=None, **kw):
```

### Comparing `nbconvert-7.3.1/nbconvert/exporters/html.py` & `nbconvert-7.4.0/nbconvert/exporters/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,18 @@
                         "image/jpeg",
                         "text/plain",
                     ]
                 },
                 "HighlightMagicsPreprocessor": {"enabled": True},
             }
         )
-        c.merge(super().default_config)
+        if super().default_config:
+            c2 = super().default_config.copy()
+            c2.merge(c)
+            c = c2
         return c
 
     @contextfilter
     def markdown2html(self, context, source):
         """Markdown to HTML filter respecting the anchor_link_text setting"""
         cell = context.get("cell", {})
         attachments = cell.get("attachments", {})
```

### Comparing `nbconvert-7.3.1/nbconvert/exporters/latex.py` & `nbconvert-7.4.0/nbconvert/exporters/latex.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,22 +50,26 @@
                         "image/png",
                         "image/jpeg",
                         "image/svg+xml",
                         "text/markdown",
                         "text/plain",
                     ]
                 },
+                "ExtractAttachmentsPreprocessor": {"enabled": True},
                 "ExtractOutputPreprocessor": {"enabled": True},
                 "SVG2PDFPreprocessor": {"enabled": True},
                 "LatexPreprocessor": {"enabled": True},
                 "SphinxPreprocessor": {"enabled": True},
                 "HighlightMagicsPreprocessor": {"enabled": True},
             }
         )
-        c.merge(super().default_config)
+        if super().default_config:
+            c2 = super().default_config.copy()
+            c2.merge(c)
+            c = c2
         return c
 
     def from_notebook_node(self, nb, resources=None, **kw):
         """Convert from notebook node."""
         langinfo = nb.metadata.get("language_info", {})
         lexer = langinfo.get("pygments_lexer", langinfo.get("name", None))
         highlight_code = self.filters.get(
```

### Comparing `nbconvert-7.3.1/nbconvert/exporters/markdown.py` & `nbconvert-7.4.0/nbconvert/exporters/markdown.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     def _raw_mimetypes_default(self):
         return ["text/markdown", "text/html", ""]
 
     @property
     def default_config(self):
         c = Config(
             {
+                "ExtractAttachmentsPreprocessor": {"enabled": True},
                 "ExtractOutputPreprocessor": {"enabled": True},
                 "NbConvertBase": {
                     "display_data_priority": [
                         "text/html",
                         "text/markdown",
                         "image/svg+xml",
                         "text/latex",
@@ -45,9 +46,12 @@
                         "image/jpeg",
                         "text/plain",
                     ]
                 },
                 "HighlightMagicsPreprocessor": {"enabled": True},
             }
         )
-        c.merge(super().default_config)
+        if super().default_config:
+            c2 = super().default_config.copy()
+            c2.merge(c)
+            c = c2
         return c
```

### Comparing `nbconvert-7.3.1/nbconvert/exporters/notebook.py` & `nbconvert-7.4.0/nbconvert/exporters/notebook.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/pdf.py` & `nbconvert-7.4.0/nbconvert/exporters/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             stdout = subprocess.PIPE if not self.verbose else None
             for _ in range(count):
                 p = subprocess.Popen(
                     command,
                     stdout=stdout,
                     stderr=subprocess.STDOUT,
                     stdin=null,
-                    shell=shell,
+                    shell=shell,  # noqa
                     env=env,
                 )
                 out, _ = p.communicate()
                 if p.returncode:
                     if self.verbose:  # noqa
                         # verbose means I didn't capture stdout with PIPE,
                         # so it's already been displayed and `out` is None.
@@ -206,12 +206,13 @@
             self.log.info("PDF successfully created")
             with open(pdf_file, "rb") as f:
                 pdf_data = f.read()
 
         # convert output extension to pdf
         # the writer above required it to be tex
         resources["output_extension"] = ".pdf"
-        # clear figure outputs, extracted by latex export,
+        # clear figure outputs and attachments, extracted by latex export,
         # so we don't claim to be a multi-file export.
         resources.pop("outputs", None)
+        resources.pop("attachments", None)
 
         return pdf_data, resources
```

### Comparing `nbconvert-7.3.1/nbconvert/exporters/python.py` & `nbconvert-7.4.0/nbconvert/exporters/python.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/qt_exporter.py` & `nbconvert-7.4.0/nbconvert/exporters/qt_exporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/qt_screenshot.py` & `nbconvert-7.4.0/nbconvert/exporters/qt_screenshot.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/qtpdf.py` & `nbconvert-7.4.0/nbconvert/exporters/qtpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/rst.py` & `nbconvert-7.4.0/nbconvert/exporters/rst.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,9 +29,12 @@
     def default_config(self):
         c = Config(
             {
                 "ExtractOutputPreprocessor": {"enabled": True},
                 "HighlightMagicsPreprocessor": {"enabled": True},
             }
         )
-        c.merge(super().default_config)
+        if super().default_config:
+            c2 = super().default_config.copy()
+            c2.merge(c)
+            c = c2
         return c
```

### Comparing `nbconvert-7.3.1/nbconvert/exporters/script.py` & `nbconvert-7.4.0/nbconvert/exporters/script.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/slides.py` & `nbconvert-7.4.0/nbconvert/exporters/slides.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/templateexporter.py` & `nbconvert-7.4.0/nbconvert/exporters/templateexporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,18 @@
     def default_config(self):
         c = Config(
             {
                 "RegexRemovePreprocessor": {"enabled": True},
                 "TagRemovePreprocessor": {"enabled": True},
             }
         )
-        c.merge(super().default_config)
+        if super().default_config:
+            c2 = super().default_config.copy()
+            c2.merge(c)
+            c = c2
         return c
 
     template_name = Unicode(help="Name of the template to use").tag(
         config=True, affects_template=True
     )
 
     template_file = Unicode(None, allow_none=True, help="Name of the template file to use").tag(
@@ -641,28 +644,24 @@
                         )
                         self.template_file = compatibility_file
                         conf = self.get_compatibility_base_template_conf(base_template)
                         self.template_name = conf.get("base_template")
                         break
                 if not found_at_least_one:
                     paths = "\n\t".join(root_dirs)
-                    raise ValueError(
-                        "No template sub-directory with name %r found in the following paths:\n\t%s"
-                        % (base_template, paths)
-                    )
+                    msg = f"No template sub-directory with name {base_template!r} found in the following paths:\n\t{paths}"
+                    raise ValueError(msg)
             merged_conf = recursive_update(dict(conf), merged_conf)
             base_template = conf.get("base_template")
         conf = merged_conf
         mimetypes = [mimetype for mimetype, enabled in conf.get("mimetypes", {}).items() if enabled]
         if self.output_mimetype and self.output_mimetype not in mimetypes and mimetypes:
             supported_mimetypes = "\n\t".join(mimetypes)
-            raise ValueError(
-                "Unsupported mimetype %r for template %r, mimetypes supported are: \n\t%s"
-                % (self.output_mimetype, self.template_name, supported_mimetypes)
-            )
+            msg = f"Unsupported mimetype {self.output_mimetype!r} for template {self.template_name!r}, mimetypes supported are: \n\t{supported_mimetypes}"
+            raise ValueError(msg)
         return template_names
 
     def get_prefix_root_dirs(self):
         """Get the prefix root dirs."""
         # We look at the usual jupyter locations, and for development purposes also
         # relative to the package directory (first entry, meaning with highest precedence)
         root_dirs = []
```

### Comparing `nbconvert-7.3.1/nbconvert/exporters/webpdf.py` & `nbconvert-7.4.0/nbconvert/exporters/webpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/base.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/cheese.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/cheese.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/test_asciidoc.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/test_asciidoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/test_export.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/test_exporter.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/test_exporter.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 # -----------------------------------------------------------------------------
 import os
 from unittest.mock import patch
 
 from traitlets.config import Config
 
 from ...preprocessors.base import Preprocessor
+from .. import Exporter, TemplateExporter
 from ..base import get_export_names
-from ..exporter import Exporter
 from .base import ExportersTestsBase
 
 # -----------------------------------------------------------------------------
 # Class
 # -----------------------------------------------------------------------------
 
 
@@ -34,14 +34,29 @@
     """
 
     def preprocess(self, nb, resources):
         nb["metadata"]["pizza"] = "cheese"
         return nb, resources
 
 
+class DummyExporter(TemplateExporter):
+    """
+    Dummy exporter to check that parent default_config gets overwritten properly
+    """
+
+    @property
+    def default_config(self):
+        c = Config({"TagRemovePreprocessor": {"enabled": False}})
+        if super().default_config:
+            c2 = super().default_config.copy()
+            c2.merge(c)
+            c = c2
+        return c
+
+
 class TestExporter(ExportersTestsBase):
     """Contains test functions for exporter.py"""
 
     def test_constructor(self):
         """Can an Exporter be constructed?"""
         Exporter()
 
@@ -83,7 +98,16 @@
             self.assertNotEqual(export_names, ["notebook"])
 
         # In the absence of this variable we should revert to
         # the normal behavior.
         del os.environ["NBCONVERT_DISABLE_CONFIG_EXPORTERS"]
         export_names = get_export_names(config=config)
         self.assertEqual(export_names, ["notebook"])
+
+    def test_default_config_merge(self):
+        """
+        Do default_configs merge properly?
+        Class config should overwrite parent config
+        """
+        e = DummyExporter()
+        self.assertFalse(e.default_config["TagRemovePreprocessor"]["enabled"])
+        self.assertTrue(e.default_config["RegexRemovePreprocessor"]["enabled"])
```

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/test_html.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/test_latex.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/test_markdown.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/test_notebook.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/test_pdf.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/test_python.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/test_qtpdf.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/test_qtpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/test_qtpng.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/test_qtpng.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/test_rst.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/test_rst.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/test_script.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/test_slides.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/test_slides.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/test_templateexporter.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/test_templateexporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/test_webpdf.py` & `nbconvert-7.4.0/nbconvert/exporters/tests/test_webpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/files/attachment.ipynb` & `nbconvert-7.4.0/nbconvert/exporters/tests/files/attachment.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/files/notebook2.ipynb` & `nbconvert-7.4.0/nbconvert/exporters/tests/files/notebook2.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/files/notebook3.ipynb` & `nbconvert-7.4.0/nbconvert/exporters/tests/files/notebook3.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/files/notebook_inject.ipynb` & `nbconvert-7.4.0/nbconvert/exporters/tests/files/notebook_inject.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/files/pngmetadata.ipynb` & `nbconvert-7.4.0/nbconvert/exporters/tests/files/pngmetadata.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/files/prompt_numbers.ipynb` & `nbconvert-7.4.0/nbconvert/exporters/tests/files/prompt_numbers.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/files/rawtest.ipynb` & `nbconvert-7.4.0/nbconvert/exporters/tests/files/rawtest.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/exporters/tests/files/svg.ipynb` & `nbconvert-7.4.0/nbconvert/exporters/tests/files/svg.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/ansi.py` & `nbconvert-7.4.0/nbconvert/filters/ansi.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/citation.py` & `nbconvert-7.4.0/nbconvert/filters/citation.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/datatypefilter.py` & `nbconvert-7.4.0/nbconvert/filters/datatypefilter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/filter_links.py` & `nbconvert-7.4.0/nbconvert/filters/filter_links.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/highlight.py` & `nbconvert-7.4.0/nbconvert/filters/highlight.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/latex.py` & `nbconvert-7.4.0/nbconvert/filters/latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/markdown.py` & `nbconvert-7.4.0/nbconvert/filters/markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/markdown_mistune.py` & `nbconvert-7.4.0/nbconvert/filters/markdown_mistune.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/pandoc.py` & `nbconvert-7.4.0/nbconvert/filters/pandoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/strings.py` & `nbconvert-7.4.0/nbconvert/filters/strings.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/svg_constants.py` & `nbconvert-7.4.0/nbconvert/filters/svg_constants.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/widgetsdatatypefilter.py` & `nbconvert-7.4.0/nbconvert/filters/widgetsdatatypefilter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/tests/test_ansi.py` & `nbconvert-7.4.0/nbconvert/filters/tests/test_ansi.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/tests/test_citation.py` & `nbconvert-7.4.0/nbconvert/filters/tests/test_citation.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/tests/test_datatypefilter.py` & `nbconvert-7.4.0/nbconvert/filters/tests/test_datatypefilter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/tests/test_highlight.py` & `nbconvert-7.4.0/nbconvert/filters/tests/test_highlight.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/tests/test_latex.py` & `nbconvert-7.4.0/nbconvert/filters/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/tests/test_markdown.py` & `nbconvert-7.4.0/nbconvert/filters/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/tests/test_metadata.py` & `nbconvert-7.4.0/nbconvert/filters/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/filters/tests/test_strings.py` & `nbconvert-7.4.0/nbconvert/filters/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/postprocessors/base.py` & `nbconvert-7.4.0/nbconvert/postprocessors/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/postprocessors/serve.py` & `nbconvert-7.4.0/nbconvert/postprocessors/serve.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/postprocessors/tests/test_serve.py` & `nbconvert-7.4.0/nbconvert/postprocessors/tests/test_serve.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/__init__.py` & `nbconvert-7.4.0/nbconvert/preprocessors/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,13 +7,14 @@
 from .clearoutput import ClearOutputPreprocessor
 
 # decorated function Preprocessors
 from .coalescestreams import coalesce_streams
 from .convertfigures import ConvertFiguresPreprocessor
 from .csshtmlheader import CSSHTMLHeaderPreprocessor
 from .execute import ExecutePreprocessor
+from .extractattachments import ExtractAttachmentsPreprocessor
 from .extractoutput import ExtractOutputPreprocessor
 from .highlightmagics import HighlightMagicsPreprocessor
 from .latex import LatexPreprocessor
 from .regexremove import RegexRemovePreprocessor
 from .svg2pdf import SVG2PDFPreprocessor
 from .tagremove import TagRemovePreprocessor
```

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/base.py` & `nbconvert-7.4.0/nbconvert/preprocessors/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/clearmetadata.py` & `nbconvert-7.4.0/nbconvert/preprocessors/clearmetadata.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/clearoutput.py` & `nbconvert-7.4.0/nbconvert/preprocessors/clearoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/coalescestreams.py` & `nbconvert-7.4.0/nbconvert/preprocessors/coalescestreams.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/convertfigures.py` & `nbconvert-7.4.0/nbconvert/preprocessors/convertfigures.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/csshtmlheader.py` & `nbconvert-7.4.0/nbconvert/preprocessors/csshtmlheader.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/execute.py` & `nbconvert-7.4.0/nbconvert/preprocessors/execute.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/extractoutput.py` & `nbconvert-7.4.0/nbconvert/preprocessors/extractoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/highlightmagics.py` & `nbconvert-7.4.0/nbconvert/preprocessors/highlightmagics.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/latex.py` & `nbconvert-7.4.0/nbconvert/preprocessors/latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/regexremove.py` & `nbconvert-7.4.0/nbconvert/preprocessors/regexremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/sanitize.py` & `nbconvert-7.4.0/nbconvert/preprocessors/sanitize.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/svg2pdf.py` & `nbconvert-7.4.0/nbconvert/preprocessors/svg2pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         This affects how the conversion command is run.
         """
     ).tag(config=True)
 
     @default("inkscape_version")
     def _inkscape_version_default(self):
         p = subprocess.Popen(
-            [self.inkscape, "--version"], stdout=subprocess.PIPE, stderr=subprocess.PIPE
+            [self.inkscape, "--version"], stdout=subprocess.PIPE, stderr=subprocess.PIPE  # noqa
         )
         output, _ = p.communicate()
         if p.returncode != 0:
             msg = "Unable to find inkscape executable --version"
             raise RuntimeError(msg)
         return output.decode("utf-8").split(" ")[1]
 
@@ -139,15 +139,15 @@
             template_vars = {"from_filename": input_filename, "to_filename": output_filename}
             if isinstance(self.command, list):
                 full_cmd = [s.format_map(FormatSafeDict(**template_vars)) for s in self.command]
             else:
                 # For backwards compatibility with specifying strings
                 # Okay-ish, since the string is trusted
                 full_cmd = self.command.format(*template_vars)
-            subprocess.call(full_cmd, shell=isinstance(full_cmd, str))
+            subprocess.call(full_cmd, shell=isinstance(full_cmd, str))  # noqa
 
             # Read output from drive
             # return value expects a filename
             if os.path.isfile(output_filename):
                 with open(output_filename, "rb") as f:
                     # PDF is a nb supported binary, data type, so base64 encode.
                     return base64.encodebytes(f.read()).decode("utf-8")
```

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/tagremove.py` & `nbconvert-7.4.0/nbconvert/preprocessors/tagremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/tests/base.py` & `nbconvert-7.4.0/nbconvert/preprocessors/tests/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """utility functions for preprocessor tests"""
 
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 
+from base64 import b64encode
+
 from nbformat import v4 as nbformat
 
 from ...exporters.exporter import ResourcesDict
 from ...tests.base import TestsBase
 
 
 class PreprocessorTestsBase(TestsBase):
     """Contains test functions preprocessor tests"""
 
-    def build_notebook(self, with_json_outputs=False):
+    def build_notebook(self, with_json_outputs=False, with_attachment=False):
         """Build a notebook in memory for use with preprocessor tests"""
 
         outputs = [
             nbformat.new_output("stream", name="stdout", text="a"),
             nbformat.new_output("display_data", data={"text/plain": "b"}),
             nbformat.new_output("stream", name="stdout", text="c"),
             nbformat.new_output("stream", name="stdout", text="d"),
@@ -38,14 +40,27 @@
             )
 
         cells = [
             nbformat.new_code_cell(source="$ e $", execution_count=1, outputs=outputs),
             nbformat.new_markdown_cell(source="$ e $"),
         ]
 
+        if with_attachment:
+            data = b"test"
+            encoded_data = b64encode(data)
+            # this is conversion of bytes to string, not base64 decoding
+            attachments = {"image.png": {"image/png": encoded_data.decode()}}
+            cells.extend(
+                [
+                    nbformat.new_markdown_cell(
+                        source="![image.png](attachment:image.png)", attachments=attachments
+                    )
+                ]
+            )
+
         return nbformat.new_notebook(cells=cells)
 
     def build_resources(self):
         """Build an empty resources dictionary."""
 
         res = ResourcesDict()
         res["metadata"] = ResourcesDict()
```

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/tests/fake_kernelmanager.py` & `nbconvert-7.4.0/nbconvert/preprocessors/tests/fake_kernelmanager.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_clearmetadata.py` & `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_clearmetadata.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_clearoutput.py` & `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_clearoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_coalescestreams.py` & `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_coalescestreams.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_csshtmlheader.py` & `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_csshtmlheader.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_execute.py` & `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_extractoutput.py` & `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_extractoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_highlightmagics.py` & `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_highlightmagics.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_latex.py` & `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_regexremove.py` & `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_regexremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_sanitize.py` & `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_svg2pdf.py` & `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_svg2pdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_tagremove.py` & `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_tagremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb` & `nbconvert-7.4.0/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/templates/skeleton/Makefile` & `nbconvert-7.4.0/nbconvert/templates/skeleton/Makefile`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/tests/base.py` & `nbconvert-7.4.0/nbconvert/tests/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
                 cmd = " ".join(cmd) + " " + parameters
             else:
                 cmd = " ".join(cmd + parameters)
         else:
             if isinstance(parameters, (str,)):
                 parameters = shlex.split(parameters)
             cmd += parameters
-        p = Popen(cmd, stdout=PIPE, stderr=PIPE, stdin=PIPE)
+        p = Popen(cmd, stdout=PIPE, stderr=PIPE, stdin=PIPE)  # noqa
         stdout, stderr = p.communicate(input=stdin)
         if not (p.returncode == 0 or ignore_return_code):
             raise OSError(stderr.decode("utf8", "replace"))
         return stdout.decode("utf8", "replace"), stderr.decode("utf8", "replace")
 
 
 def assert_big_text_equal(a, b, chunk_size=80):
```

### Comparing `nbconvert-7.3.1/nbconvert/tests/fake_exporters.py` & `nbconvert-7.4.0/nbconvert/tests/fake_exporters.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/tests/test_nbconvertapp.py` & `nbconvert-7.4.0/nbconvert/tests/test_nbconvertapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -427,15 +427,16 @@
         with self.create_temp_cwd(["notebook3_with_errors.ipynb"]):
             _, error_output = self.nbconvert(
                 "--execute --to markdown --stdout notebook3_with_errors.ipynb",
                 ignore_return_code=True,
             )
             assert 'print("Some text before the error")' in error_output
             assert 'raise RuntimeError("This is a deliberate exception")' in error_output
-            assert "RuntimeError: This is a deliberate exception" in error_output
+            assert "RuntimeError" in error_output
+            assert "This is a deliberate exception" in error_output
 
     def test_fenced_code_blocks_markdown(self):
         """
         Verify that input cells use fenced code blocks with the language
         name in nb.metadata.kernelspec.language, if that exists
         """
         with self.create_temp_cwd(["notebook1*.ipynb"]):
@@ -649,20 +650,35 @@
 
         with self.create_temp_cwd([x + ".ipynb" for x in notebook_names]):
             self.nbconvert("*.ipynb --to markdown")
 
             for nbn in notebook_names:
                 assert os.path.isfile(f"{nbn}.md")
 
-        with pytest.raises(OSError), self.create_temp_cwd([x + ".ipynb" for x in notebook_names]):
-            self.nbconvert("*.ipynb --output notebook_test_name --to markdown")
-
         # Test single output with static output name
-        with self.create_temp_cwd([notebook_names[0] + ".ipynb"]):
-            self.nbconvert("*.ipynb --output notebook_test_name --to markdown")
+        nbname = notebook_names[0]
+        with self.create_temp_cwd([nbname + ".ipynb"]):
+            self.nbconvert(f"{nbname}.ipynb --output notebook_test_name --to markdown")
             assert os.path.isfile("notebook_test_name.md")
 
+            self.nbconvert(f"{nbname}.ipynb --to notebook")
+            assert os.path.isfile("notebook1.nbconvert.ipynb")
+
+            self.nbconvert(f"{nbname}.ipynb --to notebook --output out.ipynb")
+            assert os.path.isfile("out.ipynb")
+
         # Test double extension fix
         with self.create_temp_cwd([notebook_names[0] + ".ipynb"]):
             self.nbconvert("*.ipynb --output notebook_test_name.md --to markdown")
             assert os.path.isfile("notebook_test_name.md")
             assert not os.path.isfile("notebook_test_name.md.md")
+
+    def test_same_filename_different_dir(self):
+        """
+        Check if files with same name in different directories pose a problem
+        """
+        with self.create_temp_cwd() as temp_wd:
+            self.copy_files_to(["notebook1.ipynb"], temp_wd + "/dir1")
+            self.copy_files_to(["notebook1.ipynb"], temp_wd + "/dir2")
+            self.nbconvert("dir1/notebook1.ipynb dir2/notebook1.ipynb --to markdown")
+            assert os.path.isfile("dir1/notebook1.md")
+            assert os.path.isfile("dir2/notebook1.md")
```

### Comparing `nbconvert-7.3.1/nbconvert/tests/files/Unexecuted_widget.ipynb` & `nbconvert-7.4.0/nbconvert/tests/files/Unexecuted_widget.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/tests/files/Unexecuted_widget_2.ipynb` & `nbconvert-7.4.0/nbconvert/tests/files/Unexecuted_widget_2.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/tests/files/Widget_List.ipynb` & `nbconvert-7.4.0/nbconvert/tests/files/Widget_List.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/tests/files/containerized_deployments.jpeg` & `nbconvert-7.4.0/nbconvert/tests/files/containerized_deployments.jpeg`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/tests/files/issue1849_svg.ipynb` & `nbconvert-7.4.0/nbconvert/tests/files/issue1849_svg.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/tests/files/latex-linked-image.ipynb` & `nbconvert-7.4.0/nbconvert/tests/files/latex-linked-image.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/tests/files/markdown_display_priority.ipynb` & `nbconvert-7.4.0/nbconvert/tests/files/markdown_display_priority.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/tests/files/notebook1.ipynb` & `nbconvert-7.4.0/nbconvert/tests/files/notebook1.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/tests/files/notebook2.ipynb` & `nbconvert-7.4.0/nbconvert/tests/files/notebook2.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/tests/files/notebook3_with_errors.ipynb` & `nbconvert-7.4.0/nbconvert/tests/files/notebook3_with_errors.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/tests/files/notebook4_jpeg.ipynb` & `nbconvert-7.4.0/nbconvert/tests/files/notebook4_jpeg.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/tests/files/notebook5_embed_images.ipynb` & `nbconvert-7.4.0/nbconvert/tests/files/notebook5_embed_images.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/tests/files/notebook_tags.ipynb` & `nbconvert-7.4.0/nbconvert/tests/files/notebook_tags.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/tests/files/testimage.png` & `nbconvert-7.4.0/nbconvert/tests/files/testimage.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/utils/_contextlib_chdir.py` & `nbconvert-7.4.0/nbconvert/utils/_contextlib_chdir.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/utils/base.py` & `nbconvert-7.4.0/nbconvert/utils/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/utils/exceptions.py` & `nbconvert-7.4.0/nbconvert/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/utils/io.py` & `nbconvert-7.4.0/nbconvert/utils/io.py`

 * *Files 14% similar despite different names*

```diff
@@ -113,25 +113,7 @@
                 pass
             raise
         os.rename(new_dst, dst)
     elif link_errno != 0:
         # Either link isn't supported, or the filesystem doesn't support
         # linking, or 'src' and 'dst' are on different filesystems.
         shutil.copy(src, dst)
-
-
-def ensure_dir_exists(path, mode=0o755):
-    """ensure that a directory exists
-
-    If it doesn't exist, try to create it and protect against a race condition
-    if another process is doing the same.
-
-    The default permissions are 755, which differ from os.makedirs default of 777.
-    """
-    if not os.path.exists(path):
-        try:
-            os.makedirs(path, mode=mode)
-        except OSError as e:
-            if e.errno != errno.EEXIST:
-                raise
-    elif not os.path.isdir(path):
-        raise OSError("%r exists but is not a directory" % path)
```

### Comparing `nbconvert-7.3.1/nbconvert/utils/pandoc.py` & `nbconvert-7.4.0/nbconvert/utils/pandoc.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     if extra_args:
         cmd.extend(extra_args)
 
     # this will raise an exception that will pop us out of here
     check_pandoc_version()
 
     # we can safely continue
-    p = subprocess.Popen(cmd, stdin=subprocess.PIPE, stdout=subprocess.PIPE)
+    p = subprocess.Popen(cmd, stdin=subprocess.PIPE, stdout=subprocess.PIPE)  # noqa
     out, _ = p.communicate(source.encode())
     out_str = TextIOWrapper(BytesIO(out), encoding, "replace").read()
     return out_str.rstrip("\n")
 
 
 def get_pandoc_version():
     """Gets the Pandoc version if Pandoc is installed.
@@ -71,15 +71,15 @@
     """
     global __version  # noqa
 
     if __version is None:
         if not shutil.which("pandoc"):
             raise PandocMissing()
 
-        out = subprocess.check_output(["pandoc", "-v"])
+        out = subprocess.check_output(["pandoc", "-v"])  # noqa
         out_lines = out.splitlines()
         version_pattern = re.compile(r"^\d+(\.\d+){1,}$")
         for tok in out_lines[0].decode("ascii", "replace").split():
             if version_pattern.match(tok):
                 __version = tok  # type:ignore
                 break
     return __version
```

### Comparing `nbconvert-7.3.1/nbconvert/utils/text.py` & `nbconvert-7.4.0/nbconvert/utils/text.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/utils/version.py` & `nbconvert-7.4.0/nbconvert/utils/version.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/utils/tests/test_io.py` & `nbconvert-7.4.0/nbconvert/utils/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/utils/tests/test_pandoc.py` & `nbconvert-7.4.0/nbconvert/utils/tests/test_pandoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/writers/base.py` & `nbconvert-7.4.0/nbconvert/writers/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/writers/debug.py` & `nbconvert-7.4.0/nbconvert/writers/debug.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/writers/files.py` & `nbconvert-7.4.0/nbconvert/writers/files.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Contains writer for writing nbconvert output to filesystem."""
 
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 
+import errno
 import glob
 import os
 from pathlib import Path
 
 from traitlets import Unicode, observe
 
-from nbconvert.utils.io import ensure_dir_exists, link_or_copy
+from nbconvert.utils.io import link_or_copy
 
 from .base import WriterBase
 
 
 class FilesWriter(WriterBase):
     """Consumes nbconvert output and produces files."""
 
@@ -34,26 +35,51 @@
     ).tag(config=True)
 
     # Make sure that the output directory exists.
     @observe("build_directory")
     def _build_directory_changed(self, change):
         new = change["new"]
         if new:
-            ensure_dir_exists(new)
+            self._makedir(new)
 
     def __init__(self, **kw):
         """Initialize the writer."""
         super().__init__(**kw)
         self._build_directory_changed({"new": self.build_directory})
 
-    def _makedir(self, path):
-        """Make a directory if it doesn't already exist"""
-        if path:
+    def _makedir(self, path, mode=0o755):
+        """ensure that a directory exists
+
+        If it doesn't exist, try to create it and protect against a race condition
+        if another process is doing the same.
+
+        The default permissions are 755, which differ from os.makedirs default of 777.
+        """
+        if not os.path.exists(path):
             self.log.info("Making directory %s", path)
-            ensure_dir_exists(path)
+            try:
+                os.makedirs(path, mode=mode)
+            except OSError as e:
+                if e.errno != errno.EEXIST:
+                    raise
+        elif not os.path.isdir(path):
+            raise OSError("%r exists but is not a directory" % path)
+
+    def _write_items(self, items, build_dir):
+        """Write a dict containing filename->binary data"""
+        for filename, data in items:
+            # Determine where to write the file to
+            dest = os.path.join(build_dir, filename)
+            path = os.path.dirname(dest)
+            self._makedir(path)
+
+            # Write file
+            self.log.debug("Writing %i bytes to %s", len(data), dest)
+            with open(dest, "wb") as f:
+                f.write(data)
 
     def write(self, output, resources, notebook_name=None, **kw):
         """
         Consume and write Jinja output to the file system.  Output directory
         is set via the 'build_directory' variable of this instance (a
         configurable).
 
@@ -69,34 +95,35 @@
         output_extension = resources.get("output_extension", None)
 
         # Get the relative path for copying files
         resource_path = resources.get("metadata", {}).get("path", "")
         relpath = self.relpath or resource_path
         build_directory = self.build_directory or resource_path
 
-        # Write all of the extracted resources to the destination directory.
+        # Write the extracted outputs to the destination directory.
         # NOTE: WE WRITE EVERYTHING AS-IF IT'S BINARY.  THE EXTRACT FIG
         # PREPROCESSOR SHOULD HANDLE UNIX/WINDOWS LINE ENDINGS...
 
         items = resources.get("outputs", {}).items()
         if items:
             self.log.info(
                 "Support files will be in %s",
                 os.path.join(resources.get("output_files_dir", ""), ""),
             )
-        for filename, data in items:
-            # Determine where to write the file to
-            dest = os.path.join(build_directory, filename)
-            path = os.path.dirname(dest)
-            self._makedir(path)
+            self._write_items(items, build_directory)
 
-            # Write file
-            self.log.debug("Writing %i bytes to support file %s", len(data), dest)
-            with open(dest, "wb") as f:
-                f.write(data)
+        # Write the extracted attachments
+        # if ExtractAttachmentsOutput specified a separate directory
+        attachs = resources.get("attachments", {}).items()
+        if attachs:
+            self.log.info(
+                "Attachments will be in %s",
+                os.path.join(resources.get("attachment_files_dir", ""), ""),
+            )
+            self._write_items(attachs, build_directory)
 
         # Copy referenced files to output directory
         if build_directory:
             for filename in self.files:
                 # Copy files that match search pattern
                 for matching_filename in glob.glob(filename):
                     # compute the relative path for the filename
```

### Comparing `nbconvert-7.3.1/nbconvert/writers/stdout.py` & `nbconvert-7.4.0/nbconvert/writers/stdout.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/writers/tests/test_debug.py` & `nbconvert-7.4.0/nbconvert/writers/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/nbconvert/writers/tests/test_files.py` & `nbconvert-7.4.0/nbconvert/writers/tests/test_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Contains test functions for files.py"""
 
     def test_basic_output(self):
         """Is FilesWriter basic output correct?"""
 
         # Work in a temporary directory.
         with self.create_temp_cwd():
-            # Create the resoruces dictionary
+            # Create the resources dictionary
             res: dict = {}
 
             # Create files writer, test output
             writer = FilesWriter()
             writer.write("y", res, notebook_name="z")
 
             # Check the output of the file
@@ -50,16 +50,19 @@
                 self.assertEqual(output, "y")
 
     def test_extract(self):
         """Can FilesWriter write extracted figures correctly?"""
 
         # Work in a temporary directory.
         with self.create_temp_cwd():
-            # Create the resoruces dictionary
-            res = {"outputs": {os.path.join("z_files", "a"): b"b"}}
+            # Create the resources dictionary
+            res = {
+                "outputs": {os.path.join("z_files", "a"): b"b"},
+                "attachments": {os.path.join("z_attachments", "c"): b"d"},
+            }
 
             # Create files writer, test output
             writer = FilesWriter()
             writer.write("y", res, notebook_name="z")
 
             # Check the output of the file
             with open("z") as f:
@@ -69,20 +72,26 @@
             # Check the output of the extracted file
             extracted_file_dest = os.path.join("z_files", "a")
             assert os.path.isfile(extracted_file_dest)
             with open(extracted_file_dest) as f:
                 output = f.read()
                 self.assertEqual(output, "b")
 
+            attachment_file_dest = os.path.join("z_attachments", "c")
+            assert os.path.isfile(attachment_file_dest)
+            with open(attachment_file_dest) as f:
+                content = f.read()
+                self.assertEqual(content, "d")
+
     def test_build_dir(self):
         """Can FilesWriter write to a build dir correctly?"""
 
         # Work in a temporary directory.
         with self.create_temp_cwd():
-            # Create the resoruces dictionary
+            # Create the resources dictionary
             res = {"outputs": {os.path.join("z_files", "a"): b"b"}}
 
             # Create files writer, test output
             writer = FilesWriter()
             writer.build_directory = "build"
             writer.write("y", res, notebook_name="z")
 
@@ -118,15 +127,15 @@
         # Work in a temporary directory.
         with self.create_temp_cwd():
             # Create test file
             os.mkdir("sub")
             with open(os.path.join("sub", "c"), "w") as f:
                 f.write("d")
 
-            # Create the resoruces dictionary
+            # Create the resources dictionary
             res: dict = {}
 
             # Create files writer, test output
             writer = FilesWriter()
             writer.files = [os.path.join("sub", "c")]
             writer.build_directory = "build"
             writer.write("y", res, notebook_name="z")
@@ -191,15 +200,15 @@
         # Work in a temporary directory.
         with self.create_temp_cwd():
             # Create test file
             os.mkdir("sub")
             with open(os.path.join("sub", "c"), "w") as f:
                 f.write("d")
 
-            # Create the resoruces dictionary
+            # Create the resources dictionary
             res: dict = {}
 
             # Create files writer, test output
             writer = FilesWriter()
             writer.files = [os.path.join("sub", "c")]
             writer.build_directory = "build"
             writer.relpath = "sub"
@@ -225,15 +234,15 @@
         # Work in a temporary directory.
         with self.create_temp_cwd():
             # Create test file
             os.mkdir("sub")
             with open(os.path.join("sub", "c"), "w") as f:
                 f.write("d")
 
-            # Create the resoruces dictionary
+            # Create the resources dictionary
             res = {"metadata": {"path": "sub"}}
 
             # Create files writer, test output
             writer = FilesWriter()
             writer.files = [os.path.join("sub", "c")]
             writer.build_directory = "build"
             writer.write("y", res, notebook_name="z")
@@ -258,15 +267,15 @@
         # Work in a temporary directory.
         with self.create_temp_cwd():
             # Create test file
             os.mkdir("sub")
             with open(os.path.join("sub", "c"), "w") as f:
                 f.write("d")
 
-            # Create the resoruces dictionary
+            # Create the resources dictionary
             res = {"metadata": {"path": "other_sub"}}
 
             # Create files writer, test output
             writer = FilesWriter()
             writer.files = [os.path.join("sub", "c")]
             writer.build_directory = "build"
             writer.relpath = "sub"
```

### Comparing `nbconvert-7.3.1/nbconvert/writers/tests/test_stdout.py` & `nbconvert-7.4.0/nbconvert/writers/tests/test_stdout.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/asciidoc/index.asciidoc.j2` & `nbconvert-7.4.0/share/templates/asciidoc/index.asciidoc.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/base/display_priority.j2` & `nbconvert-7.4.0/share/templates/base/display_priority.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/base/jupyter_widgets.html.j2` & `nbconvert-7.4.0/share/templates/base/jupyter_widgets.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/base/mathjax.html.j2` & `nbconvert-7.4.0/share/templates/base/mathjax.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/base/null.j2` & `nbconvert-7.4.0/share/templates/base/null.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/classic/base.html.j2` & `nbconvert-7.4.0/share/templates/classic/base.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/classic/index.html.j2` & `nbconvert-7.4.0/share/templates/classic/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/classic/static/style.css` & `nbconvert-7.4.0/share/templates/classic/static/style.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/lab/base.html.j2` & `nbconvert-7.4.0/share/templates/lab/base.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/lab/index.html.j2` & `nbconvert-7.4.0/share/templates/lab/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/lab/static/index.css` & `nbconvert-7.4.0/share/templates/lab/static/index.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/lab/static/theme-dark.css` & `nbconvert-7.4.0/share/templates/lab/static/theme-dark.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/lab/static/theme-light.css` & `nbconvert-7.4.0/share/templates/lab/static/theme-light.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/latex/base.tex.j2` & `nbconvert-7.4.0/share/templates/latex/base.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/latex/display_priority.j2` & `nbconvert-7.4.0/share/templates/latex/display_priority.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/latex/document_contents.tex.j2` & `nbconvert-7.4.0/share/templates/latex/document_contents.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/latex/null.j2` & `nbconvert-7.4.0/share/templates/latex/null.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/latex/report.tex.j2` & `nbconvert-7.4.0/share/templates/latex/report.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/latex/style_bw_ipython.tex.j2` & `nbconvert-7.4.0/share/templates/latex/style_bw_ipython.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/latex/style_ipython.tex.j2` & `nbconvert-7.4.0/share/templates/latex/style_ipython.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/latex/style_jupyter.tex.j2` & `nbconvert-7.4.0/share/templates/latex/style_jupyter.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/latex/style_python.tex.j2` & `nbconvert-7.4.0/share/templates/latex/style_python.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/markdown/index.md.j2` & `nbconvert-7.4.0/share/templates/markdown/index.md.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/reveal/base.html.j2` & `nbconvert-7.4.0/share/templates/reveal/base.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/reveal/index.html.j2` & `nbconvert-7.4.0/share/templates/reveal/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/reveal/static/custom_reveal.css` & `nbconvert-7.4.0/share/templates/reveal/static/custom_reveal.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/share/templates/rst/index.rst.j2` & `nbconvert-7.4.0/share/templates/rst/index.rst.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/.gitignore` & `nbconvert-7.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/LICENSE` & `nbconvert-7.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/README.md` & `nbconvert-7.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # nbconvert
 
 ### Jupyter Notebook Conversion
 
 [![Build Status](https://github.com/jupyter/nbconvert/actions/workflows/tests.yml/badge.svg?query=branch%3Amain++)](https://github.com/jupyter/nbconvert/actions/workflows/tests.yml/badge.svg?query=branch%3Amain++)
 [![Documentation Status](https://readthedocs.org/projects/nbconvert/badge/?version=latest)](https://nbconvert.readthedocs.io/en/latest/?badge=latest)
-[![codecov.io](https://codecov.io/gh/jupyter/nbconvert/coverage.svg?branch=main)](https://codecov.io/gh/gh/nbconvert?branch=main)
 
 The **nbconvert** tool, `jupyter nbconvert`, converts notebooks to various other
 formats via [Jinja] templates. The nbconvert tool allows you to convert an
 `.ipynb` notebook file into various static formats including:
 
 - HTML
 - LaTeX
```

### Comparing `nbconvert-7.3.1/hatch_build.py` & `nbconvert-7.4.0/hatch_build.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.1/pyproject.toml` & `nbconvert-7.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 features = ["test"]
 [tool.hatch.envs.test.scripts]
 test = "python -m pytest -vv {args}"
 nowarn = "test -W default {args}"
 
 [tool.hatch.envs.cov]
 features = ["all"]
-dependencies = ["coverage", "pytest-cov"]
+dependencies = ["coverage[toml]", "pytest-cov"]
 [tool.hatch.envs.cov.scripts]
 test = "python -m pytest -vv --cov nbconvert --cov-branch --cov-report term-missing:skip-covered {args}"
 nowarn = "test -W default {args}"
 
 [tool.hatch.envs.typing]
 features = ["test"]
 dependencies = ["mypy>=0.990"]
@@ -125,15 +125,15 @@
 test = "mypy --install-types --non-interactive {args:nbconvert}"
 
 [tool.hatch.envs.lint]
 dependencies = [
   "black[jupyter]==23.3.0",
   "mdformat>0.7",
   "mdformat-gfm>=0.3.5",
-  "ruff==0.0.260"
+  "ruff==0.0.263"
 ]
 detached = true
 [tool.hatch.envs.lint.scripts]
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
   "mdformat --check {args:docs *.md}"
@@ -175,14 +175,18 @@
   "raise NotImplementedError",
   "if 0:",
   "if __name__ == .__main__.:",
   "class .*\bProtocol\\):",
 "@(abc\\.)?abstractmethod",
 ]
 
+[tool.coverage.run]
+relative_files = true
+source = ["nbconvert"]
+
 [tool.mypy]
 check_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_decorators = true
 no_implicit_optional = true
 no_implicit_reexport = false
 pretty = true
```

### Comparing `nbconvert-7.3.1/PKG-INFO` & `nbconvert-7.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbconvert
-Version: 7.3.1
+Version: 7.4.0
 Summary: Converting Jupyter Notebooks
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
         - Copyright (c) 2001-2015, IPython Development Team
         - Copyright (c) 2015-, Jupyter Development Team
@@ -88,15 +88,14 @@
 
 # nbconvert
 
 ### Jupyter Notebook Conversion
 
 [![Build Status](https://github.com/jupyter/nbconvert/actions/workflows/tests.yml/badge.svg?query=branch%3Amain++)](https://github.com/jupyter/nbconvert/actions/workflows/tests.yml/badge.svg?query=branch%3Amain++)
 [![Documentation Status](https://readthedocs.org/projects/nbconvert/badge/?version=latest)](https://nbconvert.readthedocs.io/en/latest/?badge=latest)
-[![codecov.io](https://codecov.io/gh/jupyter/nbconvert/coverage.svg?branch=main)](https://codecov.io/gh/gh/nbconvert?branch=main)
 
 The **nbconvert** tool, `jupyter nbconvert`, converts notebooks to various other
 formats via [Jinja] templates. The nbconvert tool allows you to convert an
 `.ipynb` notebook file into various static formats including:
 
 - HTML
 - LaTeX
```

