# Comparing `tmp/aevmod-1.0.0.tar.gz` & `tmp/aevmod-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aevmod-1.0.0.tar", last modified: Thu Mar 14 15:49:52 2024, max compression
+gzip compressed data, was "aevmod-1.0.1.tar", last modified: Mon Apr 15 22:28:25 2024, max compression
```

## Comparing `aevmod-1.0.0.tar` & `aevmod-1.0.1.tar`

### file list

```diff
@@ -1,146 +1,143 @@
-drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-03-14 15:49:52.792854 aevmod-1.0.0/
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       49 2024-03-06 22:51:41.000000 aevmod-1.0.0/AUTHORS
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1342 2024-03-06 22:51:41.000000 aevmod-1.0.0/LICENSE
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      131 2024-03-13 20:37:55.000000 aevmod-1.0.0/MANIFEST.in
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     5413 2024-03-14 15:49:52.791971 aevmod-1.0.0/PKG-INFO
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3313 2024-03-06 22:51:41.000000 aevmod-1.0.0/README.rst
-drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-03-14 15:49:52.022865 aevmod-1.0.0/doc/
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     6148 2024-03-13 20:29:34.000000 aevmod-1.0.0/doc/.DS_Store
-drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-03-14 15:49:52.033741 aevmod-1.0.0/doc/report/
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)  1158508 2024-03-06 22:51:41.000000 aevmod-1.0.0/doc/report/report.pdf
-drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-03-14 15:49:52.045136 aevmod-1.0.0/examples/
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3490 2024-03-06 22:51:41.000000 aevmod-1.0.0/examples/taev.py
-drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-03-14 15:49:52.060393 aevmod-1.0.0/include/
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     6148 2024-03-13 20:35:58.000000 aevmod-1.0.0/include/.DS_Store
-drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-03-14 15:49:52.324814 aevmod-1.0.0/include/sac/
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2268 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2113 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Base.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3129 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_ConfigDefs.h
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2405 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_DisableKokkosCuda.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    24548 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_DynamicArrayTraits.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1859 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_DFad.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7296 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_DFadTraits.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    10972 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_DFad_tmpl.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7125 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_DynamicStorage.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     5403 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_Expression.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2409 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_ExpressionFwd.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3304 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_ExpressionTraits.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    19376 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_GeneralFad.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3975 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_GeneralFadExpr.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4965 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_GeneralFadTestingHelpers.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)   109352 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_Ops.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4857 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_Ops_Fwd.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    15235 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_SFad.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     8059 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_SFadTraits.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    10935 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_SFad_tmpl.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1877 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_SLFad.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7072 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_SLFadTraits.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    11604 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_SLFad_tmpl.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     8218 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_ScalarTraitsImp.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    16619 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_SerializationTraitsImp.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     6152 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_StaticStorage.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1949 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_ViewFad.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     5754 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_ViewFadTraits.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    11290 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_ViewFad_tmpl.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     6985 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Fad_ViewStorage.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    32867 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_MathFunctions.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     5560 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_SFINAE_Macros.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2801 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_StaticArrayTraits.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    23297 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Traits.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1505 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_Version.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3025 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_cmath.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2673 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_config.h
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1816 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/Sacado_dummy_arg.hpp
-drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-03-14 15:49:52.432221 aevmod-1.0.0/include/sac/exptl/
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1643 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_DFad.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1659 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_DVFad.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     8637 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_DynamicStorage.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    11072 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_ExprAssign.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4138 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_Expression.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3226 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_ExpressionTraits.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1813 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_Extender.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    11874 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_GeneralFad.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7893 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_GeneralFadTraits.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7321 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_MathFunctions.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    95392 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_Ops.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4376 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_Ops_Fwd.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1667 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_SFad.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1658 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_SLFad.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7983 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_StaticFixedStorage.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7545 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_StaticStorage.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     9865 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_VectorDynamicStorage.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     5185 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_ViewFad.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     8859 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_ViewStorage.hpp
-drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-03-14 15:49:52.609341 aevmod-1.0.0/include/sac/mpl/
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2554 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_apply.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3686 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_apply_wrap.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1576 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_at.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1572 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_begin.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7326 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_bind.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1469 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_deref.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1982 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_disable_if.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1969 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_enable_if.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1560 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_end.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2336 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_find.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2821 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_for_each.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1792 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_has_equal_to.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2032 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_has_type.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1760 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_if.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1732 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_integral_c.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2078 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_integral_nonzero_constant.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2638 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_is_convertible.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3409 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_is_placeholder.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1597 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_is_same.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4086 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_lambda.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1461 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_next.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1475 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_none.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3063 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_placeholders.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1613 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_push_back.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4306 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_quote.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3264 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_range_c.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1566 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_size.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2229 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_type_wrap.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3425 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_vector.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1786 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_vector_at_spec.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1631 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_vector_push_back_spec.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1534 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_vector_size_spec.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1540 2024-03-06 22:51:41.000000 aevmod-1.0.0/include/sac/mpl/Sacado_mpl_void.hpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1061 2024-03-14 14:24:34.000000 aevmod-1.0.0/pyproject.toml
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       38 2024-03-14 15:49:52.793053 aevmod-1.0.0/setup.cfg
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3787 2024-03-06 22:51:41.000000 aevmod-1.0.0/setup.py
-drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-03-14 15:49:52.683701 aevmod-1.0.0/src/
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     6148 2024-03-13 20:37:06.000000 aevmod-1.0.0/src/.DS_Store
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     6468 2024-03-06 22:51:41.000000 aevmod-1.0.0/src/aev.cpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4163 2024-03-06 22:51:41.000000 aevmod-1.0.0/src/aev.h
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2735 2024-03-06 22:51:41.000000 aevmod-1.0.0/src/aevmod.cpp
-drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-03-14 15:49:52.699879 aevmod-1.0.0/src/aevmod.egg-info/
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     5413 2024-03-14 15:49:51.000000 aevmod-1.0.0/src/aevmod.egg-info/PKG-INFO
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4765 2024-03-14 15:49:51.000000 aevmod-1.0.0/src/aevmod.egg-info/SOURCES.txt
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        1 2024-03-14 15:49:51.000000 aevmod-1.0.0/src/aevmod.egg-info/dependency_links.txt
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        1 2024-03-07 16:45:50.000000 aevmod-1.0.0/src/aevmod.egg-info/not-zip-safe
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       14 2024-03-14 15:49:51.000000 aevmod-1.0.0/src/aevmod.egg-info/requires.txt
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        7 2024-03-14 15:49:51.000000 aevmod-1.0.0/src/aevmod.egg-info/top_level.txt
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2893 2024-03-06 22:51:41.000000 aevmod-1.0.0/src/bld_index_sets.cpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4432 2024-03-06 22:51:41.000000 aevmod-1.0.0/src/config.cpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2227 2024-03-06 22:51:41.000000 aevmod-1.0.0/src/config.h
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    21531 2024-03-06 22:51:41.000000 aevmod-1.0.0/src/eval.cpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1504 2024-03-06 22:51:41.000000 aevmod-1.0.0/src/isEqual.h
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    18958 2024-03-06 22:51:41.000000 aevmod-1.0.0/src/sac_eval.cpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1914 2024-03-06 22:56:12.000000 aevmod-1.0.0/src/to_2d.h
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4608 2024-03-06 22:51:41.000000 aevmod-1.0.0/src/util.cpp
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2027 2024-03-06 22:51:41.000000 aevmod-1.0.0/src/util.h
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2485 2024-03-06 22:51:41.000000 aevmod-1.0.0/src/vio.h
-drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-03-14 15:49:52.790631 aevmod-1.0.0/tests/
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    10311 2024-03-12 23:16:13.000000 aevmod-1.0.0/tests/aev_c2h5_8_4_4.txt
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       87 2024-03-12 23:16:13.000000 aevmod-1.0.0/tests/ais_c2h5_8_4_4.txt
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)  4582095 2024-03-12 23:16:13.000000 aevmod-1.0.0/tests/hes_c2h5_8_4_4.txt
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)   219435 2024-03-12 23:16:13.000000 aevmod-1.0.0/tests/jac_c2h5_8_4_4.txt
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       16 2024-03-12 23:16:13.000000 aevmod-1.0.0/tests/ris_c2h5_8_4_4.txt
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2199 2024-03-12 23:16:13.000000 aevmod-1.0.0/tests/test_aev.py
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1398 2024-03-12 23:16:13.000000 aevmod-1.0.0/tests/test_ang_indsets.py
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1913 2024-03-12 23:16:13.000000 aevmod-1.0.0/tests/test_hes.py
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1867 2024-03-12 23:16:13.000000 aevmod-1.0.0/tests/test_jac.py
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1397 2024-03-12 23:16:13.000000 aevmod-1.0.0/tests/test_rad_indsets.py
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1406 2024-03-12 23:16:13.000000 aevmod-1.0.0/tests/test_structures.py
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7280 2024-03-12 23:16:13.000000 aevmod-1.0.0/tests/utils.py
--rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      301 2024-03-12 23:16:13.000000 aevmod-1.0.0/tests/xyz_c2h5.txt
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-04-15 22:28:25.900321 aevmod-1.0.1/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       49 2024-04-15 21:12:10.000000 aevmod-1.0.1/AUTHORS
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1342 2024-04-15 21:12:10.000000 aevmod-1.0.1/LICENSE
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      131 2024-04-15 22:23:31.000000 aevmod-1.0.1/MANIFEST.in
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     5442 2024-04-15 22:28:25.898987 aevmod-1.0.1/PKG-INFO
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3313 2024-04-15 21:12:10.000000 aevmod-1.0.1/README.rst
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-04-15 22:28:25.634890 aevmod-1.0.1/doc/
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-04-15 22:28:25.647122 aevmod-1.0.1/doc/report/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)  1158508 2024-04-15 21:12:10.000000 aevmod-1.0.1/doc/report/report.pdf
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-04-15 22:28:25.653219 aevmod-1.0.1/examples/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3561 2024-04-15 21:12:10.000000 aevmod-1.0.1/examples/taev.py
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-04-15 22:28:25.637006 aevmod-1.0.1/include/
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-04-15 22:28:25.712257 aevmod-1.0.1/include/sac/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2268 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2113 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Base.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3129 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_ConfigDefs.h
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2405 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_DisableKokkosCuda.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    24548 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_DynamicArrayTraits.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1859 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_DFad.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7296 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_DFadTraits.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    10972 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_DFad_tmpl.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7125 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_DynamicStorage.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     5403 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_Expression.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2409 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_ExpressionFwd.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3304 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_ExpressionTraits.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    19376 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_GeneralFad.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3975 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_GeneralFadExpr.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4965 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_GeneralFadTestingHelpers.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)   109352 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_Ops.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4857 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_Ops_Fwd.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    15235 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_SFad.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     8059 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_SFadTraits.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    10935 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_SFad_tmpl.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1877 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_SLFad.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7072 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_SLFadTraits.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    11604 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_SLFad_tmpl.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     8218 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_ScalarTraitsImp.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    16619 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_SerializationTraitsImp.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     6152 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_StaticStorage.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1949 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_ViewFad.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     5754 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_ViewFadTraits.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    11290 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_ViewFad_tmpl.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     6985 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Fad_ViewStorage.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    32867 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_MathFunctions.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     5560 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_SFINAE_Macros.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2801 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_StaticArrayTraits.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    23297 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Traits.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1505 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_Version.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3025 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_cmath.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2673 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_config.h
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1816 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/Sacado_dummy_arg.hpp
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-04-15 22:28:25.766978 aevmod-1.0.1/include/sac/exptl/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1643 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_DFad.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1659 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_DVFad.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     8637 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_DynamicStorage.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    11072 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_ExprAssign.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4138 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_Expression.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3226 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_ExpressionTraits.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1813 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_Extender.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    11874 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_GeneralFad.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7893 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_GeneralFadTraits.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7321 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_MathFunctions.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    95392 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_Ops.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4376 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_Ops_Fwd.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1667 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_SFad.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1658 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_SLFad.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7983 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_StaticFixedStorage.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7545 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_StaticStorage.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     9865 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_VectorDynamicStorage.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     5185 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_ViewFad.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     8859 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_ViewStorage.hpp
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-04-15 22:28:25.832374 aevmod-1.0.1/include/sac/mpl/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2554 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_apply.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3686 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_apply_wrap.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1576 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_at.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1572 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_begin.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7326 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_bind.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1469 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_deref.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1982 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_disable_if.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1969 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_enable_if.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1560 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_end.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2336 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_find.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2821 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_for_each.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1792 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_has_equal_to.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2032 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_has_type.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1760 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_if.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1732 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_integral_c.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2078 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_integral_nonzero_constant.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2638 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_is_convertible.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3409 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_is_placeholder.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1597 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_is_same.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4086 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_lambda.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1461 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_next.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1475 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_none.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3063 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_placeholders.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1613 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_push_back.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4306 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_quote.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3264 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_range_c.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1566 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_size.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2229 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_type_wrap.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3425 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_vector.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1786 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_vector_at_spec.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1631 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_vector_push_back_spec.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1534 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_vector_size_spec.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1540 2024-04-15 21:12:10.000000 aevmod-1.0.1/include/sac/mpl/Sacado_mpl_void.hpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1061 2024-04-15 22:26:00.000000 aevmod-1.0.1/pyproject.toml
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       38 2024-04-15 22:28:25.900483 aevmod-1.0.1/setup.cfg
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3787 2024-04-15 21:12:10.000000 aevmod-1.0.1/setup.py
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-04-15 22:28:25.850901 aevmod-1.0.1/src/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     6511 2024-04-15 21:12:10.000000 aevmod-1.0.1/src/aev.cpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4204 2024-04-15 21:12:10.000000 aevmod-1.0.1/src/aev.h
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2782 2024-04-15 21:12:10.000000 aevmod-1.0.1/src/aevmod.cpp
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-04-15 22:28:25.897833 aevmod-1.0.1/src/aevmod.egg-info/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     5442 2024-04-15 22:28:25.000000 aevmod-1.0.1/src/aevmod.egg-info/PKG-INFO
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4691 2024-04-15 22:28:25.000000 aevmod-1.0.1/src/aevmod.egg-info/SOURCES.txt
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        1 2024-04-15 22:28:25.000000 aevmod-1.0.1/src/aevmod.egg-info/dependency_links.txt
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        1 2024-04-15 22:28:25.000000 aevmod-1.0.1/src/aevmod.egg-info/not-zip-safe
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       14 2024-04-15 22:28:25.000000 aevmod-1.0.1/src/aevmod.egg-info/requires.txt
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        7 2024-04-15 22:28:25.000000 aevmod-1.0.1/src/aevmod.egg-info/top_level.txt
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2895 2024-04-15 21:12:10.000000 aevmod-1.0.1/src/bld_index_sets.cpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4435 2024-04-15 21:12:10.000000 aevmod-1.0.1/src/config.cpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2230 2024-04-15 21:12:10.000000 aevmod-1.0.1/src/config.h
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    22054 2024-04-15 21:12:10.000000 aevmod-1.0.1/src/eval.cpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1507 2024-04-15 21:12:10.000000 aevmod-1.0.1/src/isEqual.h
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    19146 2024-04-15 21:12:10.000000 aevmod-1.0.1/src/sac_eval.cpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1916 2024-04-15 21:12:10.000000 aevmod-1.0.1/src/to_2d.h
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4610 2024-04-15 21:12:10.000000 aevmod-1.0.1/src/util.cpp
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2030 2024-04-15 21:12:10.000000 aevmod-1.0.1/src/util.h
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2488 2024-04-15 21:12:10.000000 aevmod-1.0.1/src/vio.h
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2024-04-15 22:28:25.896006 aevmod-1.0.1/tests/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    10311 2024-04-15 21:12:10.000000 aevmod-1.0.1/tests/aev_c2h5_8_4_4.txt
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       87 2024-04-15 21:12:10.000000 aevmod-1.0.1/tests/ais_c2h5_8_4_4.txt
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)  4582095 2024-04-15 21:12:10.000000 aevmod-1.0.1/tests/hes_c2h5_8_4_4.txt
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)   219435 2024-04-15 21:12:10.000000 aevmod-1.0.1/tests/jac_c2h5_8_4_4.txt
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       16 2024-04-15 21:12:10.000000 aevmod-1.0.1/tests/ris_c2h5_8_4_4.txt
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2201 2024-04-15 21:12:10.000000 aevmod-1.0.1/tests/test_aev.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1400 2024-04-15 21:12:10.000000 aevmod-1.0.1/tests/test_ang_indsets.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1915 2024-04-15 21:12:10.000000 aevmod-1.0.1/tests/test_hes.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1869 2024-04-15 21:12:10.000000 aevmod-1.0.1/tests/test_jac.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1399 2024-04-15 21:12:10.000000 aevmod-1.0.1/tests/test_rad_indsets.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1408 2024-04-15 21:12:10.000000 aevmod-1.0.1/tests/test_structures.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7282 2024-04-15 21:12:10.000000 aevmod-1.0.1/tests/utils.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      301 2024-04-15 21:12:10.000000 aevmod-1.0.1/tests/xyz_c2h5.txt
```

### Comparing `aevmod-1.0.0/LICENSE` & `aevmod-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/PKG-INFO` & `aevmod-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aevmod
-Version: 1.0.0
+Version: 1.0.1
 Summary: Compute atomic environment vector (AEV) and its derivatives
 Author: Habib Najm
 Author-email: Habib N Najm <hnnajm@sandia.gov>, Christian J Devereux <cjdever@sandia.gov>, Carles Martí <cmartia@sandia.gov>
 Maintainer-email: Carles Martí <cmartia@sandia.gov>, Habib N Najm <hnnajm@sandia.gov>, Christian J Devereux <cjdever@sandia.gov>
 License: BSD 2-Clause License
         
         Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS).
