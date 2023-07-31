# Comparing `tmp/lementpro-0.1.7.tar.gz` & `tmp/lementpro-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lementpro-0.1.7.tar", last modified: Thu Apr  6 10:59:56 2023, max compression
+gzip compressed data, was "lementpro-1.0.0.tar", last modified: Mon Jul 31 15:58:55 2023, max compression
```

## Comparing `lementpro-0.1.7.tar` & `lementpro-1.0.0.tar`

### file list

```diff
@@ -1,380 +1,385 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 10:59:56.525635 lementpro-0.1.7/
--rw-rw-rw-   0        0        0      583 2023-04-06 10:59:56.520632 lementpro-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-06 10:59:46.816477 lementpro-0.1.7/lementpro/
--rw-rw-rw-   0        0        0      647 2023-04-03 10:22:22.000000 lementpro-0.1.7/lementpro/__init__.py
--rw-rw-rw-   0        0        0     1559 2023-04-03 08:14:39.000000 lementpro-0.1.7/lementpro/builders.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:59:56.244580 lementpro-0.1.7/lementpro/data/
--rw-rw-rw-   0        0        0    14775 2023-04-06 10:54:59.000000 lementpro-0.1.7/lementpro/data/__init__.py
--rw-rw-rw-   0        0        0      206 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/data/accesstokenmodel.py
--rw-rw-rw-   0        0        0      349 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/data/actionlogentryinfomodel.py
--rw-rw-rw-   0        0        0      594 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/data/attributeaddmodel.py
--rw-rw-rw-   0        0        0      613 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/data/attributeaddrelationmodel.py
--rw-rw-rw-   0        0        0      147 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/data/attributeaddresultmodel.py
--rw-rw-rw-   0        0        0      682 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/data/attributeextendedmodel.py
--rw-rw-rw-   0        0        0      547 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/data/attributeinfomodel.py
--rw-rw-rw-   0        0        0      254 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/data/attributepagingmodel.py
--rw-rw-rw-   0        0        0      577 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/data/attributepatchmodel.py
--rw-rw-rw-   0        0        0      700 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/data/attributepatchrelationmodel.py
--rw-rw-rw-   0        0        0      699 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/data/attributerelationinfomodel.py
--rw-rw-rw-   0        0        0      181 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/data/changepasswordmodel.py
--rw-rw-rw-   0        0        0      277 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/data/checkconnectionmodel.py
--rw-rw-rw-   0        0        0      202 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/data/checkconnectionresultmodel.py
--rw-rw-rw-   0        0        0      399 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/data/commentaddbyusermodel.py
--rw-rw-rw-   0        0        0      145 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/data/commentaddresultmodel.py
--rw-rw-rw-   0        0        0      378 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/commentemailextensionmodel.py
--rw-rw-rw-   0        0        0      391 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/commentextensionmodel.py
--rw-rw-rw-   0        0        0      315 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/commentpatchmodel.py
--rw-rw-rw-   0        0        0      245 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/companycontactdetailsmodel.py
--rw-rw-rw-   0        0        0      250 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/companycontactdetailspatchmodel.py
--rw-rw-rw-   0        0        0      211 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/companyextensionmodel.py
--rw-rw-rw-   0        0        0      227 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/companyinfodetailedmodel.py
--rw-rw-rw-   0        0        0     1157 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/companyinfoextendedmodel.py
--rw-rw-rw-   0        0        0      374 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/companyinfomodel.py
--rw-rw-rw-   0        0        0      213 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/companylicensemodel.py
--rw-rw-rw-   0        0        0      308 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/companymailboxaddmodel.py
--rw-rw-rw-   0        0        0      152 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/companymailboxaddresultmodel.py
--rw-rw-rw-   0        0        0      334 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/companymailboxextendedmodel.py
--rw-rw-rw-   0        0        0      310 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/companymailboxpatchmodel.py
--rw-rw-rw-   0        0        0      286 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/companypasswordpolicymodel.py
--rw-rw-rw-   0        0        0      291 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/companypasswordpolicypatchmodel.py
--rw-rw-rw-   0        0        0      747 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/companypatchmodel.py
--rw-rw-rw-   0        0        0      276 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/departmentaddmodel.py
--rw-rw-rw-   0        0        0      148 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/departmentaddresultmodel.py
--rw-rw-rw-   0        0        0      150 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/departmentbosssetmodel.py
--rw-rw-rw-   0        0        0      683 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/departmentbossuserinfomodel.py
--rw-rw-rw-   0        0        0      679 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/departmentinfoextendedmodel.py
--rw-rw-rw-   0        0        0      548 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/departmentinfomodel.py
--rw-rw-rw-   0        0        0      255 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/departmentpagingmodel.py
--rw-rw-rw-   0        0        0      279 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/departmenttreemodel.py
--rw-rw-rw-   0        0        0      307 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/departmentupdatemodel.py
--rw-rw-rw-   0        0        0      369 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/emailaddressmodel.py
--rw-rw-rw-   0        0        0      187 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/errorresponse.py
--rw-rw-rw-   0        0        0      139 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/etaginfomodel.py
--rw-rw-rw-   0        0        0      457 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/fileinfomodel.py
--rw-rw-rw-   0        0        0      253 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/fileinfopagingmodel.py
--rw-rw-rw-   0        0        0      465 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/fileuploadresultmodel.py
--rw-rw-rw-   0        0        0      183 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderaddobjectstatefilter.py
--rw-rw-rw-   0        0        0      205 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderaddobjectstatusfilter.py
--rw-rw-rw-   0        0        0      296 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderaddobjectuserfilter.py
--rw-rw-rw-   0        0        0      144 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderaddresultmodel.py
--rw-rw-rw-   0        0        0      281 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderattributepredicatemodel.py
--rw-rw-rw-   0        0        0      325 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderfilterbyattributemodel.py
--rw-rw-rw-   0        0        0      223 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/foldergroupbyattributemodel.py
--rw-rw-rw-   0        0        0      169 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/foldergroupinfomodel.py
--rw-rw-rw-   0        0        0      428 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderinfomodel.py
--rw-rw-rw-   0        0        0      225 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderjoinbyattributemodel.py
--rw-rw-rw-   0        0        0      207 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderobjecttypeinfomodel.py
--rw-rw-rw-   0        0        0      183 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderobjecttypemodel.py
--rw-rw-rw-   0        0        0      246 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderorderbyattributemodel.py
--rw-rw-rw-   0        0        0      251 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderpagingmodel.py
--rw-rw-rw-   0        0        0      150 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderpatchgroupmodel.py
--rw-rw-rw-   0        0        0      185 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderpatchobjectstatefilter.py
--rw-rw-rw-   0        0        0      207 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderpatchobjectstatusfilter.py
--rw-rw-rw-   0        0        0      298 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderpatchobjectuserfilter.py
--rw-rw-rw-   0        0        0      301 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderpatchreset.py
--rw-rw-rw-   0        0        0      156 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/foldertemplateaddgroupmodel.py
--rw-rw-rw-   0        0        0     1118 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/foldertemplateaddmodel.py
--rw-rw-rw-   0        0        0     1254 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/foldertemplateextendedmodel.py
--rw-rw-rw-   0        0        0     1176 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/foldertemplatepatchmodel.py
--rw-rw-rw-   0        0        0      419 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/foldertemplatesmenuproxymodel.py
--rw-rw-rw-   0        0        0      379 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/foldertemplatestreeproxymodel.py
--rw-rw-rw-   0        0        0      177 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/folderusertreecountmodel.py
--rw-rw-rw-   0        0        0      198 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/groupaddmodel.py
--rw-rw-rw-   0        0        0      143 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/groupaddresultmodel.py
--rw-rw-rw-   0        0        0      644 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/groupinfoextendedproxymodel.py
--rw-rw-rw-   0        0        0      357 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/groupinfomodel.py
--rw-rw-rw-   0        0        0      210 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/groupobjectexpirationaddmodel.py
--rw-rw-rw-   0        0        0      159 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/groupobjectexpirationaddresultmodel.py
--rw-rw-rw-   0        0        0      258 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/groupobjectexpirationinfomodel.py
--rw-rw-rw-   0        0        0      187 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/groupobjectexpirationpatchmodel.py
--rw-rw-rw-   0        0        0      254 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/groupobjecttypeinfomodel.py
--rw-rw-rw-   0        0        0      260 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/groupobjecttypepagingmodel.py
--rw-rw-rw-   0        0        0      184 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/groupobjecttypeupsertmodel.py
--rw-rw-rw-   0        0        0      250 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/grouppagingmodel.py
--rw-rw-rw-   0        0        0      360 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/groupupdateproxymodel.py
--rw-rw-rw-   0        0        0      319 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/integrationmailboxactionaddmodel.py
--rw-rw-rw-   0        0        0      200 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/integrationmailboxactionaddresultmodel.py
--rw-rw-rw-   0        0        0      344 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/integrationmailboxactionextendedmodel.py
--rw-rw-rw-   0        0        0      283 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/integrationmailboxactionpatchmodel.py
--rw-rw-rw-   0        0        0      311 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/integrationmailboxaddmodel.py
--rw-rw-rw-   0        0        0      156 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/integrationmailboxaddresultmodel.py
--rw-rw-rw-   0        0        0      337 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/integrationmailboxextendedmodel.py
--rw-rw-rw-   0        0        0      333 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/integrationmailboxinfomodel.py
--rw-rw-rw-   0        0        0      263 2023-04-03 08:20:46.000000 lementpro-0.1.7/lementpro/data/integrationmailboxpagingmodel.py
--rw-rw-rw-   0        0        0      313 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/integrationmailboxpatchmodel.py
--rw-rw-rw-   0        0        0      186 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/integrationmailboxrulemodel.py
--rw-rw-rw-   0        0        0      160 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/languagemodel.py
--rw-rw-rw-   0        0        0      284 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/mxgraphgetschemaresponse.py
--rw-rw-rw-   0        0        0      315 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/mxgraphschemaadddraftrequest.py
--rw-rw-rw-   0        0        0      283 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/mxgraphschemaaddrequest.py
--rw-rw-rw-   0        0        0      350 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/mxgraphschemaaddrequesttransitionactionmodel.py
--rw-rw-rw-   0        0        0      428 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/mxgraphschemaaddrequesttransitionconditionmodel.py
--rw-rw-rw-   0        0        0      320 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/mxgraphschemaaddrequesttransitionconditionpredicatemodel.py
--rw-rw-rw-   0        0        0      588 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/mxgraphschemaelementmodel.py
--rw-rw-rw-   0        0        0      217 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/mxgraphschemaline.py
--rw-rw-rw-   0        0        0      160 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/mxgraphschemapoint.py
--rw-rw-rw-   0        0        0      301 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/mxgraphschemarelatedproperty.py
--rw-rw-rw-   0        0        0      820 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/mxgraphschematransitionmodel.py
--rw-rw-rw-   0        0        0      172 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/mxgraphschemauserreference.py
--rw-rw-rw-   0        0        0      345 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/mxgraphschemavariablemodel.py
--rw-rw-rw-   0        0        0      144 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objectaddresultmodel.py
--rw-rw-rw-   0        0        0      210 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objectattributemodel.py
--rw-rw-rw-   0        0        0      223 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeaddcountermodel.py
--rw-rw-rw-   0        0        0      175 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeaddextensionmodel.py
--rw-rw-rw-   0        0        0      622 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeaddmodel.py
--rw-rw-rw-   0        0        0      148 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeaddresultmodel.py
--rw-rw-rw-   0        0        0      256 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeattributeaddformulamodel.py
--rw-rw-rw-   0        0        0      536 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeattributeaddproxymodel.py
--rw-rw-rw-   0        0        0      157 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeattributeaddresultmodel.py
--rw-rw-rw-   0        0        0      674 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeattributeaddsettingsmodel.py
--rw-rw-rw-   0        0        0      915 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeattributeextendedmodel.py
--rw-rw-rw-   0        0        0      720 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeattributeinfoattributemodel.py
--rw-rw-rw-   0        0        0      312 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeattributeinfoattributerelationmodel.py
--rw-rw-rw-   0        0        0      257 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeattributeinfoformulamodel.py
--rw-rw-rw-   0        0        0      754 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeattributeinfomodel.py
--rw-rw-rw-   0        0        0      675 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeattributeinfosettingsmodel.py
--rw-rw-rw-   0        0        0      191 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeattributeinfovaluelistentrymodel.py
--rw-rw-rw-   0        0        0      186 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeattributeinfovaluelistmodel.py
--rw-rw-rw-   0        0        0      264 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeattributepagingmodel.py
--rw-rw-rw-   0        0        0      258 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeattributepatchformulamodel.py
--rw-rw-rw-   0        0        0      516 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeattributepatchmodel.py
--rw-rw-rw-   0        0        0      676 2023-04-03 08:20:47.000000 lementpro-0.1.7/lementpro/data/objecttypeattributepatchsettingsmodel.py
--rw-rw-rw-   0        0        0      241 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypebimaddproxymodel.py
--rw-rw-rw-   0        0        0      151 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypebimaddresultmodel.py
--rw-rw-rw-   0        0        0      295 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypebiminfoextendedmodel.py
--rw-rw-rw-   0        0        0      238 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypebimpatchmodel.py
--rw-rw-rw-   0        0        0      178 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypebreadcrumbmodel.py
--rw-rw-rw-   0        0        0      237 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypecheckpointaddproxymodel.py
--rw-rw-rw-   0        0        0      158 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypecheckpointaddresultmodel.py
--rw-rw-rw-   0        0        0      291 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypecheckpointinfoextendedmodel.py
--rw-rw-rw-   0        0        0      289 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypecheckpointinfopagingmodel.py
--rw-rw-rw-   0        0        0      265 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypecheckpointpagingmodel.py
--rw-rw-rw-   0        0        0      234 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypecheckpointpatchmodel.py
--rw-rw-rw-   0        0        0      202 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeextensionmodel.py
--rw-rw-rw-   0        0        0      207 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypefileinfopagingmodel.py
--rw-rw-rw-   0        0        0      259 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypefilepagingmodel.py
--rw-rw-rw-   0        0        0      155 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypefileupsertmodel.py
--rw-rw-rw-   0        0        0      265 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeinfodetailedbimmodel.py
--rw-rw-rw-   0        0        0      252 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeinfodetailedcountermodel.py
--rw-rw-rw-   0        0        0      179 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeinfodetailedfilemodel.py
--rw-rw-rw-   0        0        0      365 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeinfodetailedmenumodel.py
--rw-rw-rw-   0        0        0      603 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeinfodetailedmodel.py
--rw-rw-rw-   0        0        0      767 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeinfoextendedmodel.py
--rw-rw-rw-   0        0        0      595 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeinfopagingmodel.py
--rw-rw-rw-   0        0        0      258 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypemenuaddproxymodel.py
--rw-rw-rw-   0        0        0      152 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypemenuaddresultmodel.py
--rw-rw-rw-   0        0        0      422 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypemenuinfoextendedmodel.py
--rw-rw-rw-   0        0        0      420 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypemenuinfopagingmodel.py
--rw-rw-rw-   0        0        0      283 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypemenupatchmodel.py
--rw-rw-rw-   0        0        0      255 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypepagingmodel.py
--rw-rw-rw-   0        0        0      225 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypepatchcountermodel.py
--rw-rw-rw-   0        0        0      177 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypepatchextensionmodel.py
--rw-rw-rw-   0        0        0      638 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypepatchmodel.py
--rw-rw-rw-   0        0        0      257 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypetreenodeproxymodel.py
--rw-rw-rw-   0        0        0     1045 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeuisettingsproxyresponse.py
--rw-rw-rw-   0        0        0      172 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeuisettingsproxyresponsecreatepage.py
--rw-rw-rw-   0        0        0      268 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeuisettingsproxyresponsecreatepageattribute.py
--rw-rw-rw-   0        0        0      197 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeuisettingsproxyresponsedetailedpage.py
--rw-rw-rw-   0        0        0      306 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeuisettingsproxyresponsedetailedpageattribute.py
--rw-rw-rw-   0        0        0      264 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeuisettingsproxyresponsedetailedpagetab.py
--rw-rw-rw-   0        0        0      170 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeuisettingsproxyresponseeditpage.py
--rw-rw-rw-   0        0        0      266 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeuisettingsproxyresponseeditpageattribute.py
--rw-rw-rw-   0        0        0      172 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeuisettingsproxyresponselistview.py
--rw-rw-rw-   0        0        0      293 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeuisettingsproxyresponselistviewattribute.py
--rw-rw-rw-   0        0        0      172 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeuisettingsproxyresponsetableview.py
--rw-rw-rw-   0        0        0      267 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objecttypeuisettingsproxyresponsetableviewattribute.py
--rw-rw-rw-   0        0        0      184 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objectuserfavoritemodel.py
--rw-rw-rw-   0        0        0      151 2023-04-03 08:20:48.000000 lementpro-0.1.7/lementpro/data/objectuserreadmodel.py
--rw-rw-rw-   0        0        0      153 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/objectuserunreadmodel.py
--rw-rw-rw-   0        0        0      252 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/pagingmodel.py
--rw-rw-rw-   0        0        0      151 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/refreshtokenmodel.py
--rw-rw-rw-   0        0        0      441 2023-04-06 10:58:49.000000 lementpro-0.1.7/lementpro/data/relatedobjectmodel.py
--rw-rw-rw-   0        0        0      273 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/relationvalue.py
--rw-rw-rw-   0        0        0      174 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/restorepasswordmodel.py
--rw-rw-rw-   0        0        0      160 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/routeactivitybuttonrequest.py
--rw-rw-rw-   0        0        0      222 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/routeextendedresponseactivityelement.py
--rw-rw-rw-   0        0        0      501 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/routeextendedresponseactivityvariable.py
--rw-rw-rw-   0        0        0      220 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/routeextendedresponsereferenceobject.py
--rw-rw-rw-   0        0        0      252 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/routeextendedresponsereferenceobjectproperty.py
--rw-rw-rw-   0        0        0      460 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/routeinforesponse.py
--rw-rw-rw-   0        0        0      255 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/routeinforesponseschema.py
--rw-rw-rw-   0        0        0      359 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/routeinforesponseschemaversion.py
--rw-rw-rw-   0        0        0      253 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/routepagingresponse.py
--rw-rw-rw-   0        0        0      220 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/schemaaddresponse.py
--rw-rw-rw-   0        0        0      327 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/schemaextendedresponse.py
--rw-rw-rw-   0        0        0      278 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/schemainforesponse.py
--rw-rw-rw-   0        0        0      260 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/schemainforesponseversion.py
--rw-rw-rw-   0        0        0      254 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/schemapagingresponse.py
--rw-rw-rw-   0        0        0      259 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationaddmodel.py
--rw-rw-rw-   0        0        0      156 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationaddresultmodel.py
--rw-rw-rw-   0        0        0      196 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationinfodetailedmodel.py
--rw-rw-rw-   0        0        0      473 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationinfoextendedmodel.py
--rw-rw-rw-   0        0        0      313 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationinfopagingmodel.py
--rw-rw-rw-   0        0        0      209 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationinfoparammodel.py
--rw-rw-rw-   0        0        0      208 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationobjecttypeaddmodel.py
--rw-rw-rw-   0        0        0      166 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationobjecttypeaddresultmodel.py
--rw-rw-rw-   0        0        0      237 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationobjecttypeinfoextendedmodel.py
--rw-rw-rw-   0        0        0      235 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationobjecttypeinfopagingmodel.py
--rw-rw-rw-   0        0        0      273 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationobjecttypepagingmodel.py
--rw-rw-rw-   0        0        0      172 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationobjecttypepatchmodel.py
--rw-rw-rw-   0        0        0      263 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationpagingmodel.py
--rw-rw-rw-   0        0        0      246 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationparamaddmodel.py
--rw-rw-rw-   0        0        0      161 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationparamaddresultmodel.py
--rw-rw-rw-   0        0        0      275 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationparaminfoextendedmodel.py
--rw-rw-rw-   0        0        0      273 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationparaminfopagingmodel.py
--rw-rw-rw-   0        0        0      268 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationparampagingmodel.py
--rw-rw-rw-   0        0        0      210 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationparampatchmodel.py
--rw-rw-rw-   0        0        0      261 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/serviceintegrationpatchmodel.py
--rw-rw-rw-   0        0        0      199 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/setobjecttyperequest.py
--rw-rw-rw-   0        0        0      190 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/setsortweightmodel.py
--rw-rw-rw-   0        0        0      169 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/signinproxymodel.py
--rw-rw-rw-   0        0        0      258 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/statisticspagingresponse.py
--rw-rw-rw-   0        0        0      453 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/statisticsrecordinforesponse.py
--rw-rw-rw-   0        0        0      163 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/timezoneinfomodel.py
--rw-rw-rw-   0        0        0      253 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/timezonepagingmodel.py
--rw-rw-rw-   0        0        0      138 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/tobccmodel.py
--rw-rw-rw-   0        0        0      137 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/toccmodel.py
--rw-rw-rw-   0        0        0      141 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/toemailsmodel.py
--rw-rw-rw-   0        0        0      270 2023-04-03 07:58:25.000000 lementpro-0.1.7/lementpro/data/user.py
--rw-rw-rw-   0        0        0      669 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/useraddmodel.py
--rw-rw-rw-   0        0        0      142 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/useraddresultmodel.py
--rw-rw-rw-   0        0        0      151 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/userassistantaddresultmodel.py
--rw-rw-rw-   0        0        0      156 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/userdepartmentmoveproxymodel.py
--rw-rw-rw-   0        0        0      254 2023-04-03 08:20:49.000000 lementpro-0.1.7/lementpro/data/userdetailedmodeldepartment.py
--rw-rw-rw-   0        0        0      195 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/userdetailedmodelgroup.py
--rw-rw-rw-   0        0        0      464 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/userdetailedmodelnotification.py
--rw-rw-rw-   0        0        0     1144 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/userfolderaddmodel.py
--rw-rw-rw-   0        0        0     1306 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/userfolderextendedmodel.py
--rw-rw-rw-   0        0        0      458 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/userfolderinfomodel.py
--rw-rw-rw-   0        0        0      255 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/userfolderpagingmodel.py
--rw-rw-rw-   0        0        0     1202 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/userfolderpatchmodel.py
--rw-rw-rw-   0        0        0      146 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/userfoldertreemodel.py
--rw-rw-rw-   0        0        0      632 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/userfoldertreenodemodel.py
--rw-rw-rw-   0        0        0      158 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateassistantaddmodel.py
--rw-rw-rw-   0        0        0      342 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateassistantmodel.py
--rw-rw-rw-   0        0        0      661 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateattributeinfomodel.py
--rw-rw-rw-   0        0        0      295 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateattributeobjecttypetreenode.py
--rw-rw-rw-   0        0        0      325 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatecategoryaddrequest.py
--rw-rw-rw-   0        0        0      151 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatecategoryaddresponse.py
--rw-rw-rw-   0        0        0      335 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatecategorypartialupdaterequest.py
--rw-rw-rw-   0        0        0      240 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatecommentmessageinfofilemodel.py
--rw-rw-rw-   0        0        0      878 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatecommentmessageinfomodel.py
--rw-rw-rw-   0        0        0      264 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatecommentmessageinfousermodel.py
--rw-rw-rw-   0        0        0      268 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatecommentmessagespagingmodel.py
--rw-rw-rw-   0        0        0      409 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateexecuteobjectactionmodel.py
--rw-rw-rw-   0        0        0      194 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateexecuteobjectactionresultmodel.py
--rw-rw-rw-   0        0        0      710 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatefolderobjectinfoattributemodel.py
--rw-rw-rw-   0        0        0      690 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatefolderobjectinfomodel.py
--rw-rw-rw-   0        0        0      370 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatefolderobjectinfomodelcommentinfo.py
--rw-rw-rw-   0        0        0      674 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatefolderobjectinfomodellastcomment.py
--rw-rw-rw-   0        0        0      273 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatefolderobjectinfomodellastcommentuser.py
--rw-rw-rw-   0        0        0      385 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatefolderobjectspagingmodel.py
--rw-rw-rw-   0        0        0      199 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergategetobjecttemplateresultmodel.py
--rw-rw-rw-   0        0        0      363 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatementioninfocommentmodel.py
--rw-rw-rw-   0        0        0      458 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatementioninfomodel.py
--rw-rw-rw-   0        0        0      197 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatementioninfoobjectmodel.py
--rw-rw-rw-   0        0        0      261 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergatementionspagingmodel.py
--rw-rw-rw-   0        0        0      282 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateobjectaddmodel.py
--rw-rw-rw-   0        0        0      667 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateobjectinfoattributemodel.py
--rw-rw-rw-   0        0        0      263 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateobjectinfochunkitemmodel.py
--rw-rw-rw-   0        0        0      176 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateobjectinfochunkmodel.py
--rw-rw-rw-   0        0        0      813 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateobjectinfoextendedattributemodel.py
--rw-rw-rw-   0        0        0      686 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateobjectinfoextendedmodel.py
--rw-rw-rw-   0        0        0      198 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateobjectinfoextendedmodelroutebutton.py
--rw-rw-rw-   0        0        0      218 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateobjectinfoextendedmodelroutedata.py
--rw-rw-rw-   0        0        0      305 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateobjectinfomodel.py
--rw-rw-rw-   0        0        0      382 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateobjectinfopagingmodel.py
--rw-rw-rw-   0        0        0      250 2023-04-03 08:20:50.000000 lementpro-0.1.7/lementpro/data/usergateobjectmodelattribute.py
--rw-rw-rw-   0        0        0      200 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergateobjectpatchmodel.py
--rw-rw-rw-   0        0        0      494 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergateobjecttypeobjectinfomodel.py
--rw-rw-rw-   0        0        0      389 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergateobjecttypeobjectspagingmodel.py
--rw-rw-rw-   0        0        0      290 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergateobjecttypetreemodel.py
--rw-rw-rw-   0        0        0      152 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergatepagingmetadata.py
--rw-rw-rw-   0        0        0      231 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergatepagingmetadatacolumn.py
--rw-rw-rw-   0        0        0      160 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergatequicksearchresultmodel.py
--rw-rw-rw-   0        0        0      203 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergatequicksearchresultobjectmodel.py
--rw-rw-rw-   0        0        0      552 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergaterouteinstanceextendedmodel.py
--rw-rw-rw-   0        0        0      574 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergaterouteinstanceextendedmodelactivity.py
--rw-rw-rw-   0        0        0      673 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergatesearchobjectinfoattributemodel.py
--rw-rw-rw-   0        0        0      463 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergatesearchobjectinfomodel.py
--rw-rw-rw-   0        0        0      384 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergatesearchresultpagingmodel.py
--rw-rw-rw-   0        0        0      257 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergatesubstitutionmodel.py
--rw-rw-rw-   0        0        0      377 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergateuserspagingmodel.py
--rw-rw-rw-   0        0        0      150 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergroupaddproxymodel.py
--rw-rw-rw-   0        0        0      147 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usergroupaddresultmodel.py
--rw-rw-rw-   0        0        0      870 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/userinfobysystemadminmodel.py
--rw-rw-rw-   0        0        0      234 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/userinfobysystemadminmodeldepartment.py
--rw-rw-rw-   0        0        0      204 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/userinfobysystemadminmodelgroup.py
--rw-rw-rw-   0        0        0     1158 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/userinfoextendedmodel.py
--rw-rw-rw-   0        0        0      290 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/userinfoextensionmodel.py
--rw-rw-rw-   0        0        0      669 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/userinfomodel.py
--rw-rw-rw-   0        0        0      332 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usermailboxaddmodel.py
--rw-rw-rw-   0        0        0      149 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usermailboxaddresultmodel.py
--rw-rw-rw-   0        0        0      412 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usermailboxextendedmodel.py
--rw-rw-rw-   0        0        0      334 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usermailboxpatchmodel.py
--rw-rw-rw-   0        0        0      155 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usermentiondeletemodel.py
--rw-rw-rw-   0        0        0      286 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usermodelextension.py
--rw-rw-rw-   0        0        0      436 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usermodelnotification.py
--rw-rw-rw-   0        0        0      440 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usernotificationinfomodel.py
--rw-rw-rw-   0        0        0      442 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usernotificationupdatemodel.py
--rw-rw-rw-   0        0        0      262 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/userpagingbysystemadminmodel.py
--rw-rw-rw-   0        0        0      180 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/userpasswordupdatemodel.py
--rw-rw-rw-   0        0        0      671 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/userpatchmodel.py
--rw-rw-rw-   0        0        0      153 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usersgroupaddproxymodel.py
--rw-rw-rw-   0        0        0      150 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/usersgroupaddresultmodel.py
--rw-rw-rw-   0        0        0      149 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/userviewaddmodel.py
--rw-rw-rw-   0        0        0      148 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/userviewaddresultmodel.py
--rw-rw-rw-   0        0        0      221 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/userviewinfomodel.py
--rw-rw-rw-   0        0        0      253 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/userviewpagingmodel.py
--rw-rw-rw-   0        0        0      172 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/validationresponse.py
--rw-rw-rw-   0        0        0      174 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/validationresponseitem.py
--rw-rw-rw-   0        0        0      171 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/valuelistaddentrymodel.py
--rw-rw-rw-   0        0        0      226 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/valuelistaddmodel.py
--rw-rw-rw-   0        0        0      147 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/valuelistaddresultmodel.py
--rw-rw-rw-   0        0        0      176 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/valuelistentryaddproxymodel.py
--rw-rw-rw-   0        0        0      152 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/valuelistentryaddresultmodel.py
--rw-rw-rw-   0        0        0      221 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/valuelistentryinfomodel.py
--rw-rw-rw-   0        0        0      259 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/valuelistentrypagingmodel.py
--rw-rw-rw-   0        0        0      150 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/valuelistentrypatchmodel.py
--rw-rw-rw-   0        0        0      305 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/valuelistextendedmodel.py
--rw-rw-rw-   0        0        0      276 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/valuelistinfomodel.py
--rw-rw-rw-   0        0        0      254 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/valuelistpagingmodel.py
--rw-rw-rw-   0        0        0      174 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/valuelistpatchmodel.py
--rw-rw-rw-   0        0        0      169 2023-04-03 08:20:51.000000 lementpro-0.1.7/lementpro/data/virtualfolderpath.py
--rw-rw-rw-   0        0        0      353 2023-04-03 07:58:25.000000 lementpro-0.1.7/lementpro/logger.py
--rw-rw-rw-   0        0        0     1849 2023-04-03 07:58:25.000000 lementpro-0.1.7/lementpro/sender.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:59:56.444279 lementpro-0.1.7/lementpro/services/
--rw-rw-rw-   0        0        0      504 2023-04-06 10:55:50.000000 lementpro-0.1.7/lementpro/services/__init__.py
--rw-rw-rw-   0        0        0     4515 2023-04-04 13:53:40.000000 lementpro-0.1.7/lementpro/services/accounts.py
--rw-rw-rw-   0        0        0    66898 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/services/admin.py
--rw-rw-rw-   0        0        0     3901 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/services/comments.py
--rw-rw-rw-   0        0        0      466 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/services/companies.py
--rw-rw-rw-   0        0        0      708 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/services/connections.py
--rw-rw-rw-   0        0        0     1200 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/services/departments.py
--rw-rw-rw-   0        0        0     2543 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/services/files.py
--rw-rw-rw-   0        0        0     5861 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/services/folder.py
--rw-rw-rw-   0        0        0      771 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/services/groups.py
--rw-rw-rw-   0        0        0     1179 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/services/localization.py
--rw-rw-rw-   0        0        0     3959 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/services/objects.py
--rw-rw-rw-   0        0        0     2376 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/services/objecttypes.py
--rw-rw-rw-   0        0        0      561 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/services/routes.py
--rw-rw-rw-   0        0        0     1153 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/services/search.py
--rw-rw-rw-   0        0        0      630 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/services/timezones.py
--rw-rw-rw-   0        0        0     5821 2023-04-03 08:20:45.000000 lementpro-0.1.7/lementpro/services/users.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:59:46.857555 lementpro-0.1.7/lementpro.egg-info/
--rw-rw-rw-   0        0        0      583 2023-04-06 10:59:46.000000 lementpro-0.1.7/lementpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    16392 2023-04-06 10:59:46.000000 lementpro-0.1.7/lementpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 10:59:46.000000 lementpro-0.1.7/lementpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-06 10:59:46.000000 lementpro-0.1.7/lementpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-06 10:59:46.000000 lementpro-0.1.7/lementpro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 10:59:56.526634 lementpro-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      831 2023-04-06 10:59:23.000000 lementpro-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:59:46.781483 lementpro-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-06 10:59:56.487734 lementpro-0.1.7/src/templates/
--rw-rw-rw-   0        0        0        0 2023-04-03 07:58:25.000000 lementpro-0.1.7/src/templates/__init__.py
--rw-rw-rw-   0        0        0     1559 2023-04-03 08:14:39.000000 lementpro-0.1.7/src/templates/builders.py
--rw-rw-rw-   0        0        0      353 2023-04-03 07:58:25.000000 lementpro-0.1.7/src/templates/logger.py
--rw-rw-rw-   0        0        0     1849 2023-04-03 07:58:25.000000 lementpro-0.1.7/src/templates/sender.py
--rw-rw-rw-   0        0        0      270 2023-04-03 07:58:25.000000 lementpro-0.1.7/src/templates/user.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:59:56.501635 lementpro-0.1.7/tests/
--rw-rw-rw-   0        0        0      863 2023-04-03 07:58:25.000000 lementpro-0.1.7/tests/test_sdk.py
+drwxr-xr-x   0 mihailcupilnik   (501) staff       (20)        0 2023-07-31 15:58:55.442353 lementpro-1.0.0/
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      617 2023-07-31 15:58:55.442215 lementpro-1.0.0/PKG-INFO
+drwxr-xr-x   0 mihailcupilnik   (501) staff       (20)        0 2023-07-31 15:58:55.360154 lementpro-1.0.0/lementpro/
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      629 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/__init__.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     1510 2023-07-31 14:38:38.000000 lementpro-1.0.0/lementpro/builders.py
+drwxr-xr-x   0 mihailcupilnik   (501) staff       (20)        0 2023-07-31 15:58:55.435182 lementpro-1.0.0/lementpro/data/
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)    14437 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/__init__.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      200 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/accesstokenmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      340 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/actionlogentryinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      577 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/attributeaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      596 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/attributeaddrelationmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      143 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/attributeaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      662 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/attributeextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      529 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/attributeinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      247 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/attributepagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      561 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/attributepatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      681 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/attributepatchrelationmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      680 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/attributerelationinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      176 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/changepasswordmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      268 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/checkconnectionmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      197 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/checkconnectionresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      388 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/commentaddbyusermodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      141 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/commentaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      369 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/commentemailextensionmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      384 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/commentextensionmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      307 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/commentpatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      237 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/companycontactdetailsmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      242 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/companycontactdetailspatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      205 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/companyextensionmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      221 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/companyinfodetailedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     1132 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/companyinfoextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      362 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/companyinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      207 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/companylicensemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      298 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/companymailboxaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      148 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/companymailboxaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      323 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/companymailboxextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      300 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/companymailboxpatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      278 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/companypasswordpolicymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      283 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/companypasswordpolicypatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      731 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/companypatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      267 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/departmentaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      144 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/departmentaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      146 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/departmentbosssetmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      662 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/departmentbossuserinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      661 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/departmentinfoextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      532 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/departmentinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      248 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/departmentpagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      272 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/departmenttreemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      297 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/departmentupdatemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      360 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/emailaddressmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      181 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/errorresponse.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      135 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/etaginfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      442 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/fileinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      246 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/fileinfopagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      450 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/fileuploadresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      178 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderaddobjectstatefilter.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      199 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderaddobjectstatusfilter.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      287 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderaddobjectuserfilter.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      140 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      273 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderattributepredicatemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      318 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderfilterbyattributemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      217 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/foldergroupbyattributemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      164 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/foldergroupinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      414 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      219 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderjoinbyattributemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      201 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderobjecttypeinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      178 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderobjecttypemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      239 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderorderbyattributemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      244 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderpagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      146 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderpatchgroupmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      180 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderpatchobjectstatefilter.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      201 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderpatchobjectstatusfilter.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      289 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderpatchobjectuserfilter.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      293 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderpatchreset.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      152 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/foldertemplateaddgroupmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     1095 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/foldertemplateaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     1226 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/foldertemplateextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     1153 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/foldertemplatepatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      405 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/foldertemplatesmenuproxymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      367 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/foldertemplatestreeproxymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      172 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/folderusertreecountmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      192 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/groupaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      139 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/groupaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      628 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/groupinfoextendedproxymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      345 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/groupinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      204 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/groupobjectexpirationaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      155 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/groupobjectexpirationaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      250 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/groupobjectexpirationinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      182 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/groupobjectexpirationpatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      246 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/groupobjecttypeinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      253 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/groupobjecttypepagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      179 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/groupobjecttypeupsertmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      243 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/grouppagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      352 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/groupupdateproxymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      310 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/integrationmailboxactionaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      195 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/integrationmailboxactionaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      334 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/integrationmailboxactionextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      275 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/integrationmailboxactionpatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      301 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/integrationmailboxaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      152 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/integrationmailboxaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      326 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/integrationmailboxextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      322 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/integrationmailboxinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      256 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/integrationmailboxpagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      303 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/integrationmailboxpatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      181 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/integrationmailboxrulemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      155 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/languagemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      275 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/mxgraphgetschemaresponse.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      305 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/mxgraphschemaadddraftrequest.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      274 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/mxgraphschemaaddrequest.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      341 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/mxgraphschemaaddrequesttransitionactionmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      430 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/mxgraphschemaaddrequesttransitionconditionmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      312 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/mxgraphschemaaddrequesttransitionconditionpredicatemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      571 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/mxgraphschemaelementmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      210 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/mxgraphschemaline.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      155 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/mxgraphschemapoint.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      292 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/mxgraphschemarelatedproperty.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      810 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/mxgraphschematransitionmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      167 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/mxgraphschemauserreference.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      335 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/mxgraphschemavariablemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      140 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objectaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      204 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objectattributemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      217 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeaddcountermodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      171 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeaddextensionmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      606 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      144 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      249 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeattributeaddformulamodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      526 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeattributeaddproxymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      153 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeattributeaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      655 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeattributeaddsettingsmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      896 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeattributeextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      705 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeattributeinfoattributemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      304 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeattributeinfoattributerelationmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      250 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeattributeinfoformulamodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      737 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeattributeinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      656 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeattributeinfosettingsmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      186 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeattributeinfovaluelistentrymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      181 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeattributeinfovaluelistmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      257 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeattributepagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      251 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeattributepatchformulamodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      507 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeattributepatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      657 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeattributepatchsettingsmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      234 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypebimaddproxymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      147 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypebimaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      286 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypebiminfoextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      231 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypebimpatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      173 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypebreadcrumbmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      230 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypecheckpointaddproxymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      154 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypecheckpointaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      282 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypecheckpointinfoextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      280 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypecheckpointinfopagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      258 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypecheckpointpagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      227 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypecheckpointpatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      197 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeextensionmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      201 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypefileinfopagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      252 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypefilepagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      151 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypefileupsertmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      257 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeinfodetailedbimmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      245 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeinfodetailedcountermodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      174 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeinfodetailedfilemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      353 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeinfodetailedmenumodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      593 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeinfodetailedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      746 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeinfoextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      577 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeinfopagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      250 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypemenuaddproxymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      148 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypemenuaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      408 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypemenuinfoextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      406 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypemenuinfopagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      274 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypemenupatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      248 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypepagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      219 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypepatchcountermodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      173 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypepatchextensionmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      622 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypepatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      249 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypetreenodeproxymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     1032 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeuisettingsproxyresponse.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      168 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeuisettingsproxyresponsecreatepage.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      261 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeuisettingsproxyresponsecreatepageattribute.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      192 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeuisettingsproxyresponsedetailedpage.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      298 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeuisettingsproxyresponsedetailedpageattribute.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      257 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeuisettingsproxyresponsedetailedpagetab.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      166 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeuisettingsproxyresponseeditpage.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      259 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeuisettingsproxyresponseeditpageattribute.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      168 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeuisettingsproxyresponselistview.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      285 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeuisettingsproxyresponselistviewattribute.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      168 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeuisettingsproxyresponsetableview.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      260 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objecttypeuisettingsproxyresponsetableviewattribute.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      179 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objectuserfavoritemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      147 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objectuserreadmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      149 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/objectuserunreadmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      243 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/pagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      147 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/refreshtokenmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      426 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/relatedobjectmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      265 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/relationvalue.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      169 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/restorepasswordmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      156 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/routeactivitybuttonrequest.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      216 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/routeextendedresponseactivityelement.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      489 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/routeextendedresponseactivityvariable.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      214 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/routeextendedresponsereferenceobject.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      245 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/routeextendedresponsereferenceobjectproperty.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      448 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/routeinforesponse.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      247 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/routeinforesponseschema.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      350 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/routeinforesponseschemaversion.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      246 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/routepagingresponse.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      213 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/schemaaddresponse.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      317 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/schemaextendedresponse.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      269 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/schemainforesponse.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      252 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/schemainforesponseversion.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      247 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/schemapagingresponse.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      251 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      152 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      191 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationinfodetailedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      461 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationinfoextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      303 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationinfopagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      203 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationinfoparammodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      203 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationobjecttypeaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      162 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationobjecttypeaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      231 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationobjecttypeinfoextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      229 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationobjecttypeinfopagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      266 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationobjecttypepagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      168 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationobjecttypepatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      256 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationpagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      239 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationparamaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      157 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationparamaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      267 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationparaminfoextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      265 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationparaminfopagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      261 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationparampagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      204 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationparampatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      253 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/serviceintegrationpatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      194 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/setobjecttyperequest.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      184 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/setsortweightmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      164 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/signinproxymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      251 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/statisticspagingresponse.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      439 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/statisticsrecordinforesponse.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      158 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/timezoneinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      246 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/timezonepagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      134 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/tobccmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      133 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/toccmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      137 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/toemailsmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      257 2023-07-31 14:38:38.000000 lementpro-1.0.0/lementpro/data/user.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      650 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/useraddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      138 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/useraddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      147 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userassistantaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      152 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userdepartmentmoveproxymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      246 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userdetailedmodeldepartment.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      189 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userdetailedmodelgroup.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      454 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userdetailedmodelnotification.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     1120 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userfolderaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     1276 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userfolderextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      443 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userfolderinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      248 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userfolderpagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     1178 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userfolderpatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      142 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userfoldertreemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      613 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userfoldertreenodemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      154 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateassistantaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      331 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateassistantmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      644 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateattributeinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      286 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateattributeobjecttypetreenode.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      315 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatecategoryaddrequest.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      147 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatecategoryaddresponse.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      325 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatecategorypartialupdaterequest.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      233 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatecommentmessageinfofilemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      857 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatecommentmessageinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      256 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatecommentmessageinfousermodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      261 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatecommentmessagespagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      399 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateexecuteobjectactionmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      189 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateexecuteobjectactionresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      692 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatefolderobjectinfoattributemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      671 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatefolderobjectinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      363 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatefolderobjectinfomodelcommentinfo.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      661 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatefolderobjectinfomodellastcomment.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      265 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatefolderobjectinfomodellastcommentuser.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      376 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatefolderobjectspagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      194 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergategetobjecttemplateresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      355 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatementioninfocommentmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      449 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatementioninfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      191 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatementioninfoobjectmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      254 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatementionspagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      274 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateobjectaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      650 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateobjectinfoattributemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      255 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateobjectinfochunkitemmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      171 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateobjectinfochunkmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      792 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateobjectinfoextendedattributemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      667 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateobjectinfoextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      193 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateobjectinfoextendedmodelroutebutton.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      212 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateobjectinfoextendedmodelroutedata.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      295 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateobjectinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      373 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateobjectinfopagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      243 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateobjectmodelattribute.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      195 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateobjectpatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      478 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateobjecttypeobjectinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      380 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateobjecttypeobjectspagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      281 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateobjecttypetreemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      148 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatepagingmetadata.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      224 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatepagingmetadatacolumn.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      156 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatequicksearchresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      197 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatequicksearchresultobjectmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      539 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergaterouteinstanceextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      561 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergaterouteinstanceextendedmodelactivity.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      656 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatesearchobjectinfoattributemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      448 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatesearchobjectinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      375 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatesearchresultpagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      249 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergatesubstitutionmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      368 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergateuserspagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      146 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergroupaddproxymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      143 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usergroupaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      846 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userinfobysystemadminmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      227 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userinfobysystemadminmodeldepartment.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      198 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userinfobysystemadminmodelgroup.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     1128 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userinfoextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      282 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userinfoextensionmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      648 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      321 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usermailboxaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      145 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usermailboxaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      398 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usermailboxextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      323 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usermailboxpatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      151 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usermentiondeletemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      278 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usermodelextension.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      427 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usermodelnotification.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      431 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usernotificationinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      433 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usernotificationupdatemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      255 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userpagingbysystemadminmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      175 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userpasswordupdatemodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      652 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userpatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      149 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usersgroupaddproxymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      146 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/usersgroupaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      145 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userviewaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      144 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userviewaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      214 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userviewinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      246 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/userviewpagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      167 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/validationresponse.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      169 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/validationresponseitem.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      166 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/valuelistaddentrymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      219 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/valuelistaddmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      143 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/valuelistaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      171 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/valuelistentryaddproxymodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      148 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/valuelistentryaddresultmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      214 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/valuelistentryinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      252 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/valuelistentrypagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      146 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/valuelistentrypatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      295 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/valuelistextendedmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      267 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/valuelistinfomodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      247 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/valuelistpagingmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      169 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/valuelistpatchmodel.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      164 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/data/virtualfolderpath.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      359 2023-07-31 14:38:38.000000 lementpro-1.0.0/lementpro/logger.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     1821 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/sender.py
+drwxr-xr-x   0 mihailcupilnik   (501) staff       (20)        0 2023-07-31 15:58:55.439999 lementpro-1.0.0/lementpro/services/
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      490 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/services/__init__.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     4751 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/services/accounts.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)    82929 2023-07-31 15:48:35.000000 lementpro-1.0.0/lementpro/services/admin.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     4694 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/services/comments.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      444 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/services/companies.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      856 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/services/connections.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     1469 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/services/departments.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     2763 2023-07-31 14:44:47.000000 lementpro-1.0.0/lementpro/services/files.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     7037 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/services/folder.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      988 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/services/groups.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     1177 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/services/localization.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     4629 2023-07-31 15:48:34.000000 lementpro-1.0.0/lementpro/services/objects.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     2674 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/services/objecttypes.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      697 2023-07-31 15:48:34.000000 lementpro-1.0.0/lementpro/services/routes.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     1369 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/services/search.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      755 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/services/timezones.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     6902 2023-07-31 14:42:28.000000 lementpro-1.0.0/lementpro/services/users.py
+drwxr-xr-x   0 mihailcupilnik   (501) staff       (20)        0 2023-07-31 15:58:55.361109 lementpro-1.0.0/lementpro.egg-info/
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      617 2023-07-31 15:58:55.000000 lementpro-1.0.0/lementpro.egg-info/PKG-INFO
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)    16527 2023-07-31 15:58:55.000000 lementpro-1.0.0/lementpro.egg-info/SOURCES.txt
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)        1 2023-07-31 15:58:55.000000 lementpro-1.0.0/lementpro.egg-info/dependency_links.txt
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)       16 2023-07-31 15:58:55.000000 lementpro-1.0.0/lementpro.egg-info/requires.txt
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)       20 2023-07-31 15:58:55.000000 lementpro-1.0.0/lementpro.egg-info/top_level.txt
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)       38 2023-07-31 15:58:55.442419 lementpro-1.0.0/setup.cfg
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      834 2023-07-31 15:57:00.000000 lementpro-1.0.0/setup.py
+drwxr-xr-x   0 mihailcupilnik   (501) staff       (20)        0 2023-07-31 15:58:55.359025 lementpro-1.0.0/src/
+drwxr-xr-x   0 mihailcupilnik   (501) staff       (20)        0 2023-07-31 15:58:55.441057 lementpro-1.0.0/src/templates/
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)        0 2023-07-31 14:38:38.000000 lementpro-1.0.0/src/templates/__init__.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     1510 2023-07-31 14:38:38.000000 lementpro-1.0.0/src/templates/builders.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      341 2023-07-31 14:38:38.000000 lementpro-1.0.0/src/templates/logger.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     1802 2023-07-31 14:42:28.000000 lementpro-1.0.0/src/templates/sender.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      257 2023-07-31 14:38:38.000000 lementpro-1.0.0/src/templates/user.py
+drwxr-xr-x   0 mihailcupilnik   (501) staff       (20)        0 2023-07-31 15:58:55.359141 lementpro-1.0.0/tests/
+drwxr-xr-x   0 mihailcupilnik   (501) staff       (20)        0 2023-07-31 15:58:55.441829 lementpro-1.0.0/tests/test_unit/
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)        0 2023-07-31 14:38:38.000000 lementpro-1.0.0/tests/test_unit/__init__.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      772 2023-07-31 14:42:28.000000 lementpro-1.0.0/tests/test_unit/conftest.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      651 2023-07-31 14:42:28.000000 lementpro-1.0.0/tests/test_unit/test_accounts.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)      818 2023-07-31 14:42:28.000000 lementpro-1.0.0/tests/test_unit/test_companies.py
+-rw-r--r--   0 mihailcupilnik   (501) staff       (20)     7220 2023-07-31 14:42:28.000000 lementpro-1.0.0/tests/test_unit/test_users.py
```

### Comparing `lementpro-0.1.7/lementpro/builders.py` & `lementpro-1.0.0/lementpro/builders.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-import _io
-from dataclasses import dataclass
-from requests import Request
-
-
-@dataclass
-class Build:
-    url: str
-
-    def post(self, **kwargs):
-        prop = self.get_url(**kwargs)
-        return Request(method="post", url=self.url, json=prop)
-
-    def put(self, **kwargs):
-        prop = self.get_url(**kwargs)
-        return Request(method="put", url=self.url, json=prop)
-
-    def patch(self, **kwargs):
-        prop = self.get_url(**kwargs)
-        return Request(method="patch", url=self.url, json=prop)
-
-    def post_with_file(self, file: _io.BufferedReader, form_field_name: str, **kwargs):
-        file = {form_field_name: file}
-        return Request(method="post", url=self.url, data=kwargs, files=file)
-
-    def get(self, **kwargs):
-        prop = self.get_url(**kwargs)
-        return Request(method="get", url=self.url, json=prop)
-
-    def delete(self, **kwargs):
-        prop = self.get_url(**kwargs)
-        return Request(method="delete", url=self.url, json=prop)
-
-    def get_vars_from_path(self):
-        vars_ = list()
-        for part_way in self.url.split("/"):
-            if "{" in part_way:
-                vars_.append(part_way.replace("{", "").replace("}", ""))
-        return vars_
-
-    def get_url(self, **kwargs):
-        var_in_path = self.get_vars_from_path()
-        if var_in_path != list():
-            self.url = self.url.format(**kwargs)
-            for var in var_in_path:
-                kwargs.pop(var)
-        return kwargs
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+import _io
+from dataclasses import dataclass
+from requests import Request
+
+
+@dataclass
+class Build:
+    url: str
+
+    def post(self, **kwargs):
+        prop = self.get_url(**kwargs)
+        return Request(method="post", url=self.url, json=prop)
+
+    def put(self, **kwargs):
+        prop = self.get_url(**kwargs)
+        return Request(method="put", url=self.url, json=prop)
+
+    def patch(self, **kwargs):
+        prop = self.get_url(**kwargs)
+        return Request(method="patch", url=self.url, json=prop)
+
+    def post_with_file(self, file: _io.BufferedReader, form_field_name: str, **kwargs):
+        file = {form_field_name: file}
+        return Request(method="post", url=self.url, data=kwargs, files=file)
+
+    def get(self, **kwargs):
+        prop = self.get_url(**kwargs)
+        return Request(method="get", url=self.url, json=prop)
+
+    def delete(self, **kwargs):
+        prop = self.get_url(**kwargs)
+        return Request(method="delete", url=self.url, json=prop)
+
+    def get_vars_from_path(self):
+        vars_ = list()
+        for part_way in self.url.split("/"):
+            if "{" in part_way:
+                vars_.append(part_way.replace("{", "").replace("}", ""))
+        return vars_
+
+    def get_url(self, **kwargs):
+        var_in_path = self.get_vars_from_path()
+        if var_in_path != list():
+            self.url = self.url.format(**kwargs)
+            for var in var_in_path:
+                kwargs.pop(var)
+        return kwargs
```

### Comparing `lementpro-0.1.7/lementpro/data/__init__.py` & `lementpro-1.0.0/lementpro/data/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,337 +1,336 @@
-from .accesstokenmodel import *
-from .actionlogentryinfomodel import *
-from .attributeaddmodel import *
-from .attributeaddrelationmodel import *
-from .attributeaddresultmodel import *
-from .attributeextendedmodel import *
-from .attributeinfomodel import *
-from .attributepagingmodel import *
-from .attributepatchmodel import *
-from .attributepatchrelationmodel import *
-from .attributerelationinfomodel import *
-from .changepasswordmodel import *
-from .checkconnectionmodel import *
-from .checkconnectionresultmodel import *
-from .commentaddbyusermodel import *
-from .commentaddresultmodel import *
-from .commentemailextensionmodel import *
-from .commentextensionmodel import *
-from .commentpatchmodel import *
-from .companycontactdetailsmodel import *
-from .companycontactdetailspatchmodel import *
-from .companyextensionmodel import *
-from .companyinfodetailedmodel import *
-from .companyinfoextendedmodel import *
-from .companyinfomodel import *
-from .companylicensemodel import *
-from .companymailboxaddmodel import *
-from .companymailboxaddresultmodel import *
-from .companymailboxextendedmodel import *
-from .companymailboxpatchmodel import *
-from .companypasswordpolicymodel import *
-from .companypasswordpolicypatchmodel import *
-from .companypatchmodel import *
-from .departmentaddmodel import *
-from .departmentaddresultmodel import *
-from .departmentbosssetmodel import *
-from .departmentbossuserinfomodel import *
-from .departmentinfoextendedmodel import *
-from .departmentinfomodel import *
-from .departmentpagingmodel import *
-from .departmenttreemodel import *
-from .departmentupdatemodel import *
-from .emailaddressmodel import *
-from .errorresponse import *
-from .etaginfomodel import *
-from .fileinfomodel import *
-from .fileinfopagingmodel import *
-from .fileuploadresultmodel import *
-from .folderaddobjectstatefilter import *
-from .folderaddobjectstatusfilter import *
-from .folderaddobjectuserfilter import *
-from .folderaddresultmodel import *
-from .folderattributepredicatemodel import *
-from .folderfilterbyattributemodel import *
-from .foldergroupbyattributemodel import *
-from .foldergroupinfomodel import *
-from .folderinfomodel import *
-from .folderjoinbyattributemodel import *
-from .folderobjecttypeinfomodel import *
-from .folderobjecttypemodel import *
-from .folderorderbyattributemodel import *
-from .folderpagingmodel import *
-from .folderpatchgroupmodel import *
-from .folderpatchobjectstatefilter import *
-from .folderpatchobjectstatusfilter import *
-from .folderpatchobjectuserfilter import *
-from .folderpatchreset import *
-from .foldertemplateaddgroupmodel import *
-from .foldertemplateaddmodel import *
-from .foldertemplateextendedmodel import *
-from .foldertemplatepatchmodel import *
-from .foldertemplatesmenuproxymodel import *
-from .foldertemplatestreeproxymodel import *
-from .folderusertreecountmodel import *
-from .groupaddmodel import *
-from .groupaddresultmodel import *
-from .groupinfoextendedproxymodel import *
-from .groupinfomodel import *
-from .groupobjectexpirationaddmodel import *
-from .groupobjectexpirationaddresultmodel import *
-from .groupobjectexpirationinfomodel import *
-from .groupobjectexpirationpatchmodel import *
-from .groupobjecttypeinfomodel import *
-from .groupobjecttypepagingmodel import *
-from .groupobjecttypeupsertmodel import *
-from .grouppagingmodel import *
-from .groupupdateproxymodel import *
-from .integrationmailboxactionaddmodel import *
-from .integrationmailboxactionaddresultmodel import *
-from .integrationmailboxactionextendedmodel import *
-from .integrationmailboxactionpatchmodel import *
-from .integrationmailboxaddmodel import *
-from .integrationmailboxaddresultmodel import *
-from .integrationmailboxextendedmodel import *
-from .integrationmailboxinfomodel import *
-from .integrationmailboxpagingmodel import *
-from .integrationmailboxpatchmodel import *
-from .integrationmailboxrulemodel import *
-from .languagemodel import *
-from .mxgraphgetschemaresponse import *
-from .mxgraphschemaadddraftrequest import *
-from .mxgraphschemaaddrequest import *
-from .mxgraphschemaaddrequesttransitionactionmodel import *
-from .mxgraphschemaaddrequesttransitionconditionmodel import *
-from .mxgraphschemaaddrequesttransitionconditionpredicatemodel import *
-from .mxgraphschemaelementmodel import *
-from .mxgraphschemaline import *
-from .mxgraphschemapoint import *
-from .mxgraphschemarelatedproperty import *
-from .mxgraphschematransitionmodel import *
-from .mxgraphschemauserreference import *
-from .mxgraphschemavariablemodel import *
-from .objectaddresultmodel import *
-from .objectattributemodel import *
-from .objecttypeaddcountermodel import *
-from .objecttypeaddextensionmodel import *
-from .objecttypeaddmodel import *
-from .objecttypeaddresultmodel import *
-from .objecttypeattributeaddformulamodel import *
-from .objecttypeattributeaddproxymodel import *
-from .objecttypeattributeaddresultmodel import *
-from .objecttypeattributeaddsettingsmodel import *
-from .objecttypeattributeextendedmodel import *
-from .objecttypeattributeinfoattributemodel import *
-from .objecttypeattributeinfoattributerelationmodel import *
-from .objecttypeattributeinfoformulamodel import *
-from .objecttypeattributeinfomodel import *
-from .objecttypeattributeinfosettingsmodel import *
-from .objecttypeattributeinfovaluelistentrymodel import *
-from .objecttypeattributeinfovaluelistmodel import *
-from .objecttypeattributepagingmodel import *
-from .objecttypeattributepatchformulamodel import *
-from .objecttypeattributepatchmodel import *
-from .objecttypeattributepatchsettingsmodel import *
-from .objecttypebimaddproxymodel import *
-from .objecttypebimaddresultmodel import *
-from .objecttypebiminfoextendedmodel import *
-from .objecttypebimpatchmodel import *
-from .objecttypebreadcrumbmodel import *
-from .objecttypecheckpointaddproxymodel import *
-from .objecttypecheckpointaddresultmodel import *
-from .objecttypecheckpointinfoextendedmodel import *
-from .objecttypecheckpointinfopagingmodel import *
-from .objecttypecheckpointpagingmodel import *
-from .objecttypecheckpointpatchmodel import *
-from .objecttypeextensionmodel import *
-from .objecttypefileinfopagingmodel import *
-from .objecttypefilepagingmodel import *
-from .objecttypefileupsertmodel import *
-from .objecttypeinfodetailedbimmodel import *
-from .objecttypeinfodetailedcountermodel import *
-from .objecttypeinfodetailedfilemodel import *
-from .objecttypeinfodetailedmenumodel import *
-from .objecttypeinfodetailedmodel import *
-from .objecttypeinfoextendedmodel import *
-from .objecttypeinfopagingmodel import *
-from .objecttypemenuaddproxymodel import *
-from .objecttypemenuaddresultmodel import *
-from .objecttypemenuinfoextendedmodel import *
-from .objecttypemenuinfopagingmodel import *
-from .objecttypemenupatchmodel import *
-from .objecttypepagingmodel import *
-from .objecttypepatchcountermodel import *
-from .objecttypepatchextensionmodel import *
-from .objecttypepatchmodel import *
-from .objecttypetreenodeproxymodel import *
-from .objecttypeuisettingsproxyresponse import *
-from .objecttypeuisettingsproxyresponsecreatepage import *
-from .objecttypeuisettingsproxyresponsecreatepageattribute import *
-from .objecttypeuisettingsproxyresponsedetailedpage import *
-from .objecttypeuisettingsproxyresponsedetailedpageattribute import *
-from .objecttypeuisettingsproxyresponsedetailedpagetab import *
-from .objecttypeuisettingsproxyresponseeditpage import *
-from .objecttypeuisettingsproxyresponseeditpageattribute import *
-from .objecttypeuisettingsproxyresponselistview import *
-from .objecttypeuisettingsproxyresponselistviewattribute import *
-from .objecttypeuisettingsproxyresponsetableview import *
-from .objecttypeuisettingsproxyresponsetableviewattribute import *
-from .objectuserfavoritemodel import *
-from .objectuserreadmodel import *
-from .objectuserunreadmodel import *
-from .pagingmodel import *
-from .refreshtokenmodel import *
-from .relatedobjectmodel import *
-from .relationvalue import *
-from .restorepasswordmodel import *
-from .routeactivitybuttonrequest import *
-from .routeextendedresponseactivityelement import *
-from .routeextendedresponseactivityvariable import *
-from .routeextendedresponsereferenceobject import *
-from .routeextendedresponsereferenceobjectproperty import *
-from .routeinforesponse import *
-from .routeinforesponseschema import *
-from .routeinforesponseschemaversion import *
-from .routepagingresponse import *
-from .schemaaddresponse import *
-from .schemaextendedresponse import *
-from .schemainforesponse import *
-from .schemainforesponseversion import *
-from .schemapagingresponse import *
-from .serviceintegrationaddmodel import *
-from .serviceintegrationaddresultmodel import *
-from .serviceintegrationinfodetailedmodel import *
-from .serviceintegrationinfoextendedmodel import *
-from .serviceintegrationinfopagingmodel import *
-from .serviceintegrationinfoparammodel import *
-from .serviceintegrationobjecttypeaddmodel import *
-from .serviceintegrationobjecttypeaddresultmodel import *
-from .serviceintegrationobjecttypeinfoextendedmodel import *
-from .serviceintegrationobjecttypeinfopagingmodel import *
-from .serviceintegrationobjecttypepagingmodel import *
-from .serviceintegrationobjecttypepatchmodel import *
-from .serviceintegrationpagingmodel import *
-from .serviceintegrationparamaddmodel import *
-from .serviceintegrationparamaddresultmodel import *
-from .serviceintegrationparaminfoextendedmodel import *
-from .serviceintegrationparaminfopagingmodel import *
-from .serviceintegrationparampagingmodel import *
-from .serviceintegrationparampatchmodel import *
-from .serviceintegrationpatchmodel import *
-from .setobjecttyperequest import *
-from .setsortweightmodel import *
-from .signinproxymodel import *
-from .statisticspagingresponse import *
-from .statisticsrecordinforesponse import *
-from .timezoneinfomodel import *
-from .timezonepagingmodel import *
-from .tobccmodel import *
-from .toccmodel import *
-from .toemailsmodel import *
-from .user import *
-from .useraddmodel import *
-from .useraddresultmodel import *
-from .userassistantaddresultmodel import *
-from .userdepartmentmoveproxymodel import *
-from .userdetailedmodeldepartment import *
-from .userdetailedmodelgroup import *
-from .userdetailedmodelnotification import *
-from .userfolderaddmodel import *
-from .userfolderextendedmodel import *
-from .userfolderinfomodel import *
-from .userfolderpagingmodel import *
-from .userfolderpatchmodel import *
-from .userfoldertreemodel import *
-from .userfoldertreenodemodel import *
-from .usergateassistantaddmodel import *
-from .usergateassistantmodel import *
-from .usergateattributeinfomodel import *
-from .usergateattributeobjecttypetreenode import *
-from .usergatecategoryaddrequest import *
-from .usergatecategoryaddresponse import *
-from .usergatecategorypartialupdaterequest import *
-from .usergatecommentmessageinfofilemodel import *
-from .usergatecommentmessageinfomodel import *
-from .usergatecommentmessageinfousermodel import *
-from .usergatecommentmessagespagingmodel import *
-from .usergateexecuteobjectactionmodel import *
-from .usergateexecuteobjectactionresultmodel import *
-from .usergatefolderobjectinfoattributemodel import *
-from .usergatefolderobjectinfomodel import *
-from .usergatefolderobjectinfomodelcommentinfo import *
-from .usergatefolderobjectinfomodellastcomment import *
-from .usergatefolderobjectinfomodellastcommentuser import *
-from .usergatefolderobjectspagingmodel import *
-from .usergategetobjecttemplateresultmodel import *
-from .usergatementioninfocommentmodel import *
-from .usergatementioninfomodel import *
-from .usergatementioninfoobjectmodel import *
-from .usergatementionspagingmodel import *
-from .usergateobjectaddmodel import *
-from .usergateobjectinfoattributemodel import *
-from .usergateobjectinfochunkitemmodel import *
-from .usergateobjectinfochunkmodel import *
-from .usergateobjectinfoextendedattributemodel import *
-from .usergateobjectinfoextendedmodel import *
-from .usergateobjectinfoextendedmodelroutebutton import *
-from .usergateobjectinfoextendedmodelroutedata import *
-from .usergateobjectinfomodel import *
-from .usergateobjectinfopagingmodel import *
-from .usergateobjectmodelattribute import *
-from .usergateobjectpatchmodel import *
-from .usergateobjecttypeobjectinfomodel import *
-from .usergateobjecttypeobjectspagingmodel import *
-from .usergateobjecttypetreemodel import *
-from .usergatepagingmetadata import *
-from .usergatepagingmetadatacolumn import *
-from .usergatequicksearchresultmodel import *
-from .usergatequicksearchresultobjectmodel import *
-from .usergaterouteinstanceextendedmodel import *
-from .usergaterouteinstanceextendedmodelactivity import *
-from .usergatesearchobjectinfoattributemodel import *
-from .usergatesearchobjectinfomodel import *
-from .usergatesearchresultpagingmodel import *
-from .usergatesubstitutionmodel import *
-from .usergateuserspagingmodel import *
-from .usergroupaddproxymodel import *
-from .usergroupaddresultmodel import *
-from .userinfobysystemadminmodel import *
-from .userinfobysystemadminmodeldepartment import *
-from .userinfobysystemadminmodelgroup import *
-from .userinfoextendedmodel import *
-from .userinfoextensionmodel import *
-from .userinfomodel import *
-from .usermailboxaddmodel import *
-from .usermailboxaddresultmodel import *
-from .usermailboxextendedmodel import *
-from .usermailboxpatchmodel import *
-from .usermentiondeletemodel import *
-from .usermodelextension import *
-from .usermodelnotification import *
-from .usernotificationinfomodel import *
-from .usernotificationupdatemodel import *
-from .userpagingbysystemadminmodel import *
-from .userpasswordupdatemodel import *
-from .userpatchmodel import *
-from .usersgroupaddproxymodel import *
-from .usersgroupaddresultmodel import *
-from .userviewaddmodel import *
-from .userviewaddresultmodel import *
-from .userviewinfomodel import *
-from .userviewpagingmodel import *
-from .validationresponse import *
-from .validationresponseitem import *
-from .valuelistaddentrymodel import *
-from .valuelistaddmodel import *
-from .valuelistaddresultmodel import *
-from .valuelistentryaddproxymodel import *
-from .valuelistentryaddresultmodel import *
-from .valuelistentryinfomodel import *
-from .valuelistentrypagingmodel import *
-from .valuelistentrypatchmodel import *
-from .valuelistextendedmodel import *
-from .valuelistinfomodel import *
-from .valuelistpagingmodel import *
-from .valuelistpatchmodel import *
-from .virtualfolderpath import *
-
+from .accesstokenmodel import *
+from .actionlogentryinfomodel import *
+from .attributeaddmodel import *
+from .attributeaddrelationmodel import *
+from .attributeaddresultmodel import *
+from .attributeextendedmodel import *
+from .attributeinfomodel import *
+from .attributepagingmodel import *
+from .attributepatchmodel import *
+from .attributepatchrelationmodel import *
+from .attributerelationinfomodel import *
+from .changepasswordmodel import *
+from .checkconnectionmodel import *
+from .checkconnectionresultmodel import *
+from .commentaddbyusermodel import *
+from .commentaddresultmodel import *
+from .commentemailextensionmodel import *
+from .commentextensionmodel import *
+from .commentpatchmodel import *
+from .companycontactdetailsmodel import *
+from .companycontactdetailspatchmodel import *
+from .companyextensionmodel import *
+from .companyinfodetailedmodel import *
+from .companyinfoextendedmodel import *
+from .companyinfomodel import *
+from .companylicensemodel import *
+from .companymailboxaddmodel import *
+from .companymailboxaddresultmodel import *
+from .companymailboxextendedmodel import *
+from .companymailboxpatchmodel import *
+from .companypasswordpolicymodel import *
+from .companypasswordpolicypatchmodel import *
+from .companypatchmodel import *
+from .departmentaddmodel import *
+from .departmentaddresultmodel import *
+from .departmentbosssetmodel import *
+from .departmentbossuserinfomodel import *
+from .departmentinfoextendedmodel import *
+from .departmentinfomodel import *
+from .departmentpagingmodel import *
+from .departmenttreemodel import *
+from .departmentupdatemodel import *
+from .emailaddressmodel import *
+from .errorresponse import *
+from .etaginfomodel import *
+from .fileinfomodel import *
+from .fileinfopagingmodel import *
+from .fileuploadresultmodel import *
+from .folderaddobjectstatefilter import *
+from .folderaddobjectstatusfilter import *
+from .folderaddobjectuserfilter import *
+from .folderaddresultmodel import *
+from .folderattributepredicatemodel import *
+from .folderfilterbyattributemodel import *
+from .foldergroupbyattributemodel import *
+from .foldergroupinfomodel import *
+from .folderinfomodel import *
+from .folderjoinbyattributemodel import *
+from .folderobjecttypeinfomodel import *
+from .folderobjecttypemodel import *
+from .folderorderbyattributemodel import *
+from .folderpagingmodel import *
+from .folderpatchgroupmodel import *
+from .folderpatchobjectstatefilter import *
+from .folderpatchobjectstatusfilter import *
+from .folderpatchobjectuserfilter import *
+from .folderpatchreset import *
+from .foldertemplateaddgroupmodel import *
+from .foldertemplateaddmodel import *
+from .foldertemplateextendedmodel import *
+from .foldertemplatepatchmodel import *
+from .foldertemplatesmenuproxymodel import *
+from .foldertemplatestreeproxymodel import *
+from .folderusertreecountmodel import *
+from .groupaddmodel import *
+from .groupaddresultmodel import *
+from .groupinfoextendedproxymodel import *
+from .groupinfomodel import *
+from .groupobjectexpirationaddmodel import *
+from .groupobjectexpirationaddresultmodel import *
+from .groupobjectexpirationinfomodel import *
+from .groupobjectexpirationpatchmodel import *
+from .groupobjecttypeinfomodel import *
+from .groupobjecttypepagingmodel import *
+from .groupobjecttypeupsertmodel import *
+from .grouppagingmodel import *
+from .groupupdateproxymodel import *
+from .integrationmailboxactionaddmodel import *
+from .integrationmailboxactionaddresultmodel import *
+from .integrationmailboxactionextendedmodel import *
+from .integrationmailboxactionpatchmodel import *
+from .integrationmailboxaddmodel import *
+from .integrationmailboxaddresultmodel import *
+from .integrationmailboxextendedmodel import *
+from .integrationmailboxinfomodel import *
+from .integrationmailboxpagingmodel import *
+from .integrationmailboxpatchmodel import *
+from .integrationmailboxrulemodel import *
+from .languagemodel import *
+from .mxgraphgetschemaresponse import *
+from .mxgraphschemaadddraftrequest import *
+from .mxgraphschemaaddrequest import *
+from .mxgraphschemaaddrequesttransitionactionmodel import *
+from .mxgraphschemaaddrequesttransitionconditionmodel import *
+from .mxgraphschemaaddrequesttransitionconditionpredicatemodel import *
+from .mxgraphschemaelementmodel import *
+from .mxgraphschemaline import *
+from .mxgraphschemapoint import *
+from .mxgraphschemarelatedproperty import *
+from .mxgraphschematransitionmodel import *
+from .mxgraphschemauserreference import *
+from .mxgraphschemavariablemodel import *
+from .objectaddresultmodel import *
+from .objectattributemodel import *
+from .objecttypeaddcountermodel import *
+from .objecttypeaddextensionmodel import *
+from .objecttypeaddmodel import *
+from .objecttypeaddresultmodel import *
+from .objecttypeattributeaddformulamodel import *
+from .objecttypeattributeaddproxymodel import *
+from .objecttypeattributeaddresultmodel import *
+from .objecttypeattributeaddsettingsmodel import *
+from .objecttypeattributeextendedmodel import *
+from .objecttypeattributeinfoattributemodel import *
+from .objecttypeattributeinfoattributerelationmodel import *
+from .objecttypeattributeinfoformulamodel import *
+from .objecttypeattributeinfomodel import *
+from .objecttypeattributeinfosettingsmodel import *
+from .objecttypeattributeinfovaluelistentrymodel import *
+from .objecttypeattributeinfovaluelistmodel import *
+from .objecttypeattributepagingmodel import *
+from .objecttypeattributepatchformulamodel import *
+from .objecttypeattributepatchmodel import *
+from .objecttypeattributepatchsettingsmodel import *
+from .objecttypebimaddproxymodel import *
+from .objecttypebimaddresultmodel import *
+from .objecttypebiminfoextendedmodel import *
+from .objecttypebimpatchmodel import *
+from .objecttypebreadcrumbmodel import *
+from .objecttypecheckpointaddproxymodel import *
+from .objecttypecheckpointaddresultmodel import *
+from .objecttypecheckpointinfoextendedmodel import *
+from .objecttypecheckpointinfopagingmodel import *
+from .objecttypecheckpointpagingmodel import *
+from .objecttypecheckpointpatchmodel import *
+from .objecttypeextensionmodel import *
+from .objecttypefileinfopagingmodel import *
+from .objecttypefilepagingmodel import *
+from .objecttypefileupsertmodel import *
+from .objecttypeinfodetailedbimmodel import *
+from .objecttypeinfodetailedcountermodel import *
+from .objecttypeinfodetailedfilemodel import *
+from .objecttypeinfodetailedmenumodel import *
+from .objecttypeinfodetailedmodel import *
+from .objecttypeinfoextendedmodel import *
+from .objecttypeinfopagingmodel import *
+from .objecttypemenuaddproxymodel import *
+from .objecttypemenuaddresultmodel import *
+from .objecttypemenuinfoextendedmodel import *
+from .objecttypemenuinfopagingmodel import *
+from .objecttypemenupatchmodel import *
+from .objecttypepagingmodel import *
+from .objecttypepatchcountermodel import *
+from .objecttypepatchextensionmodel import *
+from .objecttypepatchmodel import *
+from .objecttypetreenodeproxymodel import *
+from .objecttypeuisettingsproxyresponse import *
+from .objecttypeuisettingsproxyresponsecreatepage import *
+from .objecttypeuisettingsproxyresponsecreatepageattribute import *
+from .objecttypeuisettingsproxyresponsedetailedpage import *
+from .objecttypeuisettingsproxyresponsedetailedpageattribute import *
+from .objecttypeuisettingsproxyresponsedetailedpagetab import *
+from .objecttypeuisettingsproxyresponseeditpage import *
+from .objecttypeuisettingsproxyresponseeditpageattribute import *
+from .objecttypeuisettingsproxyresponselistview import *
+from .objecttypeuisettingsproxyresponselistviewattribute import *
+from .objecttypeuisettingsproxyresponsetableview import *
+from .objecttypeuisettingsproxyresponsetableviewattribute import *
+from .objectuserfavoritemodel import *
+from .objectuserreadmodel import *
+from .objectuserunreadmodel import *
+from .pagingmodel import *
+from .refreshtokenmodel import *
+from .relatedobjectmodel import *
+from .relationvalue import *
+from .restorepasswordmodel import *
+from .routeactivitybuttonrequest import *
+from .routeextendedresponseactivityelement import *
+from .routeextendedresponseactivityvariable import *
+from .routeextendedresponsereferenceobject import *
+from .routeextendedresponsereferenceobjectproperty import *
+from .routeinforesponse import *
+from .routeinforesponseschema import *
+from .routeinforesponseschemaversion import *
+from .routepagingresponse import *
+from .schemaaddresponse import *
+from .schemaextendedresponse import *
+from .schemainforesponse import *
+from .schemainforesponseversion import *
+from .schemapagingresponse import *
+from .serviceintegrationaddmodel import *
+from .serviceintegrationaddresultmodel import *
+from .serviceintegrationinfodetailedmodel import *
+from .serviceintegrationinfoextendedmodel import *
+from .serviceintegrationinfopagingmodel import *
+from .serviceintegrationinfoparammodel import *
+from .serviceintegrationobjecttypeaddmodel import *
+from .serviceintegrationobjecttypeaddresultmodel import *
+from .serviceintegrationobjecttypeinfoextendedmodel import *
+from .serviceintegrationobjecttypeinfopagingmodel import *
+from .serviceintegrationobjecttypepagingmodel import *
+from .serviceintegrationobjecttypepatchmodel import *
+from .serviceintegrationpagingmodel import *
+from .serviceintegrationparamaddmodel import *
+from .serviceintegrationparamaddresultmodel import *
+from .serviceintegrationparaminfoextendedmodel import *
+from .serviceintegrationparaminfopagingmodel import *
+from .serviceintegrationparampagingmodel import *
+from .serviceintegrationparampatchmodel import *
+from .serviceintegrationpatchmodel import *
+from .setobjecttyperequest import *
+from .setsortweightmodel import *
+from .signinproxymodel import *
+from .statisticspagingresponse import *
+from .statisticsrecordinforesponse import *
+from .timezoneinfomodel import *
+from .timezonepagingmodel import *
+from .tobccmodel import *
+from .toccmodel import *
+from .toemailsmodel import *
+from .user import *
+from .useraddmodel import *
+from .useraddresultmodel import *
+from .userassistantaddresultmodel import *
+from .userdepartmentmoveproxymodel import *
+from .userdetailedmodeldepartment import *
+from .userdetailedmodelgroup import *
+from .userdetailedmodelnotification import *
+from .userfolderaddmodel import *
+from .userfolderextendedmodel import *
+from .userfolderinfomodel import *
+from .userfolderpagingmodel import *
+from .userfolderpatchmodel import *
+from .userfoldertreemodel import *
+from .userfoldertreenodemodel import *
+from .usergateassistantaddmodel import *
+from .usergateassistantmodel import *
+from .usergateattributeinfomodel import *
+from .usergateattributeobjecttypetreenode import *
+from .usergatecategoryaddrequest import *
+from .usergatecategoryaddresponse import *
+from .usergatecategorypartialupdaterequest import *
+from .usergatecommentmessageinfofilemodel import *
+from .usergatecommentmessageinfomodel import *
+from .usergatecommentmessageinfousermodel import *
+from .usergatecommentmessagespagingmodel import *
+from .usergateexecuteobjectactionmodel import *
+from .usergateexecuteobjectactionresultmodel import *
+from .usergatefolderobjectinfoattributemodel import *
+from .usergatefolderobjectinfomodel import *
+from .usergatefolderobjectinfomodelcommentinfo import *
+from .usergatefolderobjectinfomodellastcomment import *
+from .usergatefolderobjectinfomodellastcommentuser import *
+from .usergatefolderobjectspagingmodel import *
+from .usergategetobjecttemplateresultmodel import *
+from .usergatementioninfocommentmodel import *
+from .usergatementioninfomodel import *
+from .usergatementioninfoobjectmodel import *
+from .usergatementionspagingmodel import *
+from .usergateobjectaddmodel import *
+from .usergateobjectinfoattributemodel import *
+from .usergateobjectinfochunkitemmodel import *
+from .usergateobjectinfochunkmodel import *
+from .usergateobjectinfoextendedattributemodel import *
+from .usergateobjectinfoextendedmodel import *
+from .usergateobjectinfoextendedmodelroutebutton import *
+from .usergateobjectinfoextendedmodelroutedata import *
+from .usergateobjectinfomodel import *
+from .usergateobjectinfopagingmodel import *
+from .usergateobjectmodelattribute import *
+from .usergateobjectpatchmodel import *
+from .usergateobjecttypeobjectinfomodel import *
+from .usergateobjecttypeobjectspagingmodel import *
+from .usergateobjecttypetreemodel import *
+from .usergatepagingmetadata import *
+from .usergatepagingmetadatacolumn import *
+from .usergatequicksearchresultmodel import *
+from .usergatequicksearchresultobjectmodel import *
+from .usergaterouteinstanceextendedmodel import *
+from .usergaterouteinstanceextendedmodelactivity import *
+from .usergatesearchobjectinfoattributemodel import *
+from .usergatesearchobjectinfomodel import *
+from .usergatesearchresultpagingmodel import *
+from .usergatesubstitutionmodel import *
+from .usergateuserspagingmodel import *
+from .usergroupaddproxymodel import *
+from .usergroupaddresultmodel import *
+from .userinfobysystemadminmodel import *
+from .userinfobysystemadminmodeldepartment import *
+from .userinfobysystemadminmodelgroup import *
+from .userinfoextendedmodel import *
+from .userinfoextensionmodel import *
+from .userinfomodel import *
+from .usermailboxaddmodel import *
+from .usermailboxaddresultmodel import *
+from .usermailboxextendedmodel import *
+from .usermailboxpatchmodel import *
+from .usermentiondeletemodel import *
+from .usermodelextension import *
+from .usermodelnotification import *
+from .usernotificationinfomodel import *
+from .usernotificationupdatemodel import *
+from .userpagingbysystemadminmodel import *
+from .userpasswordupdatemodel import *
+from .userpatchmodel import *
+from .usersgroupaddproxymodel import *
+from .usersgroupaddresultmodel import *
+from .userviewaddmodel import *
+from .userviewaddresultmodel import *
+from .userviewinfomodel import *
+from .userviewpagingmodel import *
+from .validationresponse import *
+from .validationresponseitem import *
+from .valuelistaddentrymodel import *
+from .valuelistaddmodel import *
+from .valuelistaddresultmodel import *
+from .valuelistentryaddproxymodel import *
+from .valuelistentryaddresultmodel import *
+from .valuelistentryinfomodel import *
+from .valuelistentrypagingmodel import *
+from .valuelistentrypatchmodel import *
+from .valuelistextendedmodel import *
+from .valuelistinfomodel import *
+from .valuelistpagingmodel import *
+from .valuelistpatchmodel import *
+from .virtualfolderpath import *
```

### Comparing `lementpro-0.1.7/lementpro/data/attributeaddmodel.py` & `lementpro-1.0.0/lementpro/data/attributeaddmodel.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.attributeaddrelationmodel import AttributeAddRelationModel
-@dataclass
-class AttributeAddModel:
-    name: str = None
-    description: str = None
-    knownId: str = None
-    units: str = None
-    attributeTypeId: str = None
-    valueTypeId: str = None
-    isFilterable: bool = None
-    isGroupable: bool = None
-    valueListId: int = None
-    relation: AttributeAddRelationModel = None
-    precision: int = None
-    widthInChars: int = None
-    notifyAboutChanges: bool = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.attributeaddrelationmodel import AttributeAddRelationModel
+
+
+@dataclass
+class AttributeAddModel:
+    name: str = None
+    description: str = None
+    knownId: str = None
+    units: str = None
+    attributeTypeId: str = None
+    valueTypeId: str = None
+    isFilterable: bool = None
+    isGroupable: bool = None
+    valueListId: int = None
+    relation: AttributeAddRelationModel = None
+    precision: int = None
+    widthInChars: int = None
+    notifyAboutChanges: bool = None
```

### Comparing `lementpro-0.1.7/lementpro/data/attributeaddrelationmodel.py` & `lementpro-1.0.0/lementpro/data/attributeaddrelationmodel.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-@dataclass
-class AttributeAddRelationModel:
-    multiplicity: int = None
-    relationTypeId: str = None
-    relatedTypeId: str = None
-    dependentAttributeId: int = None
-    notifyAboutExpiration: bool = None
-    notifyAboutChanges: bool = None
-    grantReadRights: bool = None
-    grantEditRights: bool = None
-    objectTypeKnownId: str = None
-    objectTypeId: int = None
-    inheritAccessRights: bool = None
-    isNotSharable: bool = None
-    isAnySubTypeAvailable: bool = None
-    bimStateGroupId: int = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+
+
+@dataclass
+class AttributeAddRelationModel:
+    multiplicity: int = None
+    relationTypeId: str = None
+    relatedTypeId: str = None
+    dependentAttributeId: int = None
+    notifyAboutExpiration: bool = None
+    notifyAboutChanges: bool = None
+    grantReadRights: bool = None
+    grantEditRights: bool = None
+    objectTypeKnownId: str = None
+    objectTypeId: int = None
+    inheritAccessRights: bool = None
+    isNotSharable: bool = None
+    isAnySubTypeAvailable: bool = None
+    bimStateGroupId: int = None
```

### Comparing `lementpro-0.1.7/lementpro/data/attributeextendedmodel.py` & `lementpro-1.0.0/lementpro/data/attributeinfomodel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.attributerelationinfomodel import AttributeRelationInfoModel
-@dataclass
-class AttributeExtendedModel:
-    id: int = None
-    knownId: str = None
-    name: str = None
-    description: str = None
-    units: str = None
-    attributeTypeId: str = None
-    valueTypeId: str = None
-    valueListId: int = None
-    isFilterable: bool = None
-    isGroupable: bool = None
-    isInternal: bool = None
-    precision: int = None
-    widthInChars: int = None
-    notifyAboutChanges: bool = None
-    nullValueHint: str = None
-    relation: AttributeRelationInfoModel = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+
+
+@dataclass
+class AttributeInfoModel:
+    id: int = None
+    knownId: str = None
+    name: str = None
+    description: str = None
+    units: str = None
+    attributeTypeId: str = None
+    valueTypeId: str = None
+    valueListId: int = None
+    isFilterable: bool = None
+    isGroupable: bool = None
+    isInternal: bool = None
+    precision: int = None
+    widthInChars: int = None
+    notifyAboutChanges: bool = None
+    nullValueHint: str = None
```

### Comparing `lementpro-0.1.7/lementpro/data/attributeinfomodel.py` & `lementpro-1.0.0/lementpro/data/usergateobjectinfoextendedattributemodel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-@dataclass
-class AttributeInfoModel:
-    id: int = None
-    knownId: str = None
-    name: str = None
-    description: str = None
-    units: str = None
-    attributeTypeId: str = None
-    valueTypeId: str = None
-    valueListId: int = None
-    isFilterable: bool = None
-    isGroupable: bool = None
-    isInternal: bool = None
-    precision: int = None
-    widthInChars: int = None
-    notifyAboutChanges: bool = None
-    nullValueHint: str = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.objecttypeattributeinfovaluelistmodel import ObjectTypeAttributeInfoValueListModel
+from lementpro.data.relationvalue import RelationValue
+
+
+@dataclass
+class UserGateObjectInfoExtendedAttributeModel:
+    id: int = None
+    knownId: str = None
+    name: str = None
+    isSystem: bool = None
+    value: str = None
+    valueList: ObjectTypeAttributeInfoValueListModel = None
+    relationValue: RelationValue = None
+    attributeTypeId: str = None
+    valueTypeId: str = None
+    relationTypeId: str = None
+    isRequired: bool = None
+    isEditable: bool = None
+    hideIfNull: bool = None
+    description: str = None
+    showOnGeneralPage: bool = None
+    showContentOnSeparatePage: bool = None
```

### Comparing `lementpro-0.1.7/lementpro/data/attributepatchmodel.py` & `lementpro-1.0.0/lementpro/data/attributepatchmodel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.attributepatchrelationmodel import AttributePatchRelationModel
-@dataclass
-class AttributePatchModel:
-    name: str = None
-    description: str = None
-    units: str = None
-    attributeTypeId: str = None
-    valueTypeId: str = None
-    isFilterable: bool = None
-    isGroupable: bool = None
-    valueListId: int = None
-    relation: AttributePatchRelationModel = None
-    precision: int = None
-    widthInChars: int = None
-    notifyAboutChanges: bool = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.attributepatchrelationmodel import AttributePatchRelationModel
+
+
+@dataclass
+class AttributePatchModel:
+    name: str = None
+    description: str = None
+    units: str = None
+    attributeTypeId: str = None
+    valueTypeId: str = None
+    isFilterable: bool = None
+    isGroupable: bool = None
+    valueListId: int = None
+    relation: AttributePatchRelationModel = None
+    precision: int = None
+    widthInChars: int = None
+    notifyAboutChanges: bool = None
```

### Comparing `lementpro-0.1.7/lementpro/data/attributepatchrelationmodel.py` & `lementpro-1.0.0/lementpro/data/attributepatchrelationmodel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-@dataclass
-class AttributePatchRelationModel:
-    multiplicity: int = None
-    relationTypeId: str = None
-    relatedTypeId: str = None
-    dependentAttributeId: int = None
-    notifyAboutExpiration: bool = None
-    notifyAboutChanges: bool = None
-    grantReadRights: bool = None
-    grantEditRights: bool = None
-    objectTypeKnownId: str = None
-    objectTypeId: int = None
-    inheritAccessRights: bool = None
-    isNotSharable: bool = None
-    isAnySubTypeAvailable: bool = None
-    detachRelatedOnArchiving: bool = None
-    detachRelatedOnDeleting: bool = None
-    bimStateGroupId: int = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+
+
+@dataclass
+class AttributePatchRelationModel:
+    multiplicity: int = None
+    relationTypeId: str = None
+    relatedTypeId: str = None
+    dependentAttributeId: int = None
+    notifyAboutExpiration: bool = None
+    notifyAboutChanges: bool = None
+    grantReadRights: bool = None
+    grantEditRights: bool = None
+    objectTypeKnownId: str = None
+    objectTypeId: int = None
+    inheritAccessRights: bool = None
+    isNotSharable: bool = None
+    isAnySubTypeAvailable: bool = None
+    detachRelatedOnArchiving: bool = None
+    detachRelatedOnDeleting: bool = None
+    bimStateGroupId: int = None
```

### Comparing `lementpro-0.1.7/lementpro/data/attributerelationinfomodel.py` & `lementpro-1.0.0/lementpro/data/attributerelationinfomodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-@dataclass
-class AttributeRelationInfoModel:
-    multiplicity: int = None
-    relationTypeId: str = None
-    relatedTypeId: str = None
-    notifyAboutExpiration: bool = None
-    notifyAboutChanges: bool = None
-    grantReadRights: bool = None
-    grantEditRights: bool = None
-    objectTypeKnownId: str = None
-    objectTypeId: int = None
-    inheritAccessRights: bool = None
-    isNotSharable: bool = None
-    isAnySubTypeAvailable: bool = None
-    dependentAttributeId: int = None
-    detachRelatedOnArchiving: bool = None
-    detachRelatedOnDeleting: bool = None
-    bimStateGroupId: int = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+
+
+@dataclass
+class AttributeRelationInfoModel:
+    multiplicity: int = None
+    relationTypeId: str = None
+    relatedTypeId: str = None
+    notifyAboutExpiration: bool = None
+    notifyAboutChanges: bool = None
+    grantReadRights: bool = None
+    grantEditRights: bool = None
+    objectTypeKnownId: str = None
+    objectTypeId: int = None
+    inheritAccessRights: bool = None
+    isNotSharable: bool = None
+    isAnySubTypeAvailable: bool = None
+    dependentAttributeId: int = None
+    detachRelatedOnArchiving: bool = None
+    detachRelatedOnDeleting: bool = None
+    bimStateGroupId: int = None
```

### Comparing `lementpro-0.1.7/lementpro/data/companyinfoextendedmodel.py` & `lementpro-1.0.0/lementpro/data/companyinfoextendedmodel.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.companycontactdetailsmodel import CompanyContactDetailsModel
-from lementpro.data.companypasswordpolicymodel import CompanyPasswordPolicyModel
-from lementpro.data.companylicensemodel import CompanyLicenseModel
-from lementpro.data.companyextensionmodel import CompanyExtensionModel
-from lementpro.data.actionlogentryinfomodel import ActionLogEntryInfoModel
-from lementpro.data.companyinfodetailedmodel import CompanyInfoDetailedModel
-@dataclass
-class CompanyInfoExtendedModel:
-    id: int = None
-    name: str = None
-    description: str = None
-    maxUploadFileSize: int = None
-    isReadOnly: bool = None
-    isDisabled: bool = None
-    timeZone: str = None
-    isSchemaReadonly: bool = None
-    contactDetails: CompanyContactDetailsModel = None
-    passwordPolicy: CompanyPasswordPolicyModel = None
-    license: CompanyLicenseModel = None
-    dateCreated: str = None
-    isSystem: bool = None
-    extension: CompanyExtensionModel = None
-    entryInfo: ActionLogEntryInfoModel = None
-    detailed: CompanyInfoDetailedModel = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.companycontactdetailsmodel import CompanyContactDetailsModel
+from lementpro.data.companypasswordpolicymodel import CompanyPasswordPolicyModel
+from lementpro.data.companylicensemodel import CompanyLicenseModel
+from lementpro.data.companyextensionmodel import CompanyExtensionModel
+from lementpro.data.actionlogentryinfomodel import ActionLogEntryInfoModel
+from lementpro.data.companyinfodetailedmodel import CompanyInfoDetailedModel
+
+
+@dataclass
+class CompanyInfoExtendedModel:
+    id: int = None
+    name: str = None
+    description: str = None
+    maxUploadFileSize: int = None
+    isReadOnly: bool = None
+    isDisabled: bool = None
+    timeZone: str = None
+    isSchemaReadonly: bool = None
+    contactDetails: CompanyContactDetailsModel = None
+    passwordPolicy: CompanyPasswordPolicyModel = None
+    license: CompanyLicenseModel = None
+    dateCreated: str = None
+    isSystem: bool = None
+    extension: CompanyExtensionModel = None
+    entryInfo: ActionLogEntryInfoModel = None
+    detailed: CompanyInfoDetailedModel = None
```

### Comparing `lementpro-0.1.7/lementpro/data/companypatchmodel.py` & `lementpro-1.0.0/lementpro/data/companypatchmodel.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.companycontactdetailspatchmodel import CompanyContactDetailsPatchModel
-from lementpro.data.companypasswordpolicypatchmodel import CompanyPasswordPolicyPatchModel
-from lementpro.data.companyextensionmodel import CompanyExtensionModel
-@dataclass
-class CompanyPatchModel:
-    name: str = None
-    description: str = None
-    maxUploadFileSize: int = None
-    isReadOnly: bool = None
-    isDisabled: bool = None
-    isSchemaReadonly: bool = None
-    timeZone: str = None
-    contactDetails: CompanyContactDetailsPatchModel = None
-    passwordPolicy: CompanyPasswordPolicyPatchModel = None
-    extension: CompanyExtensionModel = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.companycontactdetailspatchmodel import CompanyContactDetailsPatchModel
+from lementpro.data.companypasswordpolicypatchmodel import CompanyPasswordPolicyPatchModel
+from lementpro.data.companyextensionmodel import CompanyExtensionModel
+
+
+@dataclass
+class CompanyPatchModel:
+    name: str = None
+    description: str = None
+    maxUploadFileSize: int = None
+    isReadOnly: bool = None
+    isDisabled: bool = None
+    isSchemaReadonly: bool = None
+    timeZone: str = None
+    contactDetails: CompanyContactDetailsPatchModel = None
+    passwordPolicy: CompanyPasswordPolicyPatchModel = None
+    extension: CompanyExtensionModel = None
```

### Comparing `lementpro-0.1.7/lementpro/data/departmentbossuserinfomodel.py` & `lementpro-1.0.0/lementpro/data/departmentbossuserinfomodel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.userinfoextensionmodel import UserInfoExtensionModel
-@dataclass
-class DepartmentBossUserInfoModel:
-    id: int = None
-    userName: str = None
-    companyId: int = None
-    email: str = None
-    firstName: str = None
-    middleName: str = None
-    lastName: str = None
-    phoneNumber: str = None
-    preferredLocale: str = None
-    isDismissed: bool = None
-    isDisabled: bool = None
-    isSystem: bool = None
-    position: str = None
-    role: str = None
-    departmentId: int = None
-    displayName: str = None
-    extension: UserInfoExtensionModel = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.userinfoextensionmodel import UserInfoExtensionModel
+
+
+@dataclass
+class DepartmentBossUserInfoModel:
+    id: int = None
+    userName: str = None
+    companyId: int = None
+    email: str = None
+    firstName: str = None
+    middleName: str = None
+    lastName: str = None
+    phoneNumber: str = None
+    preferredLocale: str = None
+    isDismissed: bool = None
+    isDisabled: bool = None
+    isSystem: bool = None
+    position: str = None
+    role: str = None
+    departmentId: int = None
+    displayName: str = None
+    extension: UserInfoExtensionModel = None
```

### Comparing `lementpro-0.1.7/lementpro/data/departmentinfoextendedmodel.py` & `lementpro-1.0.0/lementpro/data/departmentinfoextendedmodel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.departmentbossuserinfomodel import DepartmentBossUserInfoModel
-from lementpro.data.actionlogentryinfomodel import ActionLogEntryInfoModel
-@dataclass
-class DepartmentInfoExtendedModel:
-    id: int = None
-    companyId: int = None
-    parentId: int = None
-    name: str = None
-    description: str = None
-    code: str = None
-    sortWeight: int = None
-    canHasSubDepartment: bool = None
-    isHidden: bool = None
-    isSystem: bool = None
-    boss: DepartmentBossUserInfoModel = None
-    dateCreated: str = None
-    entryInfo: ActionLogEntryInfoModel = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.departmentbossuserinfomodel import DepartmentBossUserInfoModel
+from lementpro.data.actionlogentryinfomodel import ActionLogEntryInfoModel
+
+
+@dataclass
+class DepartmentInfoExtendedModel:
+    id: int = None
+    companyId: int = None
+    parentId: int = None
+    name: str = None
+    description: str = None
+    code: str = None
+    sortWeight: int = None
+    canHasSubDepartment: bool = None
+    isHidden: bool = None
+    isSystem: bool = None
+    boss: DepartmentBossUserInfoModel = None
+    dateCreated: str = None
+    entryInfo: ActionLogEntryInfoModel = None
```

### Comparing `lementpro-0.1.7/lementpro/data/foldertemplateaddmodel.py` & `lementpro-1.0.0/lementpro/data/userfolderaddmodel.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.folderaddobjectstatusfilter import FolderAddObjectStatusFilter
-from lementpro.data.folderaddobjectstatefilter import FolderAddObjectStateFilter
-from lementpro.data.folderaddobjectuserfilter import FolderAddObjectUserFilter
-from lementpro.data.folderorderbyattributemodel import FolderOrderByAttributeModel
-from lementpro.data.folderjoinbyattributemodel import FolderJoinByAttributeModel
-@dataclass
-class FolderTemplateAddModel:
-    name: str = None
-    description: str = None
-    parentId: int = None
-    menuObjectTypeId: int = None
-    exportTemplateFileId: int = None
-    isAbstract: bool = None
-    objectTypes: list = None
-    objectStatus: FolderAddObjectStatusFilter = None
-    objectState: FolderAddObjectStateFilter = None
-    objectUser: FolderAddObjectUserFilter = None
-    orderByAttribute: FolderOrderByAttributeModel = None
-    joinByAttribute: FolderJoinByAttributeModel = None
-    groupByAttributes: list = None
-    filterByAttributes: list = None
-    userGroups: list = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.folderaddobjectstatusfilter import FolderAddObjectStatusFilter
+from lementpro.data.folderaddobjectstatefilter import FolderAddObjectStateFilter
+from lementpro.data.folderaddobjectuserfilter import FolderAddObjectUserFilter
+from lementpro.data.folderorderbyattributemodel import FolderOrderByAttributeModel
+from lementpro.data.folderjoinbyattributemodel import FolderJoinByAttributeModel
+
+
+@dataclass
+class UserFolderAddModel:
+    name: str = None
+    description: str = None
+    parentId: int = None
+    menuObjectTypeId: int = None
+    exportTemplateFileId: int = None
+    isAbstract: bool = None
+    objectTypes: list = None
+    objectStatus: FolderAddObjectStatusFilter = None
+    objectState: FolderAddObjectStateFilter = None
+    objectUser: FolderAddObjectUserFilter = None
+    orderByAttribute: FolderOrderByAttributeModel = None
+    joinByAttribute: FolderJoinByAttributeModel = None
+    groupByAttributes: list = None
+    filterByAttributes: list = None
+    viewTypeId: str = None
+    countObjects: bool = None
```

### Comparing `lementpro-0.1.7/lementpro/data/foldertemplateextendedmodel.py` & `lementpro-1.0.0/lementpro/data/foldertemplateextendedmodel.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.folderaddobjectstatusfilter import FolderAddObjectStatusFilter
-from lementpro.data.folderaddobjectstatefilter import FolderAddObjectStateFilter
-from lementpro.data.folderaddobjectuserfilter import FolderAddObjectUserFilter
-from lementpro.data.folderorderbyattributemodel import FolderOrderByAttributeModel
-from lementpro.data.folderjoinbyattributemodel import FolderJoinByAttributeModel
-@dataclass
-class FolderTemplateExtendedModel:
-    id: int = None
-    parentId: int = None
-    companyId: int = None
-    name: str = None
-    description: str = None
-    menuObjectTypeId: int = None
-    isSystem: bool = None
-    isTemplate: bool = None
-    isAbstract: bool = None
-    sortWeight: int = None
-    exportTemplateFileId: int = None
-    objectStatus: FolderAddObjectStatusFilter = None
-    objectState: FolderAddObjectStateFilter = None
-    objectUser: FolderAddObjectUserFilter = None
-    orderByAttribute: FolderOrderByAttributeModel = None
-    joinByAttribute: FolderJoinByAttributeModel = None
-    groupByAttributes: list = None
-    filterByAttributes: list = None
-    objectTypes: list = None
-    userGroups: list = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.folderaddobjectstatusfilter import FolderAddObjectStatusFilter
+from lementpro.data.folderaddobjectstatefilter import FolderAddObjectStateFilter
+from lementpro.data.folderaddobjectuserfilter import FolderAddObjectUserFilter
+from lementpro.data.folderorderbyattributemodel import FolderOrderByAttributeModel
+from lementpro.data.folderjoinbyattributemodel import FolderJoinByAttributeModel
+
+
+@dataclass
+class FolderTemplateExtendedModel:
+    id: int = None
+    parentId: int = None
+    companyId: int = None
+    name: str = None
+    description: str = None
+    menuObjectTypeId: int = None
+    isSystem: bool = None
+    isTemplate: bool = None
+    isAbstract: bool = None
+    sortWeight: int = None
+    exportTemplateFileId: int = None
+    objectStatus: FolderAddObjectStatusFilter = None
+    objectState: FolderAddObjectStateFilter = None
+    objectUser: FolderAddObjectUserFilter = None
+    orderByAttribute: FolderOrderByAttributeModel = None
+    joinByAttribute: FolderJoinByAttributeModel = None
+    groupByAttributes: list = None
+    filterByAttributes: list = None
+    objectTypes: list = None
+    userGroups: list = None
```

### Comparing `lementpro-0.1.7/lementpro/data/foldertemplatepatchmodel.py` & `lementpro-1.0.0/lementpro/data/foldertemplatepatchmodel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.folderpatchobjectstatusfilter import FolderPatchObjectStatusFilter
-from lementpro.data.folderpatchobjectstatefilter import FolderPatchObjectStateFilter
-from lementpro.data.folderpatchobjectuserfilter import FolderPatchObjectUserFilter
-from lementpro.data.folderorderbyattributemodel import FolderOrderByAttributeModel
-from lementpro.data.folderjoinbyattributemodel import FolderJoinByAttributeModel
-from lementpro.data.folderpatchreset import FolderPatchReset
-@dataclass
-class FolderTemplatePatchModel:
-    name: str = None
-    description: str = None
-    objectTypes: list = None
-    exportTemplateFileId: int = None
-    objectStatus: FolderPatchObjectStatusFilter = None
-    objectState: FolderPatchObjectStateFilter = None
-    objectUser: FolderPatchObjectUserFilter = None
-    orderByAttribute: FolderOrderByAttributeModel = None
-    joinByAttribute: FolderJoinByAttributeModel = None
-    groupByAttributes: list = None
-    filterByAttributes: list = None
-    isAbstract: bool = None
-    reset: FolderPatchReset = None
-    userGroups: list = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.folderpatchobjectstatusfilter import FolderPatchObjectStatusFilter
+from lementpro.data.folderpatchobjectstatefilter import FolderPatchObjectStateFilter
+from lementpro.data.folderpatchobjectuserfilter import FolderPatchObjectUserFilter
+from lementpro.data.folderorderbyattributemodel import FolderOrderByAttributeModel
+from lementpro.data.folderjoinbyattributemodel import FolderJoinByAttributeModel
+from lementpro.data.folderpatchreset import FolderPatchReset
+
+
+@dataclass
+class FolderTemplatePatchModel:
+    name: str = None
+    description: str = None
+    objectTypes: list = None
+    exportTemplateFileId: int = None
+    objectStatus: FolderPatchObjectStatusFilter = None
+    objectState: FolderPatchObjectStateFilter = None
+    objectUser: FolderPatchObjectUserFilter = None
+    orderByAttribute: FolderOrderByAttributeModel = None
+    joinByAttribute: FolderJoinByAttributeModel = None
+    groupByAttributes: list = None
+    filterByAttributes: list = None
+    isAbstract: bool = None
+    reset: FolderPatchReset = None
+    userGroups: list = None
```

### Comparing `lementpro-0.1.7/lementpro/data/mxgraphschemaelementmodel.py` & `lementpro-1.0.0/lementpro/data/mxgraphschemaelementmodel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.mxgraphschemapoint import MxGraphSchemaPoint
-@dataclass
-class MxGraphSchemaElementModel:
-    name: str = None
-    description: str = None
-    elementTypeId: str = None
-    objectTypeId: int = None
-    nameTemplate: str = None
-    executors: list = None
-    globalVariableName: str = None
-    resolutionInSchema: bool = None
-    subjectTemplate: str = None
-    bodyTemplate: str = None
-    properties: list = None
-    id: str = None
-    point: MxGraphSchemaPoint = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.mxgraphschemapoint import MxGraphSchemaPoint
+
+
+@dataclass
+class MxGraphSchemaElementModel:
+    name: str = None
+    description: str = None
+    elementTypeId: str = None
+    objectTypeId: int = None
+    nameTemplate: str = None
+    executors: list = None
+    globalVariableName: str = None
+    resolutionInSchema: bool = None
+    subjectTemplate: str = None
+    bodyTemplate: str = None
+    properties: list = None
+    id: str = None
+    point: MxGraphSchemaPoint = None
```

### Comparing `lementpro-0.1.7/lementpro/data/mxgraphschematransitionmodel.py` & `lementpro-1.0.0/lementpro/data/mxgraphschematransitionmodel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.mxgraphschemaaddrequesttransitionconditionmodel import MxGraphSchemaAddRequestTransitionConditionModel
-from lementpro.data.mxgraphschemapoint import MxGraphSchemaPoint
-from lementpro.data.mxgraphschemaline import MxGraphSchemaLine
-@dataclass
-class MxGraphSchemaTransitionModel:
-    name: str = None
-    description: str = None
-    sourceActions: list = None
-    targetActions: list = None
-    condition: MxGraphSchemaAddRequestTransitionConditionModel = None
-    timer: int = None
-    buttonTransition: bool = None
-    buttonObjectAction: str = None
-    id: str = None
-    point: MxGraphSchemaPoint = None
-    fromElementId: str = None
-    toElementId: str = None
-    line: MxGraphSchemaLine = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.mxgraphschemaaddrequesttransitionconditionmodel import (
+    MxGraphSchemaAddRequestTransitionConditionModel,
+)
+from lementpro.data.mxgraphschemapoint import MxGraphSchemaPoint
+from lementpro.data.mxgraphschemaline import MxGraphSchemaLine
+
+
+@dataclass
+class MxGraphSchemaTransitionModel:
+    name: str = None
+    description: str = None
+    sourceActions: list = None
+    targetActions: list = None
+    condition: MxGraphSchemaAddRequestTransitionConditionModel = None
+    timer: int = None
+    buttonTransition: bool = None
+    buttonObjectAction: str = None
+    id: str = None
+    point: MxGraphSchemaPoint = None
+    fromElementId: str = None
+    toElementId: str = None
+    line: MxGraphSchemaLine = None
```

### Comparing `lementpro-0.1.7/lementpro/data/objecttypeaddmodel.py` & `lementpro-1.0.0/lementpro/data/objecttypeaddmodel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.objecttypeaddextensionmodel import ObjectTypeAddExtensionModel
-from lementpro.data.objecttypeaddcountermodel import ObjectTypeAddCounterModel
-@dataclass
-class ObjectTypeAddModel:
-    knownId: str = None
-    name: str = None
-    description: str = None
-    isAbstract: bool = None
-    isDefault: bool = None
-    isSealed: bool = None
-    isChunk: bool = None
-    parentId: int = None
-    colorHex: str = None
-    extension: ObjectTypeAddExtensionModel = None
-    counter: ObjectTypeAddCounterModel = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.objecttypeaddextensionmodel import ObjectTypeAddExtensionModel
+from lementpro.data.objecttypeaddcountermodel import ObjectTypeAddCounterModel
+
+
+@dataclass
+class ObjectTypeAddModel:
+    knownId: str = None
+    name: str = None
+    description: str = None
+    isAbstract: bool = None
+    isDefault: bool = None
+    isSealed: bool = None
+    isChunk: bool = None
+    parentId: int = None
+    colorHex: str = None
+    extension: ObjectTypeAddExtensionModel = None
+    counter: ObjectTypeAddCounterModel = None
```

### Comparing `lementpro-0.1.7/lementpro/data/objecttypeattributeaddproxymodel.py` & `lementpro-1.0.0/lementpro/data/objecttypeattributeinfomodel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,21 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.objecttypeattributeaddsettingsmodel import ObjectTypeAttributeAddSettingsModel
-from lementpro.data.objecttypeattributeaddformulamodel import ObjectTypeAttributeAddFormulaModel
-@dataclass
-class ObjectTypeAttributeAddProxyModel:
-    attributeId: int = None
-    defaultValue: str = None
-    valueFormat: str = None
-    settings: ObjectTypeAttributeAddSettingsModel = None
-    formula: ObjectTypeAttributeAddFormulaModel = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.objecttypeattributeinfoattributemodel import ObjectTypeAttributeInfoAttributeModel
+from lementpro.data.objecttypeattributeinfosettingsmodel import ObjectTypeAttributeInfoSettingsModel
+
+
+@dataclass
+class ObjectTypeAttributeInfoModel:
+    id: int = None
+    objectTypeId: int = None
+    attributeId: int = None
+    attributeName: str = None
+    attributeDescription: str = None
+    attribute: ObjectTypeAttributeInfoAttributeModel = None
+    settings: ObjectTypeAttributeInfoSettingsModel = None
+    defaultValue: str = None
+    valueFormat: str = None
+    sortWeight: int = None
+    isCalculated: bool = None
+    isInherited: bool = None
```

### Comparing `lementpro-0.1.7/lementpro/data/objecttypeattributeaddsettingsmodel.py` & `lementpro-1.0.0/lementpro/data/objecttypeattributepatchsettingsmodel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-@dataclass
-class ObjectTypeAttributeAddSettingsModel:
-    isRequired: bool = None
-    isHidden: bool = None
-    isSearchable: bool = None
-    isImmutable: bool = None
-    showOnCreate: bool = None
-    showOnEdit: bool = None
-    showInTable: bool = None
-    showOnGeneralPage: bool = None
-    showContentOnSeparatePage: bool = None
-    showOnProjectPage: bool = None
-    showNameInListView: bool = None
-    showInListView: bool = None
-    hideIfNull: bool = None
-    wrapFieldOnNewRow: bool = None
-    fillAvailableSpaceIfSingle: bool = None
-    editorNullHint: str = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+
+
+@dataclass
+class ObjectTypeAttributePatchSettingsModel:
+    isRequired: bool = None
+    isHidden: bool = None
+    isSearchable: bool = None
+    isImmutable: bool = None
+    showOnCreate: bool = None
+    showOnEdit: bool = None
+    showInTable: bool = None
+    showOnGeneralPage: bool = None
+    showContentOnSeparatePage: bool = None
+    showOnProjectPage: bool = None
+    showNameInListView: bool = None
+    showInListView: bool = None
+    hideIfNull: bool = None
+    wrapFieldOnNewRow: bool = None
+    fillAvailableSpaceIfSingle: bool = None
+    editorNullHint: str = None
```

### Comparing `lementpro-0.1.7/lementpro/data/objecttypeattributeextendedmodel.py` & `lementpro-1.0.0/lementpro/data/objecttypeattributeextendedmodel.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.objecttypeattributeinfoattributemodel import ObjectTypeAttributeInfoAttributeModel
-from lementpro.data.objecttypeattributeinfosettingsmodel import ObjectTypeAttributeInfoSettingsModel
-from lementpro.data.objecttypeattributeinfoformulamodel import ObjectTypeAttributeInfoFormulaModel
-@dataclass
-class ObjectTypeAttributeExtendedModel:
-    id: int = None
-    objectTypeId: int = None
-    attributeId: int = None
-    attributeName: str = None
-    attributeDescription: str = None
-    attribute: ObjectTypeAttributeInfoAttributeModel = None
-    settings: ObjectTypeAttributeInfoSettingsModel = None
-    defaultValue: str = None
-    valueFormat: str = None
-    sortWeight: int = None
-    isCalculated: bool = None
-    isInherited: bool = None
-    formula: ObjectTypeAttributeInfoFormulaModel = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.objecttypeattributeinfoattributemodel import ObjectTypeAttributeInfoAttributeModel
+from lementpro.data.objecttypeattributeinfosettingsmodel import ObjectTypeAttributeInfoSettingsModel
+from lementpro.data.objecttypeattributeinfoformulamodel import ObjectTypeAttributeInfoFormulaModel
+
+
+@dataclass
+class ObjectTypeAttributeExtendedModel:
+    id: int = None
+    objectTypeId: int = None
+    attributeId: int = None
+    attributeName: str = None
+    attributeDescription: str = None
+    attribute: ObjectTypeAttributeInfoAttributeModel = None
+    settings: ObjectTypeAttributeInfoSettingsModel = None
+    defaultValue: str = None
+    valueFormat: str = None
+    sortWeight: int = None
+    isCalculated: bool = None
+    isInherited: bool = None
+    formula: ObjectTypeAttributeInfoFormulaModel = None
```

### Comparing `lementpro-0.1.7/lementpro/data/objecttypeattributeinfoattributemodel.py` & `lementpro-1.0.0/lementpro/data/objecttypeattributeaddproxymodel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.objecttypeattributeinfoattributerelationmodel import ObjectTypeAttributeInfoAttributeRelationModel
-from lementpro.data.objecttypeattributeinfovaluelistmodel import ObjectTypeAttributeInfoValueListModel
-@dataclass
-class ObjectTypeAttributeInfoAttributeModel:
-    knownId: str = None
-    name: str = None
-    description: str = None
-    attributeTypeId: str = None
-    valueTypeId: str = None
-    relation: ObjectTypeAttributeInfoAttributeRelationModel = None
-    valueList: ObjectTypeAttributeInfoValueListModel = None
-    isSystem: bool = None
-    isFilterable: bool = None
-    isGroupable: bool = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.objecttypeattributeaddsettingsmodel import ObjectTypeAttributeAddSettingsModel
+from lementpro.data.objecttypeattributeaddformulamodel import ObjectTypeAttributeAddFormulaModel
+
+
+@dataclass
+class ObjectTypeAttributeAddProxyModel:
+    attributeId: int = None
+    defaultValue: str = None
+    valueFormat: str = None
+    settings: ObjectTypeAttributeAddSettingsModel = None
+    formula: ObjectTypeAttributeAddFormulaModel = None
```

### Comparing `lementpro-0.1.7/lementpro/data/objecttypeattributepatchmodel.py` & `lementpro-1.0.0/lementpro/data/usergateattributeinfomodel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,21 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.objecttypeattributepatchsettingsmodel import ObjectTypeAttributePatchSettingsModel
-from lementpro.data.objecttypeattributepatchformulamodel import ObjectTypeAttributePatchFormulaModel
-@dataclass
-class ObjectTypeAttributePatchModel:
-    defaultValue: str = None
-    valueFormat: str = None
-    settings: ObjectTypeAttributePatchSettingsModel = None
-    formula: ObjectTypeAttributePatchFormulaModel = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.objecttypeattributeinfovaluelistmodel import ObjectTypeAttributeInfoValueListModel
+from lementpro.data.relationvalue import RelationValue
+
+
+@dataclass
+class UserGateAttributeInfoModel:
+    id: int = None
+    knownId: str = None
+    name: str = None
+    isSystem: bool = None
+    value: str = None
+    valueList: ObjectTypeAttributeInfoValueListModel = None
+    relationValue: RelationValue = None
+    attributeTypeId: str = None
+    valueTypeId: str = None
+    relationTypeId: str = None
+    isRequired: bool = None
+    isEditable: bool = None
```

### Comparing `lementpro-0.1.7/lementpro/data/objecttypeinfodetailedmodel.py` & `lementpro-1.0.0/lementpro/data/objecttypeinfodetailedmodel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.objecttypeinfodetailedcountermodel import ObjectTypeInfoDetailedCounterModel
-from lementpro.data.objecttypeinfodetailedmenumodel import ObjectTypeInfoDetailedMenuModel
-from lementpro.data.objecttypeinfodetailedbimmodel import ObjectTypeInfoDetailedBimModel
-@dataclass
-class ObjectTypeInfoDetailedModel:
-    counter: ObjectTypeInfoDetailedCounterModel = None
-    exportTemplateFiles: list = None
-    menu: ObjectTypeInfoDetailedMenuModel = None
-    bim: ObjectTypeInfoDetailedBimModel = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.objecttypeinfodetailedcountermodel import ObjectTypeInfoDetailedCounterModel
+from lementpro.data.objecttypeinfodetailedmenumodel import ObjectTypeInfoDetailedMenuModel
+from lementpro.data.objecttypeinfodetailedbimmodel import ObjectTypeInfoDetailedBimModel
+
+
+@dataclass
+class ObjectTypeInfoDetailedModel:
+    counter: ObjectTypeInfoDetailedCounterModel = None
+    exportTemplateFiles: list = None
+    menu: ObjectTypeInfoDetailedMenuModel = None
+    bim: ObjectTypeInfoDetailedBimModel = None
```

### Comparing `lementpro-0.1.7/lementpro/data/objecttypeinfoextendedmodel.py` & `lementpro-1.0.0/lementpro/data/objecttypeinfoextendedmodel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.objecttypeextensionmodel import ObjectTypeExtensionModel
-from lementpro.data.objecttypeinfodetailedmodel import ObjectTypeInfoDetailedModel
-@dataclass
-class ObjectTypeInfoExtendedModel:
-    id: int = None
-    companyId: int = None
-    knownId: str = None
-    name: str = None
-    description: str = None
-    isAbstract: bool = None
-    isDefault: bool = None
-    isSealed: bool = None
-    isChunk: bool = None
-    parentId: int = None
-    isSystem: bool = None
-    sortWeight: int = None
-    colorHex: str = None
-    extension: ObjectTypeExtensionModel = None
-    systemObjectTypeId: str = None
-    detailed: ObjectTypeInfoDetailedModel = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.objecttypeextensionmodel import ObjectTypeExtensionModel
+from lementpro.data.objecttypeinfodetailedmodel import ObjectTypeInfoDetailedModel
+
+
+@dataclass
+class ObjectTypeInfoExtendedModel:
+    id: int = None
+    companyId: int = None
+    knownId: str = None
+    name: str = None
+    description: str = None
+    isAbstract: bool = None
+    isDefault: bool = None
+    isSealed: bool = None
+    isChunk: bool = None
+    parentId: int = None
+    isSystem: bool = None
+    sortWeight: int = None
+    colorHex: str = None
+    extension: ObjectTypeExtensionModel = None
+    systemObjectTypeId: str = None
+    detailed: ObjectTypeInfoDetailedModel = None
```

### Comparing `lementpro-0.1.7/lementpro/data/objecttypeinfopagingmodel.py` & `lementpro-1.0.0/lementpro/data/objecttypeinfopagingmodel.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.objecttypeextensionmodel import ObjectTypeExtensionModel
-@dataclass
-class ObjectTypeInfoPagingModel:
-    id: int = None
-    companyId: int = None
-    knownId: str = None
-    name: str = None
-    description: str = None
-    isAbstract: bool = None
-    isDefault: bool = None
-    isSealed: bool = None
-    isChunk: bool = None
-    parentId: int = None
-    isSystem: bool = None
-    sortWeight: int = None
-    colorHex: str = None
-    extension: ObjectTypeExtensionModel = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.objecttypeextensionmodel import ObjectTypeExtensionModel
+
+
+@dataclass
+class ObjectTypeInfoPagingModel:
+    id: int = None
+    companyId: int = None
+    knownId: str = None
+    name: str = None
+    description: str = None
+    isAbstract: bool = None
+    isDefault: bool = None
+    isSealed: bool = None
+    isChunk: bool = None
+    parentId: int = None
+    isSystem: bool = None
+    sortWeight: int = None
+    colorHex: str = None
+    extension: ObjectTypeExtensionModel = None
```

### Comparing `lementpro-0.1.7/lementpro/data/objecttypepatchmodel.py` & `lementpro-1.0.0/lementpro/data/objecttypepatchmodel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.objecttypepatchextensionmodel import ObjectTypePatchExtensionModel
-from lementpro.data.objecttypepatchcountermodel import ObjectTypePatchCounterModel
-@dataclass
-class ObjectTypePatchModel:
-    knownId: str = None
-    name: str = None
-    description: str = None
-    isAbstract: bool = None
-    isDefault: bool = None
-    isSealed: bool = None
-    isChunk: bool = None
-    colorHex: str = None
-    extension: ObjectTypePatchExtensionModel = None
-    counter: ObjectTypePatchCounterModel = None
-    sortWeight: int = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.objecttypepatchextensionmodel import ObjectTypePatchExtensionModel
+from lementpro.data.objecttypepatchcountermodel import ObjectTypePatchCounterModel
+
+
+@dataclass
+class ObjectTypePatchModel:
+    knownId: str = None
+    name: str = None
+    description: str = None
+    isAbstract: bool = None
+    isDefault: bool = None
+    isSealed: bool = None
+    isChunk: bool = None
+    colorHex: str = None
+    extension: ObjectTypePatchExtensionModel = None
+    counter: ObjectTypePatchCounterModel = None
+    sortWeight: int = None
```

### Comparing `lementpro-0.1.7/lementpro/data/objecttypeuisettingsproxyresponse.py` & `lementpro-1.0.0/lementpro/data/objecttypeuisettingsproxyresponse.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.objecttypeuisettingsproxyresponsedetailedpage import ObjectTypeUiSettingsProxyResponseDetailedPage
-from lementpro.data.objecttypeuisettingsproxyresponselistview import ObjectTypeUiSettingsProxyResponseListView
-from lementpro.data.objecttypeuisettingsproxyresponsetableview import ObjectTypeUiSettingsProxyResponseTableView
-from lementpro.data.objecttypeuisettingsproxyresponseeditpage import ObjectTypeUiSettingsProxyResponseEditPage
-from lementpro.data.objecttypeuisettingsproxyresponsecreatepage import ObjectTypeUiSettingsProxyResponseCreatePage
-@dataclass
-class ObjectTypeUiSettingsProxyResponse:
-    detailedPage: ObjectTypeUiSettingsProxyResponseDetailedPage = None
-    listView: ObjectTypeUiSettingsProxyResponseListView = None
-    tableView: ObjectTypeUiSettingsProxyResponseTableView = None
-    editPage: ObjectTypeUiSettingsProxyResponseEditPage = None
-    createPage: ObjectTypeUiSettingsProxyResponseCreatePage = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.objecttypeuisettingsproxyresponsedetailedpage import ObjectTypeUiSettingsProxyResponseDetailedPage
+from lementpro.data.objecttypeuisettingsproxyresponselistview import ObjectTypeUiSettingsProxyResponseListView
+from lementpro.data.objecttypeuisettingsproxyresponsetableview import ObjectTypeUiSettingsProxyResponseTableView
+from lementpro.data.objecttypeuisettingsproxyresponseeditpage import ObjectTypeUiSettingsProxyResponseEditPage
+from lementpro.data.objecttypeuisettingsproxyresponsecreatepage import ObjectTypeUiSettingsProxyResponseCreatePage
+
+
+@dataclass
+class ObjectTypeUiSettingsProxyResponse:
+    detailedPage: ObjectTypeUiSettingsProxyResponseDetailedPage = None
+    listView: ObjectTypeUiSettingsProxyResponseListView = None
+    tableView: ObjectTypeUiSettingsProxyResponseTableView = None
+    editPage: ObjectTypeUiSettingsProxyResponseEditPage = None
+    createPage: ObjectTypeUiSettingsProxyResponseCreatePage = None
```

### Comparing `lementpro-0.1.7/lementpro/data/useraddmodel.py` & `lementpro-1.0.0/lementpro/data/useraddmodel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.usermodelextension import UserModelExtension
-from lementpro.data.usermodelnotification import UserModelNotification
-@dataclass
-class UserAddModel:
-    password: str = None
-    userName: str = None
-    email: str = None
-    firstName: str = None
-    middleName: str = None
-    lastName: str = None
-    phoneNumber: str = None
-    preferredLocale: str = None
-    isDismissed: bool = None
-    isDisabled: bool = None
-    position: str = None
-    extension: UserModelExtension = None
-    role: str = None
-    notification: UserModelNotification = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.usermodelextension import UserModelExtension
+from lementpro.data.usermodelnotification import UserModelNotification
+
+
+@dataclass
+class UserAddModel:
+    password: str = None
+    userName: str = None
+    email: str = None
+    firstName: str = None
+    middleName: str = None
+    lastName: str = None
+    phoneNumber: str = None
+    preferredLocale: str = None
+    isDismissed: bool = None
+    isDisabled: bool = None
+    position: str = None
+    extension: UserModelExtension = None
+    role: str = None
+    notification: UserModelNotification = None
```

### Comparing `lementpro-0.1.7/lementpro/data/userfolderaddmodel.py` & `lementpro-1.0.0/lementpro/data/userfolderextendedmodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,34 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.folderaddobjectstatusfilter import FolderAddObjectStatusFilter
-from lementpro.data.folderaddobjectstatefilter import FolderAddObjectStateFilter
-from lementpro.data.folderaddobjectuserfilter import FolderAddObjectUserFilter
-from lementpro.data.folderorderbyattributemodel import FolderOrderByAttributeModel
-from lementpro.data.folderjoinbyattributemodel import FolderJoinByAttributeModel
-@dataclass
-class UserFolderAddModel:
-    name: str = None
-    description: str = None
-    parentId: int = None
-    menuObjectTypeId: int = None
-    exportTemplateFileId: int = None
-    isAbstract: bool = None
-    objectTypes: list = None
-    objectStatus: FolderAddObjectStatusFilter = None
-    objectState: FolderAddObjectStateFilter = None
-    objectUser: FolderAddObjectUserFilter = None
-    orderByAttribute: FolderOrderByAttributeModel = None
-    joinByAttribute: FolderJoinByAttributeModel = None
-    groupByAttributes: list = None
-    filterByAttributes: list = None
-    viewTypeId: str = None
-    countObjects: bool = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.folderaddobjectstatusfilter import FolderAddObjectStatusFilter
+from lementpro.data.folderaddobjectstatefilter import FolderAddObjectStateFilter
+from lementpro.data.folderaddobjectuserfilter import FolderAddObjectUserFilter
+from lementpro.data.folderorderbyattributemodel import FolderOrderByAttributeModel
+from lementpro.data.folderjoinbyattributemodel import FolderJoinByAttributeModel
+
+
+@dataclass
+class UserFolderExtendedModel:
+    id: int = None
+    parentId: int = None
+    companyId: int = None
+    name: str = None
+    description: str = None
+    menuObjectTypeId: int = None
+    isSystem: bool = None
+    isTemplate: bool = None
+    isAbstract: bool = None
+    sortWeight: int = None
+    exportTemplateFileId: int = None
+    objectStatus: FolderAddObjectStatusFilter = None
+    objectState: FolderAddObjectStateFilter = None
+    objectUser: FolderAddObjectUserFilter = None
+    orderByAttribute: FolderOrderByAttributeModel = None
+    joinByAttribute: FolderJoinByAttributeModel = None
+    groupByAttributes: list = None
+    filterByAttributes: list = None
+    objectTypes: list = None
+    viewTypeId: str = None
+    countObjects: bool = None
+    isOwner: bool = None
```

### Comparing `lementpro-0.1.7/lementpro/data/userfolderpatchmodel.py` & `lementpro-1.0.0/lementpro/data/userfolderpatchmodel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.folderpatchobjectstatusfilter import FolderPatchObjectStatusFilter
-from lementpro.data.folderpatchobjectstatefilter import FolderPatchObjectStateFilter
-from lementpro.data.folderpatchobjectuserfilter import FolderPatchObjectUserFilter
-from lementpro.data.folderorderbyattributemodel import FolderOrderByAttributeModel
-from lementpro.data.folderjoinbyattributemodel import FolderJoinByAttributeModel
-from lementpro.data.folderpatchreset import FolderPatchReset
-@dataclass
-class UserFolderPatchModel:
-    name: str = None
-    description: str = None
-    objectTypes: list = None
-    exportTemplateFileId: int = None
-    objectStatus: FolderPatchObjectStatusFilter = None
-    objectState: FolderPatchObjectStateFilter = None
-    objectUser: FolderPatchObjectUserFilter = None
-    orderByAttribute: FolderOrderByAttributeModel = None
-    joinByAttribute: FolderJoinByAttributeModel = None
-    groupByAttributes: list = None
-    filterByAttributes: list = None
-    isAbstract: bool = None
-    reset: FolderPatchReset = None
-    viewTypeId: str = None
-    countObjects: bool = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.folderpatchobjectstatusfilter import FolderPatchObjectStatusFilter
+from lementpro.data.folderpatchobjectstatefilter import FolderPatchObjectStateFilter
+from lementpro.data.folderpatchobjectuserfilter import FolderPatchObjectUserFilter
+from lementpro.data.folderorderbyattributemodel import FolderOrderByAttributeModel
+from lementpro.data.folderjoinbyattributemodel import FolderJoinByAttributeModel
+from lementpro.data.folderpatchreset import FolderPatchReset
+
+
+@dataclass
+class UserFolderPatchModel:
+    name: str = None
+    description: str = None
+    objectTypes: list = None
+    exportTemplateFileId: int = None
+    objectStatus: FolderPatchObjectStatusFilter = None
+    objectState: FolderPatchObjectStateFilter = None
+    objectUser: FolderPatchObjectUserFilter = None
+    orderByAttribute: FolderOrderByAttributeModel = None
+    joinByAttribute: FolderJoinByAttributeModel = None
+    groupByAttributes: list = None
+    filterByAttributes: list = None
+    isAbstract: bool = None
+    reset: FolderPatchReset = None
+    viewTypeId: str = None
+    countObjects: bool = None
```

### Comparing `lementpro-0.1.7/lementpro/data/userfoldertreenodemodel.py` & `lementpro-1.0.0/lementpro/data/userfoldertreenodemodel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.folderusertreecountmodel import FolderUserTreeCountModel
-@dataclass
-class UserFolderTreeNodeModel:
-    id: int = None
-    path: list = None
-    parentId: int = None
-    name: str = None
-    isSystem: bool = None
-    isTemplate: bool = None
-    isAbstract: bool = None
-    isVirtual: bool = None
-    hasGrouping: bool = None
-    isOwner: bool = None
-    sortWeight: int = None
-    countObjects: bool = None
-    viewTypeId: str = None
-    objectsCounter: FolderUserTreeCountModel = None
-    children: list = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.folderusertreecountmodel import FolderUserTreeCountModel
+
+
+@dataclass
+class UserFolderTreeNodeModel:
+    id: int = None
+    path: list = None
+    parentId: int = None
+    name: str = None
+    isSystem: bool = None
+    isTemplate: bool = None
+    isAbstract: bool = None
+    isVirtual: bool = None
+    hasGrouping: bool = None
+    isOwner: bool = None
+    sortWeight: int = None
+    countObjects: bool = None
+    viewTypeId: str = None
+    objectsCounter: FolderUserTreeCountModel = None
+    children: list = None
```

### Comparing `lementpro-0.1.7/lementpro/data/usergateattributeinfomodel.py` & `lementpro-1.0.0/lementpro/data/usergatefolderobjectinfoattributemodel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.objecttypeattributeinfovaluelistmodel import ObjectTypeAttributeInfoValueListModel
-from lementpro.data.relationvalue import RelationValue
-@dataclass
-class UserGateAttributeInfoModel:
-    id: int = None
-    knownId: str = None
-    name: str = None
-    isSystem: bool = None
-    value: str = None
-    valueList: ObjectTypeAttributeInfoValueListModel = None
-    relationValue: RelationValue = None
-    attributeTypeId: str = None
-    valueTypeId: str = None
-    relationTypeId: str = None
-    isRequired: bool = None
-    isEditable: bool = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.objecttypeattributeinfovaluelistmodel import ObjectTypeAttributeInfoValueListModel
+from lementpro.data.relationvalue import RelationValue
+
+
+@dataclass
+class UserGateFolderObjectInfoAttributeModel:
+    id: int = None
+    knownId: str = None
+    name: str = None
+    isSystem: bool = None
+    value: str = None
+    valueList: ObjectTypeAttributeInfoValueListModel = None
+    relationValue: RelationValue = None
+    attributeTypeId: str = None
+    valueTypeId: str = None
+    relationTypeId: str = None
+    isRequired: bool = None
+    isEditable: bool = None
+    showNameInListView: bool = None
```

### Comparing `lementpro-0.1.7/lementpro/data/usergatecommentmessageinfomodel.py` & `lementpro-1.0.0/lementpro/data/usergatecommentmessageinfomodel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.commentextensionmodel import CommentExtensionModel
-from lementpro.data.usergatecommentmessageinfousermodel import UserGateCommentMessageInfoUserModel
-from lementpro.data.usergatecommentmessageinfousermodel import UserGateCommentMessageInfoUserModel
-@dataclass
-class UserGateCommentMessageInfoModel:
-    id: int = None
-    companyId: int = None
-    objectId: int = None
-    message: str = None
-    parentId: int = None
-    sourceId: str = None
-    externalId: str = None
-    extension: CommentExtensionModel = None
-    dateCreated: str = None
-    dateUpdated: str = None
-    canEdit: bool = None
-    dateViewed: str = None
-    user: UserGateCommentMessageInfoUserModel = None
-    userFrom: UserGateCommentMessageInfoUserModel = None
-    files: list = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.commentextensionmodel import CommentExtensionModel
+from lementpro.data.usergatecommentmessageinfousermodel import UserGateCommentMessageInfoUserModel
+from lementpro.data.usergatecommentmessageinfousermodel import UserGateCommentMessageInfoUserModel
+
+
+@dataclass
+class UserGateCommentMessageInfoModel:
+    id: int = None
+    companyId: int = None
+    objectId: int = None
+    message: str = None
+    parentId: int = None
+    sourceId: str = None
+    externalId: str = None
+    extension: CommentExtensionModel = None
+    dateCreated: str = None
+    dateUpdated: str = None
+    canEdit: bool = None
+    dateViewed: str = None
+    user: UserGateCommentMessageInfoUserModel = None
+    userFrom: UserGateCommentMessageInfoUserModel = None
+    files: list = None
```

### Comparing `lementpro-0.1.7/lementpro/data/usergatefolderobjectinfoattributemodel.py` & `lementpro-1.0.0/lementpro/data/usergateobjectinfoattributemodel.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.objecttypeattributeinfovaluelistmodel import ObjectTypeAttributeInfoValueListModel
-from lementpro.data.relationvalue import RelationValue
-@dataclass
-class UserGateFolderObjectInfoAttributeModel:
-    id: int = None
-    knownId: str = None
-    name: str = None
-    isSystem: bool = None
-    value: str = None
-    valueList: ObjectTypeAttributeInfoValueListModel = None
-    relationValue: RelationValue = None
-    attributeTypeId: str = None
-    valueTypeId: str = None
-    relationTypeId: str = None
-    isRequired: bool = None
-    isEditable: bool = None
-    showNameInListView: bool = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.objecttypeattributeinfovaluelistmodel import ObjectTypeAttributeInfoValueListModel
+from lementpro.data.relationvalue import RelationValue
+
+
+@dataclass
+class UserGateObjectInfoAttributeModel:
+    id: int = None
+    knownId: str = None
+    name: str = None
+    isSystem: bool = None
+    value: str = None
+    valueList: ObjectTypeAttributeInfoValueListModel = None
+    relationValue: RelationValue = None
+    attributeTypeId: str = None
+    valueTypeId: str = None
+    relationTypeId: str = None
+    isRequired: bool = None
+    isEditable: bool = None
```

### Comparing `lementpro-0.1.7/lementpro/data/usergatefolderobjectinfomodel.py` & `lementpro-1.0.0/lementpro/data/usergatefolderobjectinfomodel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.usergatefolderobjectinfomodelcommentinfo import UserGateFolderObjectInfoModelCommentInfo
-@dataclass
-class UserGateFolderObjectInfoModel:
-    id: int = None
-    objectTypeId: int = None
-    name: str = None
-    dateCreated: str = None
-    dateExpire: str = None
-    dateModified: str = None
-    dateArchived: str = None
-    isClosing: bool = None
-    isFavorite: bool = None
-    isModified: bool = None
-    isDebug: bool = None
-    canEdit: bool = None
-    actions: str = None
-    attributes: list = None
-    commentData: UserGateFolderObjectInfoModelCommentInfo = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.usergatefolderobjectinfomodelcommentinfo import UserGateFolderObjectInfoModelCommentInfo
+
+
+@dataclass
+class UserGateFolderObjectInfoModel:
+    id: int = None
+    objectTypeId: int = None
+    name: str = None
+    dateCreated: str = None
+    dateExpire: str = None
+    dateModified: str = None
+    dateArchived: str = None
+    isClosing: bool = None
+    isFavorite: bool = None
+    isModified: bool = None
+    isDebug: bool = None
+    canEdit: bool = None
+    actions: str = None
+    attributes: list = None
+    commentData: UserGateFolderObjectInfoModelCommentInfo = None
```

### Comparing `lementpro-0.1.7/lementpro/data/usergatefolderobjectinfomodellastcomment.py` & `lementpro-1.0.0/lementpro/data/usergatefolderobjectinfomodellastcomment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.usergatefolderobjectinfomodellastcommentuser import UserGateFolderObjectInfoModelLastCommentUser
-from lementpro.data.usergatefolderobjectinfomodellastcommentuser import UserGateFolderObjectInfoModelLastCommentUser
-@dataclass
-class UserGateFolderObjectInfoModelLastComment:
-    id: int = None
-    user: UserGateFolderObjectInfoModelLastCommentUser = None
-    userFrom: UserGateFolderObjectInfoModelLastCommentUser = None
-    message: str = None
-    messageSimplified: str = None
-    dateCreated: str = None
-    dateUpdated: str = None
-    sourceId: str = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.usergatefolderobjectinfomodellastcommentuser import UserGateFolderObjectInfoModelLastCommentUser
+from lementpro.data.usergatefolderobjectinfomodellastcommentuser import UserGateFolderObjectInfoModelLastCommentUser
+
+
+@dataclass
+class UserGateFolderObjectInfoModelLastComment:
+    id: int = None
+    user: UserGateFolderObjectInfoModelLastCommentUser = None
+    userFrom: UserGateFolderObjectInfoModelLastCommentUser = None
+    message: str = None
+    messageSimplified: str = None
+    dateCreated: str = None
+    dateUpdated: str = None
+    sourceId: str = None
```

### Comparing `lementpro-0.1.7/lementpro/data/usergateobjectinfoattributemodel.py` & `lementpro-1.0.0/lementpro/data/usergatesearchobjectinfoattributemodel.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.objecttypeattributeinfovaluelistmodel import ObjectTypeAttributeInfoValueListModel
-from lementpro.data.relationvalue import RelationValue
-@dataclass
-class UserGateObjectInfoAttributeModel:
-    id: int = None
-    knownId: str = None
-    name: str = None
-    isSystem: bool = None
-    value: str = None
-    valueList: ObjectTypeAttributeInfoValueListModel = None
-    relationValue: RelationValue = None
-    attributeTypeId: str = None
-    valueTypeId: str = None
-    relationTypeId: str = None
-    isRequired: bool = None
-    isEditable: bool = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.objecttypeattributeinfovaluelistmodel import ObjectTypeAttributeInfoValueListModel
+from lementpro.data.relationvalue import RelationValue
+
+
+@dataclass
+class UserGateSearchObjectInfoAttributeModel:
+    id: int = None
+    knownId: str = None
+    name: str = None
+    isSystem: bool = None
+    value: str = None
+    valueList: ObjectTypeAttributeInfoValueListModel = None
+    relationValue: RelationValue = None
+    attributeTypeId: str = None
+    valueTypeId: str = None
+    relationTypeId: str = None
+    isRequired: bool = None
+    isEditable: bool = None
```

### Comparing `lementpro-0.1.7/lementpro/data/usergateobjectinfoextendedmodel.py` & `lementpro-1.0.0/lementpro/data/usergateobjectinfoextendedmodel.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.usergateobjectinfoextendedmodelroutedata import UserGateObjectInfoExtendedModelRouteData
-@dataclass
-class UserGateObjectInfoExtendedModel:
-    id: int = None
-    objectTypeId: int = None
-    name: str = None
-    dateCreated: str = None
-    dateExpire: str = None
-    dateModified: str = None
-    dateArchived: str = None
-    isClosing: bool = None
-    isFavorite: bool = None
-    isModified: bool = None
-    isDebug: bool = None
-    actions: str = None
-    attributes: list = None
-    route: UserGateObjectInfoExtendedModelRouteData = None
-    canEdit: bool = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.usergateobjectinfoextendedmodelroutedata import UserGateObjectInfoExtendedModelRouteData
+
+
+@dataclass
+class UserGateObjectInfoExtendedModel:
+    id: int = None
+    objectTypeId: int = None
+    name: str = None
+    dateCreated: str = None
+    dateExpire: str = None
+    dateModified: str = None
+    dateArchived: str = None
+    isClosing: bool = None
+    isFavorite: bool = None
+    isModified: bool = None
+    isDebug: bool = None
+    actions: str = None
+    attributes: list = None
+    route: UserGateObjectInfoExtendedModelRouteData = None
+    canEdit: bool = None
```

### Comparing `lementpro-0.1.7/lementpro/data/usergaterouteinstanceextendedmodel.py` & `lementpro-1.0.0/lementpro/data/usergaterouteinstanceextendedmodelactivity.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.routeinforesponseschemaversion import RouteInfoResponseSchemaVersion
-from lementpro.data.relatedobjectmodel import RelatedObjectModel
-@dataclass
-class UserGateRouteInstanceExtendedModel:
-    id: str = None
-    dateCreated: str = None
-    dateCompleted: str = None
-    statusId: str = None
-    isDebug: bool = None
-    schemaVersion: RouteInfoResponseSchemaVersion = None
-    object: RelatedObjectModel = None
-    activities: list = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.relatedobjectmodel import RelatedObjectModel
+from lementpro.data.routeextendedresponseactivityelement import RouteExtendedResponseActivityElement
+
+
+@dataclass
+class UserGateRouteInstanceExtendedModelActivity:
+    id: str = None
+    dateCreated: str = None
+    dateStarted: str = None
+    dateCompleted: str = None
+    statusId: str = None
+    object: RelatedObjectModel = None
+    variables: list = None
+    element: RouteExtendedResponseActivityElement = None
```

### Comparing `lementpro-0.1.7/lementpro/data/usergatesearchobjectinfoattributemodel.py` & `lementpro-1.0.0/lementpro/data/usergaterouteinstanceextendedmodel.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.objecttypeattributeinfovaluelistmodel import ObjectTypeAttributeInfoValueListModel
-from lementpro.data.relationvalue import RelationValue
-@dataclass
-class UserGateSearchObjectInfoAttributeModel:
-    id: int = None
-    knownId: str = None
-    name: str = None
-    isSystem: bool = None
-    value: str = None
-    valueList: ObjectTypeAttributeInfoValueListModel = None
-    relationValue: RelationValue = None
-    attributeTypeId: str = None
-    valueTypeId: str = None
-    relationTypeId: str = None
-    isRequired: bool = None
-    isEditable: bool = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.routeinforesponseschemaversion import RouteInfoResponseSchemaVersion
+from lementpro.data.relatedobjectmodel import RelatedObjectModel
+
+
+@dataclass
+class UserGateRouteInstanceExtendedModel:
+    id: str = None
+    dateCreated: str = None
+    dateCompleted: str = None
+    statusId: str = None
+    isDebug: bool = None
+    schemaVersion: RouteInfoResponseSchemaVersion = None
+    object: RelatedObjectModel = None
+    activities: list = None
```

### Comparing `lementpro-0.1.7/lementpro/data/userinfomodel.py` & `lementpro-1.0.0/lementpro/data/userpatchmodel.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from lementpro.data.userinfoextensionmodel import UserInfoExtensionModel
-@dataclass
-class UserInfoModel:
-    id: int = None
-    userName: str = None
-    companyId: int = None
-    email: str = None
-    firstName: str = None
-    middleName: str = None
-    lastName: str = None
-    phoneNumber: str = None
-    preferredLocale: str = None
-    isDismissed: bool = None
-    isDisabled: bool = None
-    isSystem: bool = None
-    position: str = None
-    role: str = None
-    departmentId: int = None
-    displayName: str = None
-    extension: UserInfoExtensionModel = None
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+from dataclasses import dataclass
+from lementpro.data.usermodelextension import UserModelExtension
+from lementpro.data.usermodelnotification import UserModelNotification
+
+
+@dataclass
+class UserPatchModel:
+    userName: str = None
+    password: str = None
+    email: str = None
+    firstName: str = None
+    middleName: str = None
+    lastName: str = None
+    phoneNumber: str = None
+    preferredLocale: str = None
+    isDismissed: bool = None
+    isDisabled: bool = None
+    position: str = None
+    extension: UserModelExtension = None
+    role: str = None
+    notification: UserModelNotification = None
```

### Comparing `lementpro-0.1.7/lementpro/sender.py` & `lementpro-1.0.0/lementpro/sender.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-import requests
-from requests import Session
-from .data.user import User
-from .logger import logger
-
-
-class Sender:
-
-    @staticmethod
-    def send_request(request_data, by_user=None):
-        session = Sender().__set_user(by_user=by_user)
-        request_data.url = by_user.root_url + request_data.url
-        prepped = session.prepare_request(request_data)
-        Sender.logging(prepped=prepped)
-        response = session.send(request=prepped, timeout=30, verify=True)
-        Sender.logging(prepped=response)
-        return response
-
-    @staticmethod
-    def __set_user(by_user: User):
-        session = Session()
-        if by_user and by_user.access_token is not None:
-            session.headers.update(Authorization=f'Bearer {by_user.access_token}')
-        if by_user and by_user.specific_headers is not {}:
-            session.headers.update(by_user.specific_headers)
-        if by_user and by_user.cookies is not None:
-            session.cookies = by_user.cookies
-        return session
-
-    @staticmethod
-    def logging(prepped):
-        if isinstance(prepped, requests.models.PreparedRequest):
-            url, method, headers, body = prepped.url, prepped.method, prepped.headers, prepped.body
-            info = f"sent request:\n url: {url}\n method: {method}\n headers: {headers}\n body: {body}\n "
-        else:
-            headers = prepped.headers
-            info = f"received response:\n code: {prepped.status_code} {prepped.reason} \n headers: {headers} \n content: {prepped.text}"
-        logger.debug("len logging =%s" % str(len(info)))
-        if len(info) < 10000:
-            logger.debug(f'\n\n{info}')
-        else:
-            logger.debug("Log is too large.")
-            logger.debug("Return only header = %s" % headers)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+from requests import Session
+from .data.user import User
+
+# from .logger import logger
+
+
+class Sender:
+    @staticmethod
+    def send_request(request_data, by_user=None):
+        session = Sender().__set_user(by_user=by_user)
+        request_data.url = by_user.root_url + request_data.url
+        prepped = session.prepare_request(request_data)
+        # Sender.logging(prepped=prepped)
+        response = session.send(request=prepped, timeout=30, verify=True)
+        # Sender.logging(prepped=response)
+        return response
+
+    @staticmethod
+    def __set_user(by_user: User):
+        session = Session()
+        if by_user and by_user.access_token is not None:
+            session.headers.update(Authorization=f"Bearer {by_user.access_token}")
+        if by_user and by_user.specific_headers is not {}:
+            session.headers.update(by_user.specific_headers)
+        if by_user and by_user.cookies is not None:
+            session.cookies = by_user.cookies
+        return session
+
+    # @staticmethod
+    # def logging(prepped):
+    #     if isinstance(prepped, requests.models.PreparedRequest):
+    #         url, method, headers, body = prepped.url, prepped.method, prepped.headers, prepped.body
+    #         info = f"sent request:\n url: {url}\n method: {method}\n headers: {headers}\n body: {body}\n "
+    #     else:
+    #         headers = prepped.headers
+    #         info = f"received response:\n code: {prepped.status_code} {prepped.reason} \n headers: {headers} \n content: {prepped.text}"
+    #     logger.debug("len logging =%s" % str(len(info)))
+    #     if len(info) < 10000:
+    #         logger.debug(f'\n\n{info}')
+    #     else:
+    #         logger.debug("Log is too large.")
+    #         logger.debug("Return only header = %s" % headers)
```

### Comparing `lementpro-0.1.7/lementpro/services/accounts.py` & `lementpro-1.0.0/lementpro/services/accounts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,136 @@
-from lementpro.builders import Build
-from lementpro.data.user import User
-from lementpro.sender import Sender
-from lementpro.data.usermodelextension import UserModelExtension
-from lementpro.data.usermodelnotification import UserModelNotification
-
-
-class Accounts:
-    """Service for working with Accounts in UserGate Public API"""
-
-    def login(self, by_user: User, login: str = None, password: str = None):
-        """Sign in by login
-        :return: Access token model
-        """
-        request_data = Build(
-            url="/api/accounts/login").post(login=login, password=password,)
-        return Sender().send_request(request_data, by_user=by_user)
-
-    def refresh_token(self, by_user: User, refreshToken: str = None):
-        """Refresh token
-        :return: Access token model
-        """
-        request_data = Build(
-            url="/api/accounts/refresh_token").post(refreshToken=refreshToken,)
-        return Sender().send_request(request_data, by_user=by_user)
-
-    def logout(self, by_user: User):
-        """Sign out
-        :return: No Content
-        """
-        request_data = Build(url="/api/accounts/logout").post()
-        return Sender().send_request(request_data, by_user=by_user)
-
-    def restore_password(self, by_user: User, login: str = None, companyId: int = None):
-        """Restore password
-        :return: No Content
-        """
-        request_data = Build(
-            url="/api/accounts/restore_password").post(login=login, companyId=companyId,)
-        return Sender().send_request(request_data, by_user=by_user)
-
-    def get_me(self, by_user: User):
-        """Get me
-        :return: Created BlockWork identifier
-        """
-        request_data = Build(url="/api/accounts/me").get()
-        return Sender().send_request(request_data, by_user=by_user)
-
-    def patch_me(self, by_user: User, userName: str = None, password: str = None, email: str = None, firstName: str = None, middleName: str = None, lastName: str = None, phoneNumber: str = None, preferredLocale: str = None, isDismissed: bool = None, isDisabled: bool = None, position: str = None, extension: UserModelExtension = None, role: str = None, notification: UserModelNotification = None):
-        """Partial update user
-        :return: No Content
-        """
-        request_data = Build(url="/api/accounts/me").patch(userName=userName, password=password, email=email, firstName=firstName, middleName=middleName, lastName=lastName, phoneNumber=phoneNumber,
-                                                           preferredLocale=preferredLocale, isDismissed=isDismissed, isDisabled=isDisabled, position=position, extension=extension, role=role, notification=notification,)
-        return Sender().send_request(request_data, by_user=by_user)
-
-    def change_password(self, by_user: User, oldPassword: str = None, newPassword: str = None):
-        """Change password
-        :return: No Content
-        """
-        request_data = Build(url="/api/accounts/change_password").put(
-            oldPassword=oldPassword, newPassword=newPassword,)
-        return Sender().send_request(request_data, by_user=by_user)
-
-    def substitutionId(self, by_user: User):
-        """Impersonate
-        :return: Access token model
-        """
-        request_data = Build(
-            url="/api/accounts/impersonate/{substitutionId}").post()
-        return Sender().send_request(request_data, by_user=by_user)
-
-    def unimpersonate(self, by_user: User):
-        """Unimpersonate
-        :return: Access token model
-        """
-        request_data = Build(url="/api/accounts/unimpersonate").post()
-        return Sender().send_request(request_data, by_user=by_user)
-
-    def debug_start(self, by_user: User):
-        """Debug start
-        :return: No Content
-        """
-        request_data = Build(url="/api/accounts/debug_start").post()
-        return Sender().send_request(request_data, by_user=by_user)
-
-    def debug_end(self, by_user: User):
-        """Debug end
-        :return: No Content
-        """
-        request_data = Build(url="/api/accounts/debug_end").post()
-        return Sender().send_request(request_data, by_user=by_user)
-
-    def substitutions(self, by_user: User):
-        """Get account substitutions
-        :return: User paging extended info
-        """
-        request_data = Build(url="/api/accounts/substitutions").get()
-        return Sender().send_request(request_data, by_user=by_user)
+from lementpro.builders import Build
+from lementpro.data.user import User
+from lementpro.sender import Sender
+from lementpro.data.usermodelextension import UserModelExtension
+from lementpro.data.usermodelnotification import UserModelNotification
+
+
+class Accounts:
+    """Service for working with Accounts in UserGate Public API"""
+
+    def login(self, by_user: User, login: str = None, password: str = None):
+        """Sign in by login
+        :return: Access token model
+        """
+        request_data = Build(url="/api/accounts/login").post(
+            login=login,
+            password=password,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def refresh_token(self, by_user: User, refreshToken: str = None):
+        """Refresh token
+        :return: Access token model
+        """
+        request_data = Build(url="/api/accounts/refresh_token").post(
+            refreshToken=refreshToken,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def logout(self, by_user: User):
+        """Sign out
+        :return: No Content
+        """
+        request_data = Build(url="/api/accounts/logout").post()
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def restore_password(self, by_user: User, login: str = None, companyId: int = None):
+        """Restore password
+        :return: No Content
+        """
+        request_data = Build(url="/api/accounts/restore_password").post(
+            login=login,
+            companyId=companyId,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def get_me(self, by_user: User):
+        """Get me
+        :return: Created BlockWork identifier
+        """
+        request_data = Build(url="/api/accounts/me").get()
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def patch_me(
+        self,
+        by_user: User,
+        userName: str = None,
+        password: str = None,
+        email: str = None,
+        firstName: str = None,
+        middleName: str = None,
+        lastName: str = None,
+        phoneNumber: str = None,
+        preferredLocale: str = None,
+        isDismissed: bool = None,
+        isDisabled: bool = None,
+        position: str = None,
+        extension: UserModelExtension = None,
+        role: str = None,
+        notification: UserModelNotification = None,
+    ):
+        """Partial update user
+        :return: No Content
+        """
+        request_data = Build(url="/api/accounts/me").patch(
+            userName=userName,
+            password=password,
+            email=email,
+            firstName=firstName,
+            middleName=middleName,
+            lastName=lastName,
+            phoneNumber=phoneNumber,
+            preferredLocale=preferredLocale,
+            isDismissed=isDismissed,
+            isDisabled=isDisabled,
+            position=position,
+            extension=extension,
+            role=role,
+            notification=notification,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def change_password(self, by_user: User, oldPassword: str = None, newPassword: str = None):
+        """Change password
+        :return: No Content
+        """
+        request_data = Build(url="/api/accounts/change_password").put(
+            oldPassword=oldPassword,
+            newPassword=newPassword,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def substitutionId(self, by_user: User, substitutionId: str):
+        """Impersonate
+        :return: Access token model
+        """
+        request_data = Build(url=f"/api/accounts/impersonate/{substitutionId}").post()
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def unimpersonate(self, by_user: User):
+        """Unimpersonate
+        :return: Access token model
+        """
+        request_data = Build(url="/api/accounts/unimpersonate").post()
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def debug_start(self, by_user: User):
+        """Debug start
+        :return: No Content
+        """
+        request_data = Build(url="/api/accounts/debug_start").post()
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def debug_end(self, by_user: User):
+        """Debug end
+        :return: No Content
+        """
+        request_data = Build(url="/api/accounts/debug_end").post()
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def substitutions(self, by_user: User):
+        """Get account substitutions
+        :return: User paging extended info
+        """
+        request_data = Build(url="/api/accounts/substitutions").get()
+        return Sender().send_request(request_data, by_user=by_user)
```

### Comparing `lementpro-0.1.7/lementpro/services/objects.py` & `lementpro-1.0.0/lementpro/services/objects.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,138 @@
-from lementpro.builders import Build
-from lementpro.data.user import User
-from lementpro.sender import Sender
-from lementpro.data.usergateobjectaddmodel import UserGateObjectAddModel
-
-
-class Objects:
-    """Service for working with Objects in UserGate Public API"""  
-    def get_objectId(self, by_user: User, objectId: int=None):
-        """Get object info by object identifier
-        :return: Object user info
-        """
-        request_data = Build(url="/api/objects/{objectId}").get(objectId=objectId,)
-        return Sender().send_request(request_data, by_user=by_user)
-          
-    def patch_objectId(self, by_user: User, correctParentDates: bool=None, objectAttributes: list=None):
-        """Partial update object by object identifier
-        :return: No content
-        """
-        request_data = Build(url="/api/objects/{objectId}").patch(correctParentDates=correctParentDates,objectAttributes=objectAttributes,)
-        return Sender().send_request(request_data, by_user=by_user)
-          
-    def related_objects(self, by_user: User, objectId: int=None, By: int=None, Page: int=None, Order: str=None, OrderBy: str=None, AttributeKnownId: str=None):
-        """
-        :return: Success
-        """
-        request_data = Build(url="/api/objects/{objectId}/related_objects").get(objectId=objectId,By=By,Page=Page,Order=Order,OrderBy=OrderBy,AttributeKnownId=AttributeKnownId,)
-        return Sender().send_request(request_data, by_user=by_user)
-          
-    def steps(self, by_user: User, objectId: int=None):
-        """Get all objects info of all steps by object id
-        :return: List of all objects info inside all steps, incl. steps itself
-        """
-        request_data = Build(url="/api/objects/{objectId}/steps").get(objectId=objectId,)
-        return Sender().send_request(request_data, by_user=by_user)
-          
-    def objects(self, by_user: User, name: str=None, objectTypeId: int=None, correctParentDates: bool=None, bimElementIds: list=None, objectAttributes: list=None):
-        """Create new object
-        :return: Archive action info
-        """
-        request_data = Build(url="/api/objects").post(name=name,objectTypeId=objectTypeId,correctParentDates=correctParentDates,bimElementIds=bimElementIds,objectAttributes=objectAttributes,)
-        return Sender().send_request(request_data, by_user=by_user)
-          
-    def actionId(self, by_user: User, dateEnd: str=None, userIds: list=None, comment: str=None, relatedObjectIds: list=None, relationAttributeKnownId: str=None, newObject: UserGateObjectAddModel=None):
-        """Execute object action.
-        :return: Archive action info
-        """
-        request_data = Build(url="/api/objects/{objectId}/{actionId}").post(dateEnd=dateEnd,userIds=userIds,comment=comment,relatedObjectIds=relatedObjectIds,relationAttributeKnownId=relationAttributeKnownId,newObject=newObject,)
-        return Sender().send_request(request_data, by_user=by_user)
-          
-    def favorite(self, by_user: User, objectIds: list=None, isFavorite: bool=None):
-        """Toggle favorite objects
-        :return: No content
-        """
-        request_data = Build(url="/api/objects/favorite").post(objectIds=objectIds,isFavorite=isFavorite,)
-        return Sender().send_request(request_data, by_user=by_user)
-          
-    def read(self, by_user: User, objectIds: list=None):
-        """Mark read pack of objects
-        :return: No content
-        """
-        request_data = Build(url="/api/objects/read").post(objectIds=objectIds,)
-        return Sender().send_request(request_data, by_user=by_user)
-          
-    def unread(self, by_user: User, objectIds: list=None):
-        """Mark unread pack of objects
-        :return: No content
-        """
-        request_data = Build(url="/api/objects/unread").post(objectIds=objectIds,)
-        return Sender().send_request(request_data, by_user=by_user)
-        
+from lementpro.builders import Build
+from lementpro.data.user import User
+from lementpro.sender import Sender
+from lementpro.data.usergateobjectaddmodel import UserGateObjectAddModel
+
+
+class Objects:
+    """Service for working with Objects in UserGate Public API"""
+
+    def get_objectId(self, by_user: User, objectId: int = None):
+        """Get object info by object identifier
+        :return: Object user info
+        """
+        request_data = Build(url="/api/objects/{objectId}").get(
+            objectId=objectId,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def patch_objectId(
+        self, by_user: User, objectId: str, correctParentDates: bool = None, objectAttributes: list = None
+    ):
+        """Partial update object by object identifier
+        :return: No content
+        """
+        request_data = Build(url="/api/objects/{objectId}").patch(
+            objectId=objectId,
+            correctParentDates=correctParentDates,
+            objectAttributes=objectAttributes,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def related_objects(
+        self,
+        by_user: User,
+        objectId: int = None,
+        By: int = None,
+        Page: int = None,
+        Order: str = None,
+        OrderBy: str = None,
+        AttributeKnownId: str = None,
+    ):
+        """
+        :return: Success
+        """
+        request_data = Build(url="/api/objects/{objectId}/related_objects").get(
+            objectId=objectId,
+            By=By,
+            Page=Page,
+            Order=Order,
+            OrderBy=OrderBy,
+            AttributeKnownId=AttributeKnownId,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def steps(self, by_user: User, objectId: int = None):
+        """Get all objects info of all steps by object id
+        :return: List of all objects info inside all steps, incl. steps itself
+        """
+        request_data = Build(url="/api/objects/{objectId}/steps").get(
+            objectId=objectId,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def objects(
+        self,
+        by_user: User,
+        name: str = None,
+        objectTypeId: int = None,
+        correctParentDates: bool = None,
+        bimElementIds: list = None,
+        objectAttributes: list = None,
+    ):
+        """Create new object
+        :return: Archive action info
+        """
+        request_data = Build(url="/api/objects").post(
+            name=name,
+            objectTypeId=objectTypeId,
+            correctParentDates=correctParentDates,
+            bimElementIds=bimElementIds,
+            objectAttributes=objectAttributes,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def actionId(
+        self,
+        by_user: User,
+        objectId: str,
+        actionId: str,
+        dateEnd: str = None,
+        userIds: list = None,
+        comment: str = None,
+        relatedObjectIds: list = None,
+        relationAttributeKnownId: str = None,
+        newObject: UserGateObjectAddModel = None,
+    ):
+        """Execute object action.
+        :return: Archive action info
+        """
+        request_data = Build(url="/api/objects/{objectId}/{actionId}").post(
+            objectId=objectId,
+            actionId=actionId,
+            dateEnd=dateEnd,
+            userIds=userIds,
+            comment=comment,
+            relatedObjectIds=relatedObjectIds,
+            relationAttributeKnownId=relationAttributeKnownId,
+            newObject=newObject,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def favorite(self, by_user: User, objectIds: list = None, isFavorite: bool = None):
+        """Toggle favorite objects
+        :return: No content
+        """
+        request_data = Build(url="/api/objects/favorite").post(
+            objectIds=objectIds,
+            isFavorite=isFavorite,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def read(self, by_user: User, objectIds: list = None):
+        """Mark read pack of objects
+        :return: No content
+        """
+        request_data = Build(url="/api/objects/read").post(
+            objectIds=objectIds,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def unread(self, by_user: User, objectIds: list = None):
+        """Mark unread pack of objects
+        :return: No content
+        """
+        request_data = Build(url="/api/objects/unread").post(
+            objectIds=objectIds,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
```

### Comparing `lementpro-0.1.7/lementpro/services/objecttypes.py` & `lementpro-1.0.0/lementpro/services/objecttypes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,78 @@
-from lementpro.builders import Build
-from lementpro.data.user import User
-from lementpro.sender import Sender
-
-
-class ObjectTypes:
-    """Service for working with ObjectTypes in UserGate Public API"""  
-    def object_template(self, by_user: User, objectTypeId: int=None, RelatedObjectId: int=None, RelatedObjectAttributeKnownId: str=None):
-        """Get objectType object template
-        :return: ObjectType attributes paging info
-        """
-        request_data = Build(url="/api/object_types/{objectTypeId}/object_template").get(objectTypeId=objectTypeId,RelatedObjectId=RelatedObjectId,RelatedObjectAttributeKnownId=RelatedObjectAttributeKnownId,)
-        return Sender().send_request(request_data, by_user=by_user)
-          
-    def tree(self, by_user: User, objectTypeId: int=None):
-        """Get object type tree.
-        :return: Object type info
-        """
-        request_data = Build(url="/api/object_types/{objectTypeId}/tree").get(objectTypeId=objectTypeId,)
-        return Sender().send_request(request_data, by_user=by_user)
-          
-    def objects(self, by_user: User, objectTypeId: int=None, By: int=None, Page: int=None, Order: str=None, OrderBy: str=None, IsAnySubTypeAvailable: bool=None, SearchPhrase: str=None, IsArchived: bool=None, ObjectIds: list=None):
-        """Get objectType objects.
-        :return: ObjectType objects paging info
-        """
-        request_data = Build(url="/api/object_types/{objectTypeId}/objects").get(objectTypeId=objectTypeId,By=By,Page=Page,Order=Order,OrderBy=OrderBy,IsAnySubTypeAvailable=IsAnySubTypeAvailable,SearchPhrase=SearchPhrase,IsArchived=IsArchived,ObjectIds=ObjectIds,)
-        return Sender().send_request(request_data, by_user=by_user)
-          
-    def ui_settings(self, by_user: User, objectTypeId: int=None):
-        """Get objectType ui settings.
-        :return: ObjectType attributes paging info
-        """
-        request_data = Build(url="/api/object_types/{objectTypeId}/ui_settings").get(objectTypeId=objectTypeId,)
-        return Sender().send_request(request_data, by_user=by_user)
-          
-    def menu(self, by_user: User):
-        """Get object_types menu
-        :return: Menu list
-        """
-        request_data = Build(url="/api/object_types/menu").get()
-        return Sender().send_request(request_data, by_user=by_user)
-        
+from lementpro.builders import Build
+from lementpro.data.user import User
+from lementpro.sender import Sender
+
+
+class ObjectTypes:
+    """Service for working with ObjectTypes in UserGate Public API"""
+
+    def object_template(
+        self,
+        by_user: User,
+        objectTypeId: int = None,
+        RelatedObjectId: int = None,
+        RelatedObjectAttributeKnownId: str = None,
+    ):
+        """Get objectType object template
+        :return: ObjectType attributes paging info
+        """
+        request_data = Build(url="/api/object_types/{objectTypeId}/object_template").get(
+            objectTypeId=objectTypeId,
+            RelatedObjectId=RelatedObjectId,
+            RelatedObjectAttributeKnownId=RelatedObjectAttributeKnownId,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def tree(self, by_user: User, objectTypeId: int = None):
+        """Get object type tree.
+        :return: Object type info
+        """
+        request_data = Build(url="/api/object_types/{objectTypeId}/tree").get(
+            objectTypeId=objectTypeId,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def objects(
+        self,
+        by_user: User,
+        objectTypeId: int = None,
+        By: int = None,
+        Page: int = None,
+        Order: str = None,
+        OrderBy: str = None,
+        IsAnySubTypeAvailable: bool = None,
+        SearchPhrase: str = None,
+        IsArchived: bool = None,
+        ObjectIds: list = None,
+    ):
+        """Get objectType objects.
+        :return: ObjectType objects paging info
+        """
+        request_data = Build(url="/api/object_types/{objectTypeId}/objects").get(
+            objectTypeId=objectTypeId,
+            By=By,
+            Page=Page,
+            Order=Order,
+            OrderBy=OrderBy,
+            IsAnySubTypeAvailable=IsAnySubTypeAvailable,
+            SearchPhrase=SearchPhrase,
+            IsArchived=IsArchived,
+            ObjectIds=ObjectIds,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def ui_settings(self, by_user: User, objectTypeId: int = None):
+        """Get objectType ui settings.
+        :return: ObjectType attributes paging info
+        """
+        request_data = Build(url="/api/object_types/{objectTypeId}/ui_settings").get(
+            objectTypeId=objectTypeId,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
+
+    def menu(self, by_user: User):
+        """Get object_types menu
+        :return: Menu list
+        """
+        request_data = Build(url="/api/object_types/menu").get()
+        return Sender().send_request(request_data, by_user=by_user)
```

### Comparing `lementpro-0.1.7/lementpro/services/timezones.py` & `lementpro-1.0.0/lementpro/services/timezones.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,28 @@
-from lementpro.builders import Build
-from lementpro.data.user import User
-from lementpro.sender import Sender
-
-
-class TimeZones:
-    """Service for working with TimeZones in UserGate Public API"""  
-    def timezones(self, by_user: User, By: int=None, Page: int=None, Order: str=None, OrderBy: str=None, SearchString: str=None):
-        """Get timezones by list
-        :return: TimeZones paging model
-        """
-        request_data = Build(url="/api/timezones").get(By=By,Page=Page,Order=Order,OrderBy=OrderBy,SearchString=SearchString,)
-        return Sender().send_request(request_data, by_user=by_user)
-        
+from lementpro.builders import Build
+from lementpro.data.user import User
+from lementpro.sender import Sender
+
+
+class TimeZones:
+    """Service for working with TimeZones in UserGate Public API"""
+
+    def timezones(
+        self,
+        by_user: User,
+        By: int = None,
+        Page: int = None,
+        Order: str = None,
+        OrderBy: str = None,
+        SearchString: str = None,
+    ):
+        """Get timezones by list
+        :return: TimeZones paging model
+        """
+        request_data = Build(url="/api/timezones").get(
+            By=By,
+            Page=Page,
+            Order=Order,
+            OrderBy=OrderBy,
+            SearchString=SearchString,
+        )
+        return Sender().send_request(request_data, by_user=by_user)
```

### Comparing `lementpro-0.1.7/lementpro.egg-info/SOURCES.txt` & `lementpro-1.0.0/lementpro.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -363,8 +363,12 @@
 lementpro/services/timezones.py
 lementpro/services/users.py
 src/templates/__init__.py
 src/templates/builders.py
 src/templates/logger.py
 src/templates/sender.py
 src/templates/user.py
-tests/test_sdk.py
+tests/test_unit/__init__.py
+tests/test_unit/conftest.py
+tests/test_unit/test_accounts.py
+tests/test_unit/test_companies.py
+tests/test_unit/test_users.py
```

### Comparing `lementpro-0.1.7/src/templates/builders.py` & `lementpro-1.0.0/src/templates/builders.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-import _io
-from dataclasses import dataclass
-from requests import Request
-
-
-@dataclass
-class Build:
-    url: str
-
-    def post(self, **kwargs):
-        prop = self.get_url(**kwargs)
-        return Request(method="post", url=self.url, json=prop)
-
-    def put(self, **kwargs):
-        prop = self.get_url(**kwargs)
-        return Request(method="put", url=self.url, json=prop)
-
-    def patch(self, **kwargs):
-        prop = self.get_url(**kwargs)
-        return Request(method="patch", url=self.url, json=prop)
-
-    def post_with_file(self, file: _io.BufferedReader, form_field_name: str, **kwargs):
-        file = {form_field_name: file}
-        return Request(method="post", url=self.url, data=kwargs, files=file)
-
-    def get(self, **kwargs):
-        prop = self.get_url(**kwargs)
-        return Request(method="get", url=self.url, json=prop)
-
-    def delete(self, **kwargs):
-        prop = self.get_url(**kwargs)
-        return Request(method="delete", url=self.url, json=prop)
-
-    def get_vars_from_path(self):
-        vars_ = list()
-        for part_way in self.url.split("/"):
-            if "{" in part_way:
-                vars_.append(part_way.replace("{", "").replace("}", ""))
-        return vars_
-
-    def get_url(self, **kwargs):
-        var_in_path = self.get_vars_from_path()
-        if var_in_path != list():
-            self.url = self.url.format(**kwargs)
-            for var in var_in_path:
-                kwargs.pop(var)
-        return kwargs
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+import _io
+from dataclasses import dataclass
+from requests import Request
+
+
+@dataclass
+class Build:
+    url: str
+
+    def post(self, **kwargs):
+        prop = self.get_url(**kwargs)
+        return Request(method="post", url=self.url, json=prop)
+
+    def put(self, **kwargs):
+        prop = self.get_url(**kwargs)
+        return Request(method="put", url=self.url, json=prop)
+
+    def patch(self, **kwargs):
+        prop = self.get_url(**kwargs)
+        return Request(method="patch", url=self.url, json=prop)
+
+    def post_with_file(self, file: _io.BufferedReader, form_field_name: str, **kwargs):
+        file = {form_field_name: file}
+        return Request(method="post", url=self.url, data=kwargs, files=file)
+
+    def get(self, **kwargs):
+        prop = self.get_url(**kwargs)
+        return Request(method="get", url=self.url, json=prop)
+
+    def delete(self, **kwargs):
+        prop = self.get_url(**kwargs)
+        return Request(method="delete", url=self.url, json=prop)
+
+    def get_vars_from_path(self):
+        vars_ = list()
+        for part_way in self.url.split("/"):
+            if "{" in part_way:
+                vars_.append(part_way.replace("{", "").replace("}", ""))
+        return vars_
+
+    def get_url(self, **kwargs):
+        var_in_path = self.get_vars_from_path()
+        if var_in_path != list():
+            self.url = self.url.format(**kwargs)
+            for var in var_in_path:
+                kwargs.pop(var)
+        return kwargs
```

### Comparing `lementpro-0.1.7/src/templates/sender.py` & `lementpro-1.0.0/src/templates/sender.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-import requests
-from requests import Session
-from .data.user import User
-from .logger import logger
-
-
-class Sender:
-
-    @staticmethod
-    def send_request(request_data, by_user=None):
-        session = Sender().__set_user(by_user=by_user)
-        request_data.url = by_user.root_url + request_data.url
-        prepped = session.prepare_request(request_data)
-        Sender.logging(prepped=prepped)
-        response = session.send(request=prepped, timeout=30, verify=True)
-        Sender.logging(prepped=response)
-        return response
-
-    @staticmethod
-    def __set_user(by_user: User):
-        session = Session()
-        if by_user and by_user.access_token is not None:
-            session.headers.update(Authorization=f'Bearer {by_user.access_token}')
-        if by_user and by_user.specific_headers is not {}:
-            session.headers.update(by_user.specific_headers)
-        if by_user and by_user.cookies is not None:
-            session.cookies = by_user.cookies
-        return session
-
-    @staticmethod
-    def logging(prepped):
-        if isinstance(prepped, requests.models.PreparedRequest):
-            url, method, headers, body = prepped.url, prepped.method, prepped.headers, prepped.body
-            info = f"sent request:\n url: {url}\n method: {method}\n headers: {headers}\n body: {body}\n "
-        else:
-            headers = prepped.headers
-            info = f"received response:\n code: {prepped.status_code} {prepped.reason} \n headers: {headers} \n content: {prepped.text}"
-        logger.debug("len logging =%s" % str(len(info)))
-        if len(info) < 10000:
-            logger.debug(f'\n\n{info}')
-        else:
-            logger.debug("Log is too large.")
-            logger.debug("Return only header = %s" % headers)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+import requests
+from requests import Session
+from .data.user import User
+from .logger import logger
+
+
+class Sender:
+    @staticmethod
+    def send_request(request_data, by_user=None):
+        session = Sender().__set_user(by_user=by_user)
+        request_data.url = by_user.root_url + request_data.url
+        prepped = session.prepare_request(request_data)
+        Sender.logging(prepped=prepped)
+        response = session.send(request=prepped, timeout=30, verify=True)
+        Sender.logging(prepped=response)
+        return response
+
+    @staticmethod
+    def __set_user(by_user: User):
+        session = Session()
+        if by_user and by_user.access_token is not None:
+            session.headers.update(Authorization=f"Bearer {by_user.access_token}")
+        if by_user and by_user.specific_headers is not {}:
+            session.headers.update(by_user.specific_headers)
+        if by_user and by_user.cookies is not None:
+            session.cookies = by_user.cookies
+        return session
+
+    @staticmethod
+    def logging(prepped):
+        if isinstance(prepped, requests.models.PreparedRequest):
+            url, method, headers, body = prepped.url, prepped.method, prepped.headers, prepped.body
+            info = f"sent request:\n url: {url}\n method: {method}\n headers: {headers}\n body: {body}\n "
+        else:
+            headers = prepped.headers
+            info = f"received response:\n code: {prepped.status_code} {prepped.reason} \n headers: {headers} \n content: {prepped.text}"
+        logger.debug("len logging =%s" % str(len(info)))
+        if len(info) < 10000:
+            logger.debug(f"\n\n{info}")
+        else:
+            logger.debug("Log is too large.")
+            logger.debug("Return only header = %s" % headers)
```

