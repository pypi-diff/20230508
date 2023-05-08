# Comparing `tmp/gemd-1.8.1.tar.gz` & `tmp/gemd-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gemd-1.8.1.tar", last modified: Fri Jan  7 20:24:45 2022, max compression
+gzip compressed data, was "gemd-1.9.0.tar", last modified: Tue May 24 00:48:42 2022, max compression
```

## Comparing `gemd-1.8.1.tar` & `gemd-1.9.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2022-01-07 20:23:32.000000 gemd-1.8.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      578 2022-01-07 20:24:45.000000 gemd-1.8.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      656 2022-01-07 20:23:32.000000 gemd-1.8.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1517 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd/builders/
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/builders/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12370 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/builders/impl.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd/demo/
--rw-rw-r--   0 travis    (2000) travis    (2000)       50 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/demo/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38646 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/demo/cake.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4688 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/demo/material_run_example.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2407 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/demo/measurement_example.py
--rw-rw-r--   0 travis    (2000) travis    (2000)  1541363 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/demo/strehlow_and_cook.pif
--rw-rw-r--   0 travis    (2000) travis    (2000)    19852 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/demo/strehlow_and_cook.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   235566 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/demo/strehlow_and_cook_small.pif
--rw-rw-r--   0 travis    (2000) travis    (2000)      996 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/demo/table_example.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26784 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/demo/toothpick.jpg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd/entity/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1591 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd/entity/attribute/
--rw-rw-r--   0 travis    (2000) travis    (2000)      271 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/attribute/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4617 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/attribute/base_attribute.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1396 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/attribute/condition.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1497 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/attribute/parameter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1417 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/attribute/property.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2533 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/attribute/property_and_conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8561 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/base_entity.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd/entity/bounds/
--rw-rw-r--   0 travis    (2000) travis    (2000)      407 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/bounds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1135 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/bounds/base_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2430 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/bounds/categorical_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2457 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/bounds/composition_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1956 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/bounds/integer_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1471 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/bounds/molecular_structure_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3734 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/bounds/real_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1175 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/bounds_validation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6291 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/case_insensitive_dict.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5600 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/dict_serializable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      762 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/file_link.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      370 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/has_dependencies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3119 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/link_by_uid.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd/entity/object/
--rw-rw-r--   0 travis    (2000) travis    (2000)      525 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2493 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/base_object.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1514 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/has_conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      838 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/has_material.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1515 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/has_parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      833 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/has_process.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1500 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/has_properties.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4427 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/has_quantities.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      956 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/has_source.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1877 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/has_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1661 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/has_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4255 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/has_template_check_generator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7338 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/ingredient_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6096 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/ingredient_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4694 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/material_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5492 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/material_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4982 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/measurement_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3071 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/measurement_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4717 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/process_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4847 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/object/process_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1359 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/setters.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd/entity/source/
--rw-rw-r--   0 travis    (2000) travis    (2000)       92 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/source/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1443 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/source/performed_source.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd/entity/template/
--rw-rw-r--   0 travis    (2000) travis    (2000)      495 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/template/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2018 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/template/attribute_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3295 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/template/base_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/template/condition_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3614 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/template/has_condition_templates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3614 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/template/has_parameter_templates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3657 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/template/has_property_templates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1996 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/template/material_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3512 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/template/measurement_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1007 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/template/parameter_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3990 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/template/process_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      998 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/template/property_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3751 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5478 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/valid_list.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd/entity/value/
--rw-rw-r--   0 travis    (2000) travis    (2000)      759 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      841 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/base_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      713 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/categorical_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      600 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/composition_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1545 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/continuous_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2057 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/discrete_categorical.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2693 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/empirical_formula.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1331 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/inchi_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      622 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/integer_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      654 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/molecular_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1261 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/nominal_categorical.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/nominal_composition.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1469 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/nominal_integer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1293 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/nominal_real.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1265 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/normal_real.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1365 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/smiles_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2891 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/uniform_integer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1699 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/entity/value/uniform_real.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd/enumeration/
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/enumeration/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1716 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/enumeration/base_enumeration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      368 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/enumeration/origin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      327 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/enumeration/sample_type.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd/json/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2892 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/json/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      526 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/json/gemd_encoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11303 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/json/gemd_json.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd/units/
--rw-rw-r--   0 travis    (2000) travis    (2000)      255 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/units/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33977 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/units/citrine_en.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     6638 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/units/constants_en.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2204 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/units/impl.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd/units/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       40 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/units/tests/test_units.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      335 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18030 2022-01-07 20:23:32.000000 gemd-1.8.1/gemd/util/impl.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      578 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3616 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2022-01-07 20:24:45.000000 gemd-1.8.1/gemd.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-01-07 20:24:45.000000 gemd-1.8.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1162 2022-01-07 20:23:32.000000 gemd-1.8.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.360957 gemd-1.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2022-05-24 00:47:21.000000 gemd-1.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      606 2022-05-24 00:48:42.360957 gemd-1.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      656 2022-05-24 00:47:21.000000 gemd-1.9.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.340956 gemd-1.9.0/gemd/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1517 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.340956 gemd-1.9.0/gemd/builders/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/builders/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12368 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/builders/impl.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.344956 gemd-1.9.0/gemd/demo/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       50 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/demo/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38705 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/demo/cake.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4689 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/demo/material_run_example.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2407 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/demo/measurement_example.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1541363 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/demo/strehlow_and_cook.pif
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19851 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/demo/strehlow_and_cook.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   235566 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/demo/strehlow_and_cook_small.pif
+-rw-rw-r--   0 travis    (2000) travis    (2000)      996 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/demo/table_example.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26784 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/demo/toothpick.jpg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.348957 gemd-1.9.0/gemd/entity/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1591 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.348957 gemd-1.9.0/gemd/entity/attribute/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      271 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/attribute/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4617 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/attribute/base_attribute.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1396 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/attribute/condition.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1497 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/attribute/parameter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1417 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/attribute/property.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2585 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/attribute/property_and_conditions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8561 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/base_entity.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.348957 gemd-1.9.0/gemd/entity/bounds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      407 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/bounds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1135 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/bounds/base_bounds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2430 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/bounds/categorical_bounds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2457 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/bounds/composition_bounds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1956 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/bounds/integer_bounds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1471 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/bounds/molecular_structure_bounds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3734 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/bounds/real_bounds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1175 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/bounds_validation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6291 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/case_insensitive_dict.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5611 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/dict_serializable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      762 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/file_link.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      370 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/has_dependencies.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3119 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/link_by_uid.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.352957 gemd-1.9.0/gemd/entity/object/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      525 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2493 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/base_object.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1575 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/has_conditions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      848 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/has_material.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1576 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/has_parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      833 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/has_process.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1559 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/has_properties.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4427 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/has_quantities.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      956 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/has_source.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1877 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/has_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1661 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/has_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4255 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/has_template_check_generator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7374 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/ingredient_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6096 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/ingredient_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4694 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/material_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5570 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/material_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5035 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/measurement_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3107 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/measurement_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4753 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/process_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4883 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/object/process_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1584 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/setters.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.352957 gemd-1.9.0/gemd/entity/source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       92 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/source/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1443 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/source/performed_source.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.352957 gemd-1.9.0/gemd/entity/template/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      495 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/template/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2018 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/template/attribute_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3294 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/template/base_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/template/condition_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3614 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/template/has_condition_templates.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3614 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/template/has_parameter_templates.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3657 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/template/has_property_templates.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1996 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/template/material_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3512 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/template/measurement_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1007 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/template/parameter_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3990 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/template/process_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      998 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/template/property_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3883 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5661 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/valid_list.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.356957 gemd-1.9.0/gemd/entity/value/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      759 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      841 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/base_value.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      713 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/categorical_value.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      600 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/composition_value.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1545 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/continuous_value.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2057 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/discrete_categorical.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2692 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/empirical_formula.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1330 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/inchi_value.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      622 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/integer_value.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      654 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/molecular_value.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1262 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/nominal_categorical.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/nominal_composition.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1469 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/nominal_integer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1293 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/nominal_real.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1265 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/normal_real.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1364 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/smiles_value.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2891 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/uniform_integer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1699 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/entity/value/uniform_real.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.356957 gemd-1.9.0/gemd/enumeration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       79 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/enumeration/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1713 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/enumeration/base_enumeration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      368 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/enumeration/origin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      327 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/enumeration/sample_type.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.356957 gemd-1.9.0/gemd/json/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2892 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/json/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      526 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/json/gemd_encoder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11453 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/json/gemd_json.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.356957 gemd-1.9.0/gemd/units/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      255 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/units/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34010 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/units/citrine_en.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6638 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/units/constants_en.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2204 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/units/impl.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.360957 gemd-1.9.0/gemd/units/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       40 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/units/tests/test_units.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.360957 gemd-1.9.0/gemd/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      392 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18156 2022-05-24 00:47:21.000000 gemd-1.9.0/gemd/util/impl.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-24 00:48:42.340956 gemd-1.9.0/gemd.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      606 2022-05-24 00:48:41.000000 gemd-1.9.0/gemd.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3616 2022-05-24 00:48:42.000000 gemd-1.9.0/gemd.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-05-24 00:48:41.000000 gemd-1.9.0/gemd.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      149 2022-05-24 00:48:42.000000 gemd-1.9.0/gemd.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2022-05-24 00:48:42.000000 gemd-1.9.0/gemd.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-05-24 00:48:42.360957 gemd-1.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1314 2022-05-24 00:47:21.000000 gemd-1.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gemd-1.8.1/LICENSE` & `gemd-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/PKG-INFO` & `gemd-1.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: gemd
-Version: 1.8.1
+Version: 1.9.0
 Summary: Python binding for Citrine's GEMD data model
 Home-page: http://github.com/CitrineInformatics/gemd-python
 Author: Citrine Informatics
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: tests
+Provides-Extra: gemd.demo.tests
+Provides-Extra: gemd.entity.bounds.tests
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `gemd-1.8.1/README.md` & `gemd-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/__init__.py` & `gemd-1.9.0/gemd/__init__.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/builders/impl.py` & `gemd-1.9.0/gemd/builders/impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
 
     Parameters
     ----------
     target: BaseObject
         The object to attach the attribute to
     template: AttributeTemplate
         The AttributeTemplate for the attribute.
-    value: Union[BaseValue, str, float, int])
+    value: Union[BaseValue, str, float, int]
         The value for the attribute.  Accepts any GEMD Value type, or will
         attempt to generate an appropriate Value given a str, float or int.
 
     Returns
     --------
     BaseAttribute
         The generated attribute
@@ -269,15 +269,15 @@
     """
     Generate an Attribute and the contained Value.
 
     Parameters
     ----------
     template: AttributeTemplate
         The AttributeTemplate for the attribute.
-    value: Union[BaseValue, str, float, int])
+    value: Union[BaseValue, str, float, int]
         The value for the attribute.  Accepts any GEMD Value type, or will
         attempt to generate an appropriate Value given a str, float or int.
 
     Returns
     --------
     BaseAttribute
         The generated attribute
```

