# Comparing `tmp/graas-observability-utility-1.6.1.tar.gz` & `tmp/graas-observability-utility-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graas-observability-utility-1.6.1.tar", last modified: Mon Apr  8 10:50:14 2024, max compression
+gzip compressed data, was "graas-observability-utility-1.6.2.tar", last modified: Tue Apr 16 09:02:07 2024, max compression
```

## Comparing `graas-observability-utility-1.6.1.tar` & `graas-observability-utility-1.6.2.tar`

### file list

```diff
@@ -1,82 +1,77 @@
-drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-04-08 10:50:14.465496 graas-observability-utility-1.6.1/
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       43 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/MANIFEST.in
--rw-r--r--   0 priyanka  (1003) priyanka  (1003)      856 2024-04-08 10:50:14.461496 graas-observability-utility-1.6.1/PKG-INFO
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      565 2023-11-02 10:15:21.000000 graas-observability-utility-1.6.1/README.md
-drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-04-08 10:50:14.345496 graas-observability-utility-1.6.1/graas_observability_utility.egg-info/
--rw-r--r--   0 priyanka  (1003) priyanka  (1003)      856 2024-04-08 10:50:14.000000 graas-observability-utility-1.6.1/graas_observability_utility.egg-info/PKG-INFO
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4831 2024-04-08 10:50:14.000000 graas-observability-utility-1.6.1/graas_observability_utility.egg-info/SOURCES.txt
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        1 2024-04-08 10:50:14.000000 graas-observability-utility-1.6.1/graas_observability_utility.egg-info/dependency_links.txt
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       11 2024-04-08 10:50:14.000000 graas-observability-utility-1.6.1/graas_observability_utility.egg-info/requires.txt
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       16 2024-04-08 10:50:14.000000 graas-observability-utility-1.6.1/graas_observability_utility.egg-info/top_level.txt
-drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-04-08 10:50:14.345496 graas-observability-utility-1.6.1/graas_utilities/
-drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-04-08 10:50:14.461496 graas-observability-utility-1.6.1/graas_utilities/Schema/
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2215 2024-04-08 10:45:24.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Product_Performance_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2438 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Sponsored_Brands_Attributed_Purchases_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5106 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Sponsored_Brands_Campaign_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5005 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Sponsored_Display_Advertised_Product_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3585 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Sponsored_Display_Campaign_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3548 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Sponsored_Products_Advertised_Product_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3482 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Sponsored_Products_Campaign_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      692 2024-04-08 10:45:24.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Store_Key_Metrics_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1166 2024-04-08 10:45:24.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Store_Key_Metrics_Hourly_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1561 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Traffic_Metrics_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2631 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Flipkart_PLA_Campaign_Seller_Portal_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2226 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Flipkart_PLA_Consolidated_FSN_seller_Portal_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2188 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Flipkart_Search_Traffic_Report_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1488 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Lazada_Customers_Insight_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3619 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Lazada_Keywords_Onsite_daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3038 2024-04-08 10:45:24.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Lazada_Product_Performance_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1694 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Lazada_Product_Sponsored_Affiliate_Report_Daily_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2610 2024-04-08 10:45:24.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Lazada_Store_Key_Metrics_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     9612 2024-04-02 10:30:41.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Lazada_mkp_onsite_campaign_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3866 2024-01-08 08:41:17.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Lazada_offsite_campaign_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4360 2024-04-08 10:46:12.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Lazada_onsite_campaign_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3833 2024-04-08 10:47:55.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Keywords_Onsite_daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3505 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Key_Metrics_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3208 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Trends_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1833 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_BundleDeal_Overview_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1229 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Bundle_Deal_Trends_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1628 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1251 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Trends_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2994 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Detailed_Overview_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1148 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Trends_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2001 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Voucher_Performance_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1095 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Voucher_Trends_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3371 2024-04-08 10:46:12.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Product_Overview_Daily_Monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3732 2024-04-08 10:46:12.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Product_Overview_Hourly_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3867 2024-04-08 10:46:12.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Product_Performance_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2479 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Store_Metrics_Paid_Orders_Daily_monthly_report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1429 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Traffic_Overview_Daily_Monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     8522 2024-04-05 10:52:26.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_mkp_onsite_campaign_daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5554 2024-04-08 10:46:12.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_onsite_campaign_daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3500 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_store_Metrics_Placed_Order_Hourly_Daily_report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1531 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1025 2024-04-08 10:45:24.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Tokopedia_Product_Overview_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1703 2024-04-08 10:45:24.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Tokopedia_Product_Performance_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4650 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Daily_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4115 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        0 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/__init__.py
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      577 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/amount_currency_code_object.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1785 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_amazon_campaigns.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1301 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_flipkart_campaigns.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1306 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_affiliate_report_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1794 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_deals_overview_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2318 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_deals_trends_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1294 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_offsite_campaigns.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1510 2024-04-08 10:45:24.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_onsite_campaigns.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1499 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_onsite_keywords.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2141 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_product_campaign_performance.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1997 2024-04-08 10:45:24.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_product_overview_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1546 2024-04-08 10:45:24.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_product_overview_hourly.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1990 2024-04-08 10:45:24.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_product_performance.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2700 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_shop_stats_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1554 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_shop_stats_hourly.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2454 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_traffic_overview_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1330 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_traffic_overview_hourly.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1851 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_voucher_performance_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        0 2023-11-27 05:46:40.000000 graas-observability-utility-1.6.1/graas_utilities/__init__.py
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5484 2024-04-08 10:45:24.000000 graas-observability-utility-1.6.1/graas_utilities/configs.py
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      751 2024-03-26 06:37:57.000000 graas-observability-utility-1.6.1/graas_utilities/ref_Resolver.py
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3592 2024-04-08 10:46:12.000000 graas-observability-utility-1.6.1/graas_utilities/validation.py
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       38 2024-04-08 10:50:14.465496 graas-observability-utility-1.6.1/setup.cfg
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1307 2024-04-08 10:49:05.000000 graas-observability-utility-1.6.1/setup.py
+drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-04-16 09:02:07.417538 graas-observability-utility-1.6.2/
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       43 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/MANIFEST.in
+-rw-r--r--   0 priyanka  (1003) priyanka  (1003)      856 2024-04-16 09:02:07.417538 graas-observability-utility-1.6.2/PKG-INFO
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      565 2023-11-02 10:15:21.000000 graas-observability-utility-1.6.2/README.md
+drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-04-16 09:02:07.293544 graas-observability-utility-1.6.2/graas_observability_utility.egg-info/
+-rw-r--r--   0 priyanka  (1003) priyanka  (1003)      856 2024-04-16 09:02:07.000000 graas-observability-utility-1.6.2/graas_observability_utility.egg-info/PKG-INFO
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4531 2024-04-16 09:02:07.000000 graas-observability-utility-1.6.2/graas_observability_utility.egg-info/SOURCES.txt
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        1 2024-04-16 09:02:07.000000 graas-observability-utility-1.6.2/graas_observability_utility.egg-info/dependency_links.txt
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       11 2024-04-16 09:02:07.000000 graas-observability-utility-1.6.2/graas_observability_utility.egg-info/requires.txt
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       16 2024-04-16 09:02:07.000000 graas-observability-utility-1.6.2/graas_observability_utility.egg-info/top_level.txt
+drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-04-16 09:02:07.293544 graas-observability-utility-1.6.2/graas_utilities/
+drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-04-16 09:02:07.417538 graas-observability-utility-1.6.2/graas_utilities/Schema/
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4031 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Product_Performance_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2438 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Sponsored_Brands_Attributed_Purchases_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5106 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Sponsored_Brands_Campaign_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5005 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Sponsored_Display_Advertised_Product_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3585 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Sponsored_Display_Campaign_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3548 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Sponsored_Products_Advertised_Product_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3482 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Sponsored_Products_Campaign_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1873 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Store_Key_Metrics_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2962 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Store_Key_Metrics_Hourly_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1561 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Traffic_Metrics_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2631 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Flipkart_PLA_Campaign_Seller_Portal_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2226 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Flipkart_PLA_Consolidated_FSN_seller_Portal_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2188 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Flipkart_Search_Traffic_Report_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1488 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Lazada_Customers_Insight_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3619 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Lazada_Keywords_Onsite_daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5752 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Lazada_Product_Performance_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1694 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Lazada_Product_Sponsored_Affiliate_Report_Daily_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5961 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Lazada_Store_Key_Metrics_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     9612 2024-04-02 10:30:41.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Lazada_mkp_onsite_campaign_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3866 2024-01-08 08:41:17.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Lazada_offsite_campaign_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4668 2024-04-16 08:59:10.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Lazada_onsite_campaign_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3926 2024-04-16 08:59:10.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Keywords_Onsite_daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3505 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Key_Metrics_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3208 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Trends_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1833 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_BundleDeal_Overview_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1229 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Bundle_Deal_Trends_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1628 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1251 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Trends_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2994 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Detailed_Overview_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1148 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Trends_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2001 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Voucher_Performance_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1095 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Voucher_Trends_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5893 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Product_Overview_Daily_Monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     6341 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Product_Overview_Hourly_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     6387 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Product_Performance_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2479 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Store_Metrics_Paid_Orders_Daily_monthly_report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1429 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Traffic_Overview_Daily_Monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     8522 2024-04-05 10:52:26.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_mkp_onsite_campaign_daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3500 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_store_Metrics_Placed_Order_Hourly_Daily_report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1531 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2362 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Tokopedia_Product_Overview_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3318 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Tokopedia_Product_Performance_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4650 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Daily_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4115 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        0 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/__init__.py
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      577 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/amount_currency_code_object.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1785 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/graas_amazon_campaigns.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1301 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/graas_flipkart_campaigns.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1306 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_affiliate_report_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1794 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_deals_overview_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2318 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_deals_trends_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1294 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_offsite_campaigns.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1499 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_onsite_keywords.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2141 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_product_campaign_performance.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2700 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_shop_stats_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1554 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_shop_stats_hourly.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2454 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_traffic_overview_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1330 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_traffic_overview_hourly.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1851 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_voucher_performance_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        0 2023-11-27 05:46:40.000000 graas-observability-utility-1.6.2/graas_utilities/__init__.py
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5651 2024-04-16 09:00:32.000000 graas-observability-utility-1.6.2/graas_utilities/configs.py
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      751 2024-03-26 06:37:57.000000 graas-observability-utility-1.6.2/graas_utilities/ref_Resolver.py
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3986 2024-04-16 09:01:59.000000 graas-observability-utility-1.6.2/graas_utilities/validation.py
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       38 2024-04-16 09:02:07.417538 graas-observability-utility-1.6.2/setup.cfg
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1307 2024-04-16 09:02:01.000000 graas-observability-utility-1.6.2/setup.py
```

### Comparing `graas-observability-utility-1.6.1/PKG-INFO` & `graas-observability-utility-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graas-observability-utility
-Version: 1.6.1
+Version: 1.6.2
 Summary: A small wrapper around data observability
 Home-page: https://bitbucket.org/shoptimizeanalytics/graas-observability-utility
 Author: Graas
 Author-email: priyanka.patel@graas.ai
 Keywords: utility
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `graas-observability-utility-1.6.1/README.md` & `graas-observability-utility-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_observability_utility.egg-info/PKG-INFO` & `graas-observability-utility-1.6.2/graas_observability_utility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graas-observability-utility
-Version: 1.6.1
+Version: 1.6.2
 Summary: A small wrapper around data observability
 Home-page: https://bitbucket.org/shoptimizeanalytics/graas-observability-utility
 Author: Graas
 Author-email: priyanka.patel@graas.ai
 Keywords: utility
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `graas-observability-utility-1.6.1/graas_observability_utility.egg-info/SOURCES.txt` & `graas-observability-utility-1.6.2/graas_observability_utility.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -44,33 +44,28 @@
 graas_utilities/Schema/Shopee_Marketing_Voucher_Trends_Daily_Report.json
 graas_utilities/Schema/Shopee_Product_Overview_Daily_Monthly_Report.json
 graas_utilities/Schema/Shopee_Product_Overview_Hourly_Daily_Report.json
 graas_utilities/Schema/Shopee_Product_Performance_Daily_Report.json
 graas_utilities/Schema/Shopee_Store_Metrics_Paid_Orders_Daily_monthly_report.json
 graas_utilities/Schema/Shopee_Traffic_Overview_Daily_Monthly_Report.json
 graas_utilities/Schema/Shopee_mkp_onsite_campaign_daily_Report.json
-graas_utilities/Schema/Shopee_onsite_campaign_daily_Report.json
 graas_utilities/Schema/Shopee_store_Metrics_Placed_Order_Hourly_Daily_report.json
 graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json
 graas_utilities/Schema/Tokopedia_Product_Overview_Daily_Report.json
 graas_utilities/Schema/Tokopedia_Product_Performance_Daily_Report.json
 graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Daily_monthly_Report.json
 graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Monthly_Report.json
 graas_utilities/Schema/__init__.py
 graas_utilities/Schema/amount_currency_code_object.json
 graas_utilities/Schema/graas_amazon_campaigns.json
 graas_utilities/Schema/graas_flipkart_campaigns.json
 graas_utilities/Schema/graas_mkp_affiliate_report_daily.json
 graas_utilities/Schema/graas_mkp_deals_overview_daily.json
 graas_utilities/Schema/graas_mkp_deals_trends_daily.json
 graas_utilities/Schema/graas_mkp_offsite_campaigns.json
-graas_utilities/Schema/graas_mkp_onsite_campaigns.json
 graas_utilities/Schema/graas_mkp_onsite_keywords.json
 graas_utilities/Schema/graas_mkp_product_campaign_performance.json
