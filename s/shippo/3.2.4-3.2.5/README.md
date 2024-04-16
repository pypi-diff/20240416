# Comparing `tmp/shippo-3.2.4.tar.gz` & `tmp/shippo-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shippo-3.2.4.tar", last modified: Mon Apr 15 16:54:49 2024, max compression
+gzip compressed data, was "shippo-3.2.5.tar", last modified: Tue Apr 16 19:34:35 2024, max compression
```

## Comparing `shippo-3.2.4.tar` & `shippo-3.2.5.tar`

### file list

```diff
@@ -1,251 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.586234 shippo-3.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-15 16:54:49.586234 shippo-3.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-15 16:54:39.000000 shippo-3.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:54:49.586234 shippo-3.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-15 16:54:39.000000 shippo-3.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.550234 shippo-3.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.554234 shippo-3.2.4/src/shippo/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.554234 shippo-3.2.4/src/shippo/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14334 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)    19782 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/batches.py
--rw-r--r--   0 runner    (1001) docker     (127)    28938 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/carrier_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/carrier_parcel_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/customs_declarations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/customs_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/manifests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.554234 shippo-3.2.4/src/shippo/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.574234 shippo-3.2.4/src/shippo/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/addresscompletecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/addresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/addressimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/addresspaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/addressvalidationresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/addressvalidationresultsmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/alcohol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/batchcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/batchshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/batchshipmentbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/batchshipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountdpddecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountfedexcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountupscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountuspscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountwithextrainfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carriers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/cod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/connectexistingownaccountrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customerreference.py
--rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customsdeclarationcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customsdeclarationpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customsexporteridentification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customsinvoicedcharges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customsitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customsitempaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customstaxidentification.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/dangerousgoodslithiumbatteries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/dangerousgoodsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/defaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/defaultparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/departmentnumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/distanceunit.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/dryice.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/errormessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/httpmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/instanttransactionrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/insurance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/invoicenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/labelfiletype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/lineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/lineitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/liverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/liveratecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/liveratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/manifestcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/manifestpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/objectstate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/ordercreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/orderpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/parcelcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/parcelextra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/parcelinsurance.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/parcelpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/parcelrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/parceltemplateenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/pickupbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/ponumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/ratemessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/ratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/refundpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/refundrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/rmanumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/servicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/servicegroupaccountandservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/servicegroupcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/servicegrouptype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/servicegroupupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/servicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)    41991 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/servicelevelenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/shipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/shipmentcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/shipmentextra.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/shipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/shippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/shippoaccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/shippoaccountupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/trackingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/trackingstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/trackingstatuslocationbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/trackingstatussubstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/tracksrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/transactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/transactionpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/transactionstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/upsconnectexistingownaccountparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/userparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/userparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/weightunit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.574234 shippo-3.2.4/src/shippo/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/errors/badrequestwithdetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/errors/badrequestwitherror.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/errors/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.574234 shippo-3.2.4/src/shippo/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.586234 shippo-3.2.4/src/shippo/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/addshipmentstobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createliverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createpickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/deletedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/deleteservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/deleteuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getcarrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getcarrierregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getdefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/gettrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/gettransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listaddresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listcarrieraccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listcarrierparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listcustomsdeclarations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listcustomsitems.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listmanifests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listorders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listparcels.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listrefunds.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listservicegroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listshipmentrates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listshipmentratesbycurrencycode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listshipments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listshippoaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listuserparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/purchasebatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/registercarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/removeshipmentsfrombatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/updatecarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/updatedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/updateservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/updateshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/updateuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/validateaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11126 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15887 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/rates_at_checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/refunds.py
--rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/service_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/shipments.py
--rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/shippo_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/tracking_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19173 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/user_parcel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.586234 shippo-3.2.4/src/shippo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.554234 shippo-3.2.4/src/shippo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-15 16:54:49.000000 shippo-3.2.4/src/shippo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-04-15 16:54:49.000000 shippo-3.2.4/src/shippo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:54:49.000000 shippo-3.2.4/src/shippo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-15 16:54:49.000000 shippo-3.2.4/src/shippo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 16:54:49.000000 shippo-3.2.4/src/shippo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:34:35.452178 shippo-3.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-16 19:34:35.452178 shippo-3.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-16 19:34:26.000000 shippo-3.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:34:35.452178 shippo-3.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-16 19:34:26.000000 shippo-3.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:34:35.412178 shippo-3.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:34:35.416178 shippo-3.2.5/src/shippo/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:34:35.420178 shippo-3.2.5/src/shippo/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14334 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19782 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28938 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/carrier_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/carrier_parcel_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/customs_declarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/customs_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/manifests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:34:35.420178 shippo-3.2.5/src/shippo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:34:35.440178 shippo-3.2.5/src/shippo/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/addresscompletecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/addresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/addressimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/addresspaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/addressvalidationresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/addressvalidationresultsmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/batchcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/batchshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/batchshipmentbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/batchshipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountdpddecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountfedexcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountupscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountuspscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrieraccountwithextrainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/carriersenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/cod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/connectexistingownaccountrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/customerreference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/customsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/customsdeclarationcontentstypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/customsdeclarationcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/customsdeclarationeelpfcenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/customsdeclarationincotermenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/customsdeclarationnondeliveryoptionenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/customsdeclarationpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/customsexporteridentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/customsinvoicedcharges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/customsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/customsitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/customsitempaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/customstaxidentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/dangerousgoodslithiumbatteries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/dangerousgoodsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/defaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/defaultparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/departmentnumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/distanceunitenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/dryice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/errormessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/httpmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/instanttransactionrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/insurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/invoicenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/labelfiletypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/lineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/lineitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/liverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/liveratecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/liveratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/manifestcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/manifestpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/objectstateenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/ordercreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/orderpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/orderstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/parcelcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/parcelextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/parcelinsurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/parcelpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/parcelrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/parceltemplateenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/pickupbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/ponumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/ratemessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/ratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/refundpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/refundrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/rmanumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/servicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/servicegroupaccountandservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/servicegroupcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/servicegrouptypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/servicegroupupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/servicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42151 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/servicelevelenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/shipmentcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/shipmentextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/shipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/shippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/shippoaccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/shippoaccountupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/trackingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/trackingstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/trackingstatuslocationbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/trackingstatussubstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/tracksrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/transactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/transactionpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/transactionstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/upsconnectexistingownaccountparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/userparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/userparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/components/weightunitenum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:34:35.440178 shippo-3.2.5/src/shippo/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/errors/badrequestwithdetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/errors/badrequestwitherror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/errors/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:34:35.440178 shippo-3.2.5/src/shippo/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:34:35.452178 shippo-3.2.5/src/shippo/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/addshipmentstobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createliverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createpickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/createuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/deletedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/deleteservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/deleteuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/getaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/getbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/getcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/getcarrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/getcarrierregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/getcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/getcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/getdefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/getorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/getparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/getrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/getrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/getshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/getshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/gettrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/gettransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/getuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/listaddresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/listcarrieraccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/listcarrierparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/listcustomsdeclarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/listcustomsitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/listmanifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/listorders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/listparcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/listrefunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/listservicegroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/listshipmentrates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/listshipmentratesbycurrencycode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/listshipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/listshippoaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/listtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/listuserparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/purchasebatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/registercarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/removeshipmentsfrombatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/updatecarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/updatedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/updateservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/updateshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/updateuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/models/operations/validateaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11126 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15887 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/rates_at_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/refunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/shipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/shippo_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/tracking_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19173 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/user_parcel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:34:35.452178 shippo-3.2.5/src/shippo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-04-16 19:34:26.000000 shippo-3.2.5/src/shippo/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:34:35.420178 shippo-3.2.5/src/shippo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-16 19:34:35.000000 shippo-3.2.5/src/shippo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11803 2024-04-16 19:34:35.000000 shippo-3.2.5/src/shippo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:34:35.000000 shippo-3.2.5/src/shippo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-16 19:34:35.000000 shippo-3.2.5/src/shippo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 19:34:35.000000 shippo-3.2.5/src/shippo.egg-info/top_level.txt
```

### Comparing `shippo-3.2.4/PKG-INFO` & `shippo-3.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.2.4
+Version: 3.2.5
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
```

### Comparing `shippo-3.2.4/README.md` & `shippo-3.2.5/README.md`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/setup.py` & `shippo-3.2.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='shippo',
-    version='3.2.4',
+    version='3.2.5',
     author='Shippo',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/goshippo/shippo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `shippo-3.2.4/src/shippo/_hooks/registration.py` & `shippo-3.2.5/src/shippo/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/_hooks/sdkhooks.py` & `shippo-3.2.5/src/shippo/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/_hooks/types.py` & `shippo-3.2.5/src/shippo/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/addresses.py` & `shippo-3.2.5/src/shippo/addresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/batches.py` & `shippo-3.2.5/src/shippo/batches.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/carrier_accounts.py` & `shippo-3.2.5/src/shippo/carrier_accounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/carrier_parcel_templates.py` & `shippo-3.2.5/src/shippo/carrier_parcel_templates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/customs_declarations.py` & `shippo-3.2.5/src/shippo/customs_declarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/customs_items.py` & `shippo-3.2.5/src/shippo/customs_items.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/debug.py` & `shippo-3.2.5/src/shippo/debug.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/manifests.py` & `shippo-3.2.5/src/shippo/manifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/__init__.py` & `shippo-3.2.5/src/shippo/models/components/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,54 +34,60 @@
 from .carrieraccountregistrationstatus import *
 from .carrieraccountservicelevel import *
 from .carrieraccountupscreaterequest import *
 from .carrieraccountupscreaterequestparameters import *
 from .carrieraccountuspscreaterequest import *
 from .carrieraccountwithextrainfo import *
 from .carrierparceltemplate import *
-from .carriers import *
+from .carriersenum import *
 from .cod import *
 from .connectexistingownaccountrequest import *
 from .customerreference import *
 from .customsdeclaration import *
+from .customsdeclarationb13afilingoptionenum import *
+from .customsdeclarationcontentstypeenum import *
 from .customsdeclarationcreaterequest import *
+from .customsdeclarationeelpfcenum import *
+from .customsdeclarationincotermenum import *
+from .customsdeclarationnondeliveryoptionenum import *
 from .customsdeclarationpaginatedlist import *
 from .customsexporteridentification import *
 from .customsinvoicedcharges import *
 from .customsitem import *
 from .customsitembase import *
 from .customsitempaginatedlist import *
 from .customstaxidentification import *
 from .dangerousgoodsbiologicalmaterial import *
 from .dangerousgoodslithiumbatteries import *
 from .dangerousgoodsobject import *
 from .defaultparceltemplate import *
 from .defaultparceltemplateupdaterequest import *
 from .departmentnumber import *
-from .distanceunit import *
+from .distanceunitenum import *
 from .dryice import *
 from .errormessage import *
 from .httpmetadata import *
 from .instanttransactionrequestbody import *
 from .insurance import *
 from .invoicenumber import *
-from .labelfiletype import *
+from .labelfiletypeenum import *
 from .lineitem import *
 from .lineitembase import *
 from .liverate import *
 from .liveratecreaterequest import *
 from .liveratepaginatedlist import *
 from .location import *
 from .manifest import *
 from .manifestcreaterequest import *
 from .manifestpaginatedlist import *
-from .objectstate import *
+from .objectstateenum import *
 from .order import *
 from .ordercreaterequest import *
 from .orderpaginatedlist import *
+from .orderstatusenum import *
 from .parcel import *
 from .parcelcreaterequest import *
 from .parcelextra import *
 from .parcelinsurance import *
 from .parcelpaginatedlist import *
 from .parcelrequest import *
 from .parceltemplateenumset import *
@@ -95,15 +101,15 @@
 from .refundpaginatedlist import *
 from .refundrequestbody import *
 from .rmanumber import *
 from .security import *
 from .servicegroup import *
 from .servicegroupaccountandservicelevel import *
 from .servicegroupcreaterequest import *
-from .servicegrouptype import *
+from .servicegrouptypeenum import *
 from .servicegroupupdaterequest import *
 from .servicelevel import *
 from .servicelevelenumset import *
 from .shipment import *
 from .shipmentcreaterequest import *
 from .shipmentextra import *
 from .shipmentpaginatedlist import *
@@ -121,10 +127,10 @@
 from .transactionpaginatedlist import *
 from .transactionstatusenum import *
 from .upsconnectexistingownaccountparameters import *
 from .userparceltemplate import *
 from .userparceltemplateupdaterequest import *
 from .userparceltemplatewithcarriertemplatecreaterequest import *
 from .userparceltemplatewithoutcarriertemplatecreaterequest import *
-from .weightunit import *
+from .weightunitenum import *
 
-__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","B13aFilingOption","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountChronopostCreateRequestParameters","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountFedExCreateRequest","CarrierAccountFedExCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountMondialRelayCreateRequest","CarrierAccountMondialRelayCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","Carriers","Cod","Code","ConnectExistingOwnAccountRequest","ContentsType","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationCreateRequest","CustomsDeclarationCreateRequestB13aFilingOption","CustomsDeclarationCreateRequestContentsType","CustomsDeclarationCreateRequestEelPfc","CustomsDeclarationCreateRequestIncoterm","CustomsDeclarationCreateRequestNonDeliveryOption","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemBase","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnit","DryIce","EelPfc","ErrorMessage","HTTPMetadata","Incoterm","InstantTransactionRequestBody","InstantTransactionRequestBodyLabelFileType","Insurance","InvoiceNumber","LabelFileType","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","NonDeliveryOption","ObjectInfo","ObjectResults","ObjectState","Order","OrderCreateRequest","OrderCreateRequestOrderStatus","OrderPaginatedList","OrderStatus","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelObjectState","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustralia","ParcelTemplateCouriersPlease","ParcelTemplateDHLeCommerce","ParcelTemplateDPDUK","ParcelTemplateFedEx","ParcelTemplateUPS","ParcelTemplateUSPS","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupType","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostal","ServiceLevelAPG","ServiceLevelAirterra","ServiceLevelAramexAustralia","ServiceLevelAsendia","ServiceLevelAustraliaPost","ServiceLevelAxleHire","ServiceLevelBetterTrucks","ServiceLevelCDL","ServiceLevelCanadaPost","ServiceLevelChronopost","ServiceLevelColissimo","ServiceLevelCorreosEspana","ServiceLevelCouriersPlease","ServiceLevelDHLExpress","ServiceLevelDHLGermany","ServiceLevelDHLeCommerce","ServiceLevelDPDDE","ServiceLevelDPDUK","ServiceLevelDeutschePost","ServiceLevelEvriUK","ServiceLevelFedEx","ServiceLevelGLSUS","ServiceLevelGlobegistics","ServiceLevelLSO","ServiceLevelLasership","ServiceLevelMaergo","ServiceLevelMondialRelay","ServiceLevelOnTrac","ServiceLevelParcelforce","ServiceLevelPostItaliane","ServiceLevelPurolator","ServiceLevelRoyalMail","ServiceLevelSendle","ServiceLevelSwyft","ServiceLevelUDS","ServiceLevelUPS","ServiceLevelUSPS","ServiceLevelVeho","ServiceLevelePostGlobal","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnit"]
+__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountChronopostCreateRequestParameters","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountFedExCreateRequest","CarrierAccountFedExCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountMondialRelayCreateRequest","CarrierAccountMondialRelayCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","CarriersEnum","Cod","Code","ConnectExistingOwnAccountRequest","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationB13AFilingOptionEnum","CustomsDeclarationContentsTypeEnum","CustomsDeclarationCreateRequest","CustomsDeclarationEelPfcEnum","CustomsDeclarationIncotermEnum","CustomsDeclarationNonDeliveryOptionEnum","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemBase","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnitEnum","DryIce","ErrorMessage","HTTPMetadata","InstantTransactionRequestBody","Insurance","InvoiceNumber","LabelFileTypeEnum","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","ObjectInfo","ObjectResults","ObjectState","ObjectStateEnum","Order","OrderCreateRequest","OrderPaginatedList","OrderStatusEnum","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustraliaEnum","ParcelTemplateCouriersPleaseEnum","ParcelTemplateDHLeCommerceEnum","ParcelTemplateDPDUKEnum","ParcelTemplateFedExEnum","ParcelTemplateUPSEnum","ParcelTemplateUSPSEnum","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupTypeEnum","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostalEnum","ServiceLevelAPGEnum","ServiceLevelAirterraEnum","ServiceLevelAramexAustraliaEnum","ServiceLevelAsendiaEnum","ServiceLevelAustraliaPostEnum","ServiceLevelAxleHireEnum","ServiceLevelBetterTrucksEnum","ServiceLevelCDLEnum","ServiceLevelCanadaPostEnum","ServiceLevelChronopostEnum","ServiceLevelColissimoEnum","ServiceLevelCorreosEspanaEnum","ServiceLevelCouriersPleaseEnum","ServiceLevelDHLExpressEnum","ServiceLevelDHLGermanyEnum","ServiceLevelDHLeCommerceEnum","ServiceLevelDPDDEEnum","ServiceLevelDPDUKEnum","ServiceLevelDeutschePostEnum","ServiceLevelEvriUKEnum","ServiceLevelFedExEnum","ServiceLevelGLSUSEnum","ServiceLevelGlobegisticsEnum","ServiceLevelLSOEnum","ServiceLevelLasershipEnum","ServiceLevelMaergoEnum","ServiceLevelMondialRelayEnum","ServiceLevelOnTracEnum","ServiceLevelParcelforceEnum","ServiceLevelPostItalianeEnum","ServiceLevelPurolatorEnum","ServiceLevelRoyalMailEnum","ServiceLevelSendleEnum","ServiceLevelSwyftEnum","ServiceLevelUDSEnum","ServiceLevelUPSEnum","ServiceLevelUSPSEnum","ServiceLevelVehoEnum","ServiceLevelePostGlobalEnum","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnitEnum"]
```

### Comparing `shippo-3.2.4/src/shippo/models/components/address.py` & `shippo-3.2.5/src/shippo/models/components/address.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/addresscompletecreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/addresscompletecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/addresscreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/addresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/addressimporter.py` & `shippo-3.2.5/src/shippo/models/components/addressimporter.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/addresspaginatedlist.py` & `shippo-3.2.5/src/shippo/models/components/addresspaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/addressvalidationresults.py` & `shippo-3.2.5/src/shippo/models/components/addressvalidationresults.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/addressvalidationresultsmessage.py` & `shippo-3.2.5/src/shippo/models/components/addressvalidationresultsmessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/alcohol.py` & `shippo-3.2.5/src/shippo/models/components/alcohol.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/batch.py` & `shippo-3.2.5/src/shippo/models/components/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from .batchshipmentpaginatedlist import BatchShipmentPaginatedList
-from .labelfiletype import LabelFileType
+from .labelfiletypeenum import LabelFileTypeEnum
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
@@ -64,15 +64,15 @@
     status: BatchStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
     r"""Batches that are `VALIDATING` are being created and validated<br>
     `VALID` batches can be purchased<br>
     `INVALID` batches cannot be purchased, `INVALID` BatchShipments must be removed<br>
     Batches that are in the `PURCHASING` state are being purchased<br>
     `PURCHASED` batches are finished purchasing.
     """