@@ -19,14 +19,15 @@
         
 Project-URL: homepage, https://github.com/sandialabs/aevmod/
 Project-URL: documentation, https://github.com/sandialabs/aevmod/?tab=readme-ov-file#aevmod-package
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: numpy>=1.17.0
 
 aevmod package
 ================
 This package provides functionality for computing an atomic environment vector (AEV), as well as its Jacobian and Hessian. The AEV is a feature vector that is useful for representing the geometry of a molecule, or simply a set of atoms, in a manner that satisfies rotational and translational invariances. For the *i*-th atom in the system, its AEV is :math:`y_i=f_i(x)`, where *x* is a vector of Cartesian coordinates of all atoms in the set. The Jacobian and Hessian are with respect to the :math:`x` coordinates. Ther package uses `pybind11 <http://pybind11.readthedocs.io/en/stable/>`_ to expose our C++ AEV library to Python, as a python package ``aevmod``.  The package folder includes:
 
 * this README file, which can be viewed in a web browser using `restview <https://pypi.python.org/pypi/restview>`_. You can use
```

### Comparing `aevmod-1.0.0/README.rst` & `aevmod-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/doc/report/report.pdf` & `aevmod-1.0.1/doc/report/report.pdf`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/examples/taev.py` & `aevmod-1.0.1/examples/taev.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
 
@@ -28,15 +28,16 @@
 
 # define AEV structure object
 nrho_rad = 32  # number of radial aev radial shells
 nrho_ang = 8   # number of angular aev radial shells
 nalpha   = 8   # number of angular aev angular sectors dividing [0,pi]
 R_c_rad  = 4.6 # radial aev cutoff radius (Angstroms)
 R_c_ang  = 3.1 # angular aev cutoff radius (Angstroms)
-myaev    = aevmod.aev(types, nrho_rad, nrho_ang, nalpha, [R_c_rad,R_c_ang])
+beta     = 0.95 # special AEV factor for near-linear molecules
+myaev    = aevmod.aev(types, nrho_rad, nrho_ang, nalpha, [R_c_rad,R_c_ang], beta)
 print("built aev object, AEV size:",myaev.dout)
 
 # define CH2 molecule symbol list
 symb  = ['C','H','H']
 print("configuration:",symb)
 
 # define CH2 molecule object
```