-graas_utilities/Schema/graas_mkp_product_overview_daily.json
-graas_utilities/Schema/graas_mkp_product_overview_hourly.json
-graas_utilities/Schema/graas_mkp_product_performance.json
 graas_utilities/Schema/graas_mkp_shop_stats_daily.json
 graas_utilities/Schema/graas_mkp_shop_stats_hourly.json
 graas_utilities/Schema/graas_mkp_traffic_overview_daily.json
 graas_utilities/Schema/graas_mkp_traffic_overview_hourly.json
 graas_utilities/Schema/graas_mkp_voucher_performance_daily.json
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Product_Performance_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Traffic_Overview_Daily_Monthly_Report.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6292613636363636%*

 * *Differences: {"'description'": "'Overview of daily and monthly traffic metrics on Shopee platform'",*

 * * "'properties'": '{\'Date\': {\'description\': "Date of the report in the format \'DD-MM-YYYY\'"}, '*

 * *                 "'Page_Views': OrderedDict([('type', 'integer'), ('description', 'Total number of "*

 * *                 "page views on Shopee')]), 'Avg_Page_Views': OrderedDict([('type', 'number'), "*

 * *                 "('description', 'Average number of page views per visit')]), 'Avg_Time_Spent': "*

 * *                 'OrderedD […]*

```diff
@@ -1,72 +1,48 @@
 {
-    "description": "Daily report presenting the performance metrics for a specific product on Amazon",
+    "description": "Overview of daily and monthly traffic metrics on Shopee platform",
     "properties": {
-        "Child_ASIN": {
-            "description": "Child Amazon Standard Identification Number (ASIN) of the product",
+        "Avg_Page_Views": {
+            "description": "Average number of page views per visit",
+            "type": "number"
+        },
+        "Avg_Time_Spent": {
+            "description": "Average time spent on the platform per visit in the format 'HH:mm:ss'",
             "type": "string"
         },
+        "Bounce_Rate": {
+            "description": "Bounce rate, representing the percentage of visitors who navigate away from the site after viewing only one page",
+            "type": "number"
+        },
         "Date": {
-            "description": "Date of the report in the format 'MM-DD-YYYY'",
+            "description": "Date of the report in the format 'DD-MM-YYYY'",
             "format": "dd-MM-yyyy",
             "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
             "type": "string"
         },
-        "Featured_Offer_Buy_Box_Percentage": {
-            "description": "Percentage of sessions where the product is the featured offer in the buy box",
-            "type": "number"
-        },
-        "Ordered_Product_Sales": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Ordered product sales amount information",
-            "type": "object"
-        },
-        "Page_Views_Percentage_Total": {
-            "description": "Percentage of total page views for the product",
-            "type": "number"
-        },
-        "Page_Views_Total": {
-            "description": "Total number of page views for the product",
+        "Existing_Visitors": {
+            "description": "Number of existing visitors on Shopee",
             "type": "integer"
         },
-        "Parent_ASIN": {
-            "description": "Parent Amazon Standard Identification Number (ASIN) of the product",
-            "type": "string"
-        },
-        "SKU": {
-            "description": "Stock Keeping Unit (SKU) of the product",
-            "type": "string"
-        },
-        "Session_Percentage_Total": {
-            "description": "Percentage of total sessions for the product",
-            "type": "number"
-        },
-        "Sessions_Total": {
-            "description": "Total number of sessions for the product",
+        "New_Followers": {
+            "description": "Number of new followers gained",
             "type": "integer"
         },
-        "Title": {
-            "description": "Title or name of the product",
-            "type": "string"
-        },
-        "Total_Order_Items": {
-            "description": "Total number of order items for the product",
+        "New_Visitors": {
+            "description": "Number of new visitors on Shopee",
             "type": "integer"
         },
-        "Unit_Session_Percentage": {
-            "description": "Percentage of units ordered per session",
-            "type": "number"
+        "Page_Views": {
+            "description": "Total number of page views on Shopee",
+            "type": "integer"
         },
-        "Units_Ordered": {
-            "description": "Total number of units ordered for the product",
+        "Visitors": {
+            "description": "Total number of visitors on Shopee",
             "type": "integer"
         }
     },
     "required": [
-        "Parent_ASIN",
-        "Child_ASIN",
-        "SKU",
         "Date"
     ],
-    "title": "Amazon Product Performance Daily Report",
+    "title": "Shopee Traffic Overview Daily Monthly Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Sponsored_Brands_Attributed_Purchases_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Sponsored_Brands_Attributed_Purchases_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Sponsored_Brands_Campaign_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Sponsored_Brands_Campaign_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Sponsored_Display_Advertised_Product_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Sponsored_Display_Advertised_Product_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Sponsored_Display_Campaign_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Sponsored_Display_Campaign_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Sponsored_Products_Advertised_Product_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Sponsored_Products_Advertised_Product_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Sponsored_Products_Campaign_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Sponsored_Products_Campaign_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Store_Key_Metrics_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_BundleDeal_Overview_Daily_Report.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5337873931623932%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'description'": "'Daily overview report for a marketing bundle deal'",*

 * * "'properties'": "{'Date': {'description': 'Date of the report (format: DD-MM-YYYY)'}, "*

 * *                 "'Bundle_ID': OrderedDict([('type', 'integer'), ('description', 'The unique "*

 * *                 "identifier for the bundle deal')]), 'Bundle_Name': OrderedDict([('type', "*

 * *                 "'string'), ('description', 'The name of the marketing bundle deal')]), 'Period': "*

 * *   […]*

```diff
@@ -1,25 +1,61 @@
 {
-    "description": "Daily report presenting key metrics for an Amazon store",
+    "$schema": "http://json-schema.org/draft-07/schema#",
+    "description": "Daily overview report for a marketing bundle deal",
     "properties": {
+        "Bundle_Deals_Ordered": {
+            "description": "Total number of times the bundle deal was ordered",
+            "type": "integer"
+        },
+        "Bundle_ID": {
+            "description": "The unique identifier for the bundle deal",
+            "type": "integer"
+        },
+        "Bundle_Name": {
+            "description": "The name of the marketing bundle deal",
+            "type": "string"
+        },
+        "Buyers": {
+            "description": "Total number of unique buyers for the bundle deal",
+            "type": "integer"
+        },
         "Date": {
-            "description": "Date of the report in the format 'MM-DD-YYYY'",
+            "description": "Date of the report (format: DD-MM-YYYY)",
             "format": "dd-MM-yyyy",
             "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
             "type": "string"
         },
-        "Ordered_Product_Sales": {
+        "Orders": {
+            "description": "Total number of orders for the bundle deal",
+            "type": "integer"
+        },
+        "Period": {
+            "description": "The time period during which the report is generated (format: DD-MM-YYYY HH:mm - DD-MM-YYYY HH:mm)",
+            "type": "string"
+        },
+        "Sales": {
+            "$ref": "../Schema/amount_currency_code_object.json",
+            "description": "Total sales with amount and currency",
+            "type": "object"
+        },
+        "Sales_Per_Buyer": {
             "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Sales information for ordered products",
+            "description": "Sales per buyer with amount and currency",
             "type": "object"
         },
-        "Units_Ordered": {
-            "description": "Total number of units ordered",
+        "Status": {
+            "description": "Current status of the bundle deal (e.g., 'Expired')",
+            "type": "string"
+        },
+        "Units_Sold": {
+            "description": "Total units of the bundle deal sold",
             "type": "integer"
         }
     },
     "required": [
+        "Bundle_ID",
+        "Bundle_Name",
         "Date"
     ],
-    "title": "Amazon Store Key Metrics Daily Report",
+    "title": "Marketing Bundle Deal Overview Daily Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Store_Key_Metrics_Hourly_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Bundle_Deal_Trends_Daily_Report.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6%*

 * *Differences: {"'description'": "'Daily report on bundle deal trends for Shopee marketing'",*

 * * "'properties'": "{replace: OrderedDict([('Units_Sold', OrderedDict([('type', 'integer'), "*

 * *                 "('description', 'Total number of units sold for bundle deals')])), ('Sales', "*

 * *                 "OrderedDict([('type', 'object'), ('$ref', "*

 * *                 "'../Schema/amount_currency_code_object.json'), ('description', 'Sales "*

 * *                 "information for bundle deals')])), ('Orders', OrderedDict([('type', 'integ […]*

```diff
@@ -1,33 +1,42 @@
 {
-    "description": "Hourly daily report presenting key metrics for an Amazon store",
+    "description": "Daily report on bundle deal trends for Shopee marketing",
     "properties": {
-        "Same_date_range_one_year_ago_Ordered_product_sales": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Ordered product sales amount for the same date range one year ago",
-            "type": "object"
+        "Bundle_Deals_Ordered": {
+            "description": "Total number of bundle deals ordered",
+            "type": "integer"
+        },
+        "Buyers": {
+            "description": "Total number of unique buyers for bundle deals",
+            "type": "integer"
+        },
+        "Date": {
+            "description": "Date of the report in the format 'MM-DD-YYYY'",
+            "format": "dd-MM-yyyy",
+            "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
+            "type": "string"
         },
-        "Same_date_range_one_year_ago_Units_ordered": {
-            "description": "Total number of units ordered for the same date range one year ago",
+        "Orders": {
+            "description": "Total number of orders for bundle deals",
             "type": "integer"
         },
-        "Selected_date_range_Ordered_product_sales": {
+        "Sales": {
             "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Ordered product sales amount for the selected date range",
+            "description": "Sales information for bundle deals",
             "type": "object"
         },
-        "Selected_date_range_Units_ordered": {
-            "description": "Total number of units ordered for the selected date range",
-            "type": "integer"
+        "Sales_Per_Buyer": {
+            "$ref": "../Schema/amount_currency_code_object.json",
+            "description": "Sales per buyer information for bundle deals",
+            "type": "object"
         },
-        "Time": {
-            "description": "Time of the report in the format 'MM-DD-YYYY HH:mm'",
-            "format": "dd-MM-yyyy HH:mm",
-            "type": "string"
+        "Units_Sold": {
+            "description": "Total number of units sold for bundle deals",
+            "type": "integer"
         }
     },
     "required": [
-        "Time"
+        "Date"
     ],
-    "title": "Amazon Store Key Metrics Hourly Daily Report",
+    "title": "Shopee Marketing Bundle Deal Trends Daily Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Amazon_Traffic_Metrics_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Traffic_Metrics_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Flipkart_PLA_Campaign_Seller_Portal_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Flipkart_PLA_Campaign_Seller_Portal_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Flipkart_PLA_Consolidated_FSN_seller_Portal_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Flipkart_PLA_Consolidated_FSN_seller_Portal_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Flipkart_Search_Traffic_Report_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Flipkart_Search_Traffic_Report_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Lazada_Customers_Insight_monthly_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Lazada_Customers_Insight_monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Lazada_Keywords_Onsite_daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Lazada_Keywords_Onsite_daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Lazada_Product_Performance_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Tokopedia_Product_Performance_Daily_Report.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'description'": "'Daily report presenting the performance metrics for a specific product on "*

 * *                  "Tokopedia'",*

 * * "'properties'": "{replace: OrderedDict([('merchantID', OrderedDict([('type', 'string'), "*

 * *                 "('description', 'A unique merchant code for GRAAS clients')])), "*

 * *                 '(\'siteNickNameId\', OrderedDict([(\'type\', \'string\'), (\'description\', "A '*

 * *                 'unique merchant\'s store code for […]*

```diff
@@ -1,99 +1,112 @@
 {
-    "description": "Daily report presenting the performance metrics for a specific product on Lazada",
+    "$schema": "http://json-schema.org/draft-07/schema#",
+    "description": "Daily report presenting the performance metrics for a specific product on Tokopedia",
     "properties": {
-        "Add_to_Cart_Conversion_Rate": {
-            "description": "Conversion rate from product view to adding to cart as a percentage",
-            "type": "number"
-        },
-        "Add_to_Cart_Units": {
-            "description": "Total number of units added to the cart for the product",
-            "type": "integer"
-        },
-        "Add_to_Cart_Visitors": {
-            "description": "Total number of visitors who added the product to the cart",
-            "type": "integer"
-        },
-        "Buyers": {
-            "description": "Total number of buyers who made a purchase for the product",
-            "type": "integer"
-        },
-        "Conversion_Rate": {
-            "description": "Conversion rate from product view to purchase as a percentage",
-            "type": "number"
-        },
-        "Date": {
-            "description": "Date of the report in the format 'MM-DD-YYYY'",
-            "format": "dd-MM-yyyy",
-            "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
+        "countryCode": {
+            "description": "The country code, e.g., 'SG', 'MY'.",
             "type": "string"
         },
-        "Orders": {
-            "description": "Total number of orders placed for the product",
-            "type": "integer"
-        },
-        "Product_ID": {
-            "description": "Unique identifier for the product on Lazada",
-            "type": "integer"
-        },
-        "Product_Name": {
-            "description": "Name of the product being analyzed",
+        "currencyCode": {
+            "description": "The currency code, e.g., 'SGD', 'USD'.",
             "type": "string"
         },
-        "Product_Pageviews": {
-            "description": "Total number of page views for the product",
-            "type": "integer"
-        },
-        "Revenue": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Revenue information for the product",
-            "type": "object"
-        },
-        "Revenue_per_Buyer": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Revenue per buyer information",
-            "type": "object"
-        },
-        "SKU_ID": {
-            "description": "Stock Keeping Unit (SKU) identifier for the product",
+        "merchantID": {
+            "description": "A unique merchant code for GRAAS clients",
             "type": "string"
         },
-        "Seller_SKU": {
-            "description": "Seller Stock Keeping Unit (SKU) for the product",
-            "type": "string"
+        "result": {
+            "items": {
+                "properties": {
+                    "Basket": {
+                        "description": "Total number of times the product was added to the shopping basket",
+                        "type": "integer"
+                    },
+                    "Category": {
+                        "description": "Category to which the product belongs",
+                        "type": "string"
+                    },
+                    "Conversion": {
+                        "description": "Conversion rate of the product as a decimal",
+                        "type": "number"
+                    },
+                    "Date": {
+                        "description": "Date of the report in the format 'MM-DD-YYYY'",
+                        "format": "dd-MM-yyyy",
+                        "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
+                        "type": "string"
+                    },
+                    "New_Net_Income": {
+                        "description": "New net income information for the product",
+                        "properties": {
+                            "amount": {
+                                "description": "The cost amount per conversion.",
+                                "type": "number"
+                            },
+                            "currencyCode": {
+                                "description": "The currency code, e.g., 'SGD', 'USD'.",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "amount",
+                            "currencyCode"
+                        ],
+                        "type": "object"
+                    },
+                    "Order": {
+                        "description": "Total number of orders placed for the product",
+                        "type": "integer"
+                    },
+                    "Product_Viewed": {
+                        "description": "Total number of times the product was viewed",
+                        "type": "integer"
+                    },
+                    "Product_name": {
+                        "description": "Name of the product being analyzed",
+                        "type": "string"
+                    },
+                    "SKU": {
+                        "description": "Stock Keeping Unit (SKU) of the product",
+                        "type": "string"
+                    },
+                    "Sold_Products": {
+                        "description": "Total number of units sold for the product",
+                        "type": "integer"
+                    },
+                    "Wishlist": {
+                        "description": "Total number of times the product was added to the wishlist",
+                        "type": "integer"
+                    }
+                },
+                "required": [
+                    "Product_name",
+                    "SKU",
+                    "Category",
+                    "New_Net_Income",
+                    "Sold_Products",
+                    "Product_Viewed",
+                    "Basket",
+                    "Wishlist",
+                    "Conversion",
+                    "Order",
+                    "Date"
+                ],
+                "type": "object"
+            },
+            "type": "array"
         },
-        "URL": {
-            "description": "URL link to the product on Lazada",
-            "format": "uri",
+        "siteNickNameId": {
+            "description": "A unique merchant's store code for GRAAS clients",
             "type": "string"
-        },
-        "Units_Sold": {
-            "description": "Total number of units sold for the product",
-            "type": "integer"
-        },
-        "Visitor_Value": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Visitor value information",
-            "type": "object"
-        },
-        "Visitors": {
-            "description": "Total number of visitors to the product page",
-            "type": "integer"
-        },
-        "Wishlist_Users": {
-            "description": "Total number of users who added the product to their wishlist",
-            "type": "integer"
-        },
-        "Wishlists": {
-            "description": "Total number of times the product was added to wishlists",
-            "type": "integer"
         }
     },
     "required": [
-        "Product_ID",
-        "Seller_SKU",
-        "SKU_ID",
-        "Date"
+        "merchantID",
+        "siteNickNameId",
+        "countryCode",
+        "currencyCode",
+        "result"
     ],
-    "title": "Lazada Product Performance Daily Report",
+    "title": "Tokopedia Product Performance Daily Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Lazada_Product_Sponsored_Affiliate_Report_Daily_monthly_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Lazada_Product_Sponsored_Affiliate_Report_Daily_monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Lazada_Store_Key_Metrics_monthly_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Store_Metrics_Paid_Orders_Daily_monthly_report.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.709274193548387%*

 * *Differences: {"'description'": "'Daily and monthly report presenting key metrics for paid orders in a Shopee "*

 * *                  "store'",*

 * * "'properties'": "{'Orders': {'description': 'Total number of paid orders'}, 'Sales': "*

 * *                 "OrderedDict([('type', 'object'), ('$ref', "*

 * *                 "'../Schema/amount_currency_code_object.json'), ('description', 'Sales "*

 * *                 "information')]), 'Sales_per_Order': OrderedDict([('type', 'object'), ('$ref', "*

 * *                 "'../Schema/amount_currency_cod […]*

```diff
@@ -1,89 +1,80 @@
 {
-    "description": "Monthly report presenting key metrics for a Lazada store",
+    "description": "Daily and monthly report presenting key metrics for paid orders in a Shopee store",
     "properties": {
-        "Add_to_Cart_Units": {
-            "description": "Total number of units added to the cart",
+        "Cancelled_Orders": {
+            "description": "Total number of cancelled orders",
             "type": "integer"
         },
-        "Add_to_Cart_Visitors": {
-            "description": "Total number of visitors who added items to the cart",
-            "type": "integer"
-        },
-        "Average_Basket_Size": {
-            "description": "Average number of units per order",
-            "type": "number"
-        },
-        "Average_Order_Value": {
+        "Cancelled_Sales": {
             "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Average order value information",
+            "description": "Sales amount information for cancelled orders",
             "type": "object"
         },
-        "Buyers": {
-            "description": "Total number of unique buyers",
-            "type": "integer"
-        },
-        "Cancelled_Amount": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Cancelled order amount information",
-            "type": "object"
-        },
-        "Conversion_Rate": {
-            "description": "Conversion rate as a decimal",
+        "Conversion_Rate_by_paid_order": {
+            "description": "Conversion rate from store visit to paid order as a percentage",
             "type": "number"
         },
         "Date": {
             "description": "Date of the report in the format 'MM-DD-YYYY'",
             "format": "dd-MM-yyyy",
             "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
             "type": "string"
         },
+        "No_of_buyers": {
+            "description": "Total number of buyers who made a purchase",
+            "type": "integer"
+        },
+        "No_of_existing_buyers": {
+            "description": "Total number of existing buyers",
+            "type": "integer"
+        },
+        "No_of_new_buyers": {
+            "description": "Total number of new buyers",
+            "type": "integer"
+        },
+        "No_of_potential_buyers": {
+            "description": "Total number of potential buyers",
+            "type": "integer"
+        },
         "Orders": {
-            "description": "Total number of orders placed",
+            "description": "Total number of paid orders",
             "type": "integer"
         },
-        "Pageviews": {
-            "description": "Total number of pageviews",
+        "Page_Views": {
+            "description": "Total number of page views in the store",
             "type": "integer"
         },
-        "Return_Refund_Amount": {
+        "Repeat_Purchase_Rate": {
+            "description": "Rate of repeat purchases as a percentage",
+            "type": "number"
+        },
+        "Returned_Refunded_Orders": {
+            "description": "Total number of returned or refunded orders",
+            "type": "integer"
+        },
+        "Returned_Refunded_Sales": {
             "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Return and refund amount information",
+            "description": "Sales amount information for returned or refunded orders",
             "type": "object"
         },
-        "Revenue": {
+        "Sales": {
             "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Revenue information",
+            "description": "Sales information",
             "type": "object"
         },
-        "Revenue_per_Buyer": {
+        "Sales_per_Order": {
             "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Revenue per buyer information",
+            "description": "Average sales amount per order information",
             "type": "object"
         },
-        "Units_Sold": {
-            "description": "Total number of units sold",
-            "type": "integer"
-        },
-        "Visitor_Value": {
-            "description": "Average value per visitor",
-            "type": "number"
-        },
         "Visitors": {
             "description": "Total number of visitors to the store",
             "type": "integer"
-        },
-        "Wishlist_Visitors": {
-            "description": "Total number of visitors who added items to wishlists",
-            "type": "integer"
-        },
-        "Wishlists": {
-            "description": "Total number of items added to wishlists",
-            "type": "integer"
         }
     },
     "required": [
         "Date"
     ],
-    "title": "Lazada Store Key Metrics Monthly Report",
+    "title": "Shopee Store Metrics Paid Orders Daily Monthly Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Lazada_mkp_onsite_campaign_monthly_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Lazada_mkp_onsite_campaign_monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Lazada_offsite_campaign_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Lazada_offsite_campaign_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Lazada_onsite_campaign_monthly_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Lazada_onsite_campaign_monthly_Report.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9451992753623188%*

 * *Differences: {"'properties'": "{'Campaign_ID': {'type': 'number'}}",*

 * * "'required'": "{insert: [(8, 'Campaign_Objective'), (9, 'Budget'), (10, 'Spend'), (11, 'Clicks'), "*

 * *               "(12, 'CTR'), (13, 'CPC'), (14, 'Add_To_Cart_Units'), (15, 'Orders'), (16, 'CVR'), "*

 * *               "(17, 'Units_Sold'), (18, 'Revenue'), (19, 'ROAS'), (20, 'Direct_Orders'), (21, "*

 * *               "'Direct_CVR'), (22, 'Direct_Units_Sold')]}"}*

```diff
@@ -22,15 +22,15 @@
         },
         "CVR": {
             "description": "The Conversion Rate (CVR) for the campaign, expressed as a percentage.",
             "type": "string"
         },
         "Campaign_ID": {
             "description": "The unique identifier for the campaign.",
-            "type": "string"
+            "type": "number"
         },
         "Campaign_Name": {
             "description": "The name of the campaign.",
             "type": [
                 "number",
                 "string"
             ]
@@ -108,12 +108,27 @@
         "Date",
         "Campaign_Name",
         "Campaign_ID",
         "Campaign_Type",
         "Placement",
         "Direct_Add_To_Cart_Units",
         "Direct_Revenue",
-        "Impression"
+        "Impression",
+        "Campaign_Objective",
+        "Budget",
+        "Spend",
+        "Clicks",
+        "CTR",
+        "CPC",
+        "Add_To_Cart_Units",
+        "Orders",
+        "CVR",
+        "Units_Sold",
+        "Revenue",
+        "ROAS",
+        "Direct_Orders",
+        "Direct_CVR",
+        "Direct_Units_Sold"
     ],
     "title": "Lazada Onsite Campaign Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Keywords_Onsite_daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Keywords_Onsite_daily_Report.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9966666666666667%*

 * *Differences: {"'properties'": "{'Product_ID': OrderedDict([('type', 'integer'), ('description', 'ID of the "*

 * *                 "product')])}"}*

```diff
@@ -99,14 +99,18 @@
             "description": "Product click-through rate",
             "type": "number"
         },
         "Product_Clicks": {
             "description": "Number of product clicks",
             "type": "number"
         },
+        "Product_ID": {
+            "description": "ID of the product",
+            "type": "integer"
+        },
         "Product_Impressions": {
             "description": "Number of product impressions",
             "type": "number"
         },
         "Product_Name_Ad_Name": {
             "description": "Name of the product or advertisement",
             "type": "string"
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Key_Metrics_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Key_Metrics_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Trends_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Trends_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_BundleDeal_Overview_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Store_Key_Metrics_Daily_Report.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'description'": "'Daily report presenting key metrics for an Amazon store'",*

 * * "'properties'": "{replace: OrderedDict([('merchantID', OrderedDict([('type', 'string'), "*

 * *                 "('description', 'A unique merchant code for GRAAS clients')])), "*

 * *                 '(\'siteNickNameId\', OrderedDict([(\'type\', \'string\'), (\'description\', "A '*

 * *                 'unique merchant\'s store code for GRAAS clients")])), (\'countryCode\', '*

 * *                 'OrderedDict([(\'type\', \'string\'), (\'descripti […]*

```diff
@@ -1,61 +1,70 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "Daily overview report for a marketing bundle deal",
+    "description": "Daily report presenting key metrics for an Amazon store",
     "properties": {
-        "Bundle_Deals_Ordered": {
-            "description": "Total number of times the bundle deal was ordered",
-            "type": "integer"
-        },
-        "Bundle_ID": {
-            "description": "The unique identifier for the bundle deal",
-            "type": "integer"
-        },
-        "Bundle_Name": {
-            "description": "The name of the marketing bundle deal",
+        "countryCode": {
+            "description": "The country code, e.g., 'SG', 'MY'.",
             "type": "string"
         },
-        "Buyers": {
-            "description": "Total number of unique buyers for the bundle deal",
-            "type": "integer"
-        },
-        "Date": {
-            "description": "Date of the report (format: DD-MM-YYYY)",
-            "format": "dd-MM-yyyy",
-            "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
+        "currencyCode": {
+            "description": "The currency code, e.g., 'SGD', 'USD'.",
             "type": "string"
         },
-        "Orders": {
-            "description": "Total number of orders for the bundle deal",
-            "type": "integer"
-        },
-        "Period": {
-            "description": "The time period during which the report is generated (format: DD-MM-YYYY HH:mm - DD-MM-YYYY HH:mm)",
+        "merchantID": {
+            "description": "A unique merchant code for GRAAS clients",
             "type": "string"
         },
-        "Sales": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Total sales with amount and currency",
-            "type": "object"
-        },
-        "Sales_Per_Buyer": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Sales per buyer with amount and currency",
-            "type": "object"
+        "result": {
+            "items": {
+                "properties": {
+                    "Date": {
+                        "description": "Date of the report in the format 'MM-DD-YYYY'",
+                        "format": "dd-MM-yyyy",
+                        "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
+                        "type": "string"
+                    },
+                    "Ordered_Product_Sales": {
+                        "description": "Sales information for ordered products",
+                        "properties": {
+                            "amount": {
+                                "description": "The cost amount per conversion.",
+                                "type": "number"
+                            },
+                            "currencyCode": {
+                                "description": "The currency code, e.g., 'SGD', 'USD'.",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "amount",
+                            "currencyCode"
+                        ],
+                        "type": "object"
+                    },
+                    "Units_Ordered": {
+                        "description": "Total number of units ordered",
+                        "type": "integer"
+                    }
+                },
+                "required": [
+                    "Date"
+                ],
+                "type": "object"
+            },
+            "type": "array"
         },
-        "Status": {
-            "description": "Current status of the bundle deal (e.g., 'Expired')",
+        "siteNickNameId": {
+            "description": "A unique merchant's store code for GRAAS clients",
             "type": "string"
-        },
-        "Units_Sold": {
-            "description": "Total units of the bundle deal sold",
-            "type": "integer"
         }
     },
     "required": [
-        "Bundle_ID",
-        "Bundle_Name",
-        "Date"
+        "merchantID",
+        "siteNickNameId",
+        "countryCode",
+        "currencyCode",
+        "result"
     ],
-    "title": "Marketing Bundle Deal Overview Daily Report",
+    "title": "Amazon Store Key Metrics Daily Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Trends_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Trends_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Detailed_Overview_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Detailed_Overview_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Trends_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Trends_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Voucher_Performance_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Voucher_Performance_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Marketing_Voucher_Trends_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Marketing_Voucher_Trends_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Product_Overview_Daily_Monthly_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_store_Metrics_Placed_Order_Hourly_Daily_report.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6%*

 * *Differences: {"'description'": "'Hourly daily report providing key metrics related to placed orders in a Shopee "*

 * *                  "store'",*

 * * "'properties'": "{replace: OrderedDict([('Time', OrderedDict([('type', 'string'), ('description', "*

 * *                 '"Date and time of the report in the format \'MM-DD-YYYY HH:mm\'"), (\'format\', '*

 * *                 "'dd-MM-yyyy HH:mm')])), ('Sales', OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('amount', OrderedDict([('type', 'number'), "*

 * *    […]*

```diff
@@ -1,102 +1,111 @@
 {
-    "description": "Daily monthly report providing an overview of product-related metrics on Shopee",
+    "description": "Hourly daily report providing key metrics related to placed orders in a Shopee store",
     "properties": {
-        "Buyers_Paid_Order": {
-            "description": "Number of buyers who paid for the order",
-            "type": "string"
-        },
-        "Buyers_Placed_Order": {
-            "description": "Total number of buyers who placed an order",
-            "type": "integer"
-        },
-        "Conversion_Rate_Add_to_Cart": {
-            "description": "Conversion rate from product view to adding to cart as a percentage",
-            "type": "number"
-        },
-        "Conversion_Rate_Paid_Order": {
-            "description": "Conversion rate from placing an order to paying for the order as a percentage",
-            "type": "number"
-        },
-        "Conversion_Rate_Placed_Order": {
-            "description": "Conversion rate from adding to cart to placing an order as a percentage",
-            "type": "number"
-        },
-        "Conversion_Rate_Placed_to_Confirmed": {
-            "description": "Conversion rate from placing an order to order confirmation as a percentage",
-            "type": "number"
-        },
-        "Date": {
-            "description": "Date of the report in the format 'MM-DD-YYYY'",
-            "format": "dd-MM-yyyy",
-            "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
-            "type": "string"
-        },
-        "Items_Paid": {
-            "description": "Number of items paid for in the order",
-            "type": "string"
-        },
-        "Items_Placed": {
-            "description": "Total number of items placed in orders",
-            "type": "integer"
-        },
-        "Items_Visited": {
-            "description": "Total number of items visited",
+        "Cancelled_Orders": {
+            "description": "Total number of cancelled orders during the specified time period",
             "type": "integer"
         },
-        "Likes": {
-            "description": "Total number of likes received for the product",
-            "type": "integer"
+        "Cancelled_Sales": {
+            "description": "Sales information for cancelled orders",
+            "properties": {
+                "amount": {
+                    "description": "Total sales amount for cancelled orders in the specified currency (SGD)",
+                    "type": "number"
+                },
+                "currencyCode": {
+                    "description": "Currency code for the sales amount for cancelled orders (SGD)",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "amount",
+                "currencyCode"
+            ],
+            "type": "object"
         },
-        "Product_Bounce_Rate": {
-            "description": "Bounce rate for the product page as a percentage",
+        "Conversion_Rate_Placed_Orders": {
+            "description": "Conversion rate for placed orders as a percentage",
             "type": "number"
         },
-        "Product_Bounce_Visitors": {
-            "description": "Total number of visitors who bounced from the product page",
-            "type": "integer"
-        },
-        "Product_Page_Views": {
-            "description": "Total number of page views for the product",
-            "type": "integer"
-        },
-        "Product_Visitors_Add_to_Cart": {
-            "description": "Total number of visitors who added the product to the cart",
+        "Orders": {
+            "description": "Total number of orders placed during the specified time period",
             "type": "integer"
         },
-        "Product_Visitors_Visit": {
-            "description": "Total number of visitors who visited the product",
+        "Page_Views": {
+            "description": "Total number of page views during the specified time period",
             "type": "integer"
         },
-        "Sales_Paid_Order": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Sales amount information for paid orders",
+        "Returned_Refunded_Orders": {
+            "description": "Total number of returned or refunded orders during the specified time period",
+            "type": "integer"
+        },
+        "Returned_Refunded_Sales": {
+            "description": "Sales information for returned or refunded orders",
+            "properties": {
+                "amount": {
+                    "description": "Total sales amount for returned or refunded orders in the specified currency (SGD)",
+                    "type": "number"
+                },
+                "currencyCode": {
+                    "description": "Currency code for the sales amount for returned or refunded orders (SGD)",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "amount",
+                "currencyCode"
+            ],
             "type": "object"
         },
-        "Sales_Placed_Order": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Sales amount information for placed orders",
+        "Sales": {
+            "description": "Sales information for the specified time period",
+            "properties": {
+                "amount": {
+                    "description": "Total sales amount for the specified time period in the specified currency (SGD)",
+                    "type": "number"
+                },
+                "currencyCode": {
+                    "description": "Currency code for the sales amount (SGD)",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "amount",
+                "currencyCode"
+            ],
             "type": "object"
         },
-        "Search_Clicks": {
-            "description": "Total number of clicks from search results to the product",
-            "type": "integer"
-        },
-        "Units_Add_to_Cart": {
-            "description": "Total number of units added to the cart for the product",
-            "type": "integer"
+        "Sales_per_Order": {
+            "description": "Average sales amount per order information",
+            "properties": {
+                "amount": {
+                    "description": "Average sales amount per order in the specified currency (SGD)",
+                    "type": "number"
+                },
+                "currencyCode": {
+                    "description": "Currency code for the sales amount per order (SGD)",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "amount",
+                "currencyCode"
+            ],
+            "type": "object"
         },
-        "Units_Paid_Order": {
-            "description": "Number of units paid for in the order",
+        "Time": {
+            "description": "Date and time of the report in the format 'MM-DD-YYYY HH:mm'",
+            "format": "dd-MM-yyyy HH:mm",
             "type": "string"
         },
-        "Units_Placed_Order": {
-            "description": "Total number of units placed in orders",
+        "Visitors": {
+            "description": "Total number of unique visitors during the specified time period",
             "type": "integer"
         }
     },
     "required": [
-        "Date"
+        "Time"
     ],
-    "title": "Shopee Product Overview Daily Monthly Report",
+    "title": "Shopee Store Metrics Placed Order Hourly Daily Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Product_Overview_Hourly_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Product_Performance_Daily_Report.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'description'": "'Daily report presenting the performance metrics for a specific product on "*

 * *                  "Amazon'",*

 * * "'properties'": "{replace: OrderedDict([('merchantID', OrderedDict([('type', 'string'), "*

 * *                 "('description', 'A unique merchant code for GRAAS clients')])), "*

 * *                 '(\'siteNickNameId\', OrderedDict([(\'type\', \'string\'), (\'description\', "A '*

 * *                 'unique merchant\'s store code for GR […]*

```diff
@@ -1,98 +1,127 @@
 {
-    "description": "Hourly daily report providing an overview of product-related metrics on Shopee",
+    "$schema": "http://json-schema.org/draft-07/schema#",
+    "description": "Daily report presenting the performance metrics for a specific product on Amazon",
     "properties": {
-        "Buyers_Paid_Order": {
-            "description": "Number of buyers who paid for the order during the specified hour",
-            "type": "integer"
-        },
-        "Buyers_Placed_Order": {
-            "description": "Total number of buyers who placed an order during the specified hour",
-            "type": "integer"
-        },
-        "Conversion_Rate_Add_to_Cart": {
-            "description": "Conversion rate from product view to adding to cart during the specified hour as a percentage",
-            "type": "number"
-        },
-        "Conversion_Rate_Paid_Order": {
-            "description": "Conversion rate from placing an order to paying for the order during the specified hour as a percentage",
-            "type": "number"
-        },
-        "Conversion_Rate_Placed_Order": {
-            "description": "Conversion rate from adding to cart to placing an order during the specified hour as a percentage",
-            "type": "number"
-        },
-        "Date": {
-            "description": "Date and time of the report in the format 'MM-DD-YYYY HH:mm'",
-            "format": "dd-MM-yyyy",
-            "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
+        "countryCode": {
+            "description": "The country code, e.g., 'SG', 'MY'.",
             "type": "string"
         },
-        "Items_Paid": {
-            "description": "Number of items paid for in the order during the specified hour",
-            "type": "integer"
-        },
-        "Items_Placed": {
-            "description": "Total number of items placed in orders during the specified hour",
-            "type": "integer"
-        },
-        "Items_Visited": {
-            "description": "Total number of items visited during the specified hour",
-            "type": "integer"
-        },
-        "Likes": {
-            "description": "Total number of likes received for the product during the specified hour",
-            "type": "integer"
-        },
-        "Product_Bounce_Rate": {
-            "description": "Bounce rate for the product page during the specified hour as a percentage",
-            "type": "number"
-        },
-        "Product_Bounce_Visitors": {
-            "description": "Total number of visitors who bounced from the product page during the specified hour",
-            "type": "integer"
-        },
-        "Product_Page_Views": {
-            "description": "Total number of page views for the product during the specified hour",
-            "type": "integer"
-        },
-        "Product_Visitors_Add_to_Cart": {
-            "description": "Total number of visitors who added the product to the cart during the specified hour",
-            "type": "integer"
-        },
-        "Product_Visitors_Visit": {
-            "description": "Total number of visitors who visited the product during the specified hour",
-            "type": "integer"
-        },
-        "Sales_Paid_Order": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Sales amount information for paid orders during the specified hour",
-            "type": "object"
-        },
-        "Sales_Placed_Order": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Sales amount information for placed orders during the specified hour",
-            "type": "object"
-        },
-        "Search_Clicks": {
-            "description": "Total number of clicks from search results to the product during the specified hour",
-            "type": "integer"
+        "currencyCode": {
+            "description": "The currency code, e.g., 'SGD', 'USD'.",
+            "type": "string"
         },
-        "Units_Add_to_Cart": {
-            "description": "Total number of units added to the cart for the product during the specified hour",
-            "type": "integer"
+        "merchantID": {
+            "description": "A unique merchant code for GRAAS clients",
+            "type": "string"
         },
-        "Units_Paid_Order": {
-            "description": "Number of units paid for in the order during the specified hour",
-            "type": "integer"
+        "result": {
+            "items": {
+                "properties": {
+                    "Child_ASIN": {
+                        "description": "Child Amazon Standard Identification Number (ASIN) of the product",
+                        "type": "string"
+                    },
+                    "Date": {
+                        "description": "Date of the report in the format 'MM-DD-YYYY'",
+                        "format": "dd-MM-yyyy",
+                        "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
+                        "type": "string"
+                    },
+                    "Featured_Offer_Buy_Box_Percentage": {
+                        "description": "Percentage of sessions where the product is the featured offer in the buy box",
+                        "type": "number"
+                    },
+                    "Ordered_Product_Sales": {
+                        "description": "Ordered product sales amount information",
+                        "properties": {
+                            "amount": {
+                                "description": "The cost amount per conversion.",
+                                "type": "number"
+                            },
+                            "currencyCode": {
+                                "description": "The currency code, e.g., 'SGD', 'USD'.",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "amount",
+                            "currencyCode"
+                        ],
+                        "type": "object"
+                    },
+                    "Page_Views_Percentage_Total": {
+                        "description": "Percentage of total page views for the product",
+                        "type": "number"
+                    },
+                    "Page_Views_Total": {
+                        "description": "Total number of page views for the product",
+                        "type": "integer"
+                    },
+                    "Parent_ASIN": {
+                        "description": "Parent Amazon Standard Identification Number (ASIN) of the product",
+                        "type": "string"
+                    },
+                    "SKU": {
+                        "description": "Stock Keeping Unit (SKU) of the product",
+                        "type": "string"
+                    },
+                    "Session_Percentage_Total": {
+                        "description": "Percentage of total sessions for the product",
+                        "type": "number"
+                    },
+                    "Sessions_Total": {
+                        "description": "Total number of sessions for the product",
+                        "type": "integer"
+                    },
+                    "Title": {
+                        "description": "Title or name of the product",
+                        "type": "string"
+                    },
+                    "Total_Order_Items": {
+                        "description": "Total number of order items for the product",
+                        "type": "integer"
+                    },
+                    "Unit_Session_Percentage": {
+                        "description": "Percentage of units ordered per session",
+                        "type": "number"
+                    },
+                    "Units_Ordered": {
+                        "description": "Total number of units ordered for the product",
+                        "type": "integer"
+                    }
+                },
+                "required": [
+                    "Parent_ASIN",
+                    "Child_ASIN",
+                    "Title",
+                    "SKU",
+                    "Sessions_Total",
+                    "Session_Percentage_Total",
+                    "Page_Views_Total",
+                    "Page_Views_Percentage_Total",
+                    "Featured_Offer_Buy_Box_Percentage",
+                    "Units_Ordered",
+                    "Unit_Session_Percentage",
+                    "Ordered_Product_Sales",
+                    "Total_Order_Items",
+                    "Date"
+                ],
+                "type": "object"
+            },
+            "type": "array"
         },
-        "Units_Placed_Order": {
-            "description": "Total number of units placed in orders during the specified hour",
-            "type": "integer"
+        "siteNickNameId": {
+            "description": "A unique merchant's store code for GRAAS clients",
+            "type": "string"
         }
     },
     "required": [
-        "Date"
+        "merchantID",
+        "siteNickNameId",
+        "countryCode",
+        "currencyCode",
+        "result"
     ],
-    "title": "Shopee Product Overview Hourly Daily Report",
+    "title": "Amazon Product Performance Daily Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Product_Performance_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_Product_Performance_Daily_Report.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'properties'": "{replace: OrderedDict([('merchantID', OrderedDict([('type', 'string'), "*

 * *                 "('description', 'A unique merchant code for GRAAS clients')])), "*

 * *                 '(\'siteNickNameId\', OrderedDict([(\'type\', \'string\'), (\'description\', "A '*

 * *                 'unique merchant\'s store code for GRAAS clients")])), (\'countryCode\', '*

 * *                 'OrderedDict([(\'type\', \'string\'), (\'description\', "The country c […]*

```diff
@@ -1,117 +1,191 @@
 {
+    "$schema": "http://json-schema.org/draft-07/schema#",
     "description": "Daily report presenting the performance metrics for a specific product on Shopee",
     "properties": {
-        "Buyers_Paid_Order": {
-            "description": "Total number of buyers who paid for the orders for the product",
-            "type": "integer"
-        },
-        "Buyers_Placed_Order": {
-            "description": "Total number of buyers who placed an order for the product",
-            "type": "integer"
-        },
-        "Conversion_Rate_Add_to_Cart": {
-            "description": "Conversion rate from product view to adding to cart as a percentage",
-            "type": "number"
-        },
-        "Conversion_Rate_Paid_Order": {
-            "description": "Conversion rate from placing an order to paying for the order as a percentage",
-            "type": "number"
-        },
-        "Conversion_Rate_Placed_Order": {
-            "description": "Conversion rate from product view to placing an order as a percentage",
-            "type": "number"
-        },
-        "Conversion_Rate_Placed_to_Confirmed": {
-            "description": "Conversion rate from placing an order to order confirmation as a percentage",
-            "type": "number"
-        },
-        "Date": {
-            "description": "Date of the report in the format 'MM-DD-YYYY'",
-            "format": "dd-MM-yyyy",
-            "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
-            "type": "string"
-        },
-        "Item_ID": {
-            "description": "Unique identifier for the product item on Shopee",
-            "type": "integer"
-        },
-        "Likes": {
-            "description": "Total number of likes received for the product",
-            "type": "integer"
-        },
-        "Parent_SKU": {
-            "description": "Stock Keeping Unit (SKU) of the parent product (if applicable)",
-            "type": "string"
-        },
-        "Product": {
-            "description": "Name or title of the product",
+        "countryCode": {
+            "description": "The country code, e.g., 'SG', 'MY'.",
             "type": "string"
         },
-        "Product_Bounce_Rate": {
-            "description": "Bounce rate for the product page as a percentage",
-            "type": "number"
-        },
-        "Product_Bounce_Visitors": {
-            "description": "Total number of visitors who bounced from the product page",
-            "type": "integer"
-        },
-        "Product_Page_Views": {
-            "description": "Total number of page views for the product",
-            "type": "integer"
-        },
-        "Product_Visitors_Add_to_Cart": {
-            "description": "Total number of visitors who added the product to the cart",
-            "type": "integer"
-        },
-        "Product_Visitors_Visit": {
-            "description": "Total number of visitors to the product",
-            "type": "integer"
-        },
-        "SKU": {
-            "description": "Stock Keeping Unit (SKU) for the product",
+        "currencyCode": {
+            "description": "The currency code, e.g., 'SGD', 'USD'.",
             "type": "string"
         },
-        "Sales_Paid_Order": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Sales amount information for paid orders",
-            "type": "object"
-        },
-        "Sales_Placed_Order": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Sales amount information for placed orders",
-            "type": "object"
-        },
-        "Search_Clicks": {
-            "description": "Total number of clicks on search related to the product",
-            "type": "integer"
-        },
-        "Units_Add_to_Cart": {
-            "description": "Total number of units added to the cart for the product",
-            "type": "integer"
-        },
-        "Units_Paid_Order": {
-            "description": "Total number of units paid for the orders for the product",
-            "type": "integer"
-        },
-        "Units_Placed_Order": {
-            "description": "Total number of units placed in orders for the product",
-            "type": "integer"
-        },
-        "Variation_ID": {
-            "description": "Unique identifier for the product variation (if applicable)",
-            "type": "string"
+        "merchantID": {
+            "description": "A unique merchant code for GRAAS clients",
+            "type": "string"
+        },
+        "result": {
+            "items": {
+                "properties": {
+                    "Buyers_Paid_Order": {
+                        "description": "Total number of buyers who paid for the orders for the product",
+                        "type": "integer"
+                    },
+                    "Buyers_Placed_Order": {
+                        "description": "Total number of buyers who placed an order for the product",
+                        "type": "integer"
+                    },
+                    "Conversion_Rate_Add_to_Cart": {
+                        "description": "Conversion rate from product view to adding to cart as a percentage",
+                        "type": "number"
+                    },
+                    "Conversion_Rate_Paid_Order": {
+                        "description": "Conversion rate from placing an order to paying for the order as a percentage",
+                        "type": "number"
+                    },
+                    "Conversion_Rate_Placed_Order": {
+                        "description": "Conversion rate from product view to placing an order as a percentage",
+                        "type": "number"
+                    },
+                    "Date": {
+                        "description": "Date of the report in the format 'MM-DD-YYYY'",
+                        "format": "dd-MM-yyyy",
+                        "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
+                        "type": "string"
+                    },
+                    "Item_ID": {
+                        "description": "Unique identifier for the product item on Shopee",
+                        "type": "integer"
+                    },
+                    "Likes": {
+                        "description": "Total number of likes received for the product",
+                        "type": "integer"
+                    },
+                    "Parent_SKU": {
+                        "description": "Stock Keeping Unit (SKU) of the parent product (if applicable)",
+                        "type": "string"
+                    },
+                    "Product": {
+                        "description": "Name or title of the product",
+                        "type": "string"
+                    },
+                    "Product_Bounce_Rate": {
+                        "description": "Bounce rate for the product page as a percentage",
+                        "type": "number"
+                    },
+                    "Product_Bounce_Visitors": {
+                        "description": "Total number of visitors who bounced from the product page",
+                        "type": "integer"
+                    },
+                    "Product_Page_Views": {
+                        "description": "Total number of page views for the product",
+                        "type": "integer"
+                    },
+                    "Product_Visitors_Add_to_Cart": {
+                        "description": "Total number of visitors who added the product to the cart",
+                        "type": "integer"
+                    },
+                    "Product_Visitors_Visit": {
+                        "description": "Total number of visitors to the product",
+                        "type": "integer"
+                    },
+                    "SKU": {
+                        "description": "Stock Keeping Unit (SKU) for the product",
+                        "type": "string"
+                    },
+                    "Sales_Paid_Order": {
+                        "description": "Sales amount information for paid orders",
+                        "properties": {
+                            "amount": {
+                                "description": "The cost amount per conversion.",
+                                "type": "number"
+                            },
+                            "currencyCode": {
+                                "description": "The currency code, e.g., 'SGD', 'USD'.",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "amount",
+                            "currencyCode"
+                        ],
+                        "type": "object"
+                    },
+                    "Sales_Placed_Order": {
+                        "description": "Sales amount information for placed orders",
+                        "properties": {
+                            "amount": {
+                                "description": "The cost amount per conversion.",
+                                "type": "number"
+                            },
+                            "currencyCode": {
+                                "description": "The currency code, e.g., 'SGD', 'USD'.",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "amount",
+                            "currencyCode"
+                        ],
+                        "type": "object"
+                    },
+                    "Search_Clicks": {
+                        "description": "Total number of clicks on search related to the product",
+                        "type": "integer"
+                    },
+                    "Units_Add_to_Cart": {
+                        "description": "Total number of units added to the cart for the product",
+                        "type": "integer"
+                    },
+                    "Units_Paid_Order": {
+                        "description": "Total number of units paid for the orders for the product",
+                        "type": "integer"
+                    },
+                    "Units_Placed_Order": {
+                        "description": "Total number of units placed in orders for the product",
+                        "type": "integer"
+                    },
+                    "Variation_ID": {
+                        "description": "Unique identifier for the product variation (if applicable)",
+                        "type": "string"
+                    },
+                    "Variation_Name": {
+                        "description": "Name of the product variation (if applicable)",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "Item_ID",
+                    "Variation_ID",
+                    "SKU",
+                    "Date",
+                    "Product",
+                    "Variation_Name",
+                    "Parent_SKU",
+                    "Product_Visitors_Visit",
+                    "Product_Page_Views",
+                    "Product_Bounce_Visitors",
+                    "Product_Bounce_Rate",
+                    "Search_Clicks",
+                    "Likes",
+                    "Product_Visitors_Add_to_Cart",
+                    "Units_Add_to_Cart",
+                    "Conversion_Rate_Add_to_Cart",
+                    "Buyers_Placed_Order",
+                    "Units_Placed_Order",
+                    "Sales_Placed_Order",
+                    "Conversion_Rate_Placed_Order",
+                    "Buyers_Paid_Order",
+                    "Units_Paid_Order",
+                    "Sales_Paid_Order",
+                    "Conversion_Rate_Paid_Order"
+                ],
+                "type": "object"
+            },
+            "type": "array"
         },
-        "Variation_Name": {
-            "description": "Name of the product variation (if applicable)",
+        "siteNickNameId": {
+            "description": "A unique merchant's store code for GRAAS clients",
             "type": "string"
         }
     },
     "required": [
-        "Item_ID",
-        "Variation_ID",
-        "SKU",
-        "Date"
+        "merchantID",
+        "siteNickNameId",
+        "countryCode",
+        "currencyCode",
+        "result"
     ],
     "title": "Shopee Product Performance Daily Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_Store_Metrics_Paid_Orders_Daily_monthly_report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Amazon_Store_Key_Metrics_Hourly_Daily_Report.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'description'": "'Hourly daily report presenting key metrics for an Amazon store'",*

 * * "'properties'": "{replace: OrderedDict([('merchantID', OrderedDict([('type', 'string'), "*

 * *                 "('description', 'A unique merchant code for GRAAS clients')])), "*

 * *                 '(\'siteNickNameId\', OrderedDict([(\'type\', \'string\'), (\'description\', "A '*

 * *                 'unique merchant\'s store code for GRAAS clients")])), (\'countryCode\', '*

 * *  […]*

```diff
@@ -1,80 +1,95 @@
 {
-    "description": "Daily and monthly report presenting key metrics for paid orders in a Shopee store",
+    "$schema": "http://json-schema.org/draft-07/schema#",
+    "description": "Hourly daily report presenting key metrics for an Amazon store",
     "properties": {
-        "Cancelled_Orders": {
-            "description": "Total number of cancelled orders",
-            "type": "integer"
-        },
-        "Cancelled_Sales": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Sales amount information for cancelled orders",
-            "type": "object"
-        },
-        "Conversion_Rate_by_paid_order": {
-            "description": "Conversion rate from store visit to paid order as a percentage",
-            "type": "number"
-        },
-        "Date": {
-            "description": "Date of the report in the format 'MM-DD-YYYY'",
-            "format": "dd-MM-yyyy",
-            "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
+        "countryCode": {
+            "description": "The country code, e.g., 'SG', 'MY'.",
             "type": "string"
         },
-        "No_of_buyers": {
-            "description": "Total number of buyers who made a purchase",
-            "type": "integer"
-        },
-        "No_of_existing_buyers": {
-            "description": "Total number of existing buyers",
-            "type": "integer"
-        },
-        "No_of_new_buyers": {
-            "description": "Total number of new buyers",
-            "type": "integer"
-        },
-        "No_of_potential_buyers": {
-            "description": "Total number of potential buyers",
-            "type": "integer"
-        },
-        "Orders": {
-            "description": "Total number of paid orders",
-            "type": "integer"
-        },
-        "Page_Views": {
-            "description": "Total number of page views in the store",
-            "type": "integer"
-        },
-        "Repeat_Purchase_Rate": {
-            "description": "Rate of repeat purchases as a percentage",
-            "type": "number"
-        },
-        "Returned_Refunded_Orders": {
-            "description": "Total number of returned or refunded orders",
-            "type": "integer"
-        },
-        "Returned_Refunded_Sales": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Sales amount information for returned or refunded orders",
-            "type": "object"
+        "currencyCode": {
+            "description": "The currency code, e.g., 'SGD', 'USD'.",
+            "type": "string"
         },
-        "Sales": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Sales information",
-            "type": "object"
+        "merchantID": {
+            "description": "A unique merchant code for GRAAS clients",
+            "type": "string"
         },
-        "Sales_per_Order": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Average sales amount per order information",
-            "type": "object"
+        "result": {
+            "items": {
+                "properties": {
+                    "Same_date_range_one_year_ago_Ordered_product_sales": {
+                        "description": "Ordered product sales amount for the same date range one year ago",
+                        "properties": {
+                            "amount": {
+                                "description": "The cost amount per conversion.",
+                                "type": "number"
+                            },
+                            "currencyCode": {
+                                "description": "The currency code, e.g., 'SGD', 'USD'.",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "amount",
+                            "currencyCode"
+                        ],
+                        "type": "object"
+                    },
+                    "Same_date_range_one_year_ago_Units_ordered": {
+                        "description": "Total number of units ordered for the same date range one year ago",
+                        "type": "integer"
+                    },
+                    "Selected_date_range_Ordered_product_sales": {
+                        "description": "Ordered product sales amount for the selected date range",
+                        "properties": {
+                            "amount": {
+                                "description": "The cost amount per conversion.",
+                                "type": "number"
+                            },
+                            "currencyCode": {
+                                "description": "The currency code, e.g., 'SGD', 'USD'.",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "amount",
+                            "currencyCode"
+                        ],
+                        "type": "object"
+                    },
+                    "Selected_date_range_Units_ordered": {
+                        "description": "Total number of units ordered for the selected date range",
+                        "type": "integer"
+                    },
+                    "Time": {
+                        "description": "Time of the report in the format 'MM-DD-YYYY HH:mm'",
+                        "format": "dd-MM-yyyy HH:mm",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "Time",
+                    "Selected_date_range_Ordered_product_sales",
+                    "Selected_date_range_Units_ordered",
+                    "Same_date_range_one_year_ago_Ordered_product_sales",
+                    "Same_date_range_one_year_ago_Units_ordered"
+                ],
+                "type": "object"
+            },
+            "type": "array"
         },
-        "Visitors": {
-            "description": "Total number of visitors to the store",
-            "type": "integer"
+        "siteNickNameId": {
+            "description": "A unique merchant's store code for GRAAS clients",
+            "type": "string"
         }
     },
     "required": [
-        "Date"
+        "merchantID",
+        "siteNickNameId",
+        "countryCode",
+        "currencyCode",
+        "result"
     ],
-    "title": "Shopee Store Metrics Paid Orders Daily Monthly Report",
+    "title": "Amazon Store Key Metrics Hourly Daily Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_mkp_onsite_campaign_daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Shopee_mkp_onsite_campaign_daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Shopee_onsite_campaign_daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Lazada_Product_Performance_Daily_Report.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'description'": "'Daily report presenting the performance metrics for a specific product on "*

 * *                  "Lazada'",*

 * * "'properties'": "{replace: OrderedDict([('merchantID', OrderedDict([('type', 'string'), "*

 * *                 "('description', 'A unique merchant code for GRAAS clients')])), "*

 * *                 '(\'siteNickNameId\', OrderedDict([(\'type\', \'string\'), (\'description\', "A '*

 * *                 'unique merchant\'s store code for GRAAS clients")])), (\'countryCode\', '*

 * *                 'Ord […]*

```diff
@@ -1,141 +1,186 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "A JSON object representing a Shopee onsite campaign report for a specific product ad.",
+    "description": "Daily report presenting the performance metrics for a specific product on Lazada",
     "properties": {
-        "ACOS": {
-            "description": "Advertising Cost of Sales (ACOS), expressed as a percentage, for the entire campaign.",
-            "type": "number"
-        },
-        "Ads_Type": {
-            "description": "The type of ads used in the campaign, e.g., 'Discovery Ads'.",
-            "type": "string"
-        },
-        "CTR": {
-            "description": "The Click-Through Rate, expressed as a percentage.",
-            "type": "number"
-        },
-        "Clicks": {
-            "description": "The total number of clicks on the ad.",
-            "type": "integer"
-        },
-        "Conversion_Rate": {
-            "description": "The conversion rate, expressed as a percentage, for all conversions.",
-            "type": "number"
-        },
-        "Conversions": {
-            "description": "The total number of desired actions taken due to the campaign, e.g., purchases.",
-            "type": "integer"
-        },
-        "Cost_per_Conversion": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "The cost per conversion with currency information.",
-            "type": "object"
-        },
-        "Cost_per_Direct_Conversion": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "The cost per direct conversion with currency information.",
-            "type": "object"
-        },
-        "Date": {
-            "description": "The date on which this report was generated.",
-            "format": "dd-MM-yyyy",
-            "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
+        "countryCode": {
+            "description": "The country code, e.g., 'SG', 'MY'.",
             "type": "string"
         },
-        "Direct_ACOS": {
-            "description": "Advertising Cost of Sales (ACOS), expressed as a percentage, for direct conversions.",
-            "type": "number"
-        },
-        "Direct_Conversion_Rate": {
-            "description": "The conversion rate, expressed as a percentage, for direct conversions.",
-            "type": "number"
-        },
-        "Direct_Conversions": {
-            "description": "The number of conversions that directly resulted from the campaign.",
-            "type": "integer"
-        },
-        "Direct_GMV": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Gross Merchandise Value for direct sales with currency information.",
-            "type": "object"
-        },
-        "Direct_Items_Sold": {
-            "description": "The number of items directly sold due to the campaign.",
-            "type": "integer"
-        },
-        "Direct_ROAS": {
-            "description": "Return on Ad Spend (ROAS), expressed as a ratio, for direct conversions.",
-            "type": "number"
-        },
-        "End_Date": {
-            "description": "The end date of the campaign. If 'Unlimited,' the campaign has no end date.",
+        "currencyCode": {
+            "description": "The currency code, e.g., 'SGD', 'USD'.",
             "type": "string"
         },
-        "Expense": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "The total campaign expenses with currency information.",
-            "type": "object"
-        },
-        "GMV": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Gross Merchandise Value with currency information.",
-            "type": "object"
-        },
-        "Impression": {
-            "description": "The number of times the ad has been displayed to potential customers.",
-            "type": "integer"
-        },
-        "Items_Sold": {
-            "description": "The total number of items sold as a result of the campaign.",
-            "type": "integer"
-        },
-        "Placement_Keyword": {
-            "description": "The selected placement and keyword targeting for the campaign, e.g., 'All'.",
-            "type": "string"
-        },
-        "Product_CTR": {
-            "description": "The Click-Through Rate (CTR), expressed as a percentage, for the advertised product.",
-            "type": "number"
-        },
-        "Product_Clicks": {
-            "description": "The total clicks related to the advertised product.",
-            "type": "integer"
-        },
-        "Product_ID": {
-            "description": "The unique identifier for the advertised product.",
-            "type": "string"
-        },
-        "Product_Impressions": {
-            "description": "The number of impressions specific to the advertised product.",
-            "type": "integer"
-        },
-        "Product_Name_Ad_Name": {
-            "description": "The name and details of the advertised product.",
-            "type": "string"
-        },
-        "ROAS": {
-            "description": "Return on Ad Spend (ROAS), expressed as a ratio, for the entire campaign.",
-            "type": "number"
-        },
-        "Sequence": {
-            "description": "The sequence or order of this report entry.",
-            "type": "integer"
-        },
-        "Start_Date": {
-            "description": "The start date and time of the campaign.",
-            "type": "string"
+        "merchantID": {
+            "description": "A unique merchant code for GRAAS clients",
+            "type": "string"
+        },
+        "result": {
+            "items": {
+                "properties": {
+                    "Add_to_Cart_Conversion_Rate": {
+                        "description": "Conversion rate from product view to adding to cart as a percentage",
+                        "type": "number"
+                    },
+                    "Add_to_Cart_Units": {
+                        "description": "Total number of units added to the cart for the product",
+                        "type": "integer"
+                    },
+                    "Add_to_Cart_Users": {
+                        "description": "Total number of visitors who added the product to the cart",
+                        "type": "integer"
+                    },
+                    "Buyers": {
+                        "description": "Total number of buyers who made a purchase for the product",
+                        "type": "integer"
+                    },
+                    "Conversion_Rate": {
+                        "description": "Conversion rate from product view to purchase as a percentage",
+                        "type": "number"
+                    },
+                    "Date": {
+                        "description": "Date of the report in the format 'MM-DD-YYYY'",
+                        "format": "dd-MM-yyyy",
+                        "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
+                        "type": "string"
+                    },
+                    "Orders": {
+                        "description": "Total number of orders placed for the product",
+                        "type": "integer"
+                    },
+                    "Product_ID": {
+                        "description": "Unique identifier for the product on Lazada",
+                        "type": "integer"
+                    },
+                    "Product_Name": {
+                        "description": "Name of the product being analyzed",
+                        "type": "string"
+                    },
+                    "Product_Pageviews": {
+                        "description": "Total number of page views for the product",
+                        "type": "integer"
+                    },
+                    "Revenue": {
+                        "description": "Revenue information for the product",
+                        "properties": {
+                            "amount": {
+                                "description": "The cost amount per conversion.",
+                                "type": "number"
+                            },
+                            "currencyCode": {
+                                "description": "The currency code, e.g., 'SGD', 'USD'.",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "amount",
+                            "currencyCode"
+                        ],
+                        "type": "object"
+                    },
+                    "Revenue_per_Buyer": {
+                        "description": "Revenue per buyer information",
+                        "properties": {
+                            "amount": {
+                                "description": "The cost amount per conversion.",
+                                "type": "number"
+                            },
+                            "currencyCode": {
+                                "description": "The currency code, e.g., 'SGD', 'USD'.",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "amount",
+                            "currencyCode"
+                        ],
+                        "type": "object"
+                    },
+                    "SKU_ID": {
+                        "description": "Stock Keeping Unit (SKU) identifier for the product",
+                        "type": "string"
+                    },
+                    "Seller_SKU": {
+                        "description": "Seller Stock Keeping Unit (SKU) for the product",
+                        "type": "string"
+                    },
+                    "URL": {
+                        "description": "URL link to the product on Lazada",
+                        "format": "uri",
+                        "type": "string"
+                    },
+                    "Units_Sold": {
+                        "description": "Total number of units sold for the product",
+                        "type": "integer"
+                    },
+                    "Visitor_Value": {
+                        "description": "Visitor value information",
+                        "properties": {
+                            "amount": {
+                                "description": "The cost amount per conversion.",
+                                "type": "number"
+                            },
+                            "currencyCode": {
+                                "description": "The currency code, e.g., 'SGD', 'USD'.",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "amount",
+                            "currencyCode"
+                        ],
+                        "type": "object"
+                    },
+                    "Visitors": {
+                        "description": "Total number of visitors to the product page",
+                        "type": "integer"
+                    },
+                    "Wishlist_Users": {
+                        "description": "Total number of users who added the product to their wishlist",
+                        "type": "integer"
+                    },
+                    "Wishlists": {
+                        "description": "Total number of times the product was added to wishlists",
+                        "type": "integer"
+                    }
+                },
+                "required": [
+                    "Product_Name",
+                    "Product_ID",
+                    "URL",
+                    "Seller_SKU",
+                    "SKU_ID",
+                    "Visitors",
+                    "Product_Pageviews",
+                    "Visitor_Value",
+                    "Add_to_Cart_Users",
+                    "Add_to_Cart_Units",
+                    "Add_to_Cart_Conversion_Rate",
+                    "Wishlist_Users",
+                    "Wishlists",
+                    "Buyers",
+                    "Orders",
+                    "Units_Sold",
+                    "Revenue",
+                    "Conversion_Rate",
+                    "Revenue_per_Buyer",
+                    "Date"
+                ],
+                "type": "object"
+            },
+            "type": "array"
         },
-        "Status": {
-            "description": "The current status of the campaign, such as 'Ongoing' or 'Completed'.",
+        "siteNickNameId": {
+            "description": "A unique merchant's store code for GRAAS clients",
             "type": "string"
         }
     },
     "required": [
-        "Product_Name_Ad_Name",
-        "Product_ID",
-        "Placement_Keyword",
-        "Date"
+        "merchantID",
+        "siteNickNameId",
+        "countryCode",
+        "currencyCode",
+        "result"
     ],
-    "title": "Shopee Onsite Campaign Report",
+    "title": "Lazada Product Performance Daily Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Tokopedia_Product_Overview_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/graas_flipkart_campaigns.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'description'": "'A JSON object representing a Flipkart Campaign Report'",*

 * * "'properties'": "{replace: OrderedDict([('merchantID', OrderedDict([('type', 'string'), "*

 * *                 "('description', 'A unique merchant code for GRAAS clients')])), "*

 * *                 '(\'siteNickNameId\', OrderedDict([(\'type\', \'string\'), (\'description\', "A '*

 * *                 'unique merchant\'s store code for GRAAS clients")])), (\'countryCode\', '*

 * *           […]*

```diff
@@ -1,37 +1,42 @@
 {
-    "description": "Daily report providing an overview of product-related metrics on Tokopedia",
+    "$schema": "http://json-schema.org/draft-07/schema#",
+    "description": "A JSON object representing a Flipkart Campaign Report",
     "properties": {
-        "Basket": {
-            "description": "Total number of items added to the basket",
-            "type": "integer"
-        },
-        "Conversion": {
-            "description": "Conversion rate as a decimal",
-            "type": "number"
+        "countryCode": {
+            "description": "The country code, e.g., 'SG', 'MY'.",
+            "type": "string"
         },
-        "Date": {
-            "description": "Date of the report in the format 'MM-DD-YYYY'",
-            "format": "dd-MM-yyyy",
-            "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
+        "currencyCode": {
+            "description": "The currency code, e.g., 'SGD', 'USD'.",
             "type": "string"
         },
-        "New_Net_Income": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "Information about new net income",
-            "type": "object"
+        "merchantID": {
+            "description": "A unique merchant code for GRAAS clients",
+            "type": "string"
         },
-        "Product_Viewed": {
-            "description": "Total number of product views",
-            "type": "integer"
+        "result": {
+            "items": {
+                "anyOf": [
+                    {
+                        "$ref": "../graas_utilities/Schema/Flipkart_PLA_Campaign_Seller_Portal_Daily_Report.json",
+                        "description": "Flipkart PLA Campaign Seller Portal Daily Report"
+                    }
+                ]
+            },
+            "type": "array"
         },
-        "Sold_Products": {
-            "description": "Total number of products sold",
-            "type": "integer"
+        "siteNickNameId": {
+            "description": "A unique merchant's store code for GRAAS clients",
+            "type": "string"
         }
     },
     "required": [
-        "Date"
+        "merchantID",
+        "siteNickNameId",
+        "countryCode",
+        "currencyCode",
+        "result"
     ],
-    "title": "Tokopedia Product Overview Daily Report",
+    "title": "Flipkart Campaign Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Tokopedia_Product_Performance_Daily_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Tokopedia_Product_Overview_Daily_Report.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'description'": "'Daily report providing an overview of product-related metrics on Tokopedia'",*

 * * "'properties'": "{replace: OrderedDict([('merchantID', OrderedDict([('type', 'string'), "*

 * *                 "('description', 'A unique merchant code for GRAAS clients')])), "*

 * *                 '(\'siteNickNameId\', OrderedDict([(\'type\', \'string\'), (\'description\', "A '*

 * *                 'unique merchant\'s store code for GRAAS clients")])), (\'countr […]*

```diff
@@ -1,58 +1,86 @@
 {
-    "description": "Daily report presenting the performance metrics for a specific product on Tokopedia",
+    "$schema": "http://json-schema.org/draft-07/schema#",
+    "description": "Daily report providing an overview of product-related metrics on Tokopedia",
     "properties": {
-        "Basket": {
-            "description": "Total number of times the product was added to the shopping basket",
-            "type": "integer"
-        },
-        "Category": {
-            "description": "Category to which the product belongs",
-            "type": "string"
-        },
-        "Conversion": {
-            "description": "Conversion rate of the product as a decimal",
-            "type": "number"
-        },
-        "Date": {
-            "description": "Date of the report in the format 'MM-DD-YYYY'",
-            "format": "dd-MM-yyyy",
-            "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
+        "countryCode": {
+            "description": "The country code, e.g., 'SG', 'MY'.",
             "type": "string"
         },
-        "New_Net_Income": {
-            "$ref": "../Schema/amount_currency_code_object.json",
-            "description": "New net income information for the product",
-            "type": "object"
-        },
-        "Order": {
-            "description": "Total number of orders placed for the product",
-            "type": "integer"
-        },
-        "Product_Viewed": {
-            "description": "Total number of times the product was viewed",
-            "type": "integer"
-        },
-        "Product_name": {
-            "description": "Name of the product being analyzed",
+        "currencyCode": {
+            "description": "The currency code, e.g., 'SGD', 'USD'.",
             "type": "string"
         },
-        "SKU": {
-            "description": "Stock Keeping Unit (SKU) of the product",
+        "merchantID": {
+            "description": "A unique merchant code for GRAAS clients",
             "type": "string"
         },
-        "Sold_Products": {
-            "description": "Total number of units sold for the product",
-            "type": "integer"
+        "result": {
+            "items": {
+                "properties": {
+                    "Basket": {
+                        "description": "Total number of items added to the basket",
+                        "type": "integer"
+                    },
+                    "Conversion": {
+                        "description": "Conversion rate as a decimal",
+                        "type": "number"
+                    },
+                    "Date": {
+                        "description": "Date of the report in the format 'MM-DD-YYYY'",
+                        "format": "dd-MM-yyyy",
+                        "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
+                        "type": "string"
+                    },
+                    "New_Net_Income": {
+                        "properties": {
+                            "amount": {
+                                "description": "The cost amount per conversion.",
+                                "type": "number"
+                            },
+                            "currencyCode": {
+                                "description": "The currency code, e.g., 'SGD', 'USD'.",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "amount",
+                            "currencyCode"
+                        ],
+                        "type": "object"
+                    },
+                    "Product_Viewed": {
+                        "description": "Total number of product views",
+                        "type": "integer"
+                    },
+                    "Sold_Products": {
+                        "description": "Total number of products sold",
+                        "type": "integer"
+                    }
+                },
+                "required": [
+                    "Date",
+                    "New_Net_Income",
+                    "Sold_Products",
+                    "Product_Viewed",
+                    "Basket",
+                    "Conversion"
+                ],
+                "type": "object"
+            },
+            "type": "array"
         },
-        "Wishlist": {
-            "description": "Total number of times the product was added to the wishlist",
-            "type": "integer"
+        "siteNickNameId": {
+            "description": "A unique merchant's store code for GRAAS clients",
+            "type": "string"
         }
     },
     "required": [
-        "SKU",
-        "Date"
+        "merchantID",
+        "siteNickNameId",
+        "countryCode",
+        "currencyCode",
+        "result"
     ],
-    "title": "Tokopedia Product Performance Daily Report",
+    "title": "Tokopedia Product Overview Daily Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Daily_monthly_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Daily_monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Monthly_Report.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/amount_currency_code_object.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/amount_currency_code_object.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/graas_amazon_campaigns.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/graas_amazon_campaigns.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/graas_flipkart_campaigns.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_onsite_keywords.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8325520833333333%*

 * *Differences: {"'description'": "'A JSON object representing a Campaign Onsite Keywords'",*

 * * "'properties'": "{'result': {'items': {'anyOf': {1: {'$ref': "*

 * *                 "'../graas_utilities/Schema/Lazada_Keywords_Onsite_daily_Report.json', "*

 * *                 "'description': 'Lazada Keywords Onsite daily report'}, insert: [(0, "*

 * *                 "OrderedDict([('$ref', "*

 * *                 "'../graas_utilities/Schema/Shopee_Keywords_Onsite_daily_Report.json'), "*

 * *                 "('description', 'Shopee Keywords Onsite da […]*

```diff
@@ -1,10 +1,10 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "A JSON object representing a Flipkart Campaign Report",
+    "description": "A JSON object representing a Campaign Onsite Keywords",
     "properties": {
         "countryCode": {
             "description": "The country code, e.g., 'SG', 'MY'.",
             "type": "string"
         },
         "currencyCode": {
             "description": "The currency code, e.g., 'SGD', 'USD'.",
@@ -14,16 +14,20 @@
             "description": "A unique merchant code for GRAAS clients",
             "type": "string"
         },
         "result": {
             "items": {
                 "anyOf": [
                     {
-                        "$ref": "../graas_utilities/Schema/Flipkart_PLA_Campaign_Seller_Portal_Daily_Report.json",
-                        "description": "Flipkart PLA Campaign Seller Portal Daily Report"
+                        "$ref": "../graas_utilities/Schema/Shopee_Keywords_Onsite_daily_Report.json",
+                        "description": "Shopee Keywords Onsite daily Report"
+                    },
+                    {
+                        "$ref": "../graas_utilities/Schema/Lazada_Keywords_Onsite_daily_Report.json",
+                        "description": "Lazada Keywords Onsite daily report"
                     }
                 ]
             },
             "type": "array"
         },
         "siteNickNameId": {
             "description": "A unique merchant's store code for GRAAS clients",
@@ -33,10 +37,10 @@
     "required": [
         "merchantID",
         "siteNickNameId",
         "countryCode",
         "currencyCode",
         "result"
     ],
-    "title": "Flipkart Campaign Report",
+    "title": "Campaign Onsite Keywords",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_affiliate_report_daily.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_affiliate_report_daily.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_deals_overview_daily.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_deals_overview_daily.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_deals_trends_daily.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_deals_trends_daily.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_offsite_campaigns.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_offsite_campaigns.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_onsite_campaigns.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_traffic_overview_hourly.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8325520833333333%*

 * *Differences: {"'description'": "'A JSON object representing a Traffic Overview hourly Report for a specific "*

 * *                  "campaign.'",*

 * * "'properties'": "{'result': {'items': {'anyOf': {0: {'$ref': "*

 * *                 "'../graas_utilities/Schema/Shopee_Traffic_Overview_Daily_Monthly_Report.json', "*

 * *                 "'description': 'Shopee Traffic Overview Daily Monthly Report'}, delete: [0]}}}}",*

 * * "'title'": "'Traffic Overview hourly Report'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "A JSON object representing a Onsite campaign report for a specific campaign.",
+    "description": "A JSON object representing a Traffic Overview hourly Report for a specific campaign.",
     "properties": {
         "countryCode": {
             "description": "The country code, e.g., 'SG', 'MY'.",
             "type": "string"
         },
         "currencyCode": {
             "description": "The currency code, e.g., 'SGD', 'USD'.",
@@ -14,20 +14,16 @@
             "description": "A unique merchant code for GRAAS clients",
             "type": "string"
         },
         "result": {
             "items": {
                 "anyOf": [
                     {
-                        "$ref": "../graas_utilities/Schema/Lazada_onsite_campaign_monthly_Report.json",
-                        "description": "Lazada Onsite Campaign Report"
-                    },
-                    {
-                        "$ref": "../graas_utilities/Schema/Shopee_onsite_campaign_daily_Report.json",
-                        "description": "Shopee Onsite Campaign Report"
+                        "$ref": "../graas_utilities/Schema/Shopee_Traffic_Overview_Daily_Monthly_Report.json",
+                        "description": "Shopee Traffic Overview Daily Monthly Report"
                     }
                 ]
             },
             "type": "array"
         },
         "siteNickNameId": {
             "description": "A unique merchant's store code for GRAAS clients",
@@ -37,10 +33,10 @@
     "required": [
         "merchantID",
         "siteNickNameId",
         "countryCode",
         "currencyCode",
         "result"
     ],
-    "title": "Onsite Campaign Report",
+    "title": "Traffic Overview hourly Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_product_campaign_performance.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_product_campaign_performance.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_product_overview_daily.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_traffic_overview_daily.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8326388888888889%*

 * *Differences: {"'description'": "'A JSON object representing a Traffic Overview Daily Report'",*

 * * "'properties'": "{'result': {'items': {'anyOf': {2: {'$ref': "*

 * *                 "'../graas_utilities/Schema/Amazon_Traffic_Metrics_Daily_Report.json', "*

 * *                 "'description': 'Amazon Traffic Metrics Daily Report'}, 3: {'$ref': "*

 * *                 "'../graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json', "*

 * *                 "'description': 'Tokopedia Customer Insight Daily Report'}, 4: {'$ref': "*

 * *     […]*

```diff
@@ -1,10 +1,10 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "A JSON object representing a Product Overview Daily Report ",
+    "description": "A JSON object representing a Traffic Overview Daily Report",
     "properties": {
         "countryCode": {
             "description": "The country code, e.g., 'SG', 'MY'.",
             "type": "string"
         },
         "currencyCode": {
             "description": "The currency code, e.g., 'SGD', 'USD'.",
@@ -14,28 +14,36 @@
             "description": "A unique merchant code for GRAAS clients",
             "type": "string"
         },
         "result": {
             "items": {
                 "anyOf": [
                     {
-                        "$ref": "../graas_utilities/Schema/Tokopedia_Product_Overview_Daily_Report.json",
-                        "description": "Tokopedia Product Overview Daily Report"
+                        "$ref": "../graas_utilities/Schema/Shopee_Traffic_Overview_Daily_Monthly_Report.json",
+                        "description": "Shopee Traffic Overview Daily Monthly Report"
                     },
                     {
-                        "$ref": "../graas_utilities/Schema/Amazon_Store_Key_Metrics_Daily_Report.json",
-                        "description": "Amazon Store Key Metrics Daily Report "
+                        "$ref": "../graas_utilities/Schema/Lazada_Store_Key_Metrics_monthly_Report.json",
+                        "description": "Lazada Store Key Metrics Monthly Report"
                     },
                     {
-                        "$ref": "../graas_utilities/Schema/Lazada_Store_Key_Metrics_monthly_Report.json",
-                        "description": "Lazada Store Key Metrics monthly Report"
+                        "$ref": "../graas_utilities/Schema/Amazon_Traffic_Metrics_Daily_Report.json",
+                        "description": "Amazon Traffic Metrics Daily Report"
+                    },
+                    {
+                        "$ref": "../graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json",
+                        "description": "Tokopedia Customer Insight Daily Report"
+                    },
+                    {
+                        "$ref": "../graas_utilities/Schema/Flipkart_Search_Traffic_Report_Daily_Report.json",
+                        "description": "Amazon Traffic Metrics Daily Report"
                     },
                     {
-                        "$ref": "../graas_utilities/Schema/Shopee_Product_Overview_Daily_Monthly_Report.json",
-                        "description": "Shopee Product Overview Daily Monthly Report"
+                        "$ref": "../graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Monthly_Report.json",
+                        "description": "Amazon Traffic Metrics Daily Report"
                     }
                 ]
             },
             "type": "array"
         },
         "siteNickNameId": {
             "description": "A unique merchant's store code for GRAAS clients",
@@ -45,10 +53,10 @@
     "required": [
         "merchantID",
         "siteNickNameId",
         "countryCode",
         "currencyCode",
         "result"
     ],
-    "title": "Product Overview Daily Report",
+    "title": "Traffic Overview Daily Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_product_overview_hourly.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_shop_stats_hourly.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8330729166666666%*

 * *Differences: {"'description'": "'A JSON object representing a Shop Stats Hourly Report '",*

 * * "'properties'": "{'result': {'items': {'anyOf': {0: {'$ref': "*

 * *                 "'../graas_utilities/Schema/Shopee_store_Metrics_Placed_Order_Hourly_Daily_report.json', "*

 * *                 "'description': 'Shopee store Metrics Placed Order Hourly Daily report'}}}}}",*

 * * "'title'": "'Shop Stats Hourly Report'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "A JSON object representing a Product Overview Hourly Report ",
+    "description": "A JSON object representing a Shop Stats Hourly Report ",
     "properties": {
         "countryCode": {
             "description": "The country code, e.g., 'SG', 'MY'.",
             "type": "string"
         },
         "currencyCode": {
             "description": "The currency code, e.g., 'SGD', 'USD'.",
@@ -14,16 +14,16 @@
             "description": "A unique merchant code for GRAAS clients",
             "type": "string"
         },
         "result": {
             "items": {
                 "anyOf": [
                     {
-                        "$ref": "../graas_utilities/Schema/Shopee_Product_Overview_Hourly_Daily_Report.json",
-                        "description": "Shopee Product Overview Hourly Daily Report"
+                        "$ref": "../graas_utilities/Schema/Shopee_store_Metrics_Placed_Order_Hourly_Daily_report.json",
+                        "description": "Shopee store Metrics Placed Order Hourly Daily report"
                     },
                     {
                         "$ref": "../graas_utilities/Schema/Amazon_Store_Key_Metrics_Hourly_Daily_Report.json",
                         "description": "Amazon Store Key Metrics Hourly Daily Report"
                     }
                 ]
             },
@@ -37,10 +37,10 @@
     "required": [
         "merchantID",
         "siteNickNameId",
         "countryCode",
         "currencyCode",
         "result"
     ],
-    "title": "Product Overview Hourly Report",
+    "title": "Shop Stats Hourly Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_product_performance.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_shop_stats_daily.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8325892857142857%*

 * *Differences: {"'description'": "'A JSON object representing a Shop Stats Daily Report '",*

 * * "'properties'": "{'result': {'items': {'anyOf': {3: {'$ref': "*

 * *                 "'../graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Daily_monthly_Report.json', "*

 * *                 "'description': 'Tokopedia Store Key Metrics Daily report'}, 4: {'$ref': "*

 * *                 "'../graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json', "*

 * *                 "'description': 'Tokopedia Customer Insight Daily report'}, 5: {' […]*

```diff
@@ -1,10 +1,10 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "A JSON object representing a Product Performance Report ",
+    "description": "A JSON object representing a Shop Stats Daily Report ",
     "properties": {
         "countryCode": {
             "description": "The country code, e.g., 'SG', 'MY'.",
             "type": "string"
         },
         "currencyCode": {
             "description": "The currency code, e.g., 'SGD', 'USD'.",
@@ -14,28 +14,40 @@
             "description": "A unique merchant code for GRAAS clients",
             "type": "string"
         },
         "result": {
             "items": {
                 "anyOf": [
                     {
-                        "$ref": "../graas_utilities/Schema/Shopee_Product_Performance_Daily_Report.json",
-                        "description": "Shopee Product Performance Daily report"
+                        "$ref": "../graas_utilities/Schema/Lazada_Store_Key_Metrics_monthly_Report.json",
+                        "description": "Lazada Store Key Metrics monthly Report"
                     },
                     {
-                        "$ref": "../graas_utilities/Schema/Lazada_Product_Performance_Daily_Report.json",
-                        "description": "Lazada Product Performance Daily report"
+                        "$ref": "../graas_utilities/Schema/Shopee_Store_Metrics_Paid_Orders_Daily_monthly_report.json",
+                        "description": "Shopee Store Metrics Paid Orders Daily monthly report"
                     },
                     {
-                        "$ref": "../graas_utilities/Schema/Amazon_Product_Performance_Daily_Report.json",
-                        "description": "Amazon Product Performance Daily report"
+                        "$ref": "../graas_utilities/Schema/Amazon_Store_Key_Metrics_Daily_Report.json",
+                        "description": "Amazon Store Key Metrics Daily report"
                     },
                     {
-                        "$ref": "../graas_utilities/Schema/Tokopedia_Product_Performance_Daily_Report.json",
-                        "description": "Tokopedia Product Performance Daily report"
+                        "$ref": "../graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Daily_monthly_Report.json",
+                        "description": "Tokopedia Store Key Metrics Daily report"
+                    },
+                    {
+                        "$ref": "../graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json",
+                        "description": "Tokopedia Customer Insight Daily report"
+                    },
+                    {
+                        "$ref": "../graas_utilities/Schema/Lazada_Customers_Insight_monthly_Report.json",
+                        "description": "Lazada Customers Insight monthly Report"
+                    },
+                    {
+                        "$ref": "../graas_utilities/Schema/Amazon_Traffic_Metrics_Daily_Report.json",
+                        "description": "Amazon Traffic Metrics Daily report"
                     }
                 ]
             },
             "type": "array"
         },
         "siteNickNameId": {
             "description": "A unique merchant's store code for GRAAS clients",
@@ -45,10 +57,10 @@
     "required": [
         "merchantID",
         "siteNickNameId",
         "countryCode",
         "currencyCode",
         "result"
     ],
-    "title": "Product Performance Report",
+    "title": "Shop Stats Daily Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/Schema/graas_mkp_traffic_overview_daily.json` & `graas-observability-utility-1.6.2/graas_utilities/Schema/graas_mkp_voucher_performance_daily.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8325954861111112%*

 * *Differences: {"'description'": "'A JSON object representing a Voucher Performance Daily Report'",*

 * * "'properties'": "{'result': {'items': {'anyOf': {0: {'$ref': "*

 * *                 "'../graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Detailed_Overview_Daily_Report.json', "*

 * *                 "'description': 'Shopee Marketing Shipping Fee Promotion Detailed Overview Daily "*

 * *                 "Report'}, 1: {'$ref': "*

 * *                 "'../graas_utilities/Schema/Shopee_Marketing_Voucher_Performance_Daily_Report.j […]*

```diff
@@ -1,10 +1,10 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "A JSON object representing a Traffic Overview Daily Report",
+    "description": "A JSON object representing a Voucher Performance Daily Report",
     "properties": {
         "countryCode": {
             "description": "The country code, e.g., 'SG', 'MY'.",
             "type": "string"
         },
         "currencyCode": {
             "description": "The currency code, e.g., 'SGD', 'USD'.",
@@ -14,36 +14,24 @@
             "description": "A unique merchant code for GRAAS clients",
             "type": "string"
         },
         "result": {
             "items": {
                 "anyOf": [
                     {
-                        "$ref": "../graas_utilities/Schema/Shopee_Traffic_Overview_Daily_Monthly_Report.json",
-                        "description": "Shopee Traffic Overview Daily Monthly Report"
+                        "$ref": "../graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Detailed_Overview_Daily_Report.json",
+                        "description": "Shopee Marketing Shipping Fee Promotion Detailed Overview Daily Report"
                     },
                     {
-                        "$ref": "../graas_utilities/Schema/Lazada_Store_Key_Metrics_monthly_Report.json",
-                        "description": "Lazada Store Key Metrics Monthly Report"
-                    },
-                    {
-                        "$ref": "../graas_utilities/Schema/Amazon_Traffic_Metrics_Daily_Report.json",
-                        "description": "Amazon Traffic Metrics Daily Report"
-                    },
-                    {
-                        "$ref": "../graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json",
-                        "description": "Tokopedia Customer Insight Daily Report"
-                    },
-                    {
-                        "$ref": "../graas_utilities/Schema/Flipkart_Search_Traffic_Report_Daily_Report.json",
-                        "description": "Amazon Traffic Metrics Daily Report"
+                        "$ref": "../graas_utilities/Schema/Shopee_Marketing_Voucher_Performance_Daily_Report.json",
+                        "description": "Shopee Marketing Voucher Performance Daily Report"
                     },
                     {
                         "$ref": "../graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Monthly_Report.json",
-                        "description": "Amazon Traffic Metrics Daily Report"
+                        "description": "Tokopedia Store Key Metrics Monthly Report"
                     }
                 ]
             },
             "type": "array"
         },
         "siteNickNameId": {
             "description": "A unique merchant's store code for GRAAS clients",
@@ -53,10 +41,10 @@
     "required": [
         "merchantID",
         "siteNickNameId",
         "countryCode",
         "currencyCode",
         "result"
     ],
-    "title": "Traffic Overview Daily Report",
+    "title": "Voucher Performance Daily Report",
     "type": "object"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/configs.py` & `graas-observability-utility-1.6.2/graas_utilities/configs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 mappingObject = {
     "shopee_trafficOverview": "graas_mkp_traffic_overview_hourly",
     "shopee_trafficOverviewMonthly": "graas_mkp_traffic_overview_daily",
     "shopee_storeKeyMetrics": "graas_mkp_shop_stats_daily",
     "shopee_storeKeyMetricsMonthly": "graas_mkp_shop_stats_daily",
-    "shopee_productOverview": "graas_mkp_product_overview_hourly",
-    "shopee_productOverviewMonthly": "graas_mkp_product_overview_daily",
-    "shopee_onsiteCampaign": "graas_mkp_onsite_campaigns",
+    "shopee_productOverview": "Shopee_Product_Overview_Hourly_Daily_Report",
+    "shopee_productOverviewMonthly": "Shopee_Product_Overview_Daily_Monthly_Report",
+    "shopee_onsiteCampaign": "Shopee_mkp_onsite_campaign_daily_Report",
     "shopee_onsiteKeyword": "graas_mkp_onsite_keywords",
-    "shopee_productPerformance": "graas_mkp_product_performance",
+    "shopee_productPerformance": "Shopee_Product_Performance_Daily_Report",
     "shopee_marketingAddOnDeal": "graas_mkp_deals_overview_daily",
     "shopee_marketingAddOnDealMonthly": "graas_mkp_deals_trends_daily",
     "shopee_marketingShippingFeePromotion": "graas_mkp_voucher_performance_daily",
     "shopee_marketingShippingFeePromotionMonthly": "graas_mkp_deals_trends_daily",
     "shopee_marketingVoucher": "graas_mkp_voucher_performance_daily",
     "shopee_marketingVoucherMonthly": "graas_mkp_deals_trends_daily",
     "shopee_marketingBundleDeal": "graas_mkp_deals_overview_daily",
     "shopee_marketingBundleDealMonthly": "graas_mkp_deals_trends_daily",
     "shopee_marketingFlashDeal": "graas_mkp_deals_overview_daily",
     "shopee_marketingFlashDealMonthly": "graas_mkp_deals_trends_daily",
-    "shopee_productPerformanceAfterReturnPeriod": "graas_mkp_product_performance",
-    "shopee_onsiteCampaignAfterReturnPeriod": "graas_mkp_onsite_campaigns",
-    "shopee_productOverviewMonthlyBackFill": "graas_mkp_product_overview_daily",
+    "shopee_productPerformanceAfterReturnPeriod": "Shopee_Product_Performance_Daily_Report",
+    "shopee_onsiteCampaignAfterReturnPeriod": "Shopee_mkp_onsite_campaign_daily_Report",
+    "shopee_productOverviewMonthlyBackFill": "Shopee_Product_Overview_Daily_Monthly_Report",
     "shopee_marketingVoucherMonthlyBackFill": "graas_mkp_deals_trends_daily",
     "shopee_marketingShippingFeePromotionMonthlyBackFill": "graas_mkp_deals_trends_daily",
     "shopee_storeKeyMetricsMonthlyBackFill": "graas_mkp_shop_stats_daily",
     "shopee_marketingAddOnDealMonthlyBackFill": "graas_mkp_deals_trends_daily",
     "shopee_marketingBundleDealMonthlyBackFill": "graas_mkp_deals_trends_daily",
     "shopee_marketingFlashDealMonthlyBackFill": "graas_mkp_deals_trends_daily",
     "shopee_trafficOverviewMonthlyBackFill": "graas_mkp_traffic_overview_daily",
     "lazada_offsite": "graas_mkp_offsite_campaigns",
     "lazada_onsiteKeyword": "graas_mkp_onsite_keywords",
     "lazada_customerInsight": "graas_mkp_shop_stats_daily",
     "lazada_customerInsightMonthly": "graas_mkp_shop_stats_daily",
     "lazada_storeKeyMetrics": "graas_mkp_shop_stats_daily",
     "lazada_storeKeyMetricsMonthly": "graas_mkp_shop_stats_daily",
-    "lazada_sponsoredDiscoveryReport": "graas_mkp_onsite_campaigns",
-    "lazada_sponsoredDiscoveryReportMonthly": "graas_mkp_onsite_campaigns",
+    "lazada_sponsoredDiscoveryReport": "Lazada_mkp_onsite_campaign_monthly_Report",
+    "lazada_sponsoredDiscoveryReportMonthly": "Lazada_mkp_onsite_campaign_monthly_Report",
     "lazada_sponsoredAffiliateReport": "graas_mkp_affiliate_report_daily",
     "lazada_sponsoredAffiliateReportMonthly": "graas_mkp_affiliate_report_daily",
-    "lazada_productPerformance": "graas_mkp_product_performance",
-    "lazada_productPerformanceAfterReturnPeriod": "graas_mkp_product_performance",
+    "lazada_productPerformance": "Lazada_Product_Performance_Daily_Report",
+    "lazada_productPerformanceAfterReturnPeriod": "Lazada_Product_Performance_Daily_Report",
     "lazada_storeKeyMetricsMonthlyBackFill": "graas_mkp_shop_stats_daily",
-    "lazada_sponsoredDiscoveryReportMonthlyBackFill": "graas_mkp_onsite_campaigns",
+    "lazada_sponsoredDiscoveryReportMonthlyBackFill": "Lazada_mkp_onsite_campaign_monthly_Report",
     "lazada_sponsoredAffiliateReportMonthlyBackFill": "graas_mkp_affiliate_report_daily",
     "lazada_customerInsightMonthlyBackFill": "graas_mkp_shop_stats_daily",
     "amazon_onsiteSponsoredDisplayCampaign": "graas_amazon_campaigns",
     "amazon_onsiteSponsoredProductsCampaign":"graas_amazon_campaigns",
     "amazon_onsiteSponsoredBrandsCampaign":"graas_amazon_campaigns",
     "amazon_trafficKeyMetrics":"graas_mkp_traffic_overview_daily",
-    "amazon_storeKeyMetrics":"graas_mkp_product_overview_daily",
+    "amazon_storeKeyMetrics":"Amazon_Store_Key_Metrics_Daily_Report",
     "amazon_returnOrderReport":"graas_mkp_returned_orders_daily",
-    "amazon_productPerformance":"graas_mkp_product_performance",
+    "amazon_productPerformance":"Amazon_Product_Performance_Daily_Report",
     "amazon_sponsoredDisplayAdvertisedProduct":"graas_mkp_product_campaign_performance",
     "amazon_sponsoredProductsAdvertisedProduct":"graas_mkp_product_campaign_performance",
     "amazon_sponsoredBrandsAttributedPurchases":"graas_mkp_product_campaign_performance",
     "amazon_storeKeyMetricsMonthly":"graas_mkp_shop_stats_daily",
     "amazon_trafficKeyMetricsMonthly":"graas_mkp_shop_stats_daily",
     "amazon_storeKeyMetricsMonthlyBackFill":"graas_mkp_shop_stats_daily",
     "amazon_trafficKeyMetricsMonthlyBackFill":"graas_mkp_shop_stats_daily",
@@ -66,13 +66,13 @@
     "flipkart_PLAConsolidatedFSN":"graas_mkp_product_campaign_performance",
     "flipkart_PLAConsolidatedFSNSellerPortal":"graas_mkp_product_campaign_performance",
     "flipkart_PCAProductPagePerformance":"graas_mkp_product_campaign_performance",
     "flipkart_searchTrafficReport":"graas_mkp_traffic_overview_daily",
     "tokopedia_storeKeyMetrics":"graas_mkp_traffic_overview_daily",
     "tokopedia_storeKeyMetricsMonthly":"graas_mkp_shop_stats_daily",
     "tokopedia_trafficOverview":"graas_mkp_traffic_overview_daily",
-    "tokopedia_productReport":"graas_mkp_product_overview_daily",
+    "tokopedia_productReport":"Tokopedia_Product_Overview_Daily_Report",
     "tokopedia_customerInsight":"graas_mkp_traffic_overview_daily",
     "tokopedia_customerInsightMonthly":"graas_mkp_shop_stats_daily",
     "tokopedia_customerInsightMonthlyBackFill":"graas_mkp_shop_stats_daily",
     "tokopedia_storeKeyMetricsMonthlyBackFill":"graas_mkp_shop_stats_daily"
 }
```

### Comparing `graas-observability-utility-1.6.1/graas_utilities/ref_Resolver.py` & `graas-observability-utility-1.6.2/graas_utilities/ref_Resolver.py`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.1/graas_utilities/validation.py` & `graas-observability-utility-1.6.2/graas_utilities/validation.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,24 +13,30 @@
             schema,
             resolver=ExtendedRefResolver(
                 base_uri=resource_filename(__name__, '/Schema'),
                 referrer=schema,
             ),
         )
     except jsonschema.exceptions.ValidationError as err:
-        return {"status": "SCHEMA_VALIDATION_FAILED", "message": err.message}
+        validation_msg = err.message
+        if err.validator == "type" and len(err.path) > 0:
+            key = err.path[len(err.path) - 1]
+            validation_msg = f"{key} field should be a {err.validator_value}"
+        return {"status": "SCHEMA_VALIDATION_FAILED", "message": validation_msg}   
+    except Exception as err:
+        return {"status": "SCHEMA_VALIDATION_FAILED", "message": err}    
     return {
         "status": "SCHEMA_VALIDATION_SUCCESS",
         "message": "Schema successfully validated",
     }
 
 
 def extract_data_from_file(schema_file):
     path_for_schema = resource_filename(__name__, '/Schema')
-
+    
     with open(f"{path_for_schema}/{schema_file}.json", "r") as schema_file:
         schemaObj = json.load(schema_file)
 
     return schemaObj
 
 
 def validateJson(dataJsonString, reportType):
@@ -43,32 +49,33 @@
         "shopee_productSponsoredAffiliateReport",
         "shopee_onsiteCampaign",
         "shopee_onsiteCampaignAfterReturnPeriod",
         "shopee_onsiteKeyword",
         "shopee_marketingShippingFeePromotion",
         "shopee_marketingShippingFeePromotionMonthly",
         "shopee_marketingShippingFeePromotionMonthlyBackFill",
-        "shopee_productOverview",
-        "shopee_productOverviewMonthly",
-        "shopee_productOverviewMonthlyBackFill",
         "shopee_storeKeyMetricsMonthlyBackFill",
+        "lazada_sponsoredDiscoveryReport",
+        "lazada_sponsoredDiscoveryReportMonthly",
+        "lazada_sponsoredDiscoveryReportMonthlyBackFill",
         "lazada_storeKeyMetrics",
         "lazada_storeKeyMetricsMonthly",
         "lazada_storeKeyMetricsMonthlyBackFill",
         "lazada_onsiteKeyword",
         "flipkart_storeRevenue",
         "flipkart_PLAConsolidatedFSNSellerPortal",
         "flipkart_BrandAdsCampaign",
         "flipkart_DisplayAdsCampaign",
         "flipkart_PLAConsolidatedFSN",
         "flipkart_PCACampaign",
         "flipkart_PLACampaign",
         "flipkart_PLACampaignSellerPortal",
         "flipkart_searchTrafficReport",
-        "flipkart_PCAProductPagePerformance"
+        "flipkart_PCAProductPagePerformance",
+        "tokopedia_productReport"
     ]
 
     if reportType is None or not reportType:
         return {
             "status": "SCHEMA_VALIDATION_FAILED",
             "message": "Report type is Empty or None please enter valid string value!"
         }
```

### Comparing `graas-observability-utility-1.6.1/setup.py` & `graas-observability-utility-1.6.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 	'Programming Language :: Python :: 3.3', 
 	'Programming Language :: Python :: 3.4', 
 	'Programming Language :: Python :: 3.8', 
 	]
 
 # calling the setup function 
 setup(name='graas-observability-utility', 
-	version='1.6.1', 
+	version='1.6.2', 
 	description='A small wrapper around data observability', 
 	# long_description=long_description, 
 	url='https://bitbucket.org/shoptimizeanalytics/graas-observability-utility', 
 	author='Graas', 
 	author_email='priyanka.patel@graas.ai', 
 	# license='MIT',
     packages=find_packages(),
```

