# Comparing `tmp/trytond_edocument_uncefact-6.6.0.tar.gz` & `tmp/trytond_edocument_uncefact-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_edocument_uncefact-6.6.0.tar", last modified: Mon Oct 31 16:04:20 2022, max compression
+gzip compressed data, was "trytond_edocument_uncefact-6.8.0.tar", last modified: Mon May  1 11:35:28 2023, max compression
```

## Comparing `trytond_edocument_uncefact-6.6.0.tar` & `trytond_edocument_uncefact-6.8.0.tar`

### file list

```diff
@@ -1,119 +1,116 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:20.374274 trytond_edocument_uncefact-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_edocument_uncefact-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_edocument_uncefact-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2022-10-31 16:04:19.000000 trytond_edocument_uncefact-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_edocument_uncefact-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      750 2022-10-31 16:04:18.000000 trytond_edocument_uncefact-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:04:17.000000 trytond_edocument_uncefact-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_edocument_uncefact-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2403 2022-10-31 16:04:20.370940 trytond_edocument_uncefact-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2021-12-11 16:59:33.000000 trytond_edocument_uncefact-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:20.367607 trytond_edocument_uncefact-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6912 2021-12-11 16:59:33.000000 trytond_edocument_uncefact-6.6.0/edocument.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:20.350940 trytond_edocument_uncefact-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      183 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      183 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      183 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      187 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      187 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      187 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-10-29 07:50:32.000000 trytond_edocument_uncefact-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:04:20.374274 trytond_edocument_uncefact-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5330 2022-10-29 07:39:10.000000 trytond_edocument_uncefact-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:20.337607 trytond_edocument_uncefact-6.6.0/template/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:20.350940 trytond_edocument_uncefact-6.6.0/template/16B-CII/
--rw-r--r--   0 ced       (1000) ced       (1000)     9277 2021-04-03 16:26:38.000000 trytond_edocument_uncefact-6.6.0/template/16B-CII/CrossIndustryInvoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:20.350940 trytond_edocument_uncefact-6.6.0/tests/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:20.337607 trytond_edocument_uncefact-6.6.0/tests/16B-CII/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:20.337607 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:20.367607 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/
--rw-r--r--   0 ced       (1000) ced       (1000)     2224 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/EDIFICAS-EU_AccountingAccountType_D11A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2068 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/EDIFICAS-EU_AccountingAmountType_D11A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     7920 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/ISO_ISO3AlphaCurrencyCode_2012-08-31.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     5740 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_ActionCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     5468 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_AdjustmentReasonDescriptionCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     5337 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_AllowanceChargeIdentificationCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     5354 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_AllowanceChargeReasonCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2242 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_AutomaticDataCaptureMethodCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2660 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_CargoOperationalCategoryCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2155 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_CargoTypeCode_1996Rev2Final.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     1907 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_CommodityIdentificationCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_CommunicationMeansTypeCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     5198 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_ContactFunctionCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2281 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_DeliveryTermsCode_2010.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2593 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_DimensionTypeCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2698 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_DocumentNameCode_Accounting_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    26450 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_DocumentNameCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     3124 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_DocumentStatusCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     3682 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_DutyTaxFeeTypeCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2547 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_DutyorTaxorFeeCategoryCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     3203 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_EquipmentSizeTypeDescriptionCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2090 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_EventTimeReferenceCodePaymentTermsEvent_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     3995 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_EventTimeReferenceCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     1932 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_FreightChargeQuantityUnitBasisCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2245 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_FreightChargeTariffCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     1869 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_GoodsTypeCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     1896 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_GoodsTypeExtensionCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2093 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeLinear_4.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2093 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeVolume_4.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2025 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeWeight_4.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     4140 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_MessageFunctionCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    14278 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PackageTypeCode_2006.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     3579 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PackagingMarkingCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2576 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PartyRoleCode_ChargePaying_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    21946 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PartyRoleCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2263 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PaymentGuaranteeMeansCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2381 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PaymentMeansChannelCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     4538 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PaymentMeansCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     4451 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PaymentTermsTypeCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2788 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PriceTypeCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    29382 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_ReferenceTypeCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2054 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_TimePointFormatCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     4329 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_TransportEquipmentCategoryCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2302 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_TransportEquipmentFullnessCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    11400 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_TransportMeansTypeCode_2007.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2169 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_TransportModeCode_2.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2854 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_TransportMovementStageCode_D16A.xsd
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:20.337607 trytond_edocument_uncefact-6.6.0/tests/16B-CII/data/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:20.367607 trytond_edocument_uncefact-6.6.0/tests/16B-CII/data/standard/
--rw-r--r--   0 ced       (1000) ced       (1000)     3048 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/data/standard/CrossIndustryInvoice_100pD16B.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    47531 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/data/standard/CrossIndustryInvoice_QualifiedDataType_100pD16B.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    98059 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/data/standard/CrossIndustryInvoice_ReusableAggregateBusinessInformationEntity_100pD16B.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     6805 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/data/standard/CrossIndustryInvoice_UnqualifiedDataType_100pD16B.xsd
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:20.337607 trytond_edocument_uncefact-6.6.0/tests/16B-CII/identifierlist/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:20.367607 trytond_edocument_uncefact-6.6.0/tests/16B-CII/identifierlist/standard/
--rw-r--r--   0 ced       (1000) ced       (1000)    10120 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/identifierlist/standard/ISO_ISOTwo-letterCountryCode_SecondEdition2006.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    62572 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/identifierlist/standard/UNECE_FreightCostCode_4.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2127 2019-06-04 16:49:46.000000 trytond_edocument_uncefact-6.6.0/tests/16B-CII/identifierlist/standard/UNECE_PaymentTermsDescriptionIdentifier_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_edocument_uncefact-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-04-16 16:30:56.000000 trytond_edocument_uncefact-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      714 2022-10-31 15:10:09.000000 trytond_edocument_uncefact-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       99 2022-10-31 16:04:17.000000 trytond_edocument_uncefact-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:20.370940 trytond_edocument_uncefact-6.6.0/trytond_edocument_uncefact.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2403 2022-10-31 16:04:19.000000 trytond_edocument_uncefact-6.6.0/trytond_edocument_uncefact.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     9334 2022-10-31 16:04:20.000000 trytond_edocument_uncefact-6.6.0/trytond_edocument_uncefact.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:04:19.000000 trytond_edocument_uncefact-6.6.0/trytond_edocument_uncefact.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2022-10-31 16:04:19.000000 trytond_edocument_uncefact-6.6.0/trytond_edocument_uncefact.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:48.000000 trytond_edocument_uncefact-6.6.0/trytond_edocument_uncefact.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      106 2022-10-31 16:04:19.000000 trytond_edocument_uncefact-6.6.0/trytond_edocument_uncefact.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:04:19.000000 trytond_edocument_uncefact-6.6.0/trytond_edocument_uncefact.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:28.031178 trytond_edocument_uncefact-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      913 2023-05-01 10:57:05.000000 trytond_edocument_uncefact-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 10:57:05.000000 trytond_edocument_uncefact-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_edocument_uncefact-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2392 2023-05-01 11:35:28.027845 trytond_edocument_uncefact-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-04-15 07:12:15.000000 trytond_edocument_uncefact-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:28.024511 trytond_edocument_uncefact-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_edocument_uncefact-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6912 2023-04-15 07:12:15.000000 trytond_edocument_uncefact-6.8.0/edocument.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:28.001178 trytond_edocument_uncefact-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      183 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      183 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      183 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      187 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      187 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      187 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-04-29 08:02:38.000000 trytond_edocument_uncefact-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:35:28.031178 trytond_edocument_uncefact-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4516 2023-04-15 07:12:15.000000 trytond_edocument_uncefact-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:27.987844 trytond_edocument_uncefact-6.8.0/template/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:28.001178 trytond_edocument_uncefact-6.8.0/template/16B-CII/
+-rw-r--r--   0 ced       (1000) ced       (1000)     9277 2023-04-15 07:12:15.000000 trytond_edocument_uncefact-6.8.0/template/16B-CII/CrossIndustryInvoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:28.001178 trytond_edocument_uncefact-6.8.0/tests/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:27.987844 trytond_edocument_uncefact-6.8.0/tests/16B-CII/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:27.987844 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:28.021178 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2224 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/EDIFICAS-EU_AccountingAccountType_D11A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2068 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/EDIFICAS-EU_AccountingAmountType_D11A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     7920 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/ISO_ISO3AlphaCurrencyCode_2012-08-31.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     5740 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_ActionCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     5468 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_AdjustmentReasonDescriptionCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     5337 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_AllowanceChargeIdentificationCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     5354 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_AllowanceChargeReasonCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2242 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_AutomaticDataCaptureMethodCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2660 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_CargoOperationalCategoryCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2155 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_CargoTypeCode_1996Rev2Final.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     1907 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_CommodityIdentificationCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_CommunicationMeansTypeCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     5198 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_ContactFunctionCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2281 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_DeliveryTermsCode_2010.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2593 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_DimensionTypeCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2698 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_DocumentNameCode_Accounting_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    26450 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_DocumentNameCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     3124 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_DocumentStatusCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     3682 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_DutyTaxFeeTypeCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2547 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_DutyorTaxorFeeCategoryCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     3203 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_EquipmentSizeTypeDescriptionCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2090 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_EventTimeReferenceCodePaymentTermsEvent_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     3995 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_EventTimeReferenceCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     1932 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_FreightChargeQuantityUnitBasisCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2245 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_FreightChargeTariffCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     1869 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_GoodsTypeCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     1896 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_GoodsTypeExtensionCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2093 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeLinear_4.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2093 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeVolume_4.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2025 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeWeight_4.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     4140 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_MessageFunctionCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    14278 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PackageTypeCode_2006.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     3579 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PackagingMarkingCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2576 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PartyRoleCode_ChargePaying_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    21946 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PartyRoleCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2263 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PaymentGuaranteeMeansCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2381 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PaymentMeansChannelCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     4538 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PaymentMeansCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     4451 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PaymentTermsTypeCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2788 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PriceTypeCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    29382 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_ReferenceTypeCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2054 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_TimePointFormatCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     4329 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_TransportEquipmentCategoryCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2302 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_TransportEquipmentFullnessCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    11400 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_TransportMeansTypeCode_2007.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2169 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_TransportModeCode_2.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2854 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_TransportMovementStageCode_D16A.xsd
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:27.987844 trytond_edocument_uncefact-6.8.0/tests/16B-CII/data/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:28.024511 trytond_edocument_uncefact-6.8.0/tests/16B-CII/data/standard/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3048 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/data/standard/CrossIndustryInvoice_100pD16B.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    47531 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/data/standard/CrossIndustryInvoice_QualifiedDataType_100pD16B.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    98059 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/data/standard/CrossIndustryInvoice_ReusableAggregateBusinessInformationEntity_100pD16B.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     6805 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/data/standard/CrossIndustryInvoice_UnqualifiedDataType_100pD16B.xsd
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:27.987844 trytond_edocument_uncefact-6.8.0/tests/16B-CII/identifierlist/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:28.024511 trytond_edocument_uncefact-6.8.0/tests/16B-CII/identifierlist/standard/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10120 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/identifierlist/standard/ISO_ISOTwo-letterCountryCode_SecondEdition2006.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    62572 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/identifierlist/standard/UNECE_FreightCostCode_4.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2127 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-6.8.0/tests/16B-CII/identifierlist/standard/UNECE_PaymentTermsDescriptionIdentifier_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_edocument_uncefact-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-15 07:12:15.000000 trytond_edocument_uncefact-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_edocument_uncefact-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       99 2023-05-01 10:57:00.000000 trytond_edocument_uncefact-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:28.027845 trytond_edocument_uncefact-6.8.0/trytond_edocument_uncefact.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2392 2023-05-01 11:35:27.000000 trytond_edocument_uncefact-6.8.0/trytond_edocument_uncefact.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     9308 2023-05-01 11:35:27.000000 trytond_edocument_uncefact-6.8.0/trytond_edocument_uncefact.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:35:27.000000 trytond_edocument_uncefact-6.8.0/trytond_edocument_uncefact.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-05-01 11:35:27.000000 trytond_edocument_uncefact-6.8.0/trytond_edocument_uncefact.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_edocument_uncefact-6.8.0/trytond_edocument_uncefact.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      106 2023-05-01 11:35:27.000000 trytond_edocument_uncefact-6.8.0/trytond_edocument_uncefact.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:35:27.000000 trytond_edocument_uncefact-6.8.0/trytond_edocument_uncefact.egg-info/top_level.txt
```

### Comparing `trytond_edocument_uncefact-6.6.0/CHANGELOG` & `trytond_edocument_uncefact-6.8.0/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+
+Version 6.8.0 - 2023-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
+
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.10
```

### Comparing `trytond_edocument_uncefact-6.6.0/COPYRIGHT` & `trytond_edocument_uncefact-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2018-2022 Cédric Krier
-Copyright (C) 2018-2022 B2CK
+Copyright (C) 2018-2023 Cédric Krier
+Copyright (C) 2018-2023 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_edocument_uncefact-6.6.0/LICENSE` & `trytond_edocument_uncefact-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/PKG-INFO` & `trytond_edocument_uncefact-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_edocument_uncefact
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for electronic document UN/CEFACT
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/edocument_uncefact
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton electronic document UN/CEFACT UNECE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: Slovenian
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: Turkish
 Classifier: Natural Language :: Ukrainian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
 EDocument UN/CEFACT Module
 ##########################
 
 Implement electronic document from UN/CEFACT:
```

### Comparing `trytond_edocument_uncefact-6.6.0/edocument.py` & `trytond_edocument_uncefact-6.8.0/edocument.py`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/setup.py` & `trytond_edocument_uncefact-6.8.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 def read(fname):
     return io.open(
         os.path.join(os.path.dirname(__file__), fname),
         'r', encoding='utf-8').read()
 
 
 def get_require_version(name):
-    if minor_version % 2:
-        require = '%s >= %s.%s.dev0, < %s.%s'
-    else:
-        require = '%s >= %s.%s, < %s.%s'
+    require = '%s >= %s.%s, < %s.%s'
     require %= (name, major_version, minor_version,
         major_version, minor_version + 1)
     return require
 
 
 config = ConfigParser()
 config.read_file(open(os.path.join(os.path.dirname(__file__), 'tryton.cfg')))
@@ -34,63 +31,44 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_edocument_uncefact'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
 if minor_version % 2:
-    version = '%s.%s.dev0' % (major_version, minor_version)
-    download_url = (
-        'hg+http://hg.tryton.org/modules/%s#egg=%s-%s' % (
-            name[8:], name, version))
-local_version = []
-if os.environ.get('CI_JOB_ID'):
-    local_version.append(os.environ['CI_JOB_ID'])
+    download_url = ''
 else:
-    for build in ['CI_BUILD_NUMBER', 'CI_JOB_NUMBER']:
-        if os.environ.get(build):
-            local_version.append(os.environ[build])
-        else:
-            local_version = []
-            break
-if local_version:
-    version += '+' + '.'.join(local_version)
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['Genshi']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [
     'lxml',
     get_require_version('trytond_account_invoice'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module for electronic document UN/CEFACT',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/edocument_uncefact',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton electronic document UN/CEFACT UNECE',
     package_dir={'trytond.modules.edocument_uncefact': '.'},
     packages=(
         ['trytond.modules.edocument_uncefact']
         + ['trytond.modules.edocument_uncefact.%s' % p
             for p in find_packages()]
@@ -129,27 +107,26 @@
         'Natural Language :: Russian',
         'Natural Language :: Slovenian',
         'Natural Language :: Spanish',
         'Natural Language :: Turkish',
         'Natural Language :: Ukrainian',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Office/Business',
         ],
     license='GPL-3',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=requires,
     extras_require={
         'test': tests_require,
         },
-    dependency_links=dependency_links,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     edocument_uncefact = trytond.modules.edocument_uncefact
     """,
     )
```