### Comparing `aevmod-1.0.0/include/sac/Sacado.hpp` & `aevmod-1.0.1/include/sac/Sacado.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Base.hpp` & `aevmod-1.0.1/include/sac/Sacado_Base.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_ConfigDefs.h` & `aevmod-1.0.1/include/sac/Sacado_ConfigDefs.h`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_DisableKokkosCuda.hpp` & `aevmod-1.0.1/include/sac/Sacado_DisableKokkosCuda.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_DynamicArrayTraits.hpp` & `aevmod-1.0.1/include/sac/Sacado_DynamicArrayTraits.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_DFad.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_DFad.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_DFadTraits.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_DFadTraits.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_DFad_tmpl.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_DFad_tmpl.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_DynamicStorage.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_DynamicStorage.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_Expression.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_Expression.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_ExpressionFwd.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_ExpressionFwd.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_ExpressionTraits.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_ExpressionTraits.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_GeneralFad.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_GeneralFad.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_GeneralFadExpr.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_GeneralFadExpr.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_GeneralFadTestingHelpers.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_GeneralFadTestingHelpers.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_Ops.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_Ops.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_Ops_Fwd.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_Ops_Fwd.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_SFad.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_SFad.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_SFadTraits.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_SFadTraits.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_SFad_tmpl.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_SFad_tmpl.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_SLFad.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_SLFad.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_SLFadTraits.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_SLFadTraits.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_SLFad_tmpl.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_SLFad_tmpl.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_ScalarTraitsImp.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_ScalarTraitsImp.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_SerializationTraitsImp.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_SerializationTraitsImp.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_StaticStorage.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_StaticStorage.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_ViewFad.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_ViewFad.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_ViewFadTraits.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_ViewFadTraits.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_ViewFad_tmpl.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_ViewFad_tmpl.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Fad_ViewStorage.hpp` & `aevmod-1.0.1/include/sac/Sacado_Fad_ViewStorage.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_MathFunctions.hpp` & `aevmod-1.0.1/include/sac/Sacado_MathFunctions.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_SFINAE_Macros.hpp` & `aevmod-1.0.1/include/sac/Sacado_SFINAE_Macros.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_StaticArrayTraits.hpp` & `aevmod-1.0.1/include/sac/Sacado_StaticArrayTraits.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Traits.hpp` & `aevmod-1.0.1/include/sac/Sacado_Traits.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_Version.hpp` & `aevmod-1.0.1/include/sac/Sacado_Version.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_cmath.hpp` & `aevmod-1.0.1/include/sac/Sacado_cmath.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_config.h` & `aevmod-1.0.1/include/sac/Sacado_config.h`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/Sacado_dummy_arg.hpp` & `aevmod-1.0.1/include/sac/Sacado_dummy_arg.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_DFad.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_DFad.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_DVFad.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_DVFad.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_DynamicStorage.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_DynamicStorage.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_ExprAssign.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_ExprAssign.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_Expression.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_Expression.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_ExpressionTraits.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_ExpressionTraits.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_Extender.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_Extender.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_GeneralFad.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_GeneralFad.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_GeneralFadTraits.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_GeneralFadTraits.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_MathFunctions.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_MathFunctions.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_Ops.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_Ops.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_Ops_Fwd.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_Ops_Fwd.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_SFad.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_SFad.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_SLFad.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_SLFad.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_StaticFixedStorage.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_StaticFixedStorage.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_StaticStorage.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_StaticStorage.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_VectorDynamicStorage.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_VectorDynamicStorage.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_ViewFad.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_ViewFad.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/exptl/Sacado_Fad_Exp_ViewStorage.hpp` & `aevmod-1.0.1/include/sac/exptl/Sacado_Fad_Exp_ViewStorage.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_apply.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_apply.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_apply_wrap.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_apply_wrap.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_at.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_at.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_begin.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_begin.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_bind.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_bind.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_deref.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_deref.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_disable_if.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_disable_if.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_enable_if.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_enable_if.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_end.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_end.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_find.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_find.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_for_each.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_for_each.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_has_equal_to.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_has_equal_to.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_has_type.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_has_type.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_if.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_if.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_integral_c.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_integral_c.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_integral_nonzero_constant.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_integral_nonzero_constant.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_is_convertible.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_is_convertible.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_is_placeholder.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_is_placeholder.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_is_same.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_is_same.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_lambda.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_lambda.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_next.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_next.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_none.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_none.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_placeholders.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_placeholders.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_push_back.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_push_back.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_quote.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_quote.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_range_c.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_range_c.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_size.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_size.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_type_wrap.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_type_wrap.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_vector.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_vector.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_vector_at_spec.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_vector_at_spec.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_vector_push_back_spec.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_vector_push_back_spec.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_vector_size_spec.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_vector_size_spec.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/include/sac/mpl/Sacado_mpl_void.hpp` & `aevmod-1.0.1/include/sac/mpl/Sacado_mpl_void.hpp`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/pyproject.toml` & `aevmod-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel", "pybind11"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aevmod"
-version = "1.0.0"
+version = "1.0.1"
 description = "Compute atomic environment vector (AEV) and its derivatives"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 # keywords = []
 authors = [
     {name="Habib N Najm", email="hnnajm@sandia.gov"},
```

### Comparing `aevmod-1.0.0/setup.py` & `aevmod-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         # import here, cause outside the eggs aren't loaded
         import pytest
         errno = pytest.main(self.pytest_args)
         sys.exit(errno)
 
 setup(
     name='aevmod',
-    version='1.0.0',
+    version='1.1.0',
     author='Habib Najm',
     author_email='hnnajm@sandia.gov',
     long_description=open('README.rst').read(),
     ext_modules=ext_modules,
     cmdclass={
         'build_ext': BuildExt,
         'test': PyTest,
```

### Comparing `aevmod-1.0.0/src/aev.cpp` & `aevmod-1.0.1/src/aev.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
 
@@ -41,18 +41,19 @@
 	rad_dout = rad_par.size() * n_rad;
 	ang_dout = ang_par.size() * n_ang;
 	aev_tag  = tag;
 	return;
 }
 //================================================================================
 aev::aev(const std::vector<std::string>& atom_types, const int& nrho_rad, 
-         const int& nrho_ang, const int& nalpha, const std::vector<double>& R_c_in) {
+         const int& nrho_ang, const int& nalpha, const std::vector<double>& R_c_in, const double& beta_in) {
 
 	types = atom_types;
 	R_c   = R_c_in;
+	beta  = beta_in;
 
 	// spec for radial SFs
 	double drho_rad  = R_c[0]/static_cast<double>(nrho_rad);
 	double delta_rad = (2./3.)*drho_rad;
 	double eta_rad   = 1.0/pow(delta_rad,2);    // a single eta
 	std::vector<double> rhov_rad = linspace(drho_rad/2.0,R_c[0]-drho_rad/2.0,nrho_rad);
 	std::vector<double> etav_rad = {eta_rad};
```

### Comparing `aevmod-1.0.0/src/aev.h` & `aevmod-1.0.1/src/aev.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
 
@@ -25,15 +25,15 @@
 //===============================================================
 class aev {
 
 //--------------------------------------------------------------------------------
 public:
 
   aev(const std::vector<std::string>& atom_types={"C","H"}, const int& nrho_rad=32, 
-      const int& nrho_ang=8, const int& nalpha=8, const std::vector<double>& R_c={4.6,3.1});
+      const int& nrho_ang=8, const int& nalpha=8, const std::vector<double>& R_c={4.6,3.1}, const double& beta=1.0);
 
   void build_index_sets(config& conf);
 
   void bld_index_sets(
     const std::vector<std::string>& symb, 
     std::vector<std::vector<int>>& rad_ind_set, 
     std::vector<std::vector<std::vector<int>>>& ang_ind_set);
@@ -89,13 +89,14 @@
   std::vector<std::vector<double>> ang_par;
   std::vector<std::string> types;
   std::vector<double> R_c;
 
   std::vector<std::string> rad_typ;
   std::vector<std::vector<std::string>> ang_typ;
   std::vector<std::string> tag;
+  double beta;
 
 //--------------------------------------------------------------------------------
 };
 
 //================================================================================
 #endif
```

### Comparing `aevmod-1.0.0/src/aevmod.cpp` & `aevmod-1.0.1/src/aevmod.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
 
@@ -41,21 +41,22 @@
 namespace py = pybind11;
 
 PYBIND11_MODULE(aevmod, m) {
 
     m.doc() = "pybind11 aev module";
 
     py::class_<aev>(m,"aev")
-    .def(py::init<const std::vector<std::string>&, const int&, const int&, const int&, const std::vector<double>&>()
+    .def(py::init<const std::vector<std::string>&, const int&, const int&, const int&, const std::vector<double>&, const double&>()
         ,
         py::arg("atom_types")=std::vector<std::string>({"C","H"}),
         py::arg("nrho_rad")=32,
         py::arg("nrho_ang")=8,
         py::arg("nalpha")=8,
-        py::arg("R_c_in")=std::vector<double>({4.6,3.1})
+        py::arg("R_c_in")=std::vector<double>({4.6,3.1}),
+        py::arg("beta")=1.0 
         )
     .def_readwrite("dout", &aev::dout)
     .def_readwrite("n_rad", &aev::n_rad)
     .def_readwrite("n_ang", &aev::n_ang)
     .def("build_index_sets",&aev::build_index_sets)
     .def("eval",&aev::eval)
     .def("eval_sac",&aev::eval_sac)
```

### Comparing `aevmod-1.0.0/src/aevmod.egg-info/PKG-INFO` & `aevmod-1.0.1/src/aevmod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aevmod
-Version: 1.0.0
+Version: 1.0.1
 Summary: Compute atomic environment vector (AEV) and its derivatives
 Author: Habib Najm
 Author-email: Habib N Najm <hnnajm@sandia.gov>, Christian J Devereux <cjdever@sandia.gov>, Carles Martí <cmartia@sandia.gov>
 Maintainer-email: Carles Martí <cmartia@sandia.gov>, Habib N Najm <hnnajm@sandia.gov>, Christian J Devereux <cjdever@sandia.gov>
 License: BSD 2-Clause License
         
         Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS).
@@ -19,14 +19,15 @@
         
 Project-URL: homepage, https://github.com/sandialabs/aevmod/
 Project-URL: documentation, https://github.com/sandialabs/aevmod/?tab=readme-ov-file#aevmod-package
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: numpy>=1.17.0
 
 aevmod package
 ================
 This package provides functionality for computing an atomic environment vector (AEV), as well as its Jacobian and Hessian. The AEV is a feature vector that is useful for representing the geometry of a molecule, or simply a set of atoms, in a manner that satisfies rotational and translational invariances. For the *i*-th atom in the system, its AEV is :math:`y_i=f_i(x)`, where *x* is a vector of Cartesian coordinates of all atoms in the set. The Jacobian and Hessian are with respect to the :math:`x` coordinates. Ther package uses `pybind11 <http://pybind11.readthedocs.io/en/stable/>`_ to expose our C++ AEV library to Python, as a python package ``aevmod``.  The package folder includes:
 
 * this README file, which can be viewed in a web browser using `restview <https://pypi.python.org/pypi/restview>`_. You can use
```

### Comparing `aevmod-1.0.0/src/aevmod.egg-info/SOURCES.txt` & `aevmod-1.0.1/src/aevmod.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.py
-/Users/cmartia/tmp/aevmod/src/aev.cpp
-/Users/cmartia/tmp/aevmod/src/aevmod.cpp
-/Users/cmartia/tmp/aevmod/src/bld_index_sets.cpp
-/Users/cmartia/tmp/aevmod/src/config.cpp
-/Users/cmartia/tmp/aevmod/src/eval.cpp
-/Users/cmartia/tmp/aevmod/src/sac_eval.cpp
-/Users/cmartia/tmp/aevmod/src/util.cpp
-doc/.DS_Store
+/Users/cmartia/aevmod/src/aev.cpp
+/Users/cmartia/aevmod/src/aevmod.cpp
+/Users/cmartia/aevmod/src/bld_index_sets.cpp
+/Users/cmartia/aevmod/src/config.cpp
+/Users/cmartia/aevmod/src/eval.cpp
+/Users/cmartia/aevmod/src/sac_eval.cpp
+/Users/cmartia/aevmod/src/util.cpp
 doc/report/report.pdf
 examples/taev.py
-include/.DS_Store
 include/sac/Sacado.hpp
 include/sac/Sacado_Base.hpp
 include/sac/Sacado_ConfigDefs.h
 include/sac/Sacado_DisableKokkosCuda.hpp
 include/sac/Sacado_DynamicArrayTraits.hpp
 include/sac/Sacado_Fad_DFad.hpp
 include/sac/Sacado_Fad_DFadTraits.hpp
@@ -101,15 +99,14 @@
 include/sac/mpl/Sacado_mpl_size.hpp
 include/sac/mpl/Sacado_mpl_type_wrap.hpp
 include/sac/mpl/Sacado_mpl_vector.hpp
 include/sac/mpl/Sacado_mpl_vector_at_spec.hpp
 include/sac/mpl/Sacado_mpl_vector_push_back_spec.hpp
 include/sac/mpl/Sacado_mpl_vector_size_spec.hpp
 include/sac/mpl/Sacado_mpl_void.hpp
-src/.DS_Store
 src/aev.cpp
 src/aev.h
 src/aevmod.cpp
 src/bld_index_sets.cpp
 src/config.cpp
 src/config.h
 src/eval.cpp
```

### Comparing `aevmod-1.0.0/src/bld_index_sets.cpp` & `aevmod-1.0.1/src/bld_index_sets.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
```

### Comparing `aevmod-1.0.0/src/config.cpp` & `aevmod-1.0.1/src/config.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
 
@@ -128,8 +128,8 @@
 }
 
 //================================================================================================
 std::vector<std::vector<std::vector<int>>> config::get_angular_index_set(){
 	return angular_index_set;	
 }
 
-//================================================================================
+//================================================================================
```

### Comparing `aevmod-1.0.0/src/config.h` & `aevmod-1.0.1/src/config.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
 
@@ -61,8 +61,8 @@
 
   friend class aev;
 
 //--------------------------------------------------------------------------------
 };
 
 
-#endif
+#endif
```

### Comparing `aevmod-1.0.0/src/eval.cpp` & `aevmod-1.0.1/src/eval.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
 
@@ -188,15 +188,16 @@
 					if (diagnose)
 						std::cout << "Working on atom #s j: " << j << ", k: " << k << std::endl;
 					std::vector<double> vij = vdiff(x[j],x[i]);	// x_j - x_i
 					std::vector<double> vik = vdiff(x[k],x[i]);	// x_k - x_i
 					double Rij = l2_length(vij);      // ||x_j-x_i||
 					double Rik = l2_length(vik);      // ||x_k-x_i||
 					double vdv = std::inner_product(vij.begin(), vij.end(), vik.begin(), 0.0);
-					double theta = acos( std::max(-1.0, std::min( vdv/(Rij*Rik), 1.0)) );   // angle theta
+					//double theta = acos( std::max(-1.0, std::min( vdv/(Rij*Rik), 1.0)) );   // angle theta
+					double theta = acos( std::max(-1.0, std::min( beta * (vdv/(Rij*Rik)), 1.0)) );   // angle theta with beta scale, e.g. 0.95
 					for (int l=0; l<nsf; ++l){	// loop over angular SFs
 						int q = q_offset + kknsf + l;
 						std::vector<double> par = ang_par[l];
 						y[p][i][q] += ang_kern(par,Rij,Rik,theta,R_c[1]);
 					  	if (diagnose) 
 						  std::cout << "p: " << p << ", i: " << i << ", atom: " << atom << ", pair: " << elmt1 << ", " << elmt2
 						            << ", j: " << j << ", k: " << k << ", q: " << q << ", y: " << y[p][i][q] << std::endl;
@@ -392,15 +393,16 @@
 						double oRij     = 1.0/Rij;
 						double dfcconj  = -0.5*pioRc*sin(Rij*pioRc)*oRij;
 
 						double oRik     = 1.0/Rik;
 						double dfcconk  = -0.5*pioRc*sin(Rik*pioRc)*oRik;
 
 						double vdv   = std::inner_product(vij.begin(), vij.end(), vik.begin(), 0.0);
-						double theta = acos( std::max(-1.0, std::min( vdv/(Rij*Rik), 1.0)) );   // angle theta
+						//double theta = acos( std::max(-1.0, std::min( vdv/(Rij*Rik), 1.0)) );   // angle theta
+						double theta = acos( std::max(-1.0, std::min( (beta*vdv/(Rij*Rik)), 1.0)) );   // angle theta with beta scale, e.g. 0.95
 
 						double costh = cos(theta);
 						double ctden = Rij * Rik * sin(theta);
 
 						double fcij  = fc(Rij,Rc);
 						double fcik  = fc(Rik,Rc);
 						double fcijk = fcij * fcik;
@@ -495,24 +497,30 @@
 						    //  inner atom index for Jac computations     t                            l 
 						    // 
 							// dout is the dimension of the AEV for any atom in the config
 							// jac(p,i,q,s): Jac for structure p=0,...,npt , atom i=0,...,N , AEV component q=0,...,dout ; xyz-coordinate s=0,1,2,....,din=3N
 						    // s = 0,1,2 , 3,4,5 , ...     being composed of N triplets indexed by t=0,1,...,
 
 							std::vector<double> dthetadi(3);
-							for (int kc=0; kc<3; ++kc)
-								dthetadi[kc] = ( - dxxdi[kc] + costh * dRRdi[kc] ) / ctden;
+							for (int kc=0; kc<3; ++kc){
+								//dthetadi[kc] = ( - dxxdi[kc] + costh * dRRdi[kc] ) / ctden;
+							  dthetadi[kc] = beta * ( - dxxdi[kc] + costh * dRRdi[kc] ) / ctden;
+							}
 
 							std::vector<double> dthetadj(3);
-							for (int kc=0; kc<3; ++kc)
-								dthetadj[kc] = ( - dxxdj[kc] + costh * dRRdj[kc] ) / ctden;
+							for (int kc=0; kc<3; ++kc){
+								//dthetadj[kc] = ( - dxxdj[kc] + costh * dRRdj[kc] ) / ctden;
+								dthetadj[kc] = beta * ( - dxxdj[kc] + costh * dRRdj[kc] ) / ctden;
+							}
 
 							std::vector<double> dthetadk(3);
-							for (int kc=0; kc<3; ++kc)
-								dthetadk[kc] = ( - dxxdk[kc] + costh * dRRdk[kc] ) / ctden;
+							for (int kc=0; kc<3; ++kc){
+								//dthetadk[kc] = ( - dxxdk[kc] + costh * dRRdk[kc] ) / ctden;
+								dthetadk[kc] = beta * ( - dxxdk[kc] + costh * dRRdk[kc] ) / ctden;
+							}
 
 							// t = i
 							int s = i*3;
 							for (int kc=0; kc<3; ++kc)
 								jac[p][i][q][s+kc] += ct1 * dthetadi[kc] + ct2 * (dRijdi[kc] + dRikdi[kc]) + 
 													  ct3 * dfcijdi[kc]  + ct4 * dfcikdi[kc];
```

### Comparing `aevmod-1.0.0/src/isEqual.h` & `aevmod-1.0.1/src/isEqual.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
 
@@ -31,8 +31,8 @@
 template<typename T>
 bool isEqual(const std::vector<T>& v1, const std::vector<T>& v2)
 {
     return (v1.size() == v2.size() &&
             std::equal(v1.begin(), v1.end(), v2.begin()));
 }
 //===============================================================================================
-#endif
+#endif
```

### Comparing `aevmod-1.0.0/src/sac_eval.cpp` & `aevmod-1.0.1/src/sac_eval.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
 
@@ -150,15 +150,16 @@
 					if (diagnose)
 						std::cout << "Working on atom #s j: " << j << ", k: " << k << std::endl;
 					std::vector<ValueType> vij = vdiff_sac(x[j],x[i]);	// x_j - x_i
 					std::vector<ValueType> vik = vdiff_sac(x[k],x[i]);	// x_k - x_i
 					ValueType Rij = l2_length_sac(vij);      // ||x_j-x_i||
 					ValueType Rik = l2_length_sac(vik);      // ||x_k-x_i||
 					ValueType vdv = std::inner_product(vij.begin(), vij.end(), vik.begin(), static_cast<ValueType>(0.0));
-					ValueType theta = acos( std::max(-static_cast<ValueType>(1.0), std::min( vdv/(Rij*Rik), static_cast<ValueType>(1.0))) );   // angle theta
+					//ValueType theta = acos( std::max(-static_cast<ValueType>(1.0), std::min( vdv/(Rij*Rik), static_cast<ValueType>(1.0))) );   // angle theta
+          ValueType theta = acos( std::max(-static_cast<ValueType>(1.0), std::min( beta * (vdv/(Rij*Rik)), static_cast<ValueType>(1.0))) );   // angle theta with beta scale, e.g. 0.95
 					for (int l=0; l<nsf && Rij <= R_c[1] && Rik <= R_c[1]; ++l){	// loop over angular SFs if Rij and Rik both <= R_c[1]
 						int q = q_offset + kknsf + l;
 						std::vector<double> par = ang_par[l];
 						y[q] += ang_kern_sac(par,Rij,Rik,theta,R_c[1]);
 					  	if (diagnose) 
 						  std::cout << "p: " << p << ", i: " << i << ", atom: " << atom << ", pair: " << elmt1 << ", " << elmt2
 						            << ", j: " << j << ", k: " << k << ", q: " << q << ", y: " << y[q] << std::endl;
```

### Comparing `aevmod-1.0.0/src/to_2d.h` & `aevmod-1.0.1/src/to_2d.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
```

### Comparing `aevmod-1.0.0/src/util.cpp` & `aevmod-1.0.1/src/util.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
```

### Comparing `aevmod-1.0.0/src/util.h` & `aevmod-1.0.1/src/util.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
 
@@ -33,8 +33,8 @@
 bool isEqual(const std::vector<T>& v1, const std::vector<T>& v2);
 #include "isEqual.h"
 //================================================================================
 template < typename T >
 std::vector< std::vector<T> > to_2d( const std::vector<T>& flat_vec, std::size_t ncols );
 #include "to_2d.h"
 //================================================================================
-#endif
+#endif
```

### Comparing `aevmod-1.0.0/src/vio.h` & `aevmod-1.0.1/src/vio.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
 
@@ -61,8 +61,8 @@
           os << *it << " ";
     }
     os << std::endl;
   }
   return os;
 }
 //===============================================================