-    label_filetype: Optional[LabelFileType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_filetype'), 'exclude': lambda f: f is None }})
+    label_filetype: Optional[LabelFileTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_filetype'), 'exclude': lambda f: f is None }})
     r"""Print format of the <a href=\\"https://docs.goshippo.com/docs/shipments/shippinglabelsizes/\\">label</a>. If empty, will use the default format set from
     <a href=\"https://apps.goshippo.com/settings/labels\">the Shippo dashboard.</a>
     """
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""A string of up to 100 characters that can be filled with any additional information you want to attach to the object."""
     test: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('test'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.2.4/src/shippo/models/components/batchcreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/batchcreaterequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from .batchshipmentbase import BatchShipmentBase
-from .labelfiletype import LabelFileType
+from .labelfiletypeenum import LabelFileTypeEnum
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
@@ -20,15 +20,15 @@
     default_servicelevel_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('default_servicelevel_token') }})
     r"""Token of the service level to use as the default for all shipments in this Batch.
     The servicelevel can be changed on a per-shipment basis by changing the servicelevel_token in the 
     corresponding BatchShipment object. <a href=\"#tag/Service-Levels\">Servicelevel tokens can be found here.</a>
     """
     batch_shipments: List[BatchShipmentBase] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batch_shipments') }})
     r"""Array of BatchShipment objects. The response keeps the same order as in the request array."""
-    label_filetype: Optional[LabelFileType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_filetype'), 'exclude': lambda f: f is None }})
+    label_filetype: Optional[LabelFileTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_filetype'), 'exclude': lambda f: f is None }})
     r"""Print format of the <a href=\\"https://docs.goshippo.com/docs/shipments/shippinglabelsizes/\\">label</a>. If empty, will use the default format set from
     <a href=\"https://apps.goshippo.com/settings/labels\">the Shippo dashboard.</a>
     """
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""A string of up to 100 characters that can be filled with any additional information you want to attach to the object."""
```

### Comparing `shippo-3.2.4/src/shippo/models/components/batchshipment.py` & `shippo-3.2.5/src/shippo/models/components/batchshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/batchshipmentbase.py` & `shippo-3.2.5/src/shippo/models/components/batchshipmentbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/batchshipmentpaginatedlist.py` & `shippo-3.2.5/src/shippo/models/components/batchshipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/billing.py` & `shippo-3.2.5/src/shippo/models/components/billing.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccount.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountbase.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountchronopostcreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountchronopostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountcolissimocreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountcolissimocreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountcorreoscreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountcorreoscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountdpddecreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountdpddecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountdpdukcreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountdpdukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountfedexcreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountfedexcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccounthermesukcreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccounthermesukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountpaginatedlist.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountregistrationstatus.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountservicelevel.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountupscreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountupscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountupscreaterequestparameters.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountupscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountuspscreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountuspscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrieraccountwithextrainfo.py` & `shippo-3.2.5/src/shippo/models/components/carrieraccountwithextrainfo.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/carrierparceltemplate.py` & `shippo-3.2.5/src/shippo/models/components/carrierparceltemplate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .distanceunit import DistanceUnit
+from .distanceunitenum import DistanceUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CarrierParcelTemplate:
     carrier: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier'), 'exclude': lambda f: f is None }})
     r"""The name of the carrier that provides this parcel template"""
-    distance_unit: Optional[DistanceUnit] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit'), 'exclude': lambda f: f is None }})
+    distance_unit: Optional[DistanceUnitEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit'), 'exclude': lambda f: f is None }})
     r"""The measure unit used for length, width and height."""
     height: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is None }})
     r"""The height of the package, in units specified by the distance_unit attribute"""
     is_variable_dimensions: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_variable_dimensions'), 'exclude': lambda f: f is None }})
     r"""True if the carrier parcel template allows custom dimensions, such as USPS Softpack."""
     length: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('length'), 'exclude': lambda f: f is None }})
     r"""The length of the package, in units specified by the distance_unit attribute"""
```

### Comparing `shippo-3.2.4/src/shippo/models/components/carriers.py` & `shippo-3.2.5/src/shippo/models/components/carriersenum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
-class Carriers(str, Enum):
+class CarriersEnum(str, Enum):
     r"""|Token | Carrier name|
     |:---|:---|
     | airterra | Airterra |
     | apc_postal | APC Postal|
     | apg | APG|
     | aramex | Aramex|
     | asendia_us | Asendia US|
```

### Comparing `shippo-3.2.4/src/shippo/models/components/cod.py` & `shippo-3.2.5/src/shippo/models/components/cod.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/connectexistingownaccountrequest.py` & `shippo-3.2.5/src/shippo/models/components/connectexistingownaccountrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/customerreference.py` & `shippo-3.2.5/src/shippo/models/components/customerreference.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/customsdeclaration.py` & `shippo-3.2.5/src/shippo/models/components/customsdeclaration.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,25 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
+from .customsdeclarationb13afilingoptionenum import CustomsDeclarationB13AFilingOptionEnum
+from .customsdeclarationcontentstypeenum import CustomsDeclarationContentsTypeEnum
+from .customsdeclarationeelpfcenum import CustomsDeclarationEelPfcEnum
+from .customsdeclarationincotermenum import CustomsDeclarationIncotermEnum
+from .customsdeclarationnondeliveryoptionenum import CustomsDeclarationNonDeliveryOptionEnum
 from .customsexporteridentification import CustomsExporterIdentification
 from .customsinvoicedcharges import CustomsInvoicedCharges
-from .objectstate import ObjectState
+from .objectstateenum import ObjectStateEnum
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
-from enum import Enum
 from shippo import utils
 from typing import Any, List, Optional
 
-class B13aFilingOption(str, Enum):
-    r"""B13A Option details are obtained by filing a B13A Canada Export Declaration via the Canadian Export Reporting System (CERS).
-    <a href=\"https://www.cbsa-asfc.gc.ca/services/export/guide-eng.html\" target=\"_blank\" rel=\"noopener noreferrer\"> More information on reporting commercial exports from Canada. </a>
-    """
-    FILED_ELECTRONICALLY = 'FILED_ELECTRONICALLY'
-    SUMMARY_REPORTING = 'SUMMARY_REPORTING'
-    NOT_REQUIRED = 'NOT_REQUIRED'
-
-class ContentsType(str, Enum):
-    r"""Type of goods of the shipment."""
-    DOCUMENTS = 'DOCUMENTS'
-    GIFT = 'GIFT'
-    SAMPLE = 'SAMPLE'
-    MERCHANDISE = 'MERCHANDISE'
-    HUMANITARIAN_DONATION = 'HUMANITARIAN_DONATION'
-    RETURN_MERCHANDISE = 'RETURN_MERCHANDISE'
-    OTHER = 'OTHER'
-
-class EelPfc(str, Enum):
-    r"""EEL / PFC type of the shipment. For most shipments from the US to CA, `NOEEI_30_36` is applicable; for most
-    other shipments from the US, `NOEEI_30_37_a` is applicable.
-    """
-    NOEEI_30_37_A = 'NOEEI_30_37_a'
-    NOEEI_30_37_H = 'NOEEI_30_37_h'
-    NOEEI_30_37_F = 'NOEEI_30_37_f'
-    NOEEI_30_36 = 'NOEEI_30_36'
-    AES_ITN = 'AES_ITN'
-
-class Incoterm(str, Enum):
-    r"""The incoterm reference of the shipment. FCA is available for DHL Express and FedEx only.
-    eDAP is available for DPD UK only. DAP is available for DHL Express and DPD UK.
-    If expecting DAP for other carriers, please use DDU.
-    """
-    DDP = 'DDP'
-    DDU = 'DDU'
-    FCA = 'FCA'
-    DAP = 'DAP'
-    E_DAP = 'eDAP'
-
-class NonDeliveryOption(str, Enum):
-    r"""Indicates how the carrier should proceed in case the shipment can't be delivered."""
-    ABANDON = 'ABANDON'
-    RETURN = 'RETURN'
-
 
 @dataclasses.dataclass
 class CustomsDeclarationAddressImporter:
     r"""Object ID of the Importer address."""
     
 
 
@@ -69,25 +29,25 @@
 class CustomsDeclaration:
     certify: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('certify') }})
     r"""Expresses that the certify_signer has provided all information of this customs declaration truthfully."""
     certify_signer: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('certify_signer') }})
     r"""Name of the person who created the customs declaration and is responsible for the validity of all
     information provided.
     """
-    contents_type: ContentsType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contents_type') }})
+    contents_type: CustomsDeclarationContentsTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contents_type') }})
     r"""Type of goods of the shipment."""
-    non_delivery_option: NonDeliveryOption = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('non_delivery_option') }})
+    non_delivery_option: CustomsDeclarationNonDeliveryOptionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('non_delivery_option') }})
     r"""Indicates how the carrier should proceed in case the shipment can't be delivered."""
     items: List[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('items') }})
     r"""Distinct Parcel content items as Customs Items object_ids."""
     aes_itn: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aes_itn'), 'exclude': lambda f: f is None }})
     r"""**required if eel_pfc is `AES_ITN`**<br>
     AES / ITN reference of the shipment.
     """
-    b13a_filing_option: Optional[B13aFilingOption] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('b13a_filing_option'), 'exclude': lambda f: f is None }})
+    b13a_filing_option: Optional[CustomsDeclarationB13AFilingOptionEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('b13a_filing_option'), 'exclude': lambda f: f is None }})
     r"""B13A Option details are obtained by filing a B13A Canada Export Declaration via the Canadian Export Reporting System (CERS).
     <a href=\"https://www.cbsa-asfc.gc.ca/services/export/guide-eng.html\" target=\"_blank\" rel=\"noopener noreferrer\"> More information on reporting commercial exports from Canada. </a>
     """
     b13a_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('b13a_number'), 'exclude': lambda f: f is None }})
     r"""**must be provided if and only if b13a_filing_option is provided**<br>
     Represents:<br> the Proof of Report (POR) Number when b13a_filing_option is `FILED_ELECTRONICALLY`;<br> 
     the Summary ID Number when b13a_filing_option is `SUMMARY_REPORTING`;<br> 
@@ -98,23 +58,23 @@
     commercial_invoice: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('commercial_invoice'), 'exclude': lambda f: f is None }})
     contents_explanation: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contents_explanation'), 'exclude': lambda f: f is None }})
     r"""**required if contents_type is `OTHER`**<br>
     Explanation of the type of goods of the shipment.
     """
     disclaimer: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disclaimer'), 'exclude': lambda f: f is None }})
     r"""Disclaimer for the shipment and customs information that have been provided."""
-    eel_pfc: Optional[EelPfc] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eel_pfc'), 'exclude': lambda f: f is None }})
+    eel_pfc: Optional[CustomsDeclarationEelPfcEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eel_pfc'), 'exclude': lambda f: f is None }})
     r"""EEL / PFC type of the shipment. For most shipments from the US to CA, `NOEEI_30_36` is applicable; for most
     other shipments from the US, `NOEEI_30_37_a` is applicable.
     """
     exporter_reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('exporter_reference'), 'exclude': lambda f: f is None }})
     r"""Exporter reference of an export shipment."""
     importer_reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('importer_reference'), 'exclude': lambda f: f is None }})
     r"""Importer reference of an import shipment."""
-    incoterm: Optional[Incoterm] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('incoterm'), 'exclude': lambda f: f is None }})
+    incoterm: Optional[CustomsDeclarationIncotermEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('incoterm'), 'exclude': lambda f: f is None }})
     r"""The incoterm reference of the shipment. FCA is available for DHL Express and FedEx only.
     eDAP is available for DPD UK only. DAP is available for DHL Express and DPD UK.
     If expecting DAP for other carriers, please use DDU.
     """
     is_vat_collected: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_vat_collected'), 'exclude': lambda f: f is None }})
     r"""Indicates whether the shipment's destination VAT has been collected. May be required for some destinations."""
     invoice: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoice'), 'exclude': lambda f: f is None }})
@@ -135,15 +95,15 @@
     r"""Additional invoiced charges to be shown on the Customs Declaration Commercial Invoice."""
     object_created: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""Date and time of object creation."""
     object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the given object."""
     object_owner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_owner'), 'exclude': lambda f: f is None }})
     r"""Username of the user who created the object."""
-    object_state: Optional[ObjectState] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_state'), 'exclude': lambda f: f is None }})
+    object_state: Optional[ObjectStateEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_state'), 'exclude': lambda f: f is None }})
     r"""Indicates the validity of the enclosing object"""
     object_updated: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_updated'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""Date and time of last object update."""
     test: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('test'), 'exclude': lambda f: f is None }})
     r"""Indicates whether the object has been created in test mode."""