### Comparing `gemd-1.8.1/gemd/demo/cake.py` & `gemd-1.9.0/gemd/demo/cake.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Bake a cake."""
 import json
 
 import random
 
 from gemd.entity.attribute import Condition, Parameter, Property, PropertyAndConditions
+from gemd.entity.base_entity import BaseEntity
 from gemd.entity.bounds import IntegerBounds, RealBounds, CategoricalBounds, CompositionBounds, \
     MolecularStructureBounds
 from gemd.entity.object import ProcessSpec, ProcessRun, MaterialSpec, MaterialRun, \
     MeasurementSpec, MeasurementRun, IngredientSpec, IngredientRun
 from gemd.entity.template import ProcessTemplate, MaterialTemplate, MeasurementTemplate, \
     PropertyTemplate, ParameterTemplate, ConditionTemplate
 from gemd.entity.value import NominalInteger, UniformInteger, \
@@ -565,15 +566,15 @@
     sugar = _make_material(
         material_name="Sugar",
         process_tmpl_name="Procuring",
         process_kwargs={
             "tags": [
                 'purchase::dry-goods'
             ],
-            "notes": 'Purchasing all purpose flour'
+            "notes": 'Purchasing granulated sugar'
         },
         template=tmpl["Formulaic Material"],
         tags=[
             'raw material',
             'sweetener',
             'dry-goods'
         ],
@@ -792,23 +793,23 @@
     cake_obj = make_instance(cake_spec)
     operators = ['gwash', 'jadams', 'thomasj', 'jmadison', 'jmonroe']
     producers = ['Fresh Farm', 'Sunnydale', 'Greenbrook']
     drygoods = ['Acme', 'A1', 'Reliable', "Big Box"]
     cake_obj.process.source = PerformedSource(performed_by=random.choice(operators),
                                               performed_date='2015-03-14')
 
-    def _randomize_object(item):
+    def _randomize_object(item: BaseEntity):
         # Add in the randomized particular values
         if not isinstance(item, (MaterialRun, ProcessRun, IngredientRun)):
             return
 
         item.add_uid(DEMO_SCOPE, '{}-{}'.format(item.spec.uids[DEMO_SCOPE], run_key))
         if item.spec.tags is not None:
             item.tags = list(item.spec.tags)
-        if item.spec.notes:  # Neither None or empty string
+        if item.spec.notes:  # Neither None nor empty string
             item.notes = 'The spec says "{}"'.format(item.spec.notes)
         if isinstance(item, MaterialRun):
             if 'raw material' in item.tags:
                 if 'produce' in item.tags:
                     supplier = random.choice(producers)
                 else:
                     supplier = random.choice(drygoods)
```

### Comparing `gemd-1.8.1/gemd/demo/material_run_example.py` & `gemd-1.9.0/gemd/demo/material_run_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         if std >= 0:
             return NormalReal(mean=mean, std=std, units=unit)
         else:
             return NominalReal(mean, units=unit)
     # if it is just a number wrap it in a nominal value
     elif isinstance(val, (float, int)):
         return NominalReal(val, '')
-    # if it is a single string, its either a single number of a category
+    # if it is a single string, it's either a single number of a category
     elif isinstance(val, str):
         try:
             num = float(val)
             return NominalReal(num, '')
         except ValueError:
             return DiscreteCategorical(val)
     else:
```

### Comparing `gemd-1.8.1/gemd/demo/measurement_example.py` & `gemd-1.9.0/gemd/demo/measurement_example.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/demo/strehlow_and_cook.pif` & `gemd-1.9.0/gemd/demo/strehlow_and_cook.pif`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/demo/strehlow_and_cook.py` & `gemd-1.9.0/gemd/demo/strehlow_and_cook.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 from gemd.entity.value.uniform_real import UniformReal
 from gemd.entity.bounds.real_bounds import RealBounds
 
 from gemd.enumeration.origin import Origin
 
 from gemd.units import convert_units
 
+from typing import Iterable
+
 # For now, module constant, though likely this should get promoted to a package level
 DEMO_TEMPLATE_SCOPE = 'citrine-demo-sac-template'
 FULL_TABLE = "strehlow_and_cook.pif"
 SMALL_TABLE = "strehlow_and_cook_small.pif"
 
 
 def import_table(filename=SMALL_TABLE):
@@ -66,24 +68,24 @@
 
     return smaller
 
 
 def formula_latex(old):
     """Transform a formula into one with LaTeX markup."""
     import re
-    return re.sub(r"(?<=[A-Za-z])([\d\.]+)(?=[A-Za-z]|$)", r"$_{\1}$", formula_clean(old))
+    return re.sub(r"(?<=[A-Za-z])([\d.]+)(?=[A-Za-z]|$)", r"$_{\1}$", formula_clean(old))
 
 
 def formula_clean(old):
     """Transform a formula into a cleaner version."""
     import re
     return re.sub(r"(?<=[A-Za-z])1(?=[A-Za-z]|$)", '', old)
 
 
-def make_templates(template_scope=DEMO_TEMPLATE_SCOPE):
+def make_templates(template_scope: str = DEMO_TEMPLATE_SCOPE):
     """Build all templates needed for the table."""
     tmpl = dict()
 
     # Attribute Templates
     attribute_feed = {
         "Formula": [PropertyTemplate,
                     CompositionBounds(components=EmpiricalFormula.all_elements())],
@@ -186,15 +188,15 @@
                          uids={template_scope: name},
                          tags=['citrine::demo::template::object'],
                          **kw_args)
 
     return tmpl
 
 
-def make_strehlow_objects(table=None, template_scope=DEMO_TEMPLATE_SCOPE):
+def make_strehlow_objects(table: Iterable = None, template_scope: str = DEMO_TEMPLATE_SCOPE):
     """Make a table with Strehlow & Cook data."""
     tmpl = make_templates(template_scope)
 
     if table is None:
         table = import_table()
 
     # Specs
@@ -319,19 +321,15 @@
     into a Training Table, and as such we are missing the column definition component of the query
     that created this particular result set.
 
     :param compounds: a list of MaterialRun objects from the make_strehlow_objects method
     :return:
     """
     # Stash templates in convenience variables
-    for comp in compounds:
-        if comp.spec.properties:
-            chem_tmpl = comp.spec.properties[0].property.template
-            break
-
+    chem_tmpl = next(p.property.template for c in compounds for p in c.spec.properties)
     chem_mat_tmpl = compounds[0].spec.template
 
     tmpl = dict()
 
     properties = compounds[0].measurements[0].spec.template.properties
     conditions = compounds[0].measurements[0].spec.template.conditions
     parameters = compounds[0].measurements[0].spec.template.parameters
@@ -490,9 +488,9 @@
 
     print("\n\nJSON -- Training table")
     import gemd.json as je
     print(json.dumps(json.loads(je.dumps(full_table))["object"], indent=2))
 
     print("\n\nCSV -- Display table")
     display = make_display_table(full_table)
-    for row in display:
-        print(','.join(map(lambda x: str(x), row)))
+    for row_ in display:
+        print(','.join(map(lambda x: str(x), row_)))
```

### Comparing `gemd-1.8.1/gemd/demo/strehlow_and_cook_small.pif` & `gemd-1.9.0/gemd/demo/strehlow_and_cook_small.pif`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/demo/table_example.py` & `gemd-1.9.0/gemd/demo/table_example.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/demo/toothpick.jpg` & `gemd-1.9.0/gemd/demo/toothpick.jpg`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/__init__.py` & `gemd-1.9.0/gemd/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/attribute/base_attribute.py` & `gemd-1.9.0/gemd/entity/attribute/base_attribute.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/attribute/condition.py` & `gemd-1.9.0/gemd/entity/attribute/condition.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/attribute/parameter.py` & `gemd-1.9.0/gemd/entity/attribute/parameter.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/attribute/property.py` & `gemd-1.9.0/gemd/entity/attribute/property.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/attribute/property_and_conditions.py` & `gemd-1.9.0/gemd/entity/attribute/property_and_conditions.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     conditions: List[:class:`Condition <gemd.entity.attribute.condition.Condition>`]
         An optional list of conditions associated with this property.
 
     """
 
     typ = "property_and_conditions"
 
-    def __init__(self, property: Property = None, conditions: Iterable[Condition] = None):
+    def __init__(self,
+                 property: Property = None,
+                 conditions: Union[Iterable[Condition], Condition] = None):
         self._property = None
         self.property = property
         self._conditions = None
         self.conditions = conditions
 
     @property
     def conditions(self) -> List[Condition]:
```

### Comparing `gemd-1.8.1/gemd/entity/base_entity.py` & `gemd-1.9.0/gemd/entity/base_entity.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/bounds/base_bounds.py` & `gemd-1.9.0/gemd/entity/bounds/base_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/bounds/categorical_bounds.py` & `gemd-1.9.0/gemd/entity/bounds/categorical_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/bounds/composition_bounds.py` & `gemd-1.9.0/gemd/entity/bounds/composition_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/bounds/integer_bounds.py` & `gemd-1.9.0/gemd/entity/bounds/integer_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/bounds/molecular_structure_bounds.py` & `gemd-1.9.0/gemd/entity/bounds/molecular_structure_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/bounds/real_bounds.py` & `gemd-1.9.0/gemd/entity/bounds/real_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/bounds_validation.py` & `gemd-1.9.0/gemd/entity/bounds_validation.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/case_insensitive_dict.py` & `gemd-1.9.0/gemd/entity/case_insensitive_dict.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/dict_serializable.py` & `gemd-1.9.0/gemd/entity/dict_serializable.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         """
         keys = {x.lstrip('_') for x in vars(self) if x not in self.skip}
         attributes = {k: self.__getattribute__(k) for k in keys}
         attributes["type"] = self.typ
         return attributes
 
-    def dump(self) -> str:
+    def dump(self) -> Dict[str, Any]:
         """
         Convert the object to a JSON dictionary, so that every entry is serialized.
 
         Uses the json encoder client, so objects with uids are converted to LinkByUID dictionaries.
 
         Returns
         -------
```

### Comparing `gemd-1.8.1/gemd/entity/file_link.py` & `gemd-1.9.0/gemd/entity/file_link.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/link_by_uid.py` & `gemd-1.9.0/gemd/entity/link_by_uid.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/object/__init__.py` & `gemd-1.9.0/gemd/entity/object/__init__.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/object/base_object.py` & `gemd-1.9.0/gemd/entity/object/base_object.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/object/has_conditions.py` & `gemd-1.9.0/gemd/entity/object/has_conditions.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 from gemd.entity.has_dependencies import HasDependencies
 from gemd.entity.object.has_template_check_generator import HasTemplateCheckGenerator
 from gemd.entity.template.has_condition_templates import HasConditionTemplates
 from gemd.entity.attribute.condition import Condition
 from gemd.entity.setters import validate_list
 
 from typing import Union, Iterable, List, Set
+from abc import ABC
 
 
-class HasConditions(HasTemplateCheckGenerator, HasDependencies):
+class HasConditions(HasTemplateCheckGenerator, HasDependencies, ABC):
     """Mixin-trait for entities that include conditions.
 
     Parameters
     ----------
     conditions: List[:class:`Condition <gemd.entity.attribute.condition.Condition>`]
         A list of conditions associated with this entity.
 
     """
 
-    def __init__(self, conditions: Iterable[Condition]):
+    def __init__(self, conditions: Union[Condition, Iterable[Condition]]):
         self._conditions = None
         self.conditions = conditions
 
     @property
     def conditions(self) -> List[Condition]:
         """Get a list of the conditions."""
         return self._conditions
 
     @conditions.setter
-    def conditions(self, conditions: Iterable[Condition]):
+    def conditions(self, conditions: Union[Condition, Iterable[Condition]]):
         """Set the list of conditions."""
         checker = self._generate_template_check(HasConditionTemplates.validate_condition)
         self._conditions = validate_list(conditions, Condition, trigger=checker)
 
     def _local_dependencies(self) -> Set[Union["BaseEntity", "LinkByUID"]]:
         """Return a set of all immediate dependencies (no recursion)."""
         return {cond.template for cond in self.conditions if cond.template is not None}
```

### Comparing `gemd-1.8.1/gemd/entity/object/has_material.py` & `gemd-1.9.0/gemd/entity/object/has_material.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """For entities that have specs."""
 from gemd.entity.has_dependencies import HasDependencies
 from gemd.entity.object.base_object import BaseObject
 from gemd.entity.link_by_uid import LinkByUID
 
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 from typing import Union, Set
 
 
-class HasMaterial(HasDependencies):
+class HasMaterial(HasDependencies, ABC):
     """Mix-in trait for objects that can be assigned materials."""
 
     @property
     @abstractmethod
     def material(self) -> Union[BaseObject, LinkByUID]:
         """Get the material."""
```

### Comparing `gemd-1.8.1/gemd/entity/object/has_parameters.py` & `gemd-1.9.0/gemd/entity/object/has_parameters.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 from gemd.entity.has_dependencies import HasDependencies
 from gemd.entity.object.has_template_check_generator import HasTemplateCheckGenerator
 from gemd.entity.template.has_parameter_templates import HasParameterTemplates
 from gemd.entity.attribute.parameter import Parameter
 from gemd.entity.setters import validate_list
 
 from typing import Union, Iterable, List, Set
+from abc import ABC
 
 
-class HasParameters(HasTemplateCheckGenerator, HasDependencies):
+class HasParameters(HasTemplateCheckGenerator, HasDependencies, ABC):
     """Mixin-trait for entities that include parameters.
 
     Parameters
     ----------
     parameters: List[:class:`Parameter <gemd.entity.attribute.parameter.Parameter>`]
         A list of parameters associated with this entity.
 
     """
 
-    def __init__(self, parameters: Iterable[Parameter]):
+    def __init__(self, parameters: Union[Parameter, Iterable[Parameter]]):
         self._parameters = None
         self.parameters = parameters
 
     @property
     def parameters(self) -> List[Parameter]:
         """Get the list of parameters."""
         return self._parameters
 
     @parameters.setter
-    def parameters(self, parameters: Iterable[Parameter]):
+    def parameters(self, parameters: Union[Parameter, Iterable[Parameter]]):
         """Set the list of parameters."""
         checker = self._generate_template_check(HasParameterTemplates.validate_parameter)
         self._parameters = validate_list(parameters, Parameter, trigger=checker)
 
     def _local_dependencies(self) -> Set[Union["BaseEntity", "LinkByUID"]]:
         """Return a set of all immediate dependencies (no recursion)."""
         return {param.template for param in self.parameters if param.template is not None}
```

### Comparing `gemd-1.8.1/gemd/entity/object/has_process.py` & `gemd-1.9.0/gemd/entity/object/has_process.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/object/has_properties.py` & `gemd-1.9.0/gemd/entity/object/has_properties.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 from gemd.entity.has_dependencies import HasDependencies
 from gemd.entity.object.has_template_check_generator import HasTemplateCheckGenerator
 from gemd.entity.template.has_property_templates import HasPropertyTemplates
 from gemd.entity.attribute.property import Property
 from gemd.entity.setters import validate_list
 
 from typing import Union, Iterable, List, Set
+from abc import ABC
 
 
-class HasProperties(HasTemplateCheckGenerator, HasDependencies):
+class HasProperties(HasTemplateCheckGenerator, HasDependencies, ABC):
     """Mixin-trait for entities that include properties.
 
     Parameters
     ----------
     properties: List[:class:`Property <gemd.entity.attribute.property.Property>`]
         A list of properties associated with this entity
 
     """
 
-    def __init__(self, properties: Iterable[Property]):
+    def __init__(self, properties: Union[Property, Iterable[Property]]):
         self._properties = None
         self.properties = properties
 
     @property
     def properties(self) -> List[Property]:
         """Get a list of the properties."""
         return self._properties
 
     @properties.setter
-    def properties(self, properties: Iterable[Property]):
+    def properties(self, properties: Union[Property, Iterable[Property]]):
         """Set the list of properties."""
         checker = self._generate_template_check(HasPropertyTemplates.validate_property)
         self._properties = validate_list(properties, Property, trigger=checker)
 
     def _local_dependencies(self) -> Set[Union["BaseEntity", "LinkByUID"]]:
         """Return a set of all immediate dependencies (no recursion)."""
         return {prop.template for prop in self.properties if prop.template is not None}
```

### Comparing `gemd-1.8.1/gemd/entity/object/has_quantities.py` & `gemd-1.9.0/gemd/entity/object/has_quantities.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/object/has_source.py` & `gemd-1.9.0/gemd/entity/object/has_source.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/object/has_spec.py` & `gemd-1.9.0/gemd/entity/object/has_spec.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/object/has_template.py` & `gemd-1.9.0/gemd/entity/object/has_template.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/object/has_template_check_generator.py` & `gemd-1.9.0/gemd/entity/object/has_template_check_generator.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/object/ingredient_run.py` & `gemd-1.9.0/gemd/entity/object/ingredient_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,16 @@
 
         Returns
         -------
         DictSerializable
             The deserialized object.
 
         """
-        name = d.pop("name", None)
-        labels = d.pop("labels", None)
-        obj = super().from_dict(d)
+        clean = dict(d)
+        name = clean.pop("name", None)
+        labels = clean.pop("labels", None)
+        obj = super().from_dict(clean)
         if name is not None:
             obj._name = name
         if labels is not None:
             obj._labels = validate_list(labels, str)
         return obj
```

### Comparing `gemd-1.8.1/gemd/entity/object/ingredient_spec.py` & `gemd-1.9.0/gemd/entity/object/ingredient_spec.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/object/material_run.py` & `gemd-1.9.0/gemd/entity/object/material_run.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/object/material_spec.py` & `gemd-1.9.0/gemd/entity/object/material_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     typ = "material_spec"
 
     def __init__(self,
                  name: str,
                  *,
                  template: Optional[Union[MaterialTemplate, LinkByUID]] = None,
                  process: Union[ProcessSpec, LinkByUID] = None,
-                 properties: Iterable[PropertyAndConditions] = None,
+                 properties: Union[Iterable[PropertyAndConditions], PropertyAndConditions] = None,
                  uids: Mapping[str, str] = None,
                  tags: Iterable[str] = None,
                  notes: str = None,
                  file_links: Optional[Union[Iterable[FileLink], FileLink]] = None):
         BaseObject.__init__(self, name=name, uids=uids, tags=tags, notes=notes,
                             file_links=file_links)
         HasTemplate.__init__(self, template)
@@ -69,15 +69,16 @@
 
     @property
     def properties(self) -> List[PropertyAndConditions]:
         """Get the list of property-and-conditions."""
         return self._properties
 
     @properties.setter
-    def properties(self, properties: Iterable[PropertyAndConditions]):
+    def properties(self,
+                   properties: Union[Iterable[PropertyAndConditions], PropertyAndConditions]):
         """Set the list of property-and-conditions."""
         checker = self._generate_template_check(HasPropertyTemplates.validate_property)
         self._properties = validate_list(properties, PropertyAndConditions, trigger=checker)
 
     @property
     def process(self) -> Union[ProcessSpec, LinkByUID]:
         """Get the originating process spec."""
@@ -85,15 +86,15 @@
 
     @process.setter
     def process(self, process: Union[ProcessSpec, LinkByUID]):
         """
         Link to the ProcessSpec that creates this MaterialSpec.
 
         If the input, process, is not an instance of ProcessSpec, raise an error.
-        Otherwise, make a bi-directional link: this MaterialSpec is linked to
+        Otherwise, make a bidirectional link: this MaterialSpec is linked to
         process, and process has its output_material field linked to this MaterialSpec
         """
         from gemd.entity.object.process_spec import ProcessSpec
         from gemd.entity.link_by_uid import LinkByUID
         if self.process is not None and isinstance(self.process, ProcessSpec):
             self.process._output_material = None
         if process is None:
```

### Comparing `gemd-1.8.1/gemd/entity/object/measurement_run.py` & `gemd-1.9.0/gemd/entity/object/measurement_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,17 @@
     typ = "measurement_run"
 
     def __init__(self,
                  name: str,
                  *,
                  spec: Union[MeasurementSpec, LinkByUID] = None,
                  material: Union[MaterialRun, LinkByUID] = None,
-                 properties: Iterable[Property] = None,
-                 conditions: Iterable[Condition] = None,
-                 parameters: Iterable[Parameter] = None,
+                 properties: Union[Property, Iterable[Property]] = None,
+                 conditions: Union[Condition, Iterable[Condition]] = None,
+                 parameters: Union[Parameter, Iterable[Parameter]] = None,
                  uids: Mapping[str, str] = None,
                  tags: Iterable[str] = None,
                  notes: str = None,
                  file_links: Optional[Union[Iterable[FileLink], FileLink]] = None,
                  source: PerformedSource = None):
         BaseObject.__init__(self, name=name, uids=uids, tags=tags, notes=notes,
                             file_links=file_links)
```

### Comparing `gemd-1.8.1/gemd/entity/object/measurement_spec.py` & `gemd-1.9.0/gemd/entity/object/measurement_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 
     typ = "measurement_spec"
 
     def __init__(self,
                  name: str,
                  *,
                  template: Optional[Union[MeasurementTemplate, LinkByUID]] = None,
-                 conditions: Iterable[Condition] = None,
-                 parameters: Iterable[Parameter] = None,
+                 conditions: Union[Condition, Iterable[Condition]] = None,
+                 parameters: Union[Parameter, Iterable[Parameter]] = None,
                  uids: Mapping[str, str] = None,
                  tags: Iterable[str] = None,
                  notes: str = None,
                  file_links: Optional[Union[Iterable[FileLink], FileLink]] = None):
         BaseObject.__init__(self, name=name, uids=uids, tags=tags, notes=notes,
                             file_links=file_links)
         HasTemplate.__init__(self, template=template)
```

### Comparing `gemd-1.8.1/gemd/entity/object/process_run.py` & `gemd-1.9.0/gemd/entity/object/process_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,16 +64,16 @@
 
     skip = {"_output_material", "_ingredients"}
 
     def __init__(self,
                  name: str,
                  *,
                  spec: Union[ProcessSpec, LinkByUID] = None,
-                 conditions: Iterable[Condition] = None,
-                 parameters: Iterable[Parameter] = None,
+                 conditions: Union[Condition, Iterable[Condition]] = None,
+                 parameters: Union[Parameter, Iterable[Parameter]] = None,
                  uids: Mapping[str, str] = None,
                  tags: Iterable[str] = None,
                  notes: str = None,
                  file_links: Optional[Union[Iterable[FileLink], FileLink]] = None,
                  source: PerformedSource = None):
         from gemd.entity.object.ingredient_run import IngredientRun
```

### Comparing `gemd-1.8.1/gemd/entity/object/process_spec.py` & `gemd-1.9.0/gemd/entity/object/process_spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,16 +61,16 @@
 
     skip = {"_output_material", "_ingredients"}
 
     def __init__(self,
                  name: str,
                  *,
                  template: Optional[Union[ProcessTemplate, LinkByUID]] = None,
-                 conditions: Iterable[Condition] = None,
-                 parameters: Iterable[Parameter] = None,
+                 conditions: Union[Condition, Iterable[Condition]] = None,
+                 parameters: Union[Parameter, Iterable[Parameter]] = None,
                  uids: Mapping[str, str] = None,
                  tags: Iterable[str] = None,
                  notes: str = None,
                  file_links: Optional[Union[Iterable[FileLink], FileLink]] = None):
         from gemd.entity.object.ingredient_spec import IngredientSpec
         from gemd.entity.link_by_uid import LinkByUID
```

### Comparing `gemd-1.8.1/gemd/entity/source/performed_source.py` & `gemd-1.9.0/gemd/entity/source/performed_source.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/template/attribute_template.py` & `gemd-1.9.0/gemd/entity/template/attribute_template.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/template/base_template.py` & `gemd-1.9.0/gemd/entity/template/base_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         tuple [AttributeTemplate or LinkByUID, BaseBounds]
            An attribute template, optionally with another Bounds object that is more
            restrictive than the attribute template's default bounds.
 
         Returns
         -------
         List[AttributeTemplate or LinkByUID, BaseBounds]
-            The attribute template and bounds that should be applied the the attribute
+            The attribute template and bounds that should be applied to the attribute
             when used in the context of **this** object.
 
         """
         # if given a template only, use None to represent passthrough bounds
         if isinstance(template_or_tuple, (AttributeTemplate, LinkByUID)):
             return [template_or_tuple, None]
         # if given a (template, bounds) pair,
```

### Comparing `gemd-1.8.1/gemd/entity/template/condition_template.py` & `gemd-1.9.0/gemd/entity/template/condition_template.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/template/has_condition_templates.py` & `gemd-1.9.0/gemd/entity/template/has_condition_templates.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/template/has_parameter_templates.py` & `gemd-1.9.0/gemd/entity/template/has_parameter_templates.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/template/has_property_templates.py` & `gemd-1.9.0/gemd/entity/template/has_property_templates.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/template/material_template.py` & `gemd-1.9.0/gemd/entity/template/material_template.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/template/measurement_template.py` & `gemd-1.9.0/gemd/entity/template/measurement_template.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/template/parameter_template.py` & `gemd-1.9.0/gemd/entity/template/parameter_template.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/template/process_template.py` & `gemd-1.9.0/gemd/entity/template/process_template.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/template/property_template.py` & `gemd-1.9.0/gemd/entity/template/property_template.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/util.py` & `gemd-1.9.0/gemd/entity/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Utility methods."""
 from gemd.util import recursive_foreach
 
+from typing import List, Dict, Any
+
 
 def make_instance(base_spec):
     """
     Create a set of Run objects that mimic the connectivity of the passed Spec object.
 
-    Paramters
+    Parameters
     ---------
     base_spec: BaseObject
         A spec instance that may point to other specs.
 
     Returns
     -------
     BaseObject
@@ -89,24 +91,31 @@
             _array_like = (list, tuple, np.ndarray)  # pragma: no cover
     except ImportError:  # pragma: no cover
         _array_like = (list, tuple)  # pragma: no cover
 
     return _array_like
 
 
-def complete_material_history(mat):
+def complete_material_history(mat) -> List[Dict[str, Any]]:
     """
     Get a list of every single object in the material history, all as dictionaries.
 
     This is useful for testing, if we want the context list that can be used to rehydrate
     an entire material history.
 
-    :param mat: root material run
-    :return: a list containing every object connected to mat, each a dictionary with all
-        links substituted.
+    Parameters
+    ---------
+    mat: MaterialRun
+        root material run
+    Returns
+    -------
+    list
+        a list containing every object connected to mat, each a dictionary with
+        all links substituted.
+
     """
     from gemd.entity.base_entity import BaseEntity
     import json
     from gemd.json import dumps, loads
     from gemd.util.impl import substitute_links
 
     result = []
```

### Comparing `gemd-1.8.1/gemd/entity/valid_list.py` & `gemd-1.9.0/gemd/entity/valid_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """A list that can validate its contents."""
-from collections.abc import Iterable
+from typing import Optional, Union, Iterable, Callable, Type, TypeVar
+
+T = TypeVar('T')
 
 
 class ValidList(list):
     """
     A list-like class that verifies that its content conforms to specified types.
 
     Parameters
@@ -18,15 +20,18 @@
         invocation for list operations) and, if it returns something other than None,
         it will use that returned value for the assignment.
 
     """
 
     _content_type = tuple([])
 
-    def __init__(self, _list, content_type=None, trigger=None):
+    def __init__(self,
+                 _list: Iterable,
+                 content_type: Optional[Union[Iterable[Type], Type]] = None,
+                 trigger: Callable[[T], Optional[T]] = None):
         if content_type is None:
             content_type = tuple()
 
         if isinstance(content_type, dict):
             raise TypeError('A dict is not an acceptable container for content filters')
         elif isinstance(content_type, Iterable):
             self._content_type = tuple(content_type)
```

### Comparing `gemd-1.8.1/gemd/entity/value/__init__.py` & `gemd-1.9.0/gemd/entity/value/__init__.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/value/base_value.py` & `gemd-1.9.0/gemd/entity/value/base_value.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/value/categorical_value.py` & `gemd-1.9.0/gemd/entity/value/categorical_value.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/value/composition_value.py` & `gemd-1.9.0/gemd/entity/value/composition_value.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/value/continuous_value.py` & `gemd-1.9.0/gemd/entity/value/continuous_value.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/value/discrete_categorical.py` & `gemd-1.9.0/gemd/entity/value/discrete_categorical.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/value/empirical_formula.py` & `gemd-1.9.0/gemd/entity/value/empirical_formula.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""An empirical chemical formaula."""
+"""An empirical chemical formula."""
 from gemd.entity.value.composition_value import CompositionValue
 from gemd.entity.bounds import CompositionBounds
 
 
 _all_elements = {
     'Tb', 'Be', 'Sb', 'Re', 'Sr', 'Ac', 'Ho', 'Ir', 'Cr', 'Os', 'S', 'Pt', 'Si', 'C', 'V', 'Bi',
     'U', 'Pr', 'B', 'O', 'Zn', 'Xe', 'N', 'Ni', 'No', 'Ti', 'Pa', 'Am', 'Cu', 'I', 'Al', 'Ba',
```

### Comparing `gemd-1.8.1/gemd/entity/value/inchi_value.py` & `gemd-1.9.0/gemd/entity/value/inchi_value.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""An empirical chemical formaula."""
+"""An empirical chemical formula."""
 from gemd.entity.value.molecular_value import MolecularValue
 from gemd.entity.bounds import MolecularStructureBounds
 
 
 class InChI(MolecularValue):
     """
     A molecular structure encoded according to the IUPAC International Chemical Identifier (InChI).
```

### Comparing `gemd-1.8.1/gemd/entity/value/integer_value.py` & `gemd-1.9.0/gemd/entity/value/integer_value.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/value/molecular_value.py` & `gemd-1.9.0/gemd/entity/value/molecular_value.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/value/nominal_categorical.py` & `gemd-1.9.0/gemd/entity/value/nominal_categorical.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from gemd.entity.setters import validate_str
 from gemd.entity.value.categorical_value import CategoricalValue
 from gemd.entity.bounds import CategoricalBounds
 
 
 class NominalCategorical(CategoricalValue):
     """
-    A nominal category that the value is believe to have. It may not be exact.
+    A nominal category that the value is believed to have. It may not be exact.
 
     Parameters
     ----------
     category: str
         The nominal category.
 
     """
```

### Comparing `gemd-1.8.1/gemd/entity/value/nominal_composition.py` & `gemd-1.9.0/gemd/entity/value/nominal_composition.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/value/nominal_integer.py` & `gemd-1.9.0/gemd/entity/value/nominal_integer.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/value/nominal_real.py` & `gemd-1.9.0/gemd/entity/value/nominal_real.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/value/normal_real.py` & `gemd-1.9.0/gemd/entity/value/normal_real.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/value/smiles_value.py` & `gemd-1.9.0/gemd/entity/value/smiles_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""An empirical chemical formaula."""
+"""An empirical chemical formula."""
 from gemd.entity.value.molecular_value import MolecularValue
 from gemd.entity.bounds import MolecularStructureBounds
 
 
 class Smiles(MolecularValue):
     """
     A molecular structure encoded according to SMILES.
```

### Comparing `gemd-1.8.1/gemd/entity/value/uniform_integer.py` & `gemd-1.9.0/gemd/entity/value/uniform_integer.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/entity/value/uniform_real.py` & `gemd-1.9.0/gemd/entity/value/uniform_real.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/enumeration/base_enumeration.py` & `gemd-1.9.0/gemd/enumeration/base_enumeration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Base class for all enumerations."""
 from enum import Enum
 
 
 class BaseEnumeration(Enum):
     """Enumeration class that can convert between enumerations and associated values."""
 
-    def __init__(self, *args):
+    def __init__(self, *_):
         """Ensure that there are no duplicates in the enumeration."""
         cls = self.__class__
         if any(self.value == e.value for e in cls):
             raise ValueError("Duplicates not allowed in enumerated set of values {}".format(cls))
         if not isinstance(self.value, str):
             raise ValueError("All values of enum {} must be strings".format(cls))
```

### Comparing `gemd-1.8.1/gemd/json/__init__.py` & `gemd-1.9.0/gemd/json/__init__.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/json/gemd_encoder.py` & `gemd-1.9.0/gemd/json/gemd_encoder.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/json/gemd_json.py` & `gemd-1.9.0/gemd/json/gemd_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,16 +255,19 @@
         Register additional classes to the custom deserialization object hook.
 
         This allows for additional DictSerializable subclasses to be registered to the class index
         that is used to decode the type strings.  Existing keys are overwritten, allowing classes
         in the gemd package to be subclassed and overridden in the class index by their
         subclass.
 
-        :param classes: a dict mapping the type string to the class
-        :return: None
+        Parameters
+        ----------
+        classes: Dict[str, type]
+            a dict mapping the type string to the class
+
         """
         if not isinstance(classes, dict):
             raise ValueError("Must be given a dict from str -> class")
         non_string_keys = [x for x in classes.keys() if not isinstance(x, str)]
         if len(non_string_keys) > 0:
             raise ValueError(
                 "The keys must be strings, but got {} as keys".format(non_string_keys))
@@ -277,18 +280,28 @@
 
     def _load_and_index(self, d, object_index, substitute=False):
         """
         Load the class based on the type string and index it, if a BaseEntity.
 
         This function is used as the object hook when deserializing gemd objects
 
-        :param d: dictionary to try to load into a registered class instance
-        :param object_index: to add the object to if it is a BaseEntity
-        :param substitute: whether to substitute LinkByUIDs when they are found in the index
-        :return: the deserialized object, or the input dict if it wasn't recognized
+        Parameters
+        ----------
+        d: dict
+            dictionary to try to load into a registered class instance
+        object_index: dict
+            to add the object to if it is a BaseEntity
+        substitute: bool
+            whether to substitute LinkByUIDs when they are found in the index
+
+        Returns
+        -------
+        object
+            the deserialized object, or the input dict if it wasn't recognized
+
         """
         if "type" not in d:
             return d
         typ = d.pop("type")
 
         if typ in self._clazz_index:
             clz = self._clazz_index[typ]
```

### Comparing `gemd-1.8.1/gemd/units/citrine_en.txt` & `gemd-1.9.0/gemd/units/citrine_en.txt`

 * *Files 0% similar despite different names*

```diff
@@ -431,14 +431,15 @@
 
 # Charge
 [charge] = [current] * [time]
 coulomb = ampere * second = C = Coulomb
 abcoulomb = 10 * C = abC
 faraday = e * N_A * mole = _ = Faraday
 conventional_coulomb_90 = K_J90 * R_K90 / (K_J * R_K) * coulomb = C_90
+ampere_hour = ampere * hour = Ah
 
 # Electric potential
 [electric_potential] = [energy] / [charge]
 volt = joule / coulomb = V = Volt
 abvolt = 1e-8 * volt = abV
 mean_international_volt = 1.00034 * volt = V_it  # approximate
 US_international_volt = 1.00033 * volt = V_US    # approximate
```

### Comparing `gemd-1.8.1/gemd/units/constants_en.txt` & `gemd-1.9.0/gemd/units/constants_en.txt`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/units/impl.py` & `gemd-1.9.0/gemd/units/impl.py`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/gemd/util/impl.py` & `gemd-1.9.0/gemd/util/impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         if len(base_obj.uids) == 0:
             base_obj.add_uid(scope, str(uuid.uuid4()))
         return
     recursive_foreach(obj, func)
     return
 
 
-def _cached_isinstance(
+def cached_isinstance(
         obj: object,
         class_or_tuple: Union[Type, Tuple[Union[Type, Tuple[Type]]]]) -> bool:
     """
     Emulate isinstance builtin to take advantage of functools caching.
 
     Parameters
     ----------
@@ -57,25 +57,29 @@
         Whether an object is an instance of a class or of a subclass thereof.
 
     """
     obj_type = type(obj)
     return _cached_issubclass(obj_type, class_or_tuple)
 
 
+# Older unreleased versions of citrine-python referenced the private method directly
+_cached_isinstance = cached_isinstance
+
+
 @functools.lru_cache(maxsize=None)
 def _cached_issubclass(
         cls: Type,
         class_or_tuple: Union[Type, Tuple[Union[Type, Tuple[Type]]]]) -> bool:
     """
     Emulate issubclass builtin to take advantage of functools caching.
 
     Parameters
     ----------
-    obj: object
-
+    cls: type
+        The class to evaluate
     class_or_tuple: Union[Type, Tuple[Union[Type, Tuple[Type]]]]
         A single type, a tuple of types (potentially nested)
 
     Returns
     -------
     bool
         Whether 'cls' is a derived from another class or is the same class.
@@ -95,15 +99,15 @@
     values for which the sub function applies.
 
     Parameters
     ----------
     thing: Any
         The object to traverse with substitution.
     sub: Callable[[object], object]
-        Function which provides substitute for value; should not have side-effects.
+        Function which provides substitute for value; should not have side effects.
     applies: Callable[[object], bool]
         Function which defines the domain for the sub function to be invoked.
 
     """
     if visited is None:
         visited = {}
     if thing.__hash__ is not None and thing in visited:
@@ -112,22 +116,22 @@
     if applies(thing):
         replacement = sub(thing)
         if thing.__hash__ is not None:
             visited[thing] = replacement
     else:
         replacement = thing
 
-    if _cached_isinstance(replacement, MutableSequence):
+    if cached_isinstance(replacement, MutableSequence):
         new = [_substitute(x, sub, applies, visited) for x in replacement]
-    elif _cached_isinstance(replacement, Tuple):
+    elif cached_isinstance(replacement, Tuple):
         new = tuple(_substitute(x, sub, applies, visited) for x in replacement)
-    elif _cached_isinstance(replacement, Mapping):
+    elif cached_isinstance(replacement, Mapping):
         new = {_substitute(k, sub, applies, visited): _substitute(v, sub, applies, visited)
                for k, v in replacement.items()}
-    elif _cached_isinstance(replacement, DictSerializable):
+    elif cached_isinstance(replacement, DictSerializable):
         new_attrs = {_substitute(k, sub, applies, visited): _substitute(v, sub, applies, visited)
                      for k, v in replacement.as_dict().items()}
         new = replacement.build(new_attrs)
     else:
         new = replacement
 
     if thing.__hash__ is not None:
@@ -147,25 +151,25 @@
     applies(element) is true and the element is mutable.
 
     Parameters
     ----------
     thing: Any
         The object to traverse with substitution.
     sub: Callable[[object], object]
-        Function which provides substitute for value; should not have side-effects.
+        Function which provides substitute for value; should not have side effects.
     applies: Callable[[object], bool]
         Function which defines the domain for the sub function to be invoked.
 
     """
     def _key(obj):
-        if _cached_isinstance(obj, (float, int, str)):
+        if cached_isinstance(obj, (float, int, str)):
             return None
         elif obj.__hash__ is not None:
             return obj
-        elif _cached_isinstance(obj, Iterable) and not _cached_isinstance(obj, ByteString):
+        elif cached_isinstance(obj, Iterable) and not cached_isinstance(obj, ByteString):
             return id(obj)
         else:
             return None  # pragma: no cover  Fallback for caution's sake
 
     orig_key = _key(thing)
     if visited is None:
         visited = {}
@@ -173,35 +177,35 @@
         return visited[orig_key]
 
     if applies(thing):
         thing = sub(thing)
     if orig_key is not None:
         visited[orig_key] = thing  # Store before we start recursing
 
-    if _cached_isinstance(thing, MutableSequence):  # Change list in place
+    if cached_isinstance(thing, MutableSequence):  # Change list in place
         for i, x in enumerate(thing):
             thing[i] = _substitute_inplace(x, sub, applies, visited)
-    elif _cached_isinstance(thing, Tuple):  # Tuples are immutable; regenerate
+    elif cached_isinstance(thing, Tuple):  # Tuples are immutable; regenerate
         thing = tuple(_substitute_inplace(x, sub, applies, visited) for x in thing)
         visited[orig_key] = thing  # We mutated it
-    elif _cached_isinstance(thing, Mapping):  # Change dict in place, both keys & values
+    elif cached_isinstance(thing, Mapping):  # Change dict in place, both keys & values
         remove = set()  # Store todos because can't mutate a dict in a loop
         update = dict()
         for k, v in thing.items():
             new_k = _substitute_inplace(k, sub, applies, visited)
             new_v = _substitute_inplace(v, sub, applies, visited)
             if id(k) != id(new_k):
                 remove.add(k)
                 update[new_k] = v
             if id(v) != id(new_v):
                 update[new_k] = new_v
         for k in remove:
             thing.pop(k, None)
         thing.update(update)
-    elif _cached_isinstance(thing, DictSerializable):
+    elif cached_isinstance(thing, DictSerializable):
         for k, v in thing.as_dict().items():  # Assume key can't change b/c it's an attribute
             new_v = _substitute_inplace(v, sub, applies, visited)
             if id(v) != id(new_v):
                 _setter_by_attribute(type(thing), k)(thing, new_v)
 
     return thing
 
@@ -249,15 +253,15 @@
     This method builds a dictionary of GEMD objects found by recursively crawling the passed
     object, indexed by all scope:id tuples found in any of the objects.  The passed object can
     be a list, tuple, dictionary or GEMD object.
 
     Parameters
     ----------
     obj: Union[Iterable, Mapping, BaseEntity, DictSerializable]
-        target container (dict, list, ..) from which to create an index of GEMD objects
+        target container (dict, list, ...) from which to create an index of GEMD objects
 
     """
     def _make_index(_obj: BaseEntity):
         return ((LinkByUID(scope=scope, id=_obj.uids[scope]), _obj) for scope in _obj.uids)
 
     idx = {}
     for uid, target in recursive_flatmap(obj, _make_index):
@@ -303,15 +307,15 @@
     if inplace:
         method = _substitute_inplace
     else:
         method = _substitute
 
     return method(obj,
                   sub=lambda o: o.to_link(scope=scope, allow_fallback=allow_fallback),
-                  applies=lambda o: o is not obj and _cached_isinstance(o, BaseEntity))
+                  applies=lambda o: o is not obj and cached_isinstance(o, BaseEntity))
 
 
 def substitute_objects(obj,
                        index,
                        *,
                        inplace: bool = False):
     """
@@ -333,15 +337,15 @@
     if inplace:
         method = _substitute_inplace
     else:
         method = _substitute
 
     return method(obj,
                   sub=lambda l: index.get(l, l),
-                  applies=lambda o: _cached_isinstance(o, LinkByUID))
+                  applies=lambda o: cached_isinstance(o, LinkByUID))
 
 
 def flatten(obj, scope=None) -> List[BaseEntity]:
     """
     Flatten a BaseEntity (or array of them) into a list of objects connected by LinkByUID objects.
 
     This is a composite operation the amounts to:
@@ -379,15 +383,15 @@
         nonlocal known_uids
         to_return = []
         # get all the uids of this object
         uids = list(base_obj.uids.items())
         if len(uids) == 0:
             raise ValueError(f"No UID for {base_obj}; pass `flatten` a `scope` to set one")
 
-        # if none of the uids are known, then its a new object and we should return it
+        # if none of the uids are known, then it's a new object and we should return it
         if not any(uid in known_uids for uid in uids):
             to_return = [base_obj]
 
         # add all of the uids of this object into the known uid list
         for uid in uids:
             known_uids.add(uid)
 
@@ -429,29 +433,29 @@
         this = queue.pop()
         if this.__hash__ is not None:
             if this in seen:
                 continue
             else:
                 seen.add(this)
 
-        if apply_first and _cached_isinstance(this, BaseEntity):
+        if apply_first and cached_isinstance(this, BaseEntity):
             func(this)
 
-        if _cached_isinstance(this, Mapping):
+        if cached_isinstance(this, Mapping):
             for x in concatv(this.keys(), this.values()):
                 queue.append(x)
-        elif _cached_isinstance(this, DictSerializable):
+        elif cached_isinstance(this, DictSerializable):
             for k, x in this.__dict__.items():
                 queue.append(x)
-        elif _cached_isinstance(this, Iterable) \
-                and not _cached_isinstance(this, (str, ByteString)):
+        elif cached_isinstance(this, Iterable) \
+                and not cached_isinstance(this, (str, ByteString)):
             for x in this:
                 queue.append(x)
 
-        if not apply_first and _cached_isinstance(this, BaseEntity):
+        if not apply_first and cached_isinstance(this, BaseEntity):
             func(this)
 
     return
 
 
 def recursive_flatmap(obj: Union[Iterable, BaseEntity, DictSerializable],
                       func: Callable[[BaseEntity], Iterable],
@@ -484,43 +488,43 @@
 
         if this.__hash__ is not None:
             if this in seen:
                 continue
             else:
                 seen.add(this)
 
-        if _cached_isinstance(this, BaseEntity):
+        if cached_isinstance(this, BaseEntity):
             res.extend(func(this))
 
-        if _cached_isinstance(this, Mapping):
+        if cached_isinstance(this, Mapping):
             queue.extend(concatv(this.keys(), this.values()))
-        elif _cached_isinstance(this, DictSerializable):
+        elif cached_isinstance(this, DictSerializable):
             for k, x in sorted(this.__dict__.items()):
-                if unidirectional and _cached_isinstance(this, BaseEntity) and k in this.skip:
+                if unidirectional and cached_isinstance(this, BaseEntity) and k in this.skip:
                     continue
                 queue.append(x)
-        elif _cached_isinstance(this, Reversible):
+        elif cached_isinstance(this, Reversible):
             queue.extend(reversed(this))  # Preserve order of the list/tuple
-        elif _cached_isinstance(this, Iterable) \
-                and not _cached_isinstance(this, (str, ByteString)):
+        elif cached_isinstance(this, Iterable) \
+                and not cached_isinstance(this, (str, ByteString)):
             queue.extend(this)  # No control over order
 
     return res
 
 
 def writable_sort_order(key: Union[BaseEntity, str]) -> int:
     """Sort order for flattening such that the objects can be read back and re-nested."""
     from gemd.entity.object import MeasurementSpec, ProcessSpec, MaterialSpec, IngredientSpec, \
         MeasurementRun, IngredientRun, MaterialRun, ProcessRun
     from gemd.entity.template import ConditionTemplate, MaterialTemplate, MeasurementTemplate, \
         ParameterTemplate, ProcessTemplate, PropertyTemplate
 
-    if _cached_isinstance(key, BaseEntity):
+    if cached_isinstance(key, BaseEntity):
         typ = key.typ
-    elif _cached_isinstance(key, str):
+    elif cached_isinstance(key, str):
         typ = key
     else:
         raise ValueError("Can ony sort BaseEntities and type strings, not {}".format(key))
 
     if typ in [ConditionTemplate.typ, ParameterTemplate.typ, PropertyTemplate.typ]:
         return 0
     if typ in [MaterialTemplate.typ, ProcessTemplate.typ, MeasurementTemplate.typ]:
```

### Comparing `gemd-1.8.1/gemd.egg-info/PKG-INFO` & `gemd-1.9.0/gemd.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: gemd
-Version: 1.8.1
+Version: 1.9.0
 Summary: Python binding for Citrine's GEMD data model
 Home-page: http://github.com/CitrineInformatics/gemd-python
 Author: Citrine Informatics
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: tests
+Provides-Extra: gemd.demo.tests
+Provides-Extra: gemd.entity.bounds.tests
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `gemd-1.8.1/gemd.egg-info/SOURCES.txt` & `gemd-1.9.0/gemd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemd-1.8.1/setup.py` & `gemd-1.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 
 setup(name='gemd',
-      version='1.8.1',
+      version='1.9.0',
       url='http://github.com/CitrineInformatics/gemd-python',
       description="Python binding for Citrine's GEMD data model",
       author='Citrine Informatics',
       packages=find_packages(),
       package_data={
           'gemd': [
               'demo/strehlow_and_cook.pif',
@@ -21,14 +21,20 @@
           "toolz>=0.10.0,<1",
           "pint>=0.10,<1",
           "deprecation>=2.0.7,<3"
       ],
       extras_require={
           "tests": [
               "pytest>=6.2.5,<7"
+          ],
+          "gemd.demo.tests": [
+              "pandas>=1.1.5,<2"
+          ],
+          "gemd.entity.bounds.tests": [
+              "numpy"
           ]
       },
       classifiers=[
           'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
```

