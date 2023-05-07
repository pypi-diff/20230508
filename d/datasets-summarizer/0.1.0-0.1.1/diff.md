# Comparing `tmp/datasets-summarizer-0.1.0.tar.gz` & `tmp/datasets-summarizer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datasets-summarizer-0.1.0.tar", last modified: Fri May  5 20:28:31 2023, max compression
+gzip compressed data, was "dist/datasets-summarizer-0.1.1.tar", last modified: Sun May  7 22:57:45 2023, max compression
```

## Comparing `datasets-summarizer-0.1.0.tar` & `datasets-summarizer-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 soniacq    (501) staff       (20)        0 2023-05-05 20:28:31.000000 datasets-summarizer-0.1.0/
-drwxr-xr-x   0 soniacq    (501) staff       (20)        0 2023-05-05 20:28:31.000000 datasets-summarizer-0.1.0/DatasetsSummarizer/
--rw-r--r--   0 soniacq    (501) staff       (20)       93 2023-05-05 19:54:19.000000 datasets-summarizer-0.1.0/DatasetsSummarizer/__init__.py
--rw-r--r--   0 soniacq    (501) staff       (20)     1182 2023-04-12 19:07:04.000000 datasets-summarizer-0.1.0/DatasetsSummarizer/_comm_api.py
--rw-r--r--   0 soniacq    (501) staff       (20)      240 2023-05-05 19:14:12.000000 datasets-summarizer-0.1.0/DatasetsSummarizer/_demodata.py
--rw-r--r--   0 soniacq    (501) staff       (20)     2860 2023-05-05 19:54:00.000000 datasets-summarizer-0.1.0/DatasetsSummarizer/_plot_metadata_table.py
-drwxr-xr-x   0 soniacq    (501) staff       (20)        0 2023-05-05 20:28:31.000000 datasets-summarizer-0.1.0/DatasetsSummarizer/build/
--rw-r--r--   0 soniacq    (501) staff       (20)  7890580 2023-05-05 20:01:27.000000 datasets-summarizer-0.1.0/DatasetsSummarizer/build/datasetsVis.js
-drwxr-xr-x   0 soniacq    (501) staff       (20)        0 2023-05-05 20:28:31.000000 datasets-summarizer-0.1.0/DatasetsSummarizer/data/
--rw-r--r--   0 soniacq    (501) staff       (20)  4604862 2023-05-05 19:11:16.000000 datasets-summarizer-0.1.0/DatasetsSummarizer/data/taxi_metadata_cleaned_cols_only.csv
--rw-r--r--   0 soniacq    (501) staff       (20)      115 2023-05-05 20:12:06.000000 datasets-summarizer-0.1.0/MANIFEST.in
--rw-r--r--   0 soniacq    (501) staff       (20)     1546 2023-05-05 20:28:31.000000 datasets-summarizer-0.1.0/PKG-INFO
--rw-r--r--   0 soniacq    (501) staff       (20)      816 2023-05-05 20:25:50.000000 datasets-summarizer-0.1.0/README.md
-drwxr-xr-x   0 soniacq    (501) staff       (20)        0 2023-05-05 20:28:31.000000 datasets-summarizer-0.1.0/datasets_summarizer.egg-info/
--rw-r--r--   0 soniacq    (501) staff       (20)     1546 2023-05-05 20:28:30.000000 datasets-summarizer-0.1.0/datasets_summarizer.egg-info/PKG-INFO
--rw-r--r--   0 soniacq    (501) staff       (20)      482 2023-05-05 20:28:31.000000 datasets-summarizer-0.1.0/datasets_summarizer.egg-info/SOURCES.txt
--rw-r--r--   0 soniacq    (501) staff       (20)        1 2023-05-05 20:28:30.000000 datasets-summarizer-0.1.0/datasets_summarizer.egg-info/dependency_links.txt
--rw-r--r--   0 soniacq    (501) staff       (20)       89 2023-05-05 20:28:30.000000 datasets-summarizer-0.1.0/datasets_summarizer.egg-info/requires.txt
--rw-r--r--   0 soniacq    (501) staff       (20)       19 2023-05-05 20:28:30.000000 datasets-summarizer-0.1.0/datasets_summarizer.egg-info/top_level.txt
--rw-r--r--   0 soniacq    (501) staff       (20)       38 2023-05-05 20:28:31.000000 datasets-summarizer-0.1.0/setup.cfg
--rw-r--r--   0 soniacq    (501) staff       (20)      990 2023-05-05 20:07:39.000000 datasets-summarizer-0.1.0/setup.py
+drwxr-xr-x   0 soniacq    (501) staff       (20)        0 2023-05-07 22:57:45.000000 datasets-summarizer-0.1.1/
+drwxr-xr-x   0 soniacq    (501) staff       (20)        0 2023-05-07 22:57:45.000000 datasets-summarizer-0.1.1/DatasetsSummarizer/
+-rw-r--r--   0 soniacq    (501) staff       (20)      125 2023-05-07 21:36:59.000000 datasets-summarizer-0.1.1/DatasetsSummarizer/__init__.py
+-rw-r--r--   0 soniacq    (501) staff       (20)     1182 2023-04-12 19:07:04.000000 datasets-summarizer-0.1.1/DatasetsSummarizer/_comm_api.py
+-rw-r--r--   0 soniacq    (501) staff       (20)      255 2023-05-07 22:49:01.000000 datasets-summarizer-0.1.1/DatasetsSummarizer/_demodata.py
+-rw-r--r--   0 soniacq    (501) staff       (20)     3455 2023-05-07 22:53:49.000000 datasets-summarizer-0.1.1/DatasetsSummarizer/_plot_metadata_table.py
+drwxr-xr-x   0 soniacq    (501) staff       (20)        0 2023-05-07 22:57:45.000000 datasets-summarizer-0.1.1/DatasetsSummarizer/build/
+-rw-r--r--   0 soniacq    (501) staff       (20)  7890307 2023-05-07 22:53:57.000000 datasets-summarizer-0.1.1/DatasetsSummarizer/build/datasetsVis.js
+drwxr-xr-x   0 soniacq    (501) staff       (20)        0 2023-05-07 22:57:45.000000 datasets-summarizer-0.1.1/DatasetsSummarizer/data/
+-rw-r--r--   0 soniacq    (501) staff       (20)  4604862 2023-05-05 19:11:16.000000 datasets-summarizer-0.1.1/DatasetsSummarizer/data/taxi_metadata_cleaned_cols_only.csv
+-rw-r--r--   0 soniacq    (501) staff       (20)      115 2023-05-05 20:12:06.000000 datasets-summarizer-0.1.1/MANIFEST.in
+-rw-r--r--   0 soniacq    (501) staff       (20)     2537 2023-05-07 22:57:45.000000 datasets-summarizer-0.1.1/PKG-INFO
+-rw-r--r--   0 soniacq    (501) staff       (20)     1671 2023-05-07 22:43:14.000000 datasets-summarizer-0.1.1/README.md
+drwxr-xr-x   0 soniacq    (501) staff       (20)        0 2023-05-07 22:57:45.000000 datasets-summarizer-0.1.1/datasets_summarizer.egg-info/
+-rw-r--r--   0 soniacq    (501) staff       (20)     2537 2023-05-07 22:57:45.000000 datasets-summarizer-0.1.1/datasets_summarizer.egg-info/PKG-INFO
+-rw-r--r--   0 soniacq    (501) staff       (20)      482 2023-05-07 22:57:45.000000 datasets-summarizer-0.1.1/datasets_summarizer.egg-info/SOURCES.txt
+-rw-r--r--   0 soniacq    (501) staff       (20)        1 2023-05-07 22:57:45.000000 datasets-summarizer-0.1.1/datasets_summarizer.egg-info/dependency_links.txt
+-rw-r--r--   0 soniacq    (501) staff       (20)       89 2023-05-07 22:57:45.000000 datasets-summarizer-0.1.1/datasets_summarizer.egg-info/requires.txt
+-rw-r--r--   0 soniacq    (501) staff       (20)       19 2023-05-07 22:57:45.000000 datasets-summarizer-0.1.1/datasets_summarizer.egg-info/top_level.txt
+-rw-r--r--   0 soniacq    (501) staff       (20)       38 2023-05-07 22:57:45.000000 datasets-summarizer-0.1.1/setup.cfg
+-rw-r--r--   0 soniacq    (501) staff       (20)      990 2023-05-07 21:37:19.000000 datasets-summarizer-0.1.1/setup.py
```

### Comparing `datasets-summarizer-0.1.0/DatasetsSummarizer/_comm_api.py` & `datasets-summarizer-0.1.1/DatasetsSummarizer/_comm_api.py`

 * *Files identical despite different names*

### Comparing `datasets-summarizer-0.1.0/DatasetsSummarizer/_plot_metadata_table.py` & `datasets-summarizer-0.1.1/DatasetsSummarizer/_plot_metadata_table.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,47 +9,58 @@
 from collections import defaultdict
 import copy
 import random
 import datamart_profiler
 import pandas
 from io import StringIO
 