```

### Comparing `shippo-3.2.4/src/shippo/models/components/customsdeclarationcreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/customsdeclarationcreaterequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,82 +1,42 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from .addressimporter import AddressImporter
+from .customsdeclarationb13afilingoptionenum import CustomsDeclarationB13AFilingOptionEnum
+from .customsdeclarationcontentstypeenum import CustomsDeclarationContentsTypeEnum
+from .customsdeclarationeelpfcenum import CustomsDeclarationEelPfcEnum
+from .customsdeclarationincotermenum import CustomsDeclarationIncotermEnum
+from .customsdeclarationnondeliveryoptionenum import CustomsDeclarationNonDeliveryOptionEnum
 from .customsitembase import CustomsItemBase
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
 from shippo import utils
 from typing import Any, List, Optional
 
-class CustomsDeclarationCreateRequestB13aFilingOption(str, Enum):
-    r"""B13A Option details are obtained by filing a B13A Canada Export Declaration via the Canadian Export Reporting System (CERS).
-    <a href=\"https://www.cbsa-asfc.gc.ca/services/export/guide-eng.html\" target=\"_blank\" rel=\"noopener noreferrer\"> More information on reporting commercial exports from Canada. </a>
-    """
-    FILED_ELECTRONICALLY = 'FILED_ELECTRONICALLY'
-    SUMMARY_REPORTING = 'SUMMARY_REPORTING'
-    NOT_REQUIRED = 'NOT_REQUIRED'
-
-class CustomsDeclarationCreateRequestContentsType(str, Enum):
-    r"""Type of goods of the shipment."""
-    DOCUMENTS = 'DOCUMENTS'
-    GIFT = 'GIFT'
-    SAMPLE = 'SAMPLE'
-    MERCHANDISE = 'MERCHANDISE'
-    HUMANITARIAN_DONATION = 'HUMANITARIAN_DONATION'
-    RETURN_MERCHANDISE = 'RETURN_MERCHANDISE'
-    OTHER = 'OTHER'
-
-class CustomsDeclarationCreateRequestEelPfc(str, Enum):
-    r"""EEL / PFC type of the shipment. For most shipments from the US to CA, `NOEEI_30_36` is applicable; for most
-    other shipments from the US, `NOEEI_30_37_a` is applicable.
-    """
-    NOEEI_30_37_A = 'NOEEI_30_37_a'
-    NOEEI_30_37_H = 'NOEEI_30_37_h'
-    NOEEI_30_37_F = 'NOEEI_30_37_f'
-    NOEEI_30_36 = 'NOEEI_30_36'
-    AES_ITN = 'AES_ITN'
-
-class CustomsDeclarationCreateRequestIncoterm(str, Enum):
-    r"""The incoterm reference of the shipment. FCA is available for DHL Express and FedEx only.
-    eDAP is available for DPD UK only. DAP is available for DHL Express and DPD UK.
-    If expecting DAP for other carriers, please use DDU.
-    """
-    DDP = 'DDP'
-    DDU = 'DDU'
-    FCA = 'FCA'
-    DAP = 'DAP'
-    E_DAP = 'eDAP'
-
-class CustomsDeclarationCreateRequestNonDeliveryOption(str, Enum):
-    r"""Indicates how the carrier should proceed in case the shipment can't be delivered."""
-    ABANDON = 'ABANDON'
-    RETURN = 'RETURN'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CustomsDeclarationCreateRequest:
     certify: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('certify') }})
     r"""Expresses that the certify_signer has provided all information of this customs declaration truthfully."""
     certify_signer: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('certify_signer') }})
     r"""Name of the person who created the customs declaration and is responsible for the validity of all
     information provided.
     """
-    contents_type: CustomsDeclarationCreateRequestContentsType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contents_type') }})
+    contents_type: CustomsDeclarationContentsTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contents_type') }})
     r"""Type of goods of the shipment."""
-    non_delivery_option: CustomsDeclarationCreateRequestNonDeliveryOption = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('non_delivery_option') }})
+    non_delivery_option: CustomsDeclarationNonDeliveryOptionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('non_delivery_option') }})
     r"""Indicates how the carrier should proceed in case the shipment can't be delivered."""
     items: List[CustomsItemBase] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('items') }})
     aes_itn: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aes_itn'), 'exclude': lambda f: f is None }})
     r"""**required if eel_pfc is `AES_ITN`**<br>
     AES / ITN reference of the shipment.
     """
-    b13a_filing_option: Optional[CustomsDeclarationCreateRequestB13aFilingOption] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('b13a_filing_option'), 'exclude': lambda f: f is None }})
+    b13a_filing_option: Optional[CustomsDeclarationB13AFilingOptionEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('b13a_filing_option'), 'exclude': lambda f: f is None }})
     r"""B13A Option details are obtained by filing a B13A Canada Export Declaration via the Canadian Export Reporting System (CERS).
     <a href=\"https://www.cbsa-asfc.gc.ca/services/export/guide-eng.html\" target=\"_blank\" rel=\"noopener noreferrer\"> More information on reporting commercial exports from Canada. </a>
     """
     b13a_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('b13a_number'), 'exclude': lambda f: f is None }})
     r"""**must be provided if and only if b13a_filing_option is provided**<br>
     Represents:<br> the Proof of Report (POR) Number when b13a_filing_option is `FILED_ELECTRONICALLY`;<br> 
     the Summary ID Number when b13a_filing_option is `SUMMARY_REPORTING`;<br> 
@@ -87,23 +47,23 @@
     commercial_invoice: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('commercial_invoice'), 'exclude': lambda f: f is None }})
     contents_explanation: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contents_explanation'), 'exclude': lambda f: f is None }})
     r"""**required if contents_type is `OTHER`**<br>
     Explanation of the type of goods of the shipment.
     """
     disclaimer: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disclaimer'), 'exclude': lambda f: f is None }})
     r"""Disclaimer for the shipment and customs information that have been provided."""
-    eel_pfc: Optional[CustomsDeclarationCreateRequestEelPfc] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eel_pfc'), 'exclude': lambda f: f is None }})
+    eel_pfc: Optional[CustomsDeclarationEelPfcEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eel_pfc'), 'exclude': lambda f: f is None }})
     r"""EEL / PFC type of the shipment. For most shipments from the US to CA, `NOEEI_30_36` is applicable; for most
     other shipments from the US, `NOEEI_30_37_a` is applicable.
     """
     exporter_reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('exporter_reference'), 'exclude': lambda f: f is None }})
     r"""Exporter reference of an export shipment."""
     importer_reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('importer_reference'), 'exclude': lambda f: f is None }})
     r"""Importer reference of an import shipment."""
-    incoterm: Optional[CustomsDeclarationCreateRequestIncoterm] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('incoterm'), 'exclude': lambda f: f is None }})
+    incoterm: Optional[CustomsDeclarationIncotermEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('incoterm'), 'exclude': lambda f: f is None }})
     r"""The incoterm reference of the shipment. FCA is available for DHL Express and FedEx only.
     eDAP is available for DPD UK only. DAP is available for DHL Express and DPD UK.
     If expecting DAP for other carriers, please use DDU.
     """
     is_vat_collected: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_vat_collected'), 'exclude': lambda f: f is None }})
     r"""Indicates whether the shipment's destination VAT has been collected. May be required for some destinations."""
     invoice: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoice'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.2.4/src/shippo/models/components/customsdeclarationpaginatedlist.py` & `shippo-3.2.5/src/shippo/models/components/customsdeclarationpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/customsexporteridentification.py` & `shippo-3.2.5/src/shippo/models/components/customsexporteridentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/customsinvoicedcharges.py` & `shippo-3.2.5/src/shippo/models/components/customsinvoicedcharges.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/customsitem.py` & `shippo-3.2.5/src/shippo/models/components/customsitem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .objectstate import ObjectState
-from .weightunit import WeightUnit
+from .objectstateenum import ObjectStateEnum
+from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CustomsItem:
     description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
     r"""Text description of your item."""
-    mass_unit: WeightUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mass_unit') }})
+    mass_unit: WeightUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mass_unit') }})
     r"""The unit used for weight."""
     net_weight: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('net_weight') }})
     r"""Total weight of this item, i.e. quantity * weight per item."""
     origin_country: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('origin_country') }})
     r"""Country of origin of the item. Example: `US` or `DE`.
     All accepted values can be found on the <a href=\"http://www.iso.org/\" target=\"_blank\">Official ISO Website</a>.
     """
@@ -44,15 +44,15 @@
     r"""The tariff number of the item."""
     object_created: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""Date and time of object creation."""
     object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the given object."""
     object_owner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_owner'), 'exclude': lambda f: f is None }})
     r"""Username of the user who created the object."""
-    object_state: Optional[ObjectState] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_state'), 'exclude': lambda f: f is None }})
+    object_state: Optional[ObjectStateEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_state'), 'exclude': lambda f: f is None }})
     r"""Indicates the validity of the enclosing object"""
     object_updated: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_updated'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""Date and time of last object update."""
     test: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('test'), 'exclude': lambda f: f is None }})
     r"""Indicates whether the object has been created in test mode."""
```

### Comparing `shippo-3.2.4/src/shippo/models/components/customsitembase.py` & `shippo-3.2.5/src/shippo/models/components/customsitembase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .weightunit import WeightUnit
+from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CustomsItemBase:
     description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
     r"""Text description of your item."""
-    mass_unit: WeightUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mass_unit') }})
+    mass_unit: WeightUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mass_unit') }})
     r"""The unit used for weight."""
     net_weight: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('net_weight') }})
     r"""Total weight of this item, i.e. quantity * weight per item."""
     origin_country: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('origin_country') }})
     r"""Country of origin of the item. Example: `US` or `DE`.
     All accepted values can be found on the <a href=\"http://www.iso.org/\" target=\"_blank\">Official ISO Website</a>.
     """
```

### Comparing `shippo-3.2.4/src/shippo/models/components/customsitempaginatedlist.py` & `shippo-3.2.5/src/shippo/models/components/customsitempaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/customstaxidentification.py` & `shippo-3.2.5/src/shippo/models/components/customstaxidentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py` & `shippo-3.2.5/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/dangerousgoodslithiumbatteries.py` & `shippo-3.2.5/src/shippo/models/components/dangerousgoodslithiumbatteries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/dangerousgoodsobject.py` & `shippo-3.2.5/src/shippo/models/components/dangerousgoodsobject.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/defaultparceltemplate.py` & `shippo-3.2.5/src/shippo/models/components/defaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/defaultparceltemplateupdaterequest.py` & `shippo-3.2.5/src/shippo/models/components/defaultparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/departmentnumber.py` & `shippo-3.2.5/src/shippo/models/components/departmentnumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/dryice.py` & `shippo-3.2.5/src/shippo/models/components/dryice.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/errormessage.py` & `shippo-3.2.5/src/shippo/models/components/errormessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/httpmetadata.py` & `shippo-3.2.5/src/shippo/models/components/httpmetadata.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/instanttransactionrequestbody.py` & `shippo-3.2.5/src/shippo/models/components/shippoaccount.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .shipmentcreaterequest import ShipmentCreateRequest
+import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
+from datetime import datetime
 from shippo import utils
 from typing import Optional
 
-class InstantTransactionRequestBodyLabelFileType(str, Enum):
-    PNG = 'PNG'
-    PNG_2_3X7_5 = 'PNG_2.3x7.5'
-    PDF = 'PDF'
-    PDF_2_3X7_5 = 'PDF_2.3x7.5'
-    PDF_4X6 = 'PDF_4x6'
-    PDF_4X8 = 'PDF_4x8'
-    PDF_A4 = 'PDF_A4'
-    PDF_A6 = 'PDF_A6'
-    ZPLII = 'ZPLII'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class InstantTransactionRequestBody:
-    carrier_account: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_account') }})
-    servicelevel_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('servicelevel_token') }})
-    shipment: ShipmentCreateRequest = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipment') }})
-    label_file_type: Optional[InstantTransactionRequestBodyLabelFileType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_file_type'), 'exclude': lambda f: f is None }})
-    metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+class ShippoAccount:
+    email: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email') }})
+    first_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('first_name') }})
+    last_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('last_name') }})
+    company_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('company_name') }})
+    object_created: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
+    object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
+    object_updated: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_updated'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.2.4/src/shippo/models/components/insurance.py` & `shippo-3.2.5/src/shippo/models/components/insurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/invoicenumber.py` & `shippo-3.2.5/src/shippo/models/components/invoicenumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/labelfiletype.py` & `shippo-3.2.5/src/shippo/models/components/labelfiletypeenum.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
-class LabelFileType(str, Enum):
+class LabelFileTypeEnum(str, Enum):
     r"""Print format of the <a href=\\"https://docs.goshippo.com/docs/shipments/shippinglabelsizes/\\">label</a>. If empty, will use the default format set from
     <a href=\"https://apps.goshippo.com/settings/labels\">the Shippo dashboard.</a>
     """
     PNG = 'PNG'
     PNG_2_3X7_5 = 'PNG_2.3x7.5'
     PDF = 'PDF'
     PDF_2_3X7_5 = 'PDF_2.3x7.5'
```

### Comparing `shippo-3.2.4/src/shippo/models/components/lineitem.py` & `shippo-3.2.5/src/shippo/models/components/lineitem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .weightunit import WeightUnit
+from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
@@ -40,13 +40,13 @@
     Variants might be exposed as a separate resource in the future too. 
     Currently the variant title is a free text field describing the variant.
     """
     weight: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight'), 'exclude': lambda f: f is None }})
     r"""Total weight of this/these item(s). Instead of specifying the weight of all items,
     you can also set the <code>total_weight</code> value of the order object.
     """
-    weight_unit: Optional[WeightUnit] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
+    weight_unit: Optional[WeightUnitEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
     r"""The unit used for weight."""
     object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the line item object."""
```

### Comparing `shippo-3.2.4/src/shippo/models/components/lineitembase.py` & `shippo-3.2.5/src/shippo/models/components/lineitembase.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .weightunit import WeightUnit
+from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
@@ -40,11 +40,11 @@
     Variants might be exposed as a separate resource in the future too. 
     Currently the variant title is a free text field describing the variant.
     """
     weight: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight'), 'exclude': lambda f: f is None }})
     r"""Total weight of this/these item(s). Instead of specifying the weight of all items,
     you can also set the <code>total_weight</code> value of the order object.
     """
-    weight_unit: Optional[WeightUnit] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
+    weight_unit: Optional[WeightUnitEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
     r"""The unit used for weight."""
```

### Comparing `shippo-3.2.4/src/shippo/models/components/liverate.py` & `shippo-3.2.5/src/shippo/models/components/liverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/liveratecreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/liveratecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/liveratepaginatedlist.py` & `shippo-3.2.5/src/shippo/models/components/liveratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/location.py` & `shippo-3.2.5/src/shippo/models/components/location.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/manifest.py` & `shippo-3.2.5/src/shippo/models/components/manifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/manifestcreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/manifestcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/manifestpaginatedlist.py` & `shippo-3.2.5/src/shippo/models/components/manifestpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/order.py` & `shippo-3.2.5/src/shippo/models/components/order.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,20 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from .address import Address
 from .lineitem import LineItem
-from .weightunit import WeightUnit
+from .orderstatusenum import OrderStatusEnum
+from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
-class OrderStatus(str, Enum):
-    r"""Current state of the order. See the <a href=\\"https://docs.goshippo.com/docs/orders/orders/\\">orders tutorial</a>
-    for the logic of how the status is handled.
-    """
-    UNKNOWN = 'UNKNOWN'
-    AWAITPAY = 'AWAITPAY'
-    PAID = 'PAID'
-    REFUNDED = 'REFUNDED'
-    PARTIALLY_FULFILLED = 'PARTIALLY_FULFILLED'
-    SHIPPED = 'SHIPPED'
-
 class ShopApp(str, Enum):
     r"""Platform the order was created on and, if applicable, imported from.
     Orders created via the Shippo API or dashboard will have the value \"Shippo\".
     """
     AMAZON = 'Amazon'
     BIGCOMMERCE = 'Bigcommerce'
     CSV_IMPORT = 'CSV_Import'
@@ -52,15 +42,15 @@
     r"""**Required if total_price is provided**<br>
     Currency of the <code>total_price</code> and <code>total_tax</code> amounts.
     """
     notes: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
     r"""Custom buyer- or seller-provided notes about the order."""
     order_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order_number'), 'exclude': lambda f: f is None }})
     r"""An alphanumeric identifier for the order used by the seller/buyer. This identifier doesn't need to be unique."""