-#endif
+#endif
```

### Comparing `aevmod-1.0.0/tests/aev_c2h5_8_4_4.txt` & `aevmod-1.0.1/tests/aev_c2h5_8_4_4.txt`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/tests/hes_c2h5_8_4_4.txt` & `aevmod-1.0.1/tests/hes_c2h5_8_4_4.txt`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/tests/jac_c2h5_8_4_4.txt` & `aevmod-1.0.1/tests/jac_c2h5_8_4_4.txt`

 * *Files identical despite different names*

### Comparing `aevmod-1.0.0/tests/test_aev.py` & `aevmod-1.0.1/tests/test_aev.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
```

### Comparing `aevmod-1.0.0/tests/test_ang_indsets.py` & `aevmod-1.0.1/tests/test_ang_indsets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
```

### Comparing `aevmod-1.0.0/tests/test_hes.py` & `aevmod-1.0.1/tests/test_hes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
```

### Comparing `aevmod-1.0.0/tests/test_jac.py` & `aevmod-1.0.1/tests/test_jac.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
```

### Comparing `aevmod-1.0.0/tests/test_rad_indsets.py` & `aevmod-1.0.1/tests/test_rad_indsets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
```

### Comparing `aevmod-1.0.0/tests/test_structures.py` & `aevmod-1.0.1/tests/test_structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
```

### Comparing `aevmod-1.0.0/tests/utils.py` & `aevmod-1.0.1/tests/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 =====================================================================================
-aevmod version 1.0
+aevmod version 1.1.0
 Copyright (2021) NTESS
 https://github.com/sandialabs/aevmod
 
 Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains 
 certain rights in this software.
```