+
+defaultSimilarityMetrics = [
+    {"name": "Title and Description", "x": "title_and_description_x", "y": "title_and_description_y"},
+    {"name": "Title", "x": "title_x", "y": "title_y"},
+    {"name": "Description", "x": "description_x", "y": "description_y"},
+    {"name": "Column Name", "x": "column_name_x", "y": "column_name_y"}
+]
+
+def get_default_similarity_metrics():
+    return defaultSimilarityMetrics
+
 def formatMetadata(msg):
     json_data = ast.literal_eval(msg['dataneedformat'])
     data_dict = prepare_data_profiler( json_data)
     return {"newformatmetadata": data_dict}
 
 setup_comm_api('format_metadata_comm_api', formatMetadata)
 
 def id_generator(size=15):
     """Helper function to generate random div ids. This is useful for embedding
     HTML into ipython notebooks."""
     chars = list(string.ascii_uppercase)
     return ''.join(np.random.choice(chars, size, replace=True))
 
 
-def make_html(dataset_results, id):
+def make_html(dataset_results, id, similarity_metrics):
 	lib_path = pkg_resources.resource_filename(__name__, "build/datasetsVis.js")
 	bundle = open(lib_path, "r", encoding="utf8").read()
 	html_all = """
 	<html>
 	<head>
 	</head>
 	<body>
 	    <script>
 	    {bundle}
 	    </script>
 	    <div id="{id}">
 	    </div>
 	    <script>
-	        datasetsVis.renderDatasetsSummarizerBundle("#{id}", {dataset_results});
+	        datasetsVis.renderDatasetsSummarizerBundle("#{id}", {dataset_results}, {similarity_metrics});
 	    </script>
 	</body>
 	</html>
-	""".format(bundle=bundle, id=id, dataset_results=json.dumps(dataset_results))
+	""".format(bundle=bundle, id=id, dataset_results=json.dumps(dataset_results), similarity_metrics=json.dumps(similarity_metrics))
 	return html_all
 
 def getSample(text):
     df = pandas.read_csv(StringIO(text))
     result = [df.columns.values.tolist()] + df.values.tolist()
     return result
   
@@ -86,13 +97,13 @@
             item[dataframe.columns[i]] = row[i];
         items.append(item)
     all_results = {
         "datasets": items
     }
     return all_results
 
-def plot_datasets_summary(dataset_results):
+def plot_datasets_summary(dataset_results, similarity_metrics = defaultSimilarityMetrics):
     from IPython.core.display import display, HTML
     id = id_generator()
     dataset_results_dic = prepare_dataset_results(dataset_results)
-    html_all = make_html(dataset_results_dic, id)
+    html_all = make_html(dataset_results_dic, id, {"similarity_metrics": similarity_metrics})
     display(HTML(html_all))
```

### Comparing `datasets-summarizer-0.1.0/DatasetsSummarizer/build/datasetsVis.js` & `datasets-summarizer-0.1.1/DatasetsSummarizer/build/datasetsVis.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -206,15 +206,15 @@
           !*** ./js/MainView.js ***!
           \************************/
         /*! exports provided: MainView */
         /***/
         (function(module, __webpack_exports__, __webpack_require__) {
 
             "use strict";
-            eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"MainView\", function() { return MainView; });\n/* harmony import */ var react__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! react */ \"./node_modules/react/index.js\");\n/* harmony import */ var react__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(react__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var prop_types__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! prop-types */ \"./node_modules/prop-types/index.js\");\n/* harmony import */ var prop_types__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/__webpack_require__.n(prop_types__WEBPACK_IMPORTED_MODULE_1__);\n/* harmony import */ var _DatasetSample__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! ./DatasetSample */ \"./js/DatasetSample.tsx\");\n/* harmony import */ var _SummaryView__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! ./SummaryView */ \"./js/SummaryView.js\");\n/* harmony import */ var _CommAPI__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! ./CommAPI */ \"./js/CommAPI.js\");\nfunction _typeof(obj) { \"@babel/helpers - typeof\"; if (typeof Symbol === \"function\" && typeof Symbol.iterator === \"symbol\") { _typeof = function _typeof(obj) { return typeof obj; }; } else { _typeof = function _typeof(obj) { return obj && typeof Symbol === \"function\" && obj.constructor === Symbol && obj !== Symbol.prototype ? \"symbol\" : typeof obj; }; } return _typeof(obj); }\n\nfunction _classCallCheck(instance, Constructor) { if (!(instance instanceof Constructor)) { throw new TypeError(\"Cannot call a class as a function\"); } }\n\nfunction _defineProperties(target, props) { for (var i = 0; i < props.length; i++) { var descriptor = props[i]; descriptor.enumerable = descriptor.enumerable || false; descriptor.configurable = true; if (\"value\" in descriptor) descriptor.writable = true; Object.defineProperty(target, descriptor.key, descriptor); } }\n\nfunction _createClass(Constructor, protoProps, staticProps) { if (protoProps) _defineProperties(Constructor.prototype, protoProps); if (staticProps) _defineProperties(Constructor, staticProps); return Constructor; }\n\nfunction _inherits(subClass, superClass) { if (typeof superClass !== \"function\" && superClass !== null) { throw new TypeError(\"Super expression must either be null or a function\"); } subClass.prototype = Object.create(superClass && superClass.prototype, { constructor: { value: subClass, writable: true, configurable: true } }); if (superClass) _setPrototypeOf(subClass, superClass); }\n\nfunction _setPrototypeOf(o, p) { _setPrototypeOf = Object.setPrototypeOf || function _setPrototypeOf(o, p) { o.__proto__ = p; return o; }; return _setPrototypeOf(o, p); }\n\nfunction _createSuper(Derived) { var hasNativeReflectConstruct = _isNativeReflectConstruct(); return function _createSuperInternal() { var Super = _getPrototypeOf(Derived), result; if (hasNativeReflectConstruct) { var NewTarget = _getPrototypeOf(this).constructor; result = Reflect.construct(Super, arguments, NewTarget); } else { result = Super.apply(this, arguments); } return _possibleConstructorReturn(this, result); }; }\n\nfunction _possibleConstructorReturn(self, call) { if (call && (_typeof(call) === \"object\" || typeof call === \"function\")) { return call; } return _assertThisInitialized(self); }\n\nfunction _assertThisInitialized(self) { if (self === void 0) { throw new ReferenceError(\"this hasn't been initialised - super() hasn't been called\"); } return self; }\n\nfunction _isNativeReflectConstruct() { if (typeof Reflect === \"undefined\" || !Reflect.construct) return false; if (Reflect.construct.sham) return false; if (typeof Proxy === \"function\") return true; try { Date.prototype.toString.call(Reflect.construct(Date, [], function () {})); return true; } catch (e) { return false; } }\n\nfunction _getPrototypeOf(o) { _getPrototypeOf = Object.setPrototypeOf ? Object.getPrototypeOf : function _getPrototypeOf(o) { return o.__proto__ || Object.getPrototypeOf(o); }; return _getPrototypeOf(o); }\n\n\n\n\n\n\nvar MainView = /*#__PURE__*/function (_Component) {\n  _inherits(MainView, _Component);\n\n  var _super = _createSuper(MainView);\n\n  function MainView(props) {\n    var _this;\n\n    _classCallCheck(this, MainView);\n\n    _this = _super.call(this, props);\n    _this.commFormatMetadata = new _CommAPI__WEBPACK_IMPORTED_MODULE_4__[\"default\"]('format_metadata_comm_api', function (msg) {\n      _this.setState({\n        fullMetadata: msg.newformatmetadata\n      });\n    });\n    _this.state = {\n      fullMetadata: \"\"\n    };\n    _this.handleChangeDataset = _this.handleChangeDataset.bind(_assertThisInitialized(_this));\n    return _this;\n  }\n\n  _createClass(MainView, [{\n    key: \"componentDidCatch\",\n    value: function componentDidCatch(error, info) {\n      console.log(error);\n    }\n  }, {\n    key: \"componentDidUpdate\",\n    value: function componentDidUpdate(prevProps, prevState) {}\n  }, {\n    key: \"handleChangeDataset\",\n    value: function handleChangeDataset(value) {\n      this.commFormatMetadata.call({\n        dataneedformat: value\n      });\n    }\n  }, {\n    key: \"render\",\n    value: function render() {\n      var _this2 = this;\n\n      var dataset_results = this.props.dataset_results;\n      var similarityMetrics = [{\n        name: \"Title\",\n        x: \"title_x\",\n        y: \"title_y\"\n      }, {\n        name: \"Description\",\n        x: \"description_x\",\n        y: \"description_y\"\n      }, {\n        name: \"Title and Description\",\n        x: \"title_and_description_x\",\n        y: \"title_and_description_y\"\n      }, {\n        name: \"Column Name\",\n        x: \"column_name_x\",\n        y: \"column_name_y\"\n      }];\n      return /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(\"div\", {\n        ref: function ref(_ref) {\n          _this2.ref = _ref;\n        }\n      }, /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(\"div\", {\n        className: \"d-flex flex-row\"\n      }, /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(_SummaryView__WEBPACK_IMPORTED_MODULE_3__[\"SummaryView\"], {\n        hit: dataset_results,\n        similarityMetrics: similarityMetrics,\n        onClick: function onClick(selectedDataset) {\n          _this2.handleChangeDataset(selectedDataset);\n        }\n      }), /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(\"div\", {\n        className: \"row\"\n      }, /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(\"div\", {\n        className: \"column-left\"\n      }, /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(\"div\", {\n        className: \"selected-container\"\n      }, /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(\"div\", {\n        className: \"selected-header\"\n      }, \"Selected Datasets:\"), /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(\"div\", {\n        className: \"selected-body\"\n      }))), /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(\"div\", {\n        className: \"column-right\"\n      }, this.state.fullMetadata !== \"\" && /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(_DatasetSample__WEBPACK_IMPORTED_MODULE_2__[\"DatasetSample\"], {\n        hit: this.state.fullMetadata\n      })))));\n    }\n  }]);\n\n  return MainView;\n}(react__WEBPACK_IMPORTED_MODULE_0__[\"Component\"]);\nMainView.propTypes = {\n  data: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.object.isRequired\n};\n\n//# sourceURL=webpack://datasetsVis/./js/MainView.js?");
+            eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"MainView\", function() { return MainView; });\n/* harmony import */ var react__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! react */ \"./node_modules/react/index.js\");\n/* harmony import */ var react__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(react__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var prop_types__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! prop-types */ \"./node_modules/prop-types/index.js\");\n/* harmony import */ var prop_types__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/__webpack_require__.n(prop_types__WEBPACK_IMPORTED_MODULE_1__);\n/* harmony import */ var _DatasetSample__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! ./DatasetSample */ \"./js/DatasetSample.tsx\");\n/* harmony import */ var _SummaryView__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! ./SummaryView */ \"./js/SummaryView.js\");\n/* harmony import */ var _CommAPI__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! ./CommAPI */ \"./js/CommAPI.js\");\nfunction _typeof(obj) { \"@babel/helpers - typeof\"; if (typeof Symbol === \"function\" && typeof Symbol.iterator === \"symbol\") { _typeof = function _typeof(obj) { return typeof obj; }; } else { _typeof = function _typeof(obj) { return obj && typeof Symbol === \"function\" && obj.constructor === Symbol && obj !== Symbol.prototype ? \"symbol\" : typeof obj; }; } return _typeof(obj); }\n\nfunction _classCallCheck(instance, Constructor) { if (!(instance instanceof Constructor)) { throw new TypeError(\"Cannot call a class as a function\"); } }\n\nfunction _defineProperties(target, props) { for (var i = 0; i < props.length; i++) { var descriptor = props[i]; descriptor.enumerable = descriptor.enumerable || false; descriptor.configurable = true; if (\"value\" in descriptor) descriptor.writable = true; Object.defineProperty(target, descriptor.key, descriptor); } }\n\nfunction _createClass(Constructor, protoProps, staticProps) { if (protoProps) _defineProperties(Constructor.prototype, protoProps); if (staticProps) _defineProperties(Constructor, staticProps); return Constructor; }\n\nfunction _inherits(subClass, superClass) { if (typeof superClass !== \"function\" && superClass !== null) { throw new TypeError(\"Super expression must either be null or a function\"); } subClass.prototype = Object.create(superClass && superClass.prototype, { constructor: { value: subClass, writable: true, configurable: true } }); if (superClass) _setPrototypeOf(subClass, superClass); }\n\nfunction _setPrototypeOf(o, p) { _setPrototypeOf = Object.setPrototypeOf || function _setPrototypeOf(o, p) { o.__proto__ = p; return o; }; return _setPrototypeOf(o, p); }\n\nfunction _createSuper(Derived) { var hasNativeReflectConstruct = _isNativeReflectConstruct(); return function _createSuperInternal() { var Super = _getPrototypeOf(Derived), result; if (hasNativeReflectConstruct) { var NewTarget = _getPrototypeOf(this).constructor; result = Reflect.construct(Super, arguments, NewTarget); } else { result = Super.apply(this, arguments); } return _possibleConstructorReturn(this, result); }; }\n\nfunction _possibleConstructorReturn(self, call) { if (call && (_typeof(call) === \"object\" || typeof call === \"function\")) { return call; } return _assertThisInitialized(self); }\n\nfunction _assertThisInitialized(self) { if (self === void 0) { throw new ReferenceError(\"this hasn't been initialised - super() hasn't been called\"); } return self; }\n\nfunction _isNativeReflectConstruct() { if (typeof Reflect === \"undefined\" || !Reflect.construct) return false; if (Reflect.construct.sham) return false; if (typeof Proxy === \"function\") return true; try { Date.prototype.toString.call(Reflect.construct(Date, [], function () {})); return true; } catch (e) { return false; } }\n\nfunction _getPrototypeOf(o) { _getPrototypeOf = Object.setPrototypeOf ? Object.getPrototypeOf : function _getPrototypeOf(o) { return o.__proto__ || Object.getPrototypeOf(o); }; return _getPrototypeOf(o); }\n\n\n\n\n\n\nvar MainView = /*#__PURE__*/function (_Component) {\n  _inherits(MainView, _Component);\n\n  var _super = _createSuper(MainView);\n\n  function MainView(props) {\n    var _this;\n\n    _classCallCheck(this, MainView);\n\n    _this = _super.call(this, props);\n    _this.commFormatMetadata = new _CommAPI__WEBPACK_IMPORTED_MODULE_4__[\"default\"]('format_metadata_comm_api', function (msg) {\n      _this.setState({\n        fullMetadata: msg.newformatmetadata\n      });\n    });\n    _this.state = {\n      fullMetadata: \"\"\n    };\n    _this.handleChangeDataset = _this.handleChangeDataset.bind(_assertThisInitialized(_this));\n    return _this;\n  }\n\n  _createClass(MainView, [{\n    key: \"componentDidCatch\",\n    value: function componentDidCatch(error, info) {\n      console.log(error);\n    }\n  }, {\n    key: \"componentDidUpdate\",\n    value: function componentDidUpdate(prevProps, prevState) {}\n  }, {\n    key: \"handleChangeDataset\",\n    value: function handleChangeDataset(value) {\n      this.commFormatMetadata.call({\n        dataneedformat: value\n      });\n    }\n  }, {\n    key: \"render\",\n    value: function render() {\n      var _this2 = this;\n\n      var _this$props = this.props,\n          dataset_results = _this$props.dataset_results,\n          similarity_metrics = _this$props.similarity_metrics;\n      return /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(\"div\", {\n        ref: function ref(_ref) {\n          _this2.ref = _ref;\n        }\n      }, /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(\"div\", {\n        className: \"d-flex flex-row\"\n      }, /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(_SummaryView__WEBPACK_IMPORTED_MODULE_3__[\"SummaryView\"], {\n        hit: dataset_results,\n        similarityMetrics: similarity_metrics[\"similarity_metrics\"],\n        onClick: function onClick(selectedDataset) {\n          _this2.handleChangeDataset(selectedDataset);\n        }\n      }), /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(\"div\", {\n        className: \"row\"\n      }, /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(\"div\", {\n        className: \"column-left\"\n      }, /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(\"div\", {\n        className: \"selected-container\"\n      }, /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(\"div\", {\n        className: \"selected-header\"\n      }, \"Selected Datasets:\"), /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(\"div\", {\n        className: \"selected-body\"\n      }))), /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(\"div\", {\n        className: \"column-right\"\n      }, this.state.fullMetadata !== \"\" && /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(_DatasetSample__WEBPACK_IMPORTED_MODULE_2__[\"DatasetSample\"], {\n        hit: this.state.fullMetadata\n      })))));\n    }\n  }]);\n\n  return MainView;\n}(react__WEBPACK_IMPORTED_MODULE_0__[\"Component\"]);\nMainView.propTypes = {\n  data: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.object.isRequired\n};\n\n//# sourceURL=webpack://datasetsVis/./js/MainView.js?");
 
             /***/
         }),
 
     /***/
     "./js/SummaryPlots.css":
         /*!*****************************!*\
@@ -265,15 +265,15 @@
           !*** ./js/index.tsx ***!
           \**********************/
         /*! exports provided: renderDatasetsSummarizerBundle */
         /***/
         (function(module, __webpack_exports__, __webpack_require__) {
 
             "use strict";
-            eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"renderDatasetsSummarizerBundle\", function() { return renderDatasetsSummarizerBundle; });\n/* harmony import */ var react__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! react */ \"./node_modules/react/index.js\");\n/* harmony import */ var react__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(react__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var react_dom__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! react-dom */ \"./node_modules/react-dom/index.js\");\n/* harmony import */ var react_dom__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/__webpack_require__.n(react_dom__WEBPACK_IMPORTED_MODULE_1__);\n/* harmony import */ var d3_selection__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! d3-selection */ \"./node_modules/d3-selection/src/index.js\");\n/* harmony import */ var _MainView__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! ./MainView */ \"./js/MainView.js\");\n/* harmony import */ var regenerator_runtime_runtime__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! regenerator-runtime/runtime */ \"./node_modules/regenerator-runtime/runtime.js\");\n/* harmony import */ var regenerator_runtime_runtime__WEBPACK_IMPORTED_MODULE_4___default = /*#__PURE__*/__webpack_require__.n(regenerator_runtime_runtime__WEBPACK_IMPORTED_MODULE_4__);\n\n\n\n\n\nfunction renderDatasetsSummarizerBundle(divName, dataset_results) {\n  react_dom__WEBPACK_IMPORTED_MODULE_1___default.a.render( /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(_MainView__WEBPACK_IMPORTED_MODULE_3__[\"MainView\"], {\n    dataset_results: dataset_results\n  }), Object(d3_selection__WEBPACK_IMPORTED_MODULE_2__[\"select\"])(divName).node());\n}\n\n//# sourceURL=webpack://datasetsVis/./js/index.tsx?");
+            eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export (binding) */ __webpack_require__.d(__webpack_exports__, \"renderDatasetsSummarizerBundle\", function() { return renderDatasetsSummarizerBundle; });\n/* harmony import */ var react__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! react */ \"./node_modules/react/index.js\");\n/* harmony import */ var react__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(react__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var react_dom__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! react-dom */ \"./node_modules/react-dom/index.js\");\n/* harmony import */ var react_dom__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/__webpack_require__.n(react_dom__WEBPACK_IMPORTED_MODULE_1__);\n/* harmony import */ var d3_selection__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! d3-selection */ \"./node_modules/d3-selection/src/index.js\");\n/* harmony import */ var _MainView__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! ./MainView */ \"./js/MainView.js\");\n/* harmony import */ var regenerator_runtime_runtime__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! regenerator-runtime/runtime */ \"./node_modules/regenerator-runtime/runtime.js\");\n/* harmony import */ var regenerator_runtime_runtime__WEBPACK_IMPORTED_MODULE_4___default = /*#__PURE__*/__webpack_require__.n(regenerator_runtime_runtime__WEBPACK_IMPORTED_MODULE_4__);\n\n\n\n\n\nfunction renderDatasetsSummarizerBundle(divName, dataset_results, similarity_metrics) {\n  react_dom__WEBPACK_IMPORTED_MODULE_1___default.a.render( /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(_MainView__WEBPACK_IMPORTED_MODULE_3__[\"MainView\"], {\n    dataset_results: dataset_results,\n    similarity_metrics: similarity_metrics\n  }), Object(d3_selection__WEBPACK_IMPORTED_MODULE_2__[\"select\"])(divName).node());\n}\n\n//# sourceURL=webpack://datasetsVis/./js/index.tsx?");
 
             /***/
         }),
 
     /***/
     "./node_modules/array-flat-polyfill/index.mjs":
         /*!****************************************************!*\
```

### Comparing `datasets-summarizer-0.1.0/DatasetsSummarizer/data/taxi_metadata_cleaned_cols_only.csv` & `datasets-summarizer-0.1.1/DatasetsSummarizer/data/taxi_metadata_cleaned_cols_only.csv`

 * *Files identical despite different names*

### Comparing `datasets-summarizer-0.1.0/setup.py` & `datasets-summarizer-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="datasets-summarizer",
-    version="0.1.0",
+    version="0.1.1",
     author="Sonia Castelo",
     author_email="s.castelo@nyu.edu",
     description="Datasets Summary Viewer. Enables the exploration of dataset search results in Jupyter Notebooks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/soniacq/DatasetsVis",
     packages=find_packages(exclude=['js', 'node_modules']),
```