-    order_status: Optional[OrderStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order_status'), 'exclude': lambda f: f is None }})
+    order_status: Optional[OrderStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order_status'), 'exclude': lambda f: f is None }})
     r"""Current state of the order. See the <a href=\\"https://docs.goshippo.com/docs/orders/orders/\\">orders tutorial</a>
     for the logic of how the status is handled.
     """
     shipping_cost: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipping_cost'), 'exclude': lambda f: f is None }})
     r"""Amount paid by the buyer for shipping. This amount can be different from the price the seller will actually pay for shipping."""
     shipping_cost_currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipping_cost_currency'), 'exclude': lambda f: f is None }})
     r"""**Required if shipping_cost is provided**<br>
@@ -73,15 +63,15 @@
     subtotal_price: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtotal_price'), 'exclude': lambda f: f is None }})
     total_price: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total_price'), 'exclude': lambda f: f is None }})
     r"""Total amount paid by the buyer for this order."""
     total_tax: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total_tax'), 'exclude': lambda f: f is None }})
     r"""Total tax amount paid by the buyer for this order."""
     weight: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight'), 'exclude': lambda f: f is None }})
     r"""Total weight of the order."""
-    weight_unit: Optional[WeightUnit] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
+    weight_unit: Optional[WeightUnitEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
     r"""The unit used for weight."""
     from_address: Optional[Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('from_address'), 'exclude': lambda f: f is None }})
     r"""<a href=\\"#tag/Addresses\\">Address</a> object of the sender / seller. Will be returned expanded by default."""
     line_items: Optional[List[LineItem]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line_items'), 'exclude': lambda f: f is None }})
     r"""Array of <a href=\\"#section/Line-Item\\">line item</a> objects representing the items in this order.
     All objects will be returned expanded by default.
     """
```

### Comparing `shippo-3.2.4/src/shippo/models/components/ordercreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/ordercreaterequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from .addresscreaterequest import AddressCreateRequest
 from .lineitembase import LineItemBase
-from .weightunit import WeightUnit
+from .orderstatusenum import OrderStatusEnum
+from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
-class OrderCreateRequestOrderStatus(str, Enum):
-    r"""Current state of the order. See the <a href=\\"https://docs.goshippo.com/docs/orders/orders/\\">orders tutorial</a>
-    for the logic of how the status is handled.
-    """
-    UNKNOWN = 'UNKNOWN'
-    AWAITPAY = 'AWAITPAY'
-    PAID = 'PAID'
-    REFUNDED = 'REFUNDED'
-    PARTIALLY_FULFILLED = 'PARTIALLY_FULFILLED'
-    SHIPPED = 'SHIPPED'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class OrderCreateRequest:
     placed_at: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('placed_at') }})
     r"""Date and time when the order was placed. This datetime can be different from the datetime of the order object creation on Shippo."""
     to_address: AddressCreateRequest = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('to_address') }})
@@ -33,15 +22,15 @@
     r"""**Required if total_price is provided**<br>
     Currency of the <code>total_price</code> and <code>total_tax</code> amounts.
     """
     notes: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
     r"""Custom buyer- or seller-provided notes about the order."""
     order_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order_number'), 'exclude': lambda f: f is None }})
     r"""An alphanumeric identifier for the order used by the seller/buyer. This identifier doesn't need to be unique."""
-    order_status: Optional[OrderCreateRequestOrderStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order_status'), 'exclude': lambda f: f is None }})
+    order_status: Optional[OrderStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order_status'), 'exclude': lambda f: f is None }})
     r"""Current state of the order. See the <a href=\\"https://docs.goshippo.com/docs/orders/orders/\\">orders tutorial</a>
     for the logic of how the status is handled.
     """
     shipping_cost: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipping_cost'), 'exclude': lambda f: f is None }})
     r"""Amount paid by the buyer for shipping. This amount can be different from the price the seller will actually pay for shipping."""
     shipping_cost_currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipping_cost_currency'), 'exclude': lambda f: f is None }})
     r"""**Required if shipping_cost is provided**<br>
@@ -54,15 +43,15 @@
     subtotal_price: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtotal_price'), 'exclude': lambda f: f is None }})
     total_price: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total_price'), 'exclude': lambda f: f is None }})
     r"""Total amount paid by the buyer for this order."""
     total_tax: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total_tax'), 'exclude': lambda f: f is None }})
     r"""Total tax amount paid by the buyer for this order."""
     weight: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight'), 'exclude': lambda f: f is None }})
     r"""Total weight of the order."""
-    weight_unit: Optional[WeightUnit] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
+    weight_unit: Optional[WeightUnitEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
     r"""The unit used for weight."""
     from_address: Optional[AddressCreateRequest] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('from_address'), 'exclude': lambda f: f is None }})
     r"""<a href=\\"#tag/Addresses\\">Address</a> object of the sender / seller. Will be returned expanded by default.."""
     line_items: Optional[List[LineItemBase]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line_items'), 'exclude': lambda f: f is None }})
     r"""Array of <a href=\\"#section/Line-Item\\">line item</a> objects representing the items in this order.
     All objects will be returned expanded by default.
     """
```

### Comparing `shippo-3.2.4/src/shippo/models/components/orderpaginatedlist.py` & `shippo-3.2.5/src/shippo/models/components/orderpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/parcel.py` & `shippo-3.2.5/src/shippo/models/components/parcel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .distanceunit import DistanceUnit
+from .distanceunitenum import DistanceUnitEnum
 from .parcelextra import ParcelExtra
-from .parceltemplateenumset import ParcelTemplateAramexAustralia, ParcelTemplateCouriersPlease, ParcelTemplateDHLeCommerce, ParcelTemplateDPDUK, ParcelTemplateFedEx, ParcelTemplateUPS, ParcelTemplateUSPS
-from .weightunit import WeightUnit
+from .parceltemplateenumset import ParcelTemplateAramexAustraliaEnum, ParcelTemplateCouriersPleaseEnum, ParcelTemplateDHLeCommerceEnum, ParcelTemplateDPDUKEnum, ParcelTemplateFedExEnum, ParcelTemplateUPSEnum, ParcelTemplateUSPSEnum
+from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from shippo import utils
 from typing import Optional, Union
 
-class ParcelObjectState(str, Enum):
+class ObjectState(str, Enum):
     r"""A Parcel will only be valid when all required values have been sent and validated successfully."""
     VALID = 'VALID'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Parcel:
-    distance_unit: DistanceUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
+    distance_unit: DistanceUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
     r"""The measure unit used for length, width and height."""
     height: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height') }})
     r"""**Required if template is not specified**<br>
     Height of the parcel. Up to six digits in front and four digits after the decimal separator are accepted.
     """
     length: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('length') }})
     r"""**Required if template is not specified**<br>
     Length of the Parcel. Up to six digits in front and four digits after the decimal separator are accepted.
     """
-    mass_unit: WeightUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mass_unit') }})
+    mass_unit: WeightUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mass_unit') }})
     r"""The unit used for weight."""
     weight: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight') }})
     r"""Weight of the parcel. Up to six digits in front and four digits after the decimal separator are accepted."""
     width: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width') }})
     r"""**Required if template is not specified**<br>
     Width of the Parcel. Up to six digits in front and four digits after the decimal separator are accepted.
     """
@@ -47,17 +47,17 @@
     r"""A string of up to 100 characters that can be filled with any additional information you want to attach to the object."""
     object_created: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""Date and time of Parcel creation."""
     object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the given Parcel object. This ID is required to create a Shipment object."""
     object_owner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_owner'), 'exclude': lambda f: f is None }})
     r"""Username of the user who created the Parcel object."""
-    object_state: Optional[ParcelObjectState] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_state'), 'exclude': lambda f: f is None }})
+    object_state: Optional[ObjectState] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_state'), 'exclude': lambda f: f is None }})
     r"""A Parcel will only be valid when all required values have been sent and validated successfully."""
     object_updated: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_updated'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""Date and time of last Parcel update. Since you cannot update Parcels after they were created, this time stamp reflects the time when the Parcel was changed by Shippo's systems for the last time, e.g., during sorting the dimensions given."""
-    template: Optional[Union[ParcelTemplateFedEx, ParcelTemplateUPS, ParcelTemplateUSPS, ParcelTemplateDHLeCommerce, ParcelTemplateDPDUK, ParcelTemplateCouriersPlease, ParcelTemplateAramexAustralia]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('template'), 'exclude': lambda f: f is None }})
+    template: Optional[Union[ParcelTemplateFedExEnum, ParcelTemplateUPSEnum, ParcelTemplateUSPSEnum, ParcelTemplateDHLeCommerceEnum, ParcelTemplateDPDUKEnum, ParcelTemplateCouriersPleaseEnum, ParcelTemplateAramexAustraliaEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('template'), 'exclude': lambda f: f is None }})
     r"""If template is passed, `length`, `width`, `height`, and `distance_unit` are not required"""
     test: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('test'), 'exclude': lambda f: f is None }})
     r"""Indicates whether the object has been created in test mode."""
```

### Comparing `shippo-3.2.4/src/shippo/models/components/parcelcreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/parcelcreaterequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .distanceunit import DistanceUnit
-from .parceltemplateenumset import ParcelTemplateAramexAustralia, ParcelTemplateCouriersPlease, ParcelTemplateDHLeCommerce, ParcelTemplateDPDUK, ParcelTemplateFedEx, ParcelTemplateUPS, ParcelTemplateUSPS
-from .weightunit import WeightUnit
+from .distanceunitenum import DistanceUnitEnum
+from .parceltemplateenumset import ParcelTemplateAramexAustraliaEnum, ParcelTemplateCouriersPleaseEnum, ParcelTemplateDHLeCommerceEnum, ParcelTemplateDPDUKEnum, ParcelTemplateFedExEnum, ParcelTemplateUPSEnum, ParcelTemplateUSPSEnum
+from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional, Union
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ParcelCreateRequest:
-    distance_unit: DistanceUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
+    distance_unit: DistanceUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
     r"""The measure unit used for length, width and height."""
     height: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height') }})
     r"""**Required if template is not specified**<br>
     Height of the parcel. Up to six digits in front and four digits after the decimal separator are accepted.
     """
     length: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('length') }})
     r"""**Required if template is not specified**<br>
     Length of the Parcel. Up to six digits in front and four digits after the decimal separator are accepted.
     """
-    mass_unit: WeightUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mass_unit') }})
+    mass_unit: WeightUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mass_unit') }})
     r"""The unit used for weight."""
     weight: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight') }})
     r"""Weight of the parcel. Up to six digits in front and four digits after the decimal separator are accepted."""
     width: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width') }})
     r"""**Required if template is not specified**<br>
     Width of the Parcel. Up to six digits in front and four digits after the decimal separator are accepted.
     """
-    template: Optional[Union[ParcelTemplateFedEx, ParcelTemplateUPS, ParcelTemplateUSPS, ParcelTemplateDHLeCommerce, ParcelTemplateDPDUK, ParcelTemplateCouriersPlease, ParcelTemplateAramexAustralia]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('template'), 'exclude': lambda f: f is None }})
+    template: Optional[Union[ParcelTemplateFedExEnum, ParcelTemplateUPSEnum, ParcelTemplateUSPSEnum, ParcelTemplateDHLeCommerceEnum, ParcelTemplateDPDUKEnum, ParcelTemplateCouriersPleaseEnum, ParcelTemplateAramexAustraliaEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('template'), 'exclude': lambda f: f is None }})
     r"""If template is passed, `length`, `width`, `height`, and `distance_unit` are not required"""
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.2.4/src/shippo/models/components/parcelextra.py` & `shippo-3.2.5/src/shippo/models/components/parcelextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/parcelinsurance.py` & `shippo-3.2.5/src/shippo/models/components/parcelinsurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/parcelpaginatedlist.py` & `shippo-3.2.5/src/shippo/models/components/parcelpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/parcelrequest.py` & `shippo-3.2.5/src/shippo/models/components/parcelrequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .distanceunit import DistanceUnit
+from .distanceunitenum import DistanceUnitEnum
 from .parcelextra import ParcelExtra
-from .parceltemplateenumset import ParcelTemplateAramexAustralia, ParcelTemplateCouriersPlease, ParcelTemplateDHLeCommerce, ParcelTemplateDPDUK, ParcelTemplateFedEx, ParcelTemplateUPS, ParcelTemplateUSPS
-from .weightunit import WeightUnit
+from .parceltemplateenumset import ParcelTemplateAramexAustraliaEnum, ParcelTemplateCouriersPleaseEnum, ParcelTemplateDHLeCommerceEnum, ParcelTemplateDPDUKEnum, ParcelTemplateFedExEnum, ParcelTemplateUPSEnum, ParcelTemplateUSPSEnum
+from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional, Union
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ParcelRequest:
-    distance_unit: DistanceUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
+    distance_unit: DistanceUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
     r"""The measure unit used for length, width and height."""
     height: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height') }})
     r"""Required if template is not specified. Height of the parcel. Up to six digits in front and four digits after the decimal separator are accepted."""
     length: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('length') }})
     r"""Required if template is not specified. Length of the Parcel. Up to six digits in front and four digits after the decimal separator are accepted."""