### Comparing `trytond_edocument_uncefact-6.6.0/template/16B-CII/CrossIndustryInvoice.xml` & `trytond_edocument_uncefact-6.8.0/template/16B-CII/CrossIndustryInvoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/EDIFICAS-EU_AccountingAccountType_D11A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/EDIFICAS-EU_AccountingAccountType_D11A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/EDIFICAS-EU_AccountingAmountType_D11A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/EDIFICAS-EU_AccountingAmountType_D11A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/ISO_ISO3AlphaCurrencyCode_2012-08-31.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/ISO_ISO3AlphaCurrencyCode_2012-08-31.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_ActionCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_ActionCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_AdjustmentReasonDescriptionCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_AdjustmentReasonDescriptionCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_AllowanceChargeIdentificationCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_AllowanceChargeIdentificationCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_AllowanceChargeReasonCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_AllowanceChargeReasonCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_AutomaticDataCaptureMethodCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_AutomaticDataCaptureMethodCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_CargoOperationalCategoryCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_CargoOperationalCategoryCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_CargoTypeCode_1996Rev2Final.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_CargoTypeCode_1996Rev2Final.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_CommodityIdentificationCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_CommodityIdentificationCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_CommunicationMeansTypeCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_CommunicationMeansTypeCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_ContactFunctionCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_ContactFunctionCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_DeliveryTermsCode_2010.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_DeliveryTermsCode_2010.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_DimensionTypeCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_DimensionTypeCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_DocumentNameCode_Accounting_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_DocumentNameCode_Accounting_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_DocumentNameCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_DocumentNameCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_DocumentStatusCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_DocumentStatusCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_DutyTaxFeeTypeCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_DutyTaxFeeTypeCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_DutyorTaxorFeeCategoryCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_DutyorTaxorFeeCategoryCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_EquipmentSizeTypeDescriptionCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_EquipmentSizeTypeDescriptionCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_EventTimeReferenceCodePaymentTermsEvent_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_EventTimeReferenceCodePaymentTermsEvent_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_EventTimeReferenceCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_EventTimeReferenceCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_FreightChargeQuantityUnitBasisCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_FreightChargeQuantityUnitBasisCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_FreightChargeTariffCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_FreightChargeTariffCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_GoodsTypeCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_GoodsTypeCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_GoodsTypeExtensionCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_GoodsTypeExtensionCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeLinear_4.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeLinear_4.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeVolume_4.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeVolume_4.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeWeight_4.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeWeight_4.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_MessageFunctionCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_MessageFunctionCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PackageTypeCode_2006.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PackageTypeCode_2006.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PackagingMarkingCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PackagingMarkingCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PartyRoleCode_ChargePaying_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PartyRoleCode_ChargePaying_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PartyRoleCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PartyRoleCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PaymentGuaranteeMeansCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PaymentGuaranteeMeansCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PaymentMeansChannelCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PaymentMeansChannelCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PaymentMeansCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PaymentMeansCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PaymentTermsTypeCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PaymentTermsTypeCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_PriceTypeCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_PriceTypeCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_ReferenceTypeCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_ReferenceTypeCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_TimePointFormatCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_TimePointFormatCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_TransportEquipmentCategoryCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_TransportEquipmentCategoryCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_TransportEquipmentFullnessCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_TransportEquipmentFullnessCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_TransportMeansTypeCode_2007.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_TransportMeansTypeCode_2007.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_TransportModeCode_2.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_TransportModeCode_2.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/codelist/standard/UNECE_TransportMovementStageCode_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/codelist/standard/UNECE_TransportMovementStageCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/data/standard/CrossIndustryInvoice_100pD16B.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/data/standard/CrossIndustryInvoice_100pD16B.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/data/standard/CrossIndustryInvoice_QualifiedDataType_100pD16B.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/data/standard/CrossIndustryInvoice_QualifiedDataType_100pD16B.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/data/standard/CrossIndustryInvoice_ReusableAggregateBusinessInformationEntity_100pD16B.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/data/standard/CrossIndustryInvoice_ReusableAggregateBusinessInformationEntity_100pD16B.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/data/standard/CrossIndustryInvoice_UnqualifiedDataType_100pD16B.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/data/standard/CrossIndustryInvoice_UnqualifiedDataType_100pD16B.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/identifierlist/standard/ISO_ISOTwo-letterCountryCode_SecondEdition2006.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/identifierlist/standard/ISO_ISOTwo-letterCountryCode_SecondEdition2006.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/identifierlist/standard/UNECE_FreightCostCode_4.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/identifierlist/standard/UNECE_FreightCostCode_4.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/16B-CII/identifierlist/standard/UNECE_PaymentTermsDescriptionIdentifier_D16A.xsd` & `trytond_edocument_uncefact-6.8.0/tests/16B-CII/identifierlist/standard/UNECE_PaymentTermsDescriptionIdentifier_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/tests/test_module.py` & `trytond_edocument_uncefact-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-6.6.0/trytond_edocument_uncefact.egg-info/PKG-INFO` & `trytond_edocument_uncefact-6.8.0/trytond_edocument_uncefact.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-edocument-uncefact
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for electronic document UN/CEFACT
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/edocument_uncefact
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton electronic document UN/CEFACT UNECE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: Slovenian
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: Turkish
 Classifier: Natural Language :: Ukrainian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
 EDocument UN/CEFACT Module
 ##########################
 
 Implement electronic document from UN/CEFACT:
```

### Comparing `trytond_edocument_uncefact-6.6.0/trytond_edocument_uncefact.egg-info/SOURCES.txt` & `trytond_edocument_uncefact-6.8.0/trytond_edocument_uncefact.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-.drone.yml
-.flake8
-.hgtags
-.isort.cfg
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 edocument.py
@@ -92,14 +88,15 @@
 ./tests/16B-CII/data/standard/CrossIndustryInvoice_100pD16B.xsd
 ./tests/16B-CII/data/standard/CrossIndustryInvoice_QualifiedDataType_100pD16B.xsd
 ./tests/16B-CII/data/standard/CrossIndustryInvoice_ReusableAggregateBusinessInformationEntity_100pD16B.xsd
 ./tests/16B-CII/data/standard/CrossIndustryInvoice_UnqualifiedDataType_100pD16B.xsd
 ./tests/16B-CII/identifierlist/standard/ISO_ISOTwo-letterCountryCode_SecondEdition2006.xsd
 ./tests/16B-CII/identifierlist/standard/UNECE_FreightCostCode_4.xsd
 ./tests/16B-CII/identifierlist/standard/UNECE_PaymentTermsDescriptionIdentifier_D16A.xsd
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