-    mass_unit: WeightUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mass_unit') }})
+    mass_unit: WeightUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mass_unit') }})
     r"""The unit used for weight."""
     weight: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight') }})
     r"""Weight of the parcel. Up to six digits in front and four digits after the decimal separator are accepted."""
     width: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width') }})
     r"""Required if template is not specified. Width of the Parcel. Up to six digits in front and four digits after the decimal separator are accepted."""
     extra: Optional[ParcelExtra] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extra'), 'exclude': lambda f: f is None }})
     r"""An object holding optional extra services to be requested for each parcel in a multi-piece shipment.
     See the <a href=\"#section/Parcel-Extras\">Parcel Extra table below</a> for all available services.
     """
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""A string of up to 100 characters that can be filled with any additional information you want to attach to the object."""
-    template: Optional[Union[ParcelTemplateFedEx, ParcelTemplateUPS, ParcelTemplateUSPS, ParcelTemplateDHLeCommerce, ParcelTemplateDPDUK, ParcelTemplateCouriersPlease, ParcelTemplateAramexAustralia]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('template'), 'exclude': lambda f: f is None }})
+    template: Optional[Union[ParcelTemplateFedExEnum, ParcelTemplateUPSEnum, ParcelTemplateUSPSEnum, ParcelTemplateDHLeCommerceEnum, ParcelTemplateDPDUKEnum, ParcelTemplateCouriersPleaseEnum, ParcelTemplateAramexAustraliaEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('template'), 'exclude': lambda f: f is None }})
     r"""If template is passed, `length`, `width`, `height`, and `distance_unit` are not required"""
     test: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('test'), 'exclude': lambda f: f is None }})
     r"""Indicates whether the object has been created in test mode."""
```

### Comparing `shippo-3.2.4/src/shippo/models/components/parceltemplateenumset.py` & `shippo-3.2.5/src/shippo/models/components/parceltemplateenumset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
-class ParcelTemplateAramexAustralia(str, Enum):
+class ParcelTemplateAramexAustraliaEnum(str, Enum):
     r"""|Token | Name | Dimensions|
     |:---|:---|:---|
     | Fastway_Australia_Satchel_A2 | Satchel A2 | 594.00 x 420.00 x 48.00 mm|
     | Fastway_Australia_Satchel_A3 | Satchel A3 | 420.00 x 297.00 x 64.00 mm|
     | Fastway_Australia_Satchel_A4 | Satchel A4 | 297.00 x 210.00 x 64.00 mm|
     | Fastway_Australia_Satchel_A5 | Satchel A5 | 210.00 x 148.00 x 64.00 mm|
     """
     FASTWAY_AUSTRALIA_SATCHEL_A2 = 'Fastway_Australia_Satchel_A2'
     FASTWAY_AUSTRALIA_SATCHEL_A3 = 'Fastway_Australia_Satchel_A3'
     FASTWAY_AUSTRALIA_SATCHEL_A4 = 'Fastway_Australia_Satchel_A4'
     FASTWAY_AUSTRALIA_SATCHEL_A5 = 'Fastway_Australia_Satchel_A5'
 
-class ParcelTemplateCouriersPlease(str, Enum):
+class ParcelTemplateCouriersPleaseEnum(str, Enum):
     r"""|Token | Name | Dimensions|
     |:---|:---|:---|
     | couriersplease_500g_satchel | 500g Satchel | 22.00 x 33.50 x 0.10 cm|
     | couriersplease_1kg_satchel | 1kg Satchel | 28.00 x 35.00 x 0.10 cm|
     | couriersplease_3kg_satchel | 3kg Satchel | 34.00 x 42.00 x 0.10 cm|
     | couriersplease_5kg_satchel | 5kg Satchel | 43.70 x 59.70 x 0.10 cm|
     """
     COURIERSPLEASE_500G_SATCHEL = 'couriersplease_500g_satchel'
     COURIERSPLEASE_1KG_SATCHEL = 'couriersplease_1kg_satchel'
     COURIERSPLEASE_3KG_SATCHEL = 'couriersplease_3kg_satchel'
     COURIERSPLEASE_5KG_SATCHEL = 'couriersplease_5kg_satchel'
 
-class ParcelTemplateDPDUK(str, Enum):
+class ParcelTemplateDPDUKEnum(str, Enum):
     r"""|Token | Name | Dimensions|
     |:---|:---|:---|
     | DPD_UK_Express_Pak| DPD UK Express Pak | 530.00 x 400.00 x 100.00 mm|
     """
     DPD_UK_EXPRESS_PAK = 'DPD_UK_Express_Pak'
 
-class ParcelTemplateDHLeCommerce(str, Enum):
+class ParcelTemplateDHLeCommerceEnum(str, Enum):
     r"""|Token | Name | Dimensions|
     |:---|:---|:---|
     | DHLeC_Irregular | Irregular Shipment | 10.00 x 10.00 x 10.00 in|
     | DHLeC_SM_Flats | Flats | 27.00 x 17.00 x 17.00 in|
     """
     DH_LE_C_IRREGULAR = 'DHLeC_Irregular'
     DH_LE_C_SM_FLATS = 'DHLeC_SM_Flats'
 
-class ParcelTemplateUSPS(str, Enum):
+class ParcelTemplateUSPSEnum(str, Enum):
     r"""|Token | Name | Dimensions|
     |:---|:---|:---|
     | USPS_FlatRateCardboardEnvelope | Flat Rate Cardboard Envelope |  12.50 x 9.50 x 0.75 in |
     | USPS_FlatRateEnvelope | Flat Rate Envelope |  12.50 x 9.50 x 0.75 in |
     | USPS_FlatRateGiftCardEnvelope | Flat Rate Gift Card Envelope |  10.00 x 7.00 x 0.75 in |
     | USPS_FlatRateLegalEnvelope | Flat Rate Legal Envelope |  15.00 x 9.50 x 0.75 in |
     | USPS_FlatRatePaddedEnvelope | Flat Rate Padded Envelope |  12.50 x 9.50 x 1.00 in |
@@ -86,15 +86,15 @@
     USPS_REGIONAL_RATE_BOX_A2 = 'USPS_RegionalRateBoxA2'
     USPS_REGIONAL_RATE_BOX_B1 = 'USPS_RegionalRateBoxB1'
     USPS_REGIONAL_RATE_BOX_B2 = 'USPS_RegionalRateBoxB2'
     USPS_SMALL_FLAT_RATE_BOX = 'USPS_SmallFlatRateBox'
     USPS_SMALL_FLAT_RATE_ENVELOPE = 'USPS_SmallFlatRateEnvelope'
     USPS_SOFT_PACK = 'USPS_SoftPack'
 
-class ParcelTemplateUPS(str, Enum):
+class ParcelTemplateUPSEnum(str, Enum):
     r"""|Token | Name | Dimensions|
     |:---|:---|:---|
     | UPS_Box_10kg | Box 10kg | 410.00 x 335.00 x 265.00 mm|
     | UPS_Box_25kg | Box 25kg | 484.00 x 433.00 x 350.00 mm|
     | UPS_Express_Box | Express Box | 460.00 x 315.00 x 95.00 mm|
     | UPS_Express_Box_Large | Express Box Large | 18.00 x 13.00 x 3.00 in|
     | UPS_Express_Box_Medium | Express Box Medium | 15.00 x 11.00 x 3.00 in|
@@ -141,15 +141,15 @@
     UPS_MI_MEDIA_MAIL = 'UPS_MI_MEDIA_MAIL'
     UPS_MI_PARCEL_POST = 'UPS_MI_Parcel_Post'
     UPS_MI_PRIORITY = 'UPS_MI_Priority'
     UPS_MI_STANDARD_FLAT = 'UPS_MI_Standard_Flat'
     UPS_PAD_PAK = 'UPS_Pad_Pak'
     UPS_PALLET = 'UPS_Pallet'
 
-class ParcelTemplateFedEx(str, Enum):
+class ParcelTemplateFedExEnum(str, Enum):
     r"""|Token | Name | Dimensions|
     |:---|:---|:---|
     | FedEx_Box_10kg | FedEx® 10kg Box | 15.81 x 12.94 x 10.19 in|
     | FedEx_Box_25kg | FedEx® 25kg Box | 54.80 x 42.10 x 33.50 in|
     | FedEx_Box_Extra_Large_1 | FedEx® Extra Large Box (X1) | 11.88 x 11.00 x 10.75 in|
     | FedEx_Box_Extra_Large_2 | FedEx® Extra Large Box (X2) | 15.75 x 14.13 x 6.00 in|
     | FedEx_Box_Large_1 | FedEx® Large Box (L1) | 17.50 x 12.38 x 3.00 in|
```

### Comparing `shippo-3.2.4/src/shippo/models/components/pickup.py` & `shippo-3.2.5/src/shippo/models/components/pickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/pickupbase.py` & `shippo-3.2.5/src/shippo/models/components/pickupbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/ponumber.py` & `shippo-3.2.5/src/shippo/models/components/ponumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/rate.py` & `shippo-3.2.5/src/shippo/models/components/rate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/ratemessage.py` & `shippo-3.2.5/src/shippo/models/components/ratemessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/ratepaginatedlist.py` & `shippo-3.2.5/src/shippo/models/components/ratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/refund.py` & `shippo-3.2.5/src/shippo/models/components/refund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/refundpaginatedlist.py` & `shippo-3.2.5/src/shippo/models/components/refundpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/refundrequestbody.py` & `shippo-3.2.5/src/shippo/models/components/refundrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/rmanumber.py` & `shippo-3.2.5/src/shippo/models/components/rmanumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/servicegroup.py` & `shippo-3.2.5/src/shippo/models/components/servicegroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .servicegrouptype import ServiceGroupType
+from .servicegrouptypeenum import ServiceGroupTypeEnum
 from .servicelevel import ServiceLevel
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ServiceGroup:
     description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
     r"""Description for the service group"""
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     r"""Name for the service group that will be shown to customers in the response"""
-    type: ServiceGroupType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    type: ServiceGroupTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
     r"""The type of the service group.<br> `LIVE_RATE` - Shippo will make a rating request and return real-time rates for the shipping group, only falling back to the specified flat rate amount if no rates match a service level in the service group.<br> `FLAT_RATE` - Returns a shipping option with the specified flat rate amount.<br> `FREE_SHIPPING` - Returns a shipping option with a price of $0 only if the total cost of items exceeds the amount defined by `free_shipping_threshold_min`"""
     object_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id') }})
     r"""The unique identifier of the given Service Group object."""
     service_levels: List[ServiceLevel] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service_levels') }})
     flat_rate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('flat_rate'), 'exclude': lambda f: f is None }})
     r"""String representation of an amount to be returned as the flat rate
     if 1. The service group is of type `LIVE_RATE` and no matching rates
```

### Comparing `shippo-3.2.4/src/shippo/models/components/servicegroupaccountandservicelevel.py` & `shippo-3.2.5/src/shippo/models/components/servicegroupaccountandservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/servicegroupcreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/servicegroupcreaterequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from .servicegroupaccountandservicelevel import ServiceGroupAccountAndServiceLevel
-from .servicegrouptype import ServiceGroupType
+from .servicegrouptypeenum import ServiceGroupTypeEnum
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ServiceGroupCreateRequest:
     description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
     r"""Description for the service group"""
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     r"""Name for the service group that will be shown to customers in the response"""
-    type: ServiceGroupType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    type: ServiceGroupTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
     r"""The type of the service group.<br> `LIVE_RATE` - Shippo will make a rating request and return real-time rates for the shipping group, only falling back to the specified flat rate amount if no rates match a service level in the service group.<br> `FLAT_RATE` - Returns a shipping option with the specified flat rate amount.<br> `FREE_SHIPPING` - Returns a shipping option with a price of $0 only if the total cost of items exceeds the amount defined by `free_shipping_threshold_min`"""
     service_levels: List[ServiceGroupAccountAndServiceLevel] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service_levels') }})
     flat_rate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('flat_rate'), 'exclude': lambda f: f is None }})
     r"""String representation of an amount to be returned as the flat rate
     if 1. The service group is of type `LIVE_RATE` and no matching rates
     were found; or 2. The service group is of type `FLAT_RATE`. Either
     integers or decimals are accepted. Required unless type is
```

### Comparing `shippo-3.2.4/src/shippo/models/components/servicegrouptype.py` & `shippo-3.2.5/src/shippo/models/components/servicegrouptypeenum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
-class ServiceGroupType(str, Enum):
+class ServiceGroupTypeEnum(str, Enum):
     r"""The type of the service group.<br> `LIVE_RATE` - Shippo will make a rating request and return real-time rates for the shipping group, only falling back to the specified flat rate amount if no rates match a service level in the service group.<br> `FLAT_RATE` - Returns a shipping option with the specified flat rate amount.<br> `FREE_SHIPPING` - Returns a shipping option with a price of $0 only if the total cost of items exceeds the amount defined by `free_shipping_threshold_min`"""
     LIVE_RATE = 'LIVE_RATE'
     FLAT_RATE = 'FLAT_RATE'
     FREE_SHIPPING = 'FREE_SHIPPING'
```

### Comparing `shippo-3.2.4/src/shippo/models/components/servicegroupupdaterequest.py` & `shippo-3.2.5/src/shippo/models/components/servicegroupupdaterequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from .servicegroupaccountandservicelevel import ServiceGroupAccountAndServiceLevel
-from .servicegrouptype import ServiceGroupType
+from .servicegrouptypeenum import ServiceGroupTypeEnum
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ServiceGroupUpdateRequest:
     description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
     r"""Description for the service group"""
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     r"""Name for the service group that will be shown to customers in the response"""
-    type: ServiceGroupType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    type: ServiceGroupTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
     r"""The type of the service group.<br> `LIVE_RATE` - Shippo will make a rating request and return real-time rates for the shipping group, only falling back to the specified flat rate amount if no rates match a service level in the service group.<br> `FLAT_RATE` - Returns a shipping option with the specified flat rate amount.<br> `FREE_SHIPPING` - Returns a shipping option with a price of $0 only if the total cost of items exceeds the amount defined by `free_shipping_threshold_min`"""
     object_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id') }})
     r"""The unique identifier of the given Service Group object."""
     is_active: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_active') }})
     r"""True if the service group is enabled, false otherwise."""
     service_levels: List[ServiceGroupAccountAndServiceLevel] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service_levels') }})
     flat_rate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('flat_rate'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.2.4/src/shippo/models/components/servicelevel.py` & `shippo-3.2.5/src/shippo/models/components/servicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/servicelevelenumset.py` & `shippo-3.2.5/src/shippo/models/components/servicelevelenumset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
-class ServiceLevelSwyft(str, Enum):
+class ServiceLevelSwyftEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | same_day | Next Day|
     | next_day | Next Day|
     """
     SAME_DAY = 'same_day'
     NEXT_DAY = 'next_day'
 
-class ServiceLevelVeho(str, Enum):
+class ServiceLevelVehoEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | veho_next_day | Veho Next Day |
     """
     VEHO_NEXT_DAY = 'veho_next_day'
 
-class ServiceLevelUDS(str, Enum):
+class ServiceLevelUDSEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | uds_next_day | Next Day|
     """
     UDS_NEXT_DAY = 'uds_next_day'
 
-class ServiceLevelEvriUK(str, Enum):
+class ServiceLevelEvriUKEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | hermes_uk_courier_service | Courier Collection|
     | hermes_uk_parcelshop_dropoff | ParcelShop Drop-Off|
     | hermes_uk_parcelshop_dropoff_nextday | ParcelShop Drop-Off Next Day|
     | hermes_uk_postable | Postable|
     | hermes_uk_postable_nextday | Postable Next Day|
     """
     HERMES_UK_COURIER_SERVICE = 'hermes_uk_courier_service'
     HERMES_UK_PARCELSHOP_DROPOFF = 'hermes_uk_parcelshop_dropoff'
     HERMES_UK_PARCELSHOP_DROPOFF_NEXTDAY = 'hermes_uk_parcelshop_dropoff_nextday'
     HERMES_UK_POSTABLE = 'hermes_uk_postable'
     HERMES_UK_POSTABLE_NEXTDAY = 'hermes_uk_postable_nextday'
 
-class ServiceLevelLasership(str, Enum):
+class ServiceLevelLasershipEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | lasership_routed_delivery | Routed Delivery|
     """
     LASERSHIP_ROUTED_DELIVERY = 'lasership_routed_delivery'
 
-class ServiceLevelOnTrac(str, Enum):
+class ServiceLevelOnTracEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | ontrac_ground | Ground|
     | ontrac_sunrise_gold | Sunrise Gold|
     | ontrac_sunrise | Sunrise|
     """
     ONTRAC_GROUND = 'ontrac_ground'
     ONTRAC_SUNRISE_GOLD = 'ontrac_sunrise_gold'
     ONTRAC_SUNRISE = 'ontrac_sunrise'
 
-class ServiceLevelSendle(str, Enum):
+class ServiceLevelSendleEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | sendle_parcel | Sendle Parcel|
     """
     SENDLE_PARCEL = 'sendle_parcel'
 
-class ServiceLevelRoyalMail(str, Enum):
+class ServiceLevelRoyalMailEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | royal_mail_tracked_letter_boxable_24_no_signature | Royal Mail Tracked Letter-Boxable 24 No Signature|
     | royal_mail_tracked_letter_boxable_48_no_signature | Royal Mail Tracked Letter-Boxable 48 No Signature|
     | royal_mail_tracked_24_returns | Royal Mail Tracked Returns 24|
     | royal_mail_tracked_48_returns | Royal Mail Tracked Returns 48|
     | royal_mail_special_delivery_guaranteed_1pm | Special Delivery Guaranteed by 1pm
@@ -107,15 +107,15 @@
     ROYAL_MAIL_INTL_BUS_MAIL_LRG_LTR_ZONE_SORT_PRI = 'royal_mail_intl_bus_mail_lrg_ltr_zone_sort_pri'
     ROYAL_MAIL_INTL_BUS_PARCELS_TRACKED_ZONE_SORT = 'royal_mail_intl_bus_parcels_tracked_zone_sort'
     ROYAL_MAIL_INTL_BUS_PARCELS_TRACKED_COUNTRY_PRICED = 'royal_mail_intl_bus_parcels_tracked_country_priced'
     ROYAL_MAIL_INTL_BUS_PARCELS_TRACKED_SIGNED_ZONE_SRT = 'royal_mail_intl_bus_parcels_tracked_signed_zone_srt'
     ROYAL_MAIL_24_FLAT_RATE = 'royal_mail_24_flat_rate'
     ROYAL_MAIL_48_FLAT_RATE = 'royal_mail_48_flat_rate'
 
-class ServiceLevelePostGlobal(str, Enum):
+class ServiceLevelePostGlobalEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | rr_donnelley_domestic_economy_parcel | Domestic Economy Parcel|
     | rr_donnelley_domestic_priority_parcel | Domestic Priority Parcel |
     | rr_donnelley_domestic_parcel_bpm | Domestic Parcel BPM|
     | rr_donnelley_priority_domestic_priority_parcel_bpm | Domestic Priority Parcel BPM|
     | rr_donnelley_priority_parcel_delcon | International Priority Parcel DelCon|
@@ -138,47 +138,47 @@
     RR_DONNELLEY_IPA = 'rr_donnelley_ipa'
     RR_DONNELLEY_COURIER = 'rr_donnelley_courier'
     RR_DONNELLEY_ISAL = 'rr_donnelley_isal'
     RR_DONNELLEY_EPACKET = 'rr_donnelley_epacket'
     RR_DONNELLEY_PMI = 'rr_donnelley_pmi'
     RR_DONNELLEY_EMI = 'rr_donnelley_emi'
 
-class ServiceLevelPostItaliane(str, Enum):
+class ServiceLevelPostItalianeEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | poste_italiane_delivery_business_express | Poste Delivery Business Express|
     """
     POSTE_ITALIANE_DELIVERY_BUSINESS_EXPRESS = 'poste_italiane_delivery_business_express'
 
-class ServiceLevelParcelforce(str, Enum):
+class ServiceLevelParcelforceEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | parcelforce_express48 | Express 48|
     | parcelforce_express24 | Express 24|
     | parcelforce_expressam | Express AM|
     """
     PARCELFORCE_EXPRESS48 = 'parcelforce_express48'
     PARCELFORCE_EXPRESS24 = 'parcelforce_express24'
     PARCELFORCE_EXPRESSAM = 'parcelforce_expressam'
 
-class ServiceLevelMaergo(str, Enum):
+class ServiceLevelMaergoEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | x_delivery_expedited | Expedited|
     """
     X_DELIVERY_EXPEDITED = 'x_delivery_expedited'
 
-class ServiceLevelMondialRelay(str, Enum):
+class ServiceLevelMondialRelayEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | mondial_relay_pointrelais | Point Relais|
     """
     MONDIAL_RELAY_POINTRELAIS = 'mondial_relay_pointrelais'
 
-class ServiceLevelLSO(str, Enum):
+class ServiceLevelLSOEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | lso_ground | Ground|
     | lso_economy_next_day | Economy Next Day|
     | lso_saturday_delivery | Saturday Delivery|
     | lso_2nd_day | 2nd Day|
     | lso_priority_next_day | Priority Next Day|
@@ -187,15 +187,15 @@
     LSO_GROUND = 'lso_ground'
     LSO_ECONOMY_NEXT_DAY = 'lso_economy_next_day'
     LSO_SATURDAY_DELIVERY = 'lso_saturday_delivery'
     LSO_2ND_DAY = 'lso_2nd_day'
     LSO_PRIORITY_NEXT_DAY = 'lso_priority_next_day'
     LSO_EARLY_OVERNIGHT = 'lso_early_overnight'
 
-class ServiceLevelGLSUS(str, Enum):
+class ServiceLevelGLSUSEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | gls_us_cps | GSO Ground|
     | gls_us_eps | Early Priority Overnight|
     | gls_us_ess | Early Saturday Delivery|
     | gls_us_nps | Noon Priority Overnight|
     | gls_us_pds | Priority Overnight|
@@ -204,15 +204,15 @@
     GLS_US_CPS = 'gls_us_cps'
     GLS_US_EPS = 'gls_us_eps'
     GLS_US_ESS = 'gls_us_ess'
     GLS_US_NPS = 'gls_us_nps'
     GLS_US_PDS = 'gls_us_pds'
     GLS_US_SDS = 'gls_us_sds'
 
-class ServiceLevelGlobegistics(str, Enum):
+class ServiceLevelGlobegisticsEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | globegistics_priority_mail_express_international | Globegistics Priority Mail Express International|
     | globegistics_priority_mail_international | Globegistics Priority Mail International|
     | globegistics_priority_mail_express_international_pds | Globegistics Priority Mail Express International PreSort Drop Ship|
     | globegistics_priority_mail_international_pds | Globegistics Priority Mail International PreSort Drop Ship|
     | globegistics_epacket | Globegistics ePacket|
@@ -233,30 +233,30 @@
     GLOBEGISTICS_ECOM_PACKET_DDP = 'globegistics_ecom_packet_ddp'
     GLOBEGISTICS_ECOM_PRIORITY_MAIL_INTERNATIONAL_DDP = 'globegistics_ecom_priority_mail_international_ddp'
     GLOBEGISTICS_ECOM_PRIORITY_MAIL_EXPRESS_INTERNATIONAL_DDP = 'globegistics_ecom_priority_mail_express_international_ddp'
     GLOBEGISTICS_ECOM_EXTRA = 'globegistics_ecom_extra'
     GLOBEGISTICS_ECOM_INTERNATIONAL_PRIORITY_AIRMAIL = 'globegistics_ecom_international_priority_airmail'
     GLOBEGISTICS_ECOM_INTERNATIONAL_SURFACE_AIRLIFT = 'globegistics_ecom_international_surface_airlift'
 
-class ServiceLevelAramexAustralia(str, Enum):
+class ServiceLevelAramexAustraliaEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | fastway_australia_parcel | Parcel|
     | fastway_australia_satchel | Satchel|
     | fastway_australia_box_small | Box Small|
     | fastway_australia_box_medium | Box Medium|
     | fastway_australia_box_large | Box Large|
     """
     FASTWAY_AUSTRALIA_PARCEL = 'fastway_australia_parcel'
     FASTWAY_AUSTRALIA_SATCHEL = 'fastway_australia_satchel'
     FASTWAY_AUSTRALIA_BOX_SMALL = 'fastway_australia_box_small'
     FASTWAY_AUSTRALIA_BOX_MEDIUM = 'fastway_australia_box_medium'
     FASTWAY_AUSTRALIA_BOX_LARGE = 'fastway_australia_box_large'
 
-class ServiceLevelDeutschePost(str, Enum):
+class ServiceLevelDeutschePostEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | deutsche_post_postkarte | Postkarte|
     | deutsche_post_standardbrief | Standardbrief|
     | deutsche_post_kompaktbrief | Kompaktbrief|
     | deutsche_post_grossbrief | Grossbrief|
     | deutsche_post_maxibrief | Maxibrief|
@@ -273,15 +273,15 @@
     DEUTSCHE_POST_MAXIBRIEF = 'deutsche_post_maxibrief'
     DEUTSCHE_POST_MAXIBRIEF_PLUS = 'deutsche_post_maxibrief_plus'
     DEUTSCHE_POST_WARENPOST_INTERNATIONAL_XS = 'deutsche_post_warenpost_international_xs'
     DEUTSCHE_POST_WARENPOST_INTERNATIONAL_S = 'deutsche_post_warenpost_international_s'
     DEUTSCHE_POST_WARENPOST_INTERNATIONAL_M = 'deutsche_post_warenpost_international_m'
     DEUTSCHE_POST_WARENPOST_INTERNATIONAL_L = 'deutsche_post_warenpost_international_l'
 
-class ServiceLevelDPDUK(str, Enum):
+class ServiceLevelDPDUKEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | dpd_uk_ship_to_shop | Ship to shop|
     | dpd_uk_1030 | Door to door 10.30 next day|
     | dpd_uk_1200 | Door to door 12.00 next day|
     | dpd_uk_saturday | Saturday Delivery|
     | dpd_uk_saturday_1030 | Saturday Delivery 10.30|
@@ -312,22 +312,22 @@
     DPD_UK_CLASSIC = 'dpd_uk_classic'
     DPD_UK_AIR_CLASSIC = 'dpd_uk_air_classic'
     DPD_UK_AIR_EXPRESS = 'dpd_uk_air_express'
     DPD_UK_DIRECT = 'dpd_uk_direct'
     DPD_UK_DIRECT_TRACKED_MAIL = 'dpd_uk_direct_tracked_mail'
     DPD_UK_PICKUP_RETURNS = 'dpd_uk_pickup_returns'
 
-class ServiceLevelDPDDE(str, Enum):
+class ServiceLevelDPDDEEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | dpd_de_classic | DPD Classic|
     """
     DPD_DE_CLASSIC = 'dpd_de_classic'
 
-class ServiceLevelDHLGermany(str, Enum):
+class ServiceLevelDHLGermanyEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | dhl_germany_europaket | DHL Germany Europaket|
     | dhl_germany_paket | DHL Germany Paket|
     | dhl_germany_paket_connect | DHL Germany Paket Connect|
     | dhl_germany_paket_international | DHL Germany Paket International|
     | dhl_germany_paket_priority | DHL Germany Paket Priority|
@@ -336,15 +336,15 @@
     DHL_GERMANY_EUROPAKET = 'dhl_germany_europaket'
     DHL_GERMANY_PAKET = 'dhl_germany_paket'
     DHL_GERMANY_PAKET_CONNECT = 'dhl_germany_paket_connect'
     DHL_GERMANY_PAKET_INTERNATIONAL = 'dhl_germany_paket_international'
     DHL_GERMANY_PAKET_PRIORITY = 'dhl_germany_paket_priority'
     DHL_GERMANY_PAKET_SAMEDAY = 'dhl_germany_paket_sameday'
 
-class ServiceLevelDHLeCommerce(str, Enum):
+class ServiceLevelDHLeCommerceEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | dhl_ecommerce_marketing_parcel_expedited | Marketing Parcel Expedited|
     | dhl_ecommerce_globalmail_business_ipa | GlobalMail Business IPA|
     | dhl_ecommerce_parcel_international_direct | Parcel International Direct|
     | dhl_ecommerce_parcels_expedited_max | Parcels Expedited Max|
     | dhl_ecommerce_bpm_ground | Bounded Printed Matter Ground|
@@ -397,15 +397,15 @@
     DHL_ECOMMERCE_GLOBALMAIL_PACKET_PRIORITY = 'dhl_ecommerce_globalmail_packet_priority'
     DHL_ECOMMERCE_EASY_RETURN_LIGHT = 'dhl_ecommerce_easy_return_light'
     DHL_ECOMMERCE_PARCEL_PLUS_EXPEDITED = 'dhl_ecommerce_parcel_plus_expedited'
     DHL_ECOMMERCE_GLOBALMAIL_BUSINESS_STANDARD = 'dhl_ecommerce_globalmail_business_standard'
     DHL_ECOMMERCE_GROUND = 'dhl_ecommerce_ground'
     DHL_ECOMMERCE_GLOBALMAIL_PACKET_STANDARD = 'dhl_ecommerce_globalmail_packet_standard'
 
-class ServiceLevelDHLExpress(str, Enum):
+class ServiceLevelDHLExpressEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | dhl_express_domestic_express_doc | Domestic Express Doc|
     | dhl_express_economy_select_doc | Economy Select Doc|
     | dhl_express_worldwide_nondoc | Express Worldwide Nondoc|
     | dhl_express_worldwide_doc | Express Worldwide Doc|
     | dhl_express_worldwide | Worldwide|
@@ -446,15 +446,15 @@
     DHL_EXPRESS_EXPRESS_12_00_NONDOC = 'dhl_express_express_12_00_nondoc'
     DHL_EXPRESS_EXPRESS_12_DOC = 'dhl_express_express_12_doc'
     DHL_EXPRESS_WORLDWIDE_B2C_DOC = 'dhl_express_worldwide_b2c_doc'
     DHL_EXPRESS_WORLDWIDE_B2C_NONDOC = 'dhl_express_worldwide_b2c_nondoc'
     DHL_EXPRESS_MEDICAL_EXPRESS = 'dhl_express_medical_express'
     DHL_EXPRESS_EXPRESS_EASY_NONDOC = 'dhl_express_express_easy_nondoc'
 
-class ServiceLevelPurolator(str, Enum):
+class ServiceLevelPurolatorEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | purolator_ground | Ground|
     | purolator_ground9_am | Ground 9am|
     | purolator_ground1030_am | Ground 10:30am|
     | purolator_ground_distribution | Ground Distribution|
     | purolator_ground_evening | Ground Evening|
@@ -487,35 +487,35 @@
     PUROLATOR_EXPRESS_US1030_AM = 'purolator_express_us1030_am'
     PUROLATOR_EXPRESS_US1200 = 'purolator_express_us1200'
     PUROLATOR_EXPRESS_INTERNATIONAL = 'purolator_express_international'
     PUROLATOR_EXPRESS_INTERNATIONAL9_AM = 'purolator_express_international9_am'
     PUROLATOR_EXPRESS_INTERNATIONAL1030_AM = 'purolator_express_international1030_am'
     PUROLATOR_EXPRESS_INTERNATIONAL1200 = 'purolator_express_international1200'
 
-class ServiceLevelColissimo(str, Enum):
+class ServiceLevelColissimoEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | colissimo_home | Domicile|
     | colissimo_pick_up_point | Point Retrait|
     | colissimo_return_mainland_france | Retour France|
     """
     COLISSIMO_HOME = 'colissimo_home'
     COLISSIMO_PICK_UP_POINT = 'colissimo_pick_up_point'
     COLISSIMO_RETURN_MAINLAND_FRANCE = 'colissimo_return_mainland_france'
 
-class ServiceLevelCorreosEspana(str, Enum):
+class ServiceLevelCorreosEspanaEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | correos_standard_home| Paquete Estándar|
     | correos_premium_home | Paquete Premium|
     """
     CORREOS_STANDARD_HOME = 'correos_standard_home'
     CORREOS_PREMIUM_HOME = 'correos_premium_home'
 
-class ServiceLevelCouriersPlease(str, Enum):
+class ServiceLevelCouriersPleaseEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | couriersplease_domestic_priority_auth_to_leave | Domestic Priority - Authority To Leave/POPPoints|
     | couriersplease_domestic_priority_sign_required | Domestic Priority - Signature Required|
     | couriersplease_gold_domestic_auth_to_leave | Gold Domestic - Authority To Leave/POPPoints|
     | couriersplease_gold_domestic_sign_required | Gold Domestic - Signature Required|
     | couriersplease_off_peak_auth_to_leave | Off Peak - Authority To Leave/POPPoints|
@@ -534,15 +534,15 @@
     COURIERSPLEASE_OFF_PEAK_SIGN_REQUIRED = 'couriersplease_off_peak_sign_required'
     COURIERSPLEASE_PARCEL_AUTH_TO_LEAVE = 'couriersplease_parcel_auth_to_leave'
     COURIERSPLEASE_PARCEL_SIGN_REQUIRED = 'couriersplease_parcel_sign_required'
     COURIERSPLEASE_ROAD_EXPRESS = 'couriersplease_road_express'
     COURIERSPLEASE_SATCHEL_AUTH_TO_LEAVE = 'couriersplease_satchel_auth_to_leave'
     COURIERSPLEASE_SATCHEL_SIGN_REQUIRED = 'couriersplease_satchel_sign_required'
 
-class ServiceLevelChronopost(str, Enum):
+class ServiceLevelChronopostEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | chronopost_13 | Chrono 13|
     | chronopost_10 | Chrono 10|
     | chronopost_18| Chrono 18|
     | chronopost_relais_fr | Chrono Point Relais|
     | chronopost_classic | Chrono Classic International|
@@ -551,22 +551,22 @@
     CHRONOPOST_13 = 'chronopost_13'
     CHRONOPOST_10 = 'chronopost_10'
     CHRONOPOST_18 = 'chronopost_18'
     CHRONOPOST_RELAIS_FR = 'chronopost_relais_fr'
     CHRONOPOST_CLASSIC = 'chronopost_classic'
     CHRONOPOST_EXPRESS = 'chronopost_express'
 
-class ServiceLevelCDL(str, Enum):
+class ServiceLevelCDLEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | cdl_next_day | Next Day|
     """
     CDL_NEXT_DAY = 'cdl_next_day'
 
-class ServiceLevelCanadaPost(str, Enum):
+class ServiceLevelCanadaPostEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | canada_post_regular_parcel | Regular Parcel|
     | canada_post_expedited_parcel | Expedited Parcel|
     | canada_post_priority | Priority|
     | canada_post_xpresspost | Xpresspost|
     | canada_post_xpresspost_international | Xpresspost International|
@@ -585,46 +585,46 @@
     CANADA_POST_XPRESSPOST_USA = 'canada_post_xpresspost_usa'
     CANADA_POST_EXPEDITED_PARCEL_USA = 'canada_post_expedited_parcel_usa'
     CANADA_POST_TRACKED_PACKET_USA = 'canada_post_tracked_packet_usa'
     CANADA_POST_SMALL_PACKET_USA_AIR = 'canada_post_small_packet_usa_air'
     CANADA_POST_TRACKED_PACKET_INTERNATIONAL = 'canada_post_tracked_packet_international'
     CANADA_POST_SMALL_PACKET_INTERNATIONAL_AIR = 'canada_post_small_packet_international_air'
 
-class ServiceLevelBetterTrucks(str, Enum):
+class ServiceLevelBetterTrucksEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | better_trucks_same_day | Same Day|
     | better_trucks_next_day | Next Day|
     """
     BETTER_TRUCKS_SAME_DAY = 'better_trucks_same_day'
     BETTER_TRUCKS_NEXT_DAY = 'better_trucks_next_day'
 
-class ServiceLevelAPG(str, Enum):
+class ServiceLevelAPGEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | epacket | ePacket|
     | epacket_plus | ePacket Plus|
     | eparcel_premium | eParcel premium|
     | apg_eparcel_expedited | eParcel Expedited|
     """
     EPACKET = 'epacket'
     EPACKET_PLUS = 'epacket_plus'
     EPARCEL_PREMIUM = 'eparcel_premium'
     APG_EPARCEL_EXPEDITED = 'apg_eparcel_expedited'
 
-class ServiceLevelAxleHire(str, Enum):
+class ServiceLevelAxleHireEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | axlehire_same_day | Same Day|
     | axlehire_next_day | Next Day|
     """
     AXLEHIRE_SAME_DAY = 'axlehire_same_day'
     AXLEHIRE_NEXT_DAY = 'axlehire_next_day'
 
-class ServiceLevelAustraliaPost(str, Enum):
+class ServiceLevelAustraliaPostEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | australia_post_express_post | Express Post|
     | australia_post_parcel_post | Parcel Post|
     | australia_post_pack_and_track_international | Pack and Track International|
     | australia_post_international_airmail | International Airmail|
     | australia_post_express_post_international | Express Post International|
@@ -641,15 +641,15 @@
     AUSTRALIA_POST_EXPRESS_POST_INTERNATIONAL = 'australia_post_express_post_international'
     AUSTRALIA_POST_EXPRESS_COURIER_INTERNATIONAL = 'australia_post_express_courier_international'
     AUSTRALIA_POST_INTERNATIONAL_EXPRESS = 'australia_post_international_express'
     AUSTRALIA_POST_INTERNATIONAL_STANDARD = 'australia_post_international_standard'
     AUSTRALIA_POST_INTERNATIONAL_ECONOMY = 'australia_post_international_economy'
     AUSTRALIA_POST_PARCEL_POST_RETURN = 'australia_post_parcel_post_return'
 
-class ServiceLevelAsendia(str, Enum):
+class ServiceLevelAsendiaEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | asendia_us_priority_tracked | Asendia USA Priority Tracked|
     | asendia_us_international_express | Asendia USA International Express|
     | asendia_us_international_priority_airmail | Asendia USA International Priority Airmail|
     | asendia_us_international_surface_airlift | Asendia USA International Surface Air Lift|
     | asendia_us_priority_mail_international | Asendia USA Priority Mail International|
@@ -662,15 +662,15 @@
     ASENDIA_US_INTERNATIONAL_PRIORITY_AIRMAIL = 'asendia_us_international_priority_airmail'
     ASENDIA_US_INTERNATIONAL_SURFACE_AIRLIFT = 'asendia_us_international_surface_airlift'
     ASENDIA_US_PRIORITY_MAIL_INTERNATIONAL = 'asendia_us_priority_mail_international'
     ASENDIA_US_PRIORITY_MAIL_EXPRESS_INTERNATIONAL = 'asendia_us_priority_mail_express_international'
     ASENDIA_US_EPACKET = 'asendia_us_epacket'
     ASENDIA_US_OTHER = 'asendia_us_other'
 
-class ServiceLevelAPCPostal(str, Enum):
+class ServiceLevelAPCPostalEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | apc_postal_parcelconnect_expedited | parcelConnect Expedited|
     | apc_postal_parcelconnect_priority | parcelConnect Priority|
     | apc_postal_parcelconnect_priority_delcon | parcelConnect Priority Delcon|
     | apc_postal_parcelconnect_priority_pqw | parcelConnect Priority PQW|
     | apc_postal_parcelconnect_book_service | parcelConnect Book Service|
@@ -685,24 +685,24 @@
     APC_POSTAL_PARCELCONNECT_PRIORITY_PQW = 'apc_postal_parcelconnect_priority_pqw'
     APC_POSTAL_PARCELCONNECT_BOOK_SERVICE = 'apc_postal_parcelconnect_book_service'
     APC_POSTAL_PARCELCONNECT_STANDARD = 'apc_postal_parcelconnect_standard'
     APC_POSTAL_PARCELCONNECT_EPMI = 'apc_postal_parcelconnect_epmi'
     APC_POSTAL_PARCELCONNECT_EPACKET = 'apc_postal_parcelconnect_epacket'
     APC_POSTAL_PARCELCONNECT_EPMEI = 'apc_postal_parcelconnect_epmei'
 
-class ServiceLevelAirterra(str, Enum):
+class ServiceLevelAirterraEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | airterra_ground | GroundXC|
     | airterra_postal | FastPost|
     """
     AIRTERRA_GROUND = 'airterra_ground'
     AIRTERRA_POSTAL = 'airterra_postal'
 
-class ServiceLevelUPS(str, Enum):
+class ServiceLevelUPSEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | ups_standard | Standard℠|
     | ups_ground | Ground|
     | ups_saver | Saver®|
     | ups_3_day_select | 3 Day Select®|
     | ups_second_day_air | 2nd Day Air®|
@@ -749,15 +749,15 @@
     UPS_EXPRESS = 'ups_express'
     UPS_EXPRESS_1200 = 'ups_express_1200'
     UPS_EXPRESS_PLUS = 'ups_express_plus'
     UPS_EXPEDITED = 'ups_expedited'
     UPS_EXPRESS_EARLY = 'ups_express_early'
     UPS_ACCESS_POINT_ECONOMY = 'ups_access_point_economy'
 
-class ServiceLevelFedEx(str, Enum):
+class ServiceLevelFedExEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | fedex_ground | FedEx Ground®|
     | fedex_home_delivery | FedEx Home Delivery®|
     | fedex_ground_economy | FedEx Ground® Economy|
     | fedex_2_day | FedEx 2Day®|
     | fedex_2_day_am | FedEx 2Day® A.M.|
@@ -795,15 +795,15 @@
     FEDEX_INTERNATIONAL_PRIORITY = 'fedex_international_priority'
     FEDEX_INTERNATIONAL_FIRST = 'fedex_international_first'
     FEDEX_EUROPE_FIRST_INTERNATIONAL_PRIORITY = 'fedex_europe_first_international_priority'
     FEDEX_INTERNATIONAL_CONNECT_PLUS = 'fedex_international_connect_plus'
     INTERNATIONAL_ECONOMY_FREIGHT = 'international_economy_freight'
     INTERNATIONAL_PRIORITY_FREIGHT = 'international_priority_freight'
 
-class ServiceLevelUSPS(str, Enum):
+class ServiceLevelUSPSEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | usps_priority | Priority Mail|
     | usps_priority_express | Priority Mail Express|
     | usps_media_mail | Media Mail, only for existing Shippo customers with grandfathered Media Mail option.|
     | usps_priority_mail_international | Priority Mail International|
     | usps_priority_mail_express_international | Priority Mail Express International|
```

### Comparing `shippo-3.2.4/src/shippo/models/components/shipment.py` & `shippo-3.2.5/src/shippo/models/components/shipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/shipmentcreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/shipmentcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/shipmentextra.py` & `shippo-3.2.5/src/shippo/models/components/shipmentextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/shipmentpaginatedlist.py` & `shippo-3.2.5/src/shippo/models/components/shipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/shippoaccount.py` & `shippo-3.2.5/src/shippo/models/components/tracksrequest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ShippoAccount:
-    email: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email') }})
-    first_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('first_name') }})
-    last_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('last_name') }})
-    company_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('company_name') }})
-    object_created: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
-    object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
-    object_updated: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_updated'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
+class TracksRequest:
+    carrier: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier') }})
+    r"""Name of the carrier of the shipment to track."""
+    tracking_number: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_number') }})
+    r"""Tracking number to track."""
+    metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+    r"""A string of up to 100 characters that can be filled with any additional information you want to attach to the object."""
```

### Comparing `shippo-3.2.4/src/shippo/models/components/shippoaccountpaginatedlist.py` & `shippo-3.2.5/src/shippo/models/components/shippoaccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/shippoaccountupdaterequest.py` & `shippo-3.2.5/src/shippo/models/components/shippoaccountupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/track.py` & `shippo-3.2.5/src/shippo/models/components/track.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/trackingstatus.py` & `shippo-3.2.5/src/shippo/models/components/trackingstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/trackingstatuslocationbase.py` & `shippo-3.2.5/src/shippo/models/components/trackingstatuslocationbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/trackingstatussubstatus.py` & `shippo-3.2.5/src/shippo/models/components/trackingstatussubstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/tracksrequest.py` & `shippo-3.2.5/src/shippo/models/errors/badrequestwitherror.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class TracksRequest:
-    carrier: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier') }})
-    r"""Name of the carrier of the shipment to track."""
-    tracking_number: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_number') }})
-    r"""Tracking number to track."""
-    metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    r"""A string of up to 100 characters that can be filled with any additional information you want to attach to the object."""
+class BadRequestWithError(Exception):
+    error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
     
 
+    def __str__(self) -> str:
+        return utils.marshal_json(self, type(self))
```

### Comparing `shippo-3.2.4/src/shippo/models/components/transaction.py` & `shippo-3.2.5/src/shippo/models/components/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .labelfiletype import LabelFileType
-from .objectstate import ObjectState
+from .labelfiletypeenum import LabelFileTypeEnum
+from .objectstateenum import ObjectStateEnum
 from .trackingstatusenum import TrackingStatusEnum
 from .transactionstatusenum import TransactionStatusEnum
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from shippo import utils
 from typing import List, Optional
 
@@ -23,15 +23,15 @@
 class Transaction:
     commercial_invoice_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('commercial_invoice_url'), 'exclude': lambda f: f is None }})
     r"""A URL pointing to the commercial invoice as a 8.5x11 inch PDF file.
     A value will only be returned if the Transactions has been processed successfully and if the shipment is international.
     """
     eta: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eta'), 'exclude': lambda f: f is None }})
     r"""The estimated time of arrival according to the carrier."""
-    label_file_type: Optional[LabelFileType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_file_type'), 'exclude': lambda f: f is None }})
+    label_file_type: Optional[LabelFileTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_file_type'), 'exclude': lambda f: f is None }})
     r"""Print format of the <a href=\\"https://docs.goshippo.com/docs/shipments/shippinglabelsizes/\\">label</a>. If empty, will use the default format set from
     <a href=\"https://apps.goshippo.com/settings/labels\">the Shippo dashboard.</a>
     """
     label_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_url'), 'exclude': lambda f: f is None }})
     r"""A URL pointing directly to the label in the format you've set in your settings.
     A value will only be returned if the Transactions has been processed successfully.
     """
@@ -46,15 +46,15 @@
     """
     object_created: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""Date and time of Transaction creation."""
     object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the given Transaction object."""
     object_owner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_owner'), 'exclude': lambda f: f is None }})
     r"""Username of the user who created the Transaction object."""
-    object_state: Optional[ObjectState] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_state'), 'exclude': lambda f: f is None }})
+    object_state: Optional[ObjectStateEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_state'), 'exclude': lambda f: f is None }})
     r"""Indicates the validity of the enclosing object"""
     object_updated: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_updated'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""Date and time of last Transaction update."""
     qr_code_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('qr_code_url'), 'exclude': lambda f: f is None }})
     r"""A URL pointing directly to the QR code in PNG format.
     A value will only be returned if requested using qr_code_requested flag and the carrier provides such an option.
     """
```

### Comparing `shippo-3.2.4/src/shippo/models/components/transactioncreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/transactioncreaterequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .labelfiletype import LabelFileType
+from .labelfiletypeenum import LabelFileTypeEnum
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TransactionCreateRequest:
     rate: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rate') }})
     async_: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('async'), 'exclude': lambda f: f is None }})
-    label_file_type: Optional[LabelFileType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_file_type'), 'exclude': lambda f: f is None }})
+    label_file_type: Optional[LabelFileTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_file_type'), 'exclude': lambda f: f is None }})
     r"""Print format of the <a href=\\"https://docs.goshippo.com/docs/shipments/shippinglabelsizes/\\">label</a>. If empty, will use the default format set from
     <a href=\"https://apps.goshippo.com/settings/labels\">the Shippo dashboard.</a>
     """
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.2.4/src/shippo/models/components/transactionpaginatedlist.py` & `shippo-3.2.5/src/shippo/models/components/transactionpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/upsconnectexistingownaccountparameters.py` & `shippo-3.2.5/src/shippo/models/components/upsconnectexistingownaccountparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/components/userparceltemplate.py` & `shippo-3.2.5/src/shippo/models/components/userparceltemplate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from .carrierparceltemplate import CarrierParcelTemplate
-from .distanceunit import DistanceUnit
-from .weightunit import WeightUnit
+from .distanceunitenum import DistanceUnitEnum
+from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class UserParcelTemplate:
-    distance_unit: Optional[DistanceUnit] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit'), 'exclude': lambda f: f is None }})
+    distance_unit: Optional[DistanceUnitEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit'), 'exclude': lambda f: f is None }})
     r"""The measure unit used for length, width and height."""
     height: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is None }})
     r"""The height of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     length: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('length'), 'exclude': lambda f: f is None }})
     r"""The length of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     r"""The name of the User Parcel Template"""
     weight: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight'), 'exclude': lambda f: f is None }})
     r"""The weight of the package, in units specified by the weight_unit attribute."""
-    weight_unit: Optional[WeightUnit] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
+    weight_unit: Optional[WeightUnitEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
     r"""The unit used for weight."""
     width: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is None }})
     r"""The width of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     object_created: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""Date and time of User Parcel Template creation"""
     object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the given User Parcel Template object"""
```

### Comparing `shippo-3.2.4/src/shippo/models/components/userparceltemplateupdaterequest.py` & `shippo-3.2.5/src/shippo/models/components/userparceltemplateupdaterequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .distanceunit import DistanceUnit
-from .weightunit import WeightUnit
+from .distanceunitenum import DistanceUnitEnum
+from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class UserParcelTemplateUpdateRequest:
-    distance_unit: DistanceUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
+    distance_unit: DistanceUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
     r"""The measure unit used for length, width and height."""
     height: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height') }})
     r"""The height of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     length: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('length') }})
     r"""The length of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     r"""The name of the User Parcel Template"""
     width: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width') }})
     r"""The width of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     weight: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight'), 'exclude': lambda f: f is None }})
     r"""The weight of the package, in units specified by the weight_unit attribute."""
-    weight_unit: Optional[WeightUnit] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
+    weight_unit: Optional[WeightUnitEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
     r"""The unit used for weight."""
```

### Comparing `shippo-3.2.4/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .weightunit import WeightUnit
+from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class UserParcelTemplateWithCarrierTemplateCreateRequest:
     template: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('template'), 'exclude': lambda f: f is None }})
     r"""The object representing the carrier parcel template"""
     weight: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight'), 'exclude': lambda f: f is None }})
     r"""The weight of the package, in units specified by the weight_unit attribute."""
-    weight_unit: Optional[WeightUnit] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
+    weight_unit: Optional[WeightUnitEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
     r"""The unit used for weight."""
```

### Comparing `shippo-3.2.4/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py` & `shippo-3.2.5/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .distanceunit import DistanceUnit
-from .weightunit import WeightUnit
+from .distanceunitenum import DistanceUnitEnum
+from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class UserParcelTemplateWithoutCarrierTemplateCreateRequest:
-    distance_unit: DistanceUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
+    distance_unit: DistanceUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
     r"""The measure unit used for length, width and height."""
     height: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height') }})
     r"""The height of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     length: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('length') }})
     r"""The length of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     r"""The name of the User Parcel Template"""
     width: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width') }})
     r"""The width of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     weight: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight'), 'exclude': lambda f: f is None }})
     r"""The weight of the package, in units specified by the weight_unit attribute."""
-    weight_unit: Optional[WeightUnit] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
+    weight_unit: Optional[WeightUnitEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
     r"""The unit used for weight."""
```

### Comparing `shippo-3.2.4/src/shippo/models/errors/badrequestwithdetail.py` & `shippo-3.2.5/src/shippo/models/errors/badrequestwithdetail.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/errors/initiateoauth2signin.py` & `shippo-3.2.5/src/shippo/models/errors/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/errors/sdkerror.py` & `shippo-3.2.5/src/shippo/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/__init__.py` & `shippo-3.2.5/src/shippo/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/addshipmentstobatch.py` & `shippo-3.2.5/src/shippo/models/operations/addshipmentstobatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createaddress.py` & `shippo-3.2.5/src/shippo/models/operations/createaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createbatch.py` & `shippo-3.2.5/src/shippo/models/operations/createbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createcarrieraccount.py` & `shippo-3.2.5/src/shippo/models/operations/createcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createcustomsdeclaration.py` & `shippo-3.2.5/src/shippo/models/operations/createcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createcustomsitem.py` & `shippo-3.2.5/src/shippo/models/operations/createcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createliverate.py` & `shippo-3.2.5/src/shippo/models/operations/createliverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createmanifest.py` & `shippo-3.2.5/src/shippo/models/operations/createmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createorder.py` & `shippo-3.2.5/src/shippo/models/operations/createorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createparcel.py` & `shippo-3.2.5/src/shippo/models/operations/createparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createpickup.py` & `shippo-3.2.5/src/shippo/models/operations/createpickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createrefund.py` & `shippo-3.2.5/src/shippo/models/operations/createrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createservicegroup.py` & `shippo-3.2.5/src/shippo/models/operations/createservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createshipment.py` & `shippo-3.2.5/src/shippo/models/operations/createshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createshippoaccount.py` & `shippo-3.2.5/src/shippo/models/operations/createshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createtrack.py` & `shippo-3.2.5/src/shippo/models/operations/createtrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createtransaction.py` & `shippo-3.2.5/src/shippo/models/operations/createtransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/createuserparceltemplate.py` & `shippo-3.2.5/src/shippo/models/operations/createuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/deletedefaultparceltemplate.py` & `shippo-3.2.5/src/shippo/models/operations/deletedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/deleteservicegroup.py` & `shippo-3.2.5/src/shippo/models/operations/deleteservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/deleteuserparceltemplate.py` & `shippo-3.2.5/src/shippo/models/operations/deleteuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/getaddress.py` & `shippo-3.2.5/src/shippo/models/operations/getaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/getbatch.py` & `shippo-3.2.5/src/shippo/models/operations/getbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/getcarrieraccount.py` & `shippo-3.2.5/src/shippo/models/operations/getcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/getcarrierparceltemplate.py` & `shippo-3.2.5/src/shippo/models/operations/getcarrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/getcarrierregistrationstatus.py` & `shippo-3.2.5/src/shippo/models/operations/getcarrierregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/getcustomsdeclaration.py` & `shippo-3.2.5/src/shippo/models/operations/getcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/getcustomsitem.py` & `shippo-3.2.5/src/shippo/models/operations/getcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/getdefaultparceltemplate.py` & `shippo-3.2.5/src/shippo/models/operations/getdefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/getmanifest.py` & `shippo-3.2.5/src/shippo/models/operations/getmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/getorder.py` & `shippo-3.2.5/src/shippo/models/operations/getorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/getparcel.py` & `shippo-3.2.5/src/shippo/models/operations/getparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/getrate.py` & `shippo-3.2.5/src/shippo/models/operations/getrate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/getrefund.py` & `shippo-3.2.5/src/shippo/models/operations/getrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/getshipment.py` & `shippo-3.2.5/src/shippo/models/operations/getshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/getshippoaccount.py` & `shippo-3.2.5/src/shippo/models/operations/getshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/gettrack.py` & `shippo-3.2.5/src/shippo/models/operations/gettrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/gettransaction.py` & `shippo-3.2.5/src/shippo/models/operations/gettransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/getuserparceltemplate.py` & `shippo-3.2.5/src/shippo/models/operations/getuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/initiateoauth2signin.py` & `shippo-3.2.5/src/shippo/models/operations/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/listaddresses.py` & `shippo-3.2.5/src/shippo/models/operations/listaddresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/listcarrieraccounts.py` & `shippo-3.2.5/src/shippo/models/operations/listcarrieraccounts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import carriers as components_carriers
+from ...models.components import carriersenum as components_carriersenum
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListCarrierAccountsGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
@@ -14,15 +14,15 @@
 
 
 
 @dataclasses.dataclass
 class ListCarrierAccountsRequest:
     service_levels: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'service_levels', 'style': 'form', 'explode': True }})
     r"""Appends the property `service_levels` to each returned carrier account"""
-    carrier: Optional[components_carriers.Carriers] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'carrier', 'style': 'form', 'explode': True }})
+    carrier: Optional[components_carriersenum.CarriersEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'carrier', 'style': 'form', 'explode': True }})
     r"""Filter the response by the specified carrier"""
     account_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'account_id', 'style': 'form', 'explode': True }})
     r"""Filter the response by the specified carrier account Id"""
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     results: Optional[int] = dataclasses.field(default=5, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
     r"""The number of results to return per page (max 100, default 5)"""
```

### Comparing `shippo-3.2.4/src/shippo/models/operations/listcarrierparceltemplates.py` & `shippo-3.2.5/src/shippo/models/operations/listcarrierparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/listcustomsdeclarations.py` & `shippo-3.2.5/src/shippo/models/operations/listcustomsdeclarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/listcustomsitems.py` & `shippo-3.2.5/src/shippo/models/operations/listcustomsitems.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/listmanifests.py` & `shippo-3.2.5/src/shippo/models/operations/listmanifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/listorders.py` & `shippo-3.2.5/src/shippo/models/operations/listorders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/listparcels.py` & `shippo-3.2.5/src/shippo/models/operations/listparcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/listrefunds.py` & `shippo-3.2.5/src/shippo/models/operations/listrefunds.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/listservicegroups.py` & `shippo-3.2.5/src/shippo/models/operations/listservicegroups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/listshipmentrates.py` & `shippo-3.2.5/src/shippo/models/operations/listshipmentrates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/listshipmentratesbycurrencycode.py` & `shippo-3.2.5/src/shippo/models/operations/listshipmentratesbycurrencycode.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/listshipments.py` & `shippo-3.2.5/src/shippo/models/operations/listshipments.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/listshippoaccounts.py` & `shippo-3.2.5/src/shippo/models/operations/listshippoaccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/listtransactions.py` & `shippo-3.2.5/src/shippo/models/operations/listtransactions.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/listuserparceltemplates.py` & `shippo-3.2.5/src/shippo/models/operations/listuserparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/purchasebatch.py` & `shippo-3.2.5/src/shippo/models/operations/purchasebatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/registercarrieraccount.py` & `shippo-3.2.5/src/shippo/models/operations/registercarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/removeshipmentsfrombatch.py` & `shippo-3.2.5/src/shippo/models/operations/removeshipmentsfrombatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/updatecarrieraccount.py` & `shippo-3.2.5/src/shippo/models/operations/updatecarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/updatedefaultparceltemplate.py` & `shippo-3.2.5/src/shippo/models/operations/updatedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/updateservicegroup.py` & `shippo-3.2.5/src/shippo/models/operations/updateservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/updateshippoaccount.py` & `shippo-3.2.5/src/shippo/models/operations/updateshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/updateuserparceltemplate.py` & `shippo-3.2.5/src/shippo/models/operations/updateuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/models/operations/validateaddress.py` & `shippo-3.2.5/src/shippo/models/operations/validateaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/orders.py` & `shippo-3.2.5/src/shippo/orders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/parcels.py` & `shippo-3.2.5/src/shippo/parcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/pickups.py` & `shippo-3.2.5/src/shippo/pickups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/rates.py` & `shippo-3.2.5/src/shippo/rates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/rates_at_checkout.py` & `shippo-3.2.5/src/shippo/rates_at_checkout.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/refunds.py` & `shippo-3.2.5/src/shippo/refunds.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/sdk.py` & `shippo-3.2.5/src/shippo/sdk.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/sdkconfiguration.py` & `shippo-3.2.5/src/shippo/sdkconfiguration.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '2018-02-08'
-    sdk_version: str = '3.2.4'
-    gen_version: str = '2.306.0'
-    user_agent: str = 'speakeasy-sdk/python 3.2.4 2.306.0 2018-02-08 shippo'
+    sdk_version: str = '3.2.5'
+    gen_version: str = '2.306.3'
+    user_agent: str = 'speakeasy-sdk/python 3.2.5 2.306.3 2018-02-08 shippo'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `shippo-3.2.4/src/shippo/service_groups.py` & `shippo-3.2.5/src/shippo/service_groups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/shipments.py` & `shippo-3.2.5/src/shippo/shipments.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/shippo_accounts.py` & `shippo-3.2.5/src/shippo/shippo_accounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/tracking_status.py` & `shippo-3.2.5/src/shippo/tracking_status.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/transactions.py` & `shippo-3.2.5/src/shippo/transactions.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/user_parcel_templates.py` & `shippo-3.2.5/src/shippo/user_parcel_templates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/utils/retries.py` & `shippo-3.2.5/src/shippo/utils/retries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo/utils/utils.py` & `shippo-3.2.5/src/shippo/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.4/src/shippo.egg-info/PKG-INFO` & `shippo-3.2.5/src/shippo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.2.4
+Version: 3.2.5
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
```

### Comparing `shippo-3.2.4/src/shippo.egg-info/SOURCES.txt` & `shippo-3.2.5/src/shippo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -68,54 +68,60 @@
 src/shippo/models/components/carrieraccountregistrationstatus.py
 src/shippo/models/components/carrieraccountservicelevel.py
 src/shippo/models/components/carrieraccountupscreaterequest.py
 src/shippo/models/components/carrieraccountupscreaterequestparameters.py
 src/shippo/models/components/carrieraccountuspscreaterequest.py
 src/shippo/models/components/carrieraccountwithextrainfo.py
 src/shippo/models/components/carrierparceltemplate.py
-src/shippo/models/components/carriers.py
+src/shippo/models/components/carriersenum.py
 src/shippo/models/components/cod.py
 src/shippo/models/components/connectexistingownaccountrequest.py
 src/shippo/models/components/customerreference.py
 src/shippo/models/components/customsdeclaration.py
+src/shippo/models/components/customsdeclarationb13afilingoptionenum.py
+src/shippo/models/components/customsdeclarationcontentstypeenum.py
 src/shippo/models/components/customsdeclarationcreaterequest.py
+src/shippo/models/components/customsdeclarationeelpfcenum.py
+src/shippo/models/components/customsdeclarationincotermenum.py
+src/shippo/models/components/customsdeclarationnondeliveryoptionenum.py
 src/shippo/models/components/customsdeclarationpaginatedlist.py
 src/shippo/models/components/customsexporteridentification.py
 src/shippo/models/components/customsinvoicedcharges.py
 src/shippo/models/components/customsitem.py
 src/shippo/models/components/customsitembase.py
 src/shippo/models/components/customsitempaginatedlist.py
 src/shippo/models/components/customstaxidentification.py
 src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
 src/shippo/models/components/dangerousgoodslithiumbatteries.py
 src/shippo/models/components/dangerousgoodsobject.py
 src/shippo/models/components/defaultparceltemplate.py
 src/shippo/models/components/defaultparceltemplateupdaterequest.py
 src/shippo/models/components/departmentnumber.py
-src/shippo/models/components/distanceunit.py
+src/shippo/models/components/distanceunitenum.py
 src/shippo/models/components/dryice.py
 src/shippo/models/components/errormessage.py
 src/shippo/models/components/httpmetadata.py
 src/shippo/models/components/instanttransactionrequestbody.py
 src/shippo/models/components/insurance.py
 src/shippo/models/components/invoicenumber.py
-src/shippo/models/components/labelfiletype.py
+src/shippo/models/components/labelfiletypeenum.py
 src/shippo/models/components/lineitem.py
 src/shippo/models/components/lineitembase.py
 src/shippo/models/components/liverate.py
 src/shippo/models/components/liveratecreaterequest.py
 src/shippo/models/components/liveratepaginatedlist.py
 src/shippo/models/components/location.py
 src/shippo/models/components/manifest.py
 src/shippo/models/components/manifestcreaterequest.py
 src/shippo/models/components/manifestpaginatedlist.py
-src/shippo/models/components/objectstate.py
+src/shippo/models/components/objectstateenum.py
 src/shippo/models/components/order.py
 src/shippo/models/components/ordercreaterequest.py
 src/shippo/models/components/orderpaginatedlist.py
+src/shippo/models/components/orderstatusenum.py
 src/shippo/models/components/parcel.py
 src/shippo/models/components/parcelcreaterequest.py
 src/shippo/models/components/parcelextra.py
 src/shippo/models/components/parcelinsurance.py
 src/shippo/models/components/parcelpaginatedlist.py
 src/shippo/models/components/parcelrequest.py
 src/shippo/models/components/parceltemplateenumset.py
@@ -129,15 +135,15 @@
 src/shippo/models/components/refundpaginatedlist.py
 src/shippo/models/components/refundrequestbody.py
 src/shippo/models/components/rmanumber.py
 src/shippo/models/components/security.py
 src/shippo/models/components/servicegroup.py
 src/shippo/models/components/servicegroupaccountandservicelevel.py
 src/shippo/models/components/servicegroupcreaterequest.py
-src/shippo/models/components/servicegrouptype.py
+src/shippo/models/components/servicegrouptypeenum.py
 src/shippo/models/components/servicegroupupdaterequest.py
 src/shippo/models/components/servicelevel.py
 src/shippo/models/components/servicelevelenumset.py
 src/shippo/models/components/shipment.py
 src/shippo/models/components/shipmentcreaterequest.py
 src/shippo/models/components/shipmentextra.py
 src/shippo/models/components/shipmentpaginatedlist.py
@@ -155,15 +161,15 @@
 src/shippo/models/components/transactionpaginatedlist.py
 src/shippo/models/components/transactionstatusenum.py
 src/shippo/models/components/upsconnectexistingownaccountparameters.py
 src/shippo/models/components/userparceltemplate.py
 src/shippo/models/components/userparceltemplateupdaterequest.py
 src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
 src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
-src/shippo/models/components/weightunit.py
+src/shippo/models/components/weightunitenum.py
 src/shippo/models/errors/__init__.py
 src/shippo/models/errors/badrequestwithdetail.py
 src/shippo/models/errors/badrequestwitherror.py
 src/shippo/models/errors/initiateoauth2signin.py
 src/shippo/models/errors/sdkerror.py
 src/shippo/models/internal/__init__.py
 src/shippo/models/internal/globals.py
```

