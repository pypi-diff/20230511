# Comparing `tmp/testgear-api-client-3.0.0.tar.gz` & `tmp/testgear-api-client-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgear-api-client-3.0.0.tar", last modified: Wed Mar 22 12:38:23 2023, max compression
+gzip compressed data, was "testgear-api-client-3.1.0.tar", last modified: Thu May 11 08:31:41 2023, max compression
```

## Comparing `testgear-api-client-3.0.0.tar` & `testgear-api-client-3.1.0.tar`

### file list

```diff
@@ -1,541 +1,292 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 12:38:23.953594 testgear-api-client-3.0.0/
--rw-rw-rw-   0        0        0       57 2023-03-01 09:37:24.000000 testgear-api-client-3.0.0/.gitignore
--rw-rw-rw-   0        0        0     2720 2023-03-01 09:29:54.000000 testgear-api-client-3.0.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0    11539 2023-03-01 09:29:54.000000 testgear-api-client-3.0.0/LICENSE.md
--rw-rw-rw-   0        0        0    45982 2023-03-22 12:38:23.953594 testgear-api-client-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    42939 2023-03-01 09:42:23.000000 testgear-api-client-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-22 12:38:23.702606 testgear-api-client-3.0.0/docs/
--rw-rw-rw-   0        0        0      470 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AttachmentChangeViewModel.md
--rw-rw-rw-   0        0        0      554 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AttachmentChangeViewModelArrayWorkItemChangedFieldViewModel.md
--rw-rw-rw-   0        0        0      671 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AttachmentModel.md
--rw-rw-rw-   0        0        0     1519 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AttachmentModelAutoTestStepResultsModel.md
--rw-rw-rw-   0        0        0      357 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AttachmentPutModel.md
--rw-rw-rw-   0        0        0     1534 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AttachmentPutModelAutoTestStepResultsModel.md
--rw-rw-rw-   0        0        0      381 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AttachmentSubGetModel.md
--rw-rw-rw-   0        0        0    12241 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/AttachmentsApi.md
--rw-rw-rw-   0        0        0      421 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutoTestAverageDurationModel.md
--rw-rw-rw-   0        0        0      473 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutoTestChangeViewModel.md
--rw-rw-rw-   0        0        0      544 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutoTestChangeViewModelArrayWorkItemChangedFieldViewModel.md
--rw-rw-rw-   0        0        0      328 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutoTestIdModel.md
--rw-rw-rw-   0        0        0     2690 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutoTestModel.md
--rw-rw-rw-   0        0        0     1489 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutoTestModelV2GetModel.md
--rw-rw-rw-   0        0        0      400 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutoTestNamespaceModel.md
--rw-rw-rw-   0        0        0     1799 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutoTestPostModel.md
--rw-rw-rw-   0        0        0     1745 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutoTestPutModel.md
--rw-rw-rw-   0        0        0     2710 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutoTestResultsForTestRunModel.md
--rw-rw-rw-   0        0        0      515 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutoTestShortModel.md
--rw-rw-rw-   0        0        0      614 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutoTestStepModel.md
--rw-rw-rw-   0        0        0    91779 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/AutoTestsApi.md
--rw-rw-rw-   0        0        0     2091 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutotestFilterModel.md
--rw-rw-rw-   0        0        0      789 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutotestHistoricalResultSelectModel.md
--rw-rw-rw-   0        0        0     1092 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutotestResultHistoricalGetModel.md
--rw-rw-rw-   0        0        0      400 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutotestResultOutcome.md
--rw-rw-rw-   0        0        0      449 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutotestResultReasonSubGetModel.md
--rw-rw-rw-   0        0        0      478 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutotestSelectModel.md
--rw-rw-rw-   0        0        0      380 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutotestsExtractionModel.md
--rw-rw-rw-   0        0        0      489 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AutotestsSelectModel.md
--rw-rw-rw-   0        0        0      391 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/AvailableTestResultOutcome.md
--rw-rw-rw-   0        0        0      429 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/BooleanNullableTestPlanChangedFieldViewModel.md
--rw-rw-rw-   0        0        0      399 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/BooleanTestPlanChangedFieldViewModel.md
--rw-rw-rw-   0        0        0      399 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/BooleanWorkItemChangedFieldViewModel.md
--rw-rw-rw-   0        0        0      465 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/ConfigurationByParametersModel.md
--rw-rw-rw-   0        0        0     1116 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/ConfigurationModel.md
--rw-rw-rw-   0        0        0      700 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/ConfigurationPostModel.md
--rw-rw-rw-   0        0        0      722 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/ConfigurationPutModel.md
--rw-rw-rw-   0        0        0      754 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/docs/ConfigurationSelectModel.md
--rw-rw-rw-   0        0        0    18757 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/ConfigurationsApi.md
--rw-rw-rw-   0        0        0      670 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/CustomAttributeChangeModel.md
--rw-rw-rw-   0        0        0     1016 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/CustomAttributeGetModel.md
--rw-rw-rw-   0        0        0     1092 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/CustomAttributeModel.md
--rw-rw-rw-   0        0        0      632 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/CustomAttributeOptionModel.md
--rw-rw-rw-   0        0        0      481 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/CustomAttributeOptionPostModel.md
--rw-rw-rw-   0        0        0      960 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/CustomAttributePostModel.md
--rw-rw-rw-   0        0        0     1092 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/CustomAttributePutModel.md
--rw-rw-rw-   0        0        0      951 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/CustomAttributeSearchQueryModel.md
--rw-rw-rw-   0        0        0      440 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/CustomAttributeTemplateModel.md
--rw-rw-rw-   0        0        0      459 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/CustomAttributeTemplatePostModel.md
--rw-rw-rw-   0        0        0      516 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/CustomAttributeTemplatePutModel.md
--rw-rw-rw-   0        0        0      594 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/CustomAttributeTemplateSearchQueryModel.md
--rw-rw-rw-   0        0        0    30052 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/CustomAttributeTemplatesApi.md
--rw-rw-rw-   0        0        0      553 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/CustomAttributeTestPlanProjectRelationPutModel.md
--rw-rw-rw-   0        0        0      407 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/CustomAttributeTypesEnum.md
--rw-rw-rw-   0        0        0    17562 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/CustomAttributesApi.md
--rw-rw-rw-   0        0        0      438 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/DateRangeModel.md
--rw-rw-rw-   0        0        0      408 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/DateTimeRangeSelectorModel.md
--rw-rw-rw-   0        0        0      744 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ExternalLinkModel.md
--rw-rw-rw-   0        0        0      410 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/FailureCategoryModel.md
--rw-rw-rw-   0        0        0      895 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/FailureClassModel.md
--rw-rw-rw-   0        0        0      547 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/FailureClassRegexModel.md
--rw-rw-rw-   0        0        0      916 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/FilterModel.md
--rw-rw-rw-   0        0        0      428 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/FlakyBulkModel.md
--rw-rw-rw-   0        0        0     1034 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/GetXlsxTestPointsByTestPlanModel.md
--rw-rw-rw-   0        0        0      895 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/GlobalCustomAttributePostModel.md
--rw-rw-rw-   0        0        0      812 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/GlobalCustomAttributeUpdateModel.md
--rw-rw-rw-   0        0        0      402 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/GuidExtractionModel.md
--rw-rw-rw-   0        0        0      394 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/GuidWorkItemChangedFieldViewModel.md
--rw-rw-rw-   0        0        0      370 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ImageResizeType.md
--rw-rw-rw-   0        0        0      395 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/Int32RangeSelectorModel.md
--rw-rw-rw-   0        0        0      395 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/Int32WorkItemChangedFieldViewModel.md
--rw-rw-rw-   0        0        0      395 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/Int64RangeSelectorModel.md
--rw-rw-rw-   0        0        0      395 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/Int64WorkItemChangedFieldViewModel.md
--rw-rw-rw-   0        0        0      424 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/IterationModel.md
--rw-rw-rw-   0        0        0      413 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/IterationPutModel.md
--rw-rw-rw-   0        0        0      329 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/LabelPostModel.md
--rw-rw-rw-   0        0        0      371 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/LabelShortModel.md
--rw-rw-rw-   0        0        0      694 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/LastTestResultModel.md
--rw-rw-rw-   0        0        0      647 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/LinkModel.md
--rw-rw-rw-   0        0        0      617 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/LinkPostModel.md
--rw-rw-rw-   0        0        0      650 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/LinkPutModel.md
--rw-rw-rw-   0        0        0      387 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/LinkSubGetModel.md
--rw-rw-rw-   0        0        0      403 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/LinkType.md
--rw-rw-rw-   0        0        0      337 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/NoContentResult.md
--rw-rw-rw-   0        0        0     1059 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/NotificationModel.md
--rw-rw-rw-   0        0        0      554 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/NotificationQueryFilterModel.md
--rw-rw-rw-   0        0        0      445 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/NotificationTypeModel.md
--rw-rw-rw-   0        0        0    17652 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/NotificationsApi.md
--rw-rw-rw-   0        0        0      462 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ParameterGroupModel.md
--rw-rw-rw-   0        0        0      325 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ParameterIterationModel.md
--rw-rw-rw-   0        0        0      681 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ParameterModel.md
--rw-rw-rw-   0        0        0      348 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ParameterPostModel.md
--rw-rw-rw-   0        0        0      381 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ParameterPutModel.md
--rw-rw-rw-   0        0        0      431 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ParameterShortModel.md
--rw-rw-rw-   0        0        0    42974 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/ParametersApi.md
--rw-rw-rw-   0        0        0      408 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/PeriodViewModel.md
--rw-rw-rw-   0        0        0      473 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/PeriodViewModelTestPlanChangedFieldViewModel.md
--rw-rw-rw-   0        0        0      706 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ProblemDetails.md
--rw-rw-rw-   0        0        0      855 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ProjectAttributesFilterModel.md
--rw-rw-rw-   0        0        0      712 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ProjectCustomAttributeTemplateGetModel.md
--rw-rw-rw-   0        0        0      599 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ProjectCustomAttributesTemplatesFilterModel.md
--rw-rw-rw-   0        0        0      909 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ProjectExportQueryModel.md
--rw-rw-rw-   0        0        0      653 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ProjectExportWithTestPlansPostModel.md
--rw-rw-rw-   0        0        0     1726 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ProjectModel.md
--rw-rw-rw-   0        0        0      419 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ProjectPostModel.md
--rw-rw-rw-   0        0        0      465 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ProjectPutModel.md
--rw-rw-rw-   0        0        0      559 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ProjectShortestModel.md
--rw-rw-rw-   0        0        0   184972 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/ProjectsApi.md
--rw-rw-rw-   0        0        0     1287 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ProjectsFilterModel.md
--rw-rw-rw-   0        0        0      607 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/PublicTestPointModel.md
--rw-rw-rw-   0        0        0      929 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/PublicTestRunModel.md
--rw-rw-rw-   0        0        0      364 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/RequestTypeModel.md
--rw-rw-rw-   0        0        0      554 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/SearchAutoTestsQueryIncludesModel.md
--rw-rw-rw-   0        0        0      664 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/SearchCustomAttributeTemplateGetModel.md
--rw-rw-rw-   0        0        0      867 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/SearchWebhooksQueryModel.md
--rw-rw-rw-   0        0        0      710 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/SectionModel.md
--rw-rw-rw-   0        0        0      617 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/SectionMoveModel.md
--rw-rw-rw-   0        0        0      586 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/SectionPostModel.md
--rw-rw-rw-   0        0        0      608 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/SectionPutModel.md
--rw-rw-rw-   0        0        0      345 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/SectionRenameModel.md
--rw-rw-rw-   0        0        0      890 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/SectionWithStepsModel.md
--rw-rw-rw-   0        0        0    28128 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/SectionsApi.md
--rw-rw-rw-   0        0        0      534 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/SharedStepChangeViewModel.md
--rw-rw-rw-   0        0        0      539 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/SharedStepModel.md
--rw-rw-rw-   0        0        0     1331 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/SharedStepReferenceModel.md
--rw-rw-rw-   0        0        0      796 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/SharedStepReferenceSectionModel.md
--rw-rw-rw-   0        0        0      837 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/SharedStepReferenceSectionsQueryFilterModel.md
--rw-rw-rw-   0        0        0     1640 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/SharedStepReferencesQueryFilterModel.md
--rw-rw-rw-   0        0        0      389 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/SharedStepResultModel.md
--rw-rw-rw-   0        0        0      378 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ShortConfiguration.md
--rw-rw-rw-   0        0        0      798 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/StepCommentModel.md
--rw-rw-rw-   0        0        0      655 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/StepModel.md
--rw-rw-rw-   0        0        0      583 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/StepPutModel.md
--rw-rw-rw-   0        0        0      558 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/StepResultModel.md
--rw-rw-rw-   0        0        0      427 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/StringArrayTestPlanChangedFieldViewModel.md
--rw-rw-rw-   0        0        0      427 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/StringArrayWorkItemChangedFieldViewModel.md
--rw-rw-rw-   0        0        0      418 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/StringTestPlanChangedFieldViewModel.md
--rw-rw-rw-   0        0        0      418 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/StringWorkItemChangedFieldViewModel.md
--rw-rw-rw-   0        0        0      317 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TagShortModel.md
--rw-rw-rw-   0        0        0     6866 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/TagsApi.md
--rw-rw-rw-   0        0        0      601 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPlanChangeModel.md
--rw-rw-rw-   0        0        0     1974 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPlanChangedFieldsViewModel.md
--rw-rw-rw-   0        0        0      386 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPlanGroupByStatus.md
--rw-rw-rw-   0        0        0      443 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPlanGroupByTestSuite.md
--rw-rw-rw-   0        0        0      387 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPlanGroupByTester.md
--rw-rw-rw-   0        0        0      445 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPlanGroupByTesterAndStatus.md
--rw-rw-rw-   0        0        0      713 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPlanLink.md
--rw-rw-rw-   0        0        0     1723 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPlanModel.md
--rw-rw-rw-   0        0        0      929 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPlanPostModel.md
--rw-rw-rw-   0        0        0     1006 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPlanPutModel.md
--rw-rw-rw-   0        0        0     1317 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPlanSearchQueryModel.md
--rw-rw-rw-   0        0        0      420 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPlanShortModel.md
--rw-rw-rw-   0        0        0      386 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPlanStatusModel.md
--rw-rw-rw-   0        0        0     1825 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPlanWithAnalyticModel.md
--rw-rw-rw-   0        0        0     1852 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPlanWithTestSuiteTreeModel.md
--rw-rw-rw-   0        0        0    99257 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/TestPlansApi.md
--rw-rw-rw-   0        0        0      899 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPointAnalyticResult.md
--rw-rw-rw-   0        0        0      722 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPointByTestSuiteModel.md
--rw-rw-rw-   0        0        0      442 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPointChangeViewModel.md
--rw-rw-rw-   0        0        0      518 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPointChangeViewModelTestPlanChangedFieldViewModel.md
--rw-rw-rw-   0        0        0     2070 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPointFilterModel.md
--rw-rw-rw-   0        0        0      796 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPointPutModel.md
--rw-rw-rw-   0        0        0      787 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPointResultModel.md
--rw-rw-rw-   0        0        0      566 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPointSelector.md
--rw-rw-rw-   0        0        0     2435 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPointShortGetModel.md
--rw-rw-rw-   0        0        0      761 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPointShortModel.md
--rw-rw-rw-   0        0        0      407 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPointStatus.md
--rw-rw-rw-   0        0        0     1732 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestPointWithLastResultModel.md
--rw-rw-rw-   0        0        0    16661 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/TestPointsApi.md
--rw-rw-rw-   0        0        0      352 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestResultChangeViewModel.md
--rw-rw-rw-   0        0        0      523 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestResultChangeViewModelTestPlanChangedFieldViewModel.md
--rw-rw-rw-   0        0        0      391 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestResultChronologyModel.md
--rw-rw-rw-   0        0        0     3048 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestResultHistoryReportModel.md
--rw-rw-rw-   0        0        0     2535 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestResultModel.md
--rw-rw-rw-   0        0        0      396 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestResultOutcome.md
--rw-rw-rw-   0        0        0     1604 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestResultShortGetModel.md
--rw-rw-rw-   0        0        0      848 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestResultShortModel.md
--rw-rw-rw-   0        0        0      570 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestResultStepCommentPutModel.md
--rw-rw-rw-   0        0        0     1193 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestResultUpdateModel.md
--rw-rw-rw-   0        0        0     1676 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestResultV2GetModel.md
--rw-rw-rw-   0        0        0     1502 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestResultV2ShortModel.md
--rw-rw-rw-   0        0        0    44962 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/TestResultsApi.md
--rw-rw-rw-   0        0        0     1025 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestResultsFilterModel.md
--rw-rw-rw-   0        0        0      923 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestResultsLocalFilterModel.md
--rw-rw-rw-   0        0        0      552 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestResultsStatisticsGetModel.md
--rw-rw-rw-   0        0        0      564 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunAnalyticResultModel.md
--rw-rw-rw-   0        0        0      933 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunFillByAutoTestsPostModel.md
--rw-rw-rw-   0        0        0      950 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunFillByConfigurationsPostModel.md
--rw-rw-rw-   0        0        0     1061 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunFillByWorkItemsPostModel.md
--rw-rw-rw-   0        0        0      832 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunFilterModel.md
--rw-rw-rw-   0        0        0      406 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunGroupByFailureClassModel.md
--rw-rw-rw-   0        0        0      390 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunGroupByStatusModel.md
--rw-rw-rw-   0        0        0     1807 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunModel.md
--rw-rw-rw-   0        0        0      749 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunSearchQueryModel.md
--rw-rw-rw-   0        0        0     1317 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunShortGetModel.md
--rw-rw-rw-   0        0        0      698 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunShortModel.md
--rw-rw-rw-   0        0        0      387 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunState.md
--rw-rw-rw-   0        0        0      890 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunStatisticsErrorCategoriesGetModel.md
--rw-rw-rw-   0        0        0      759 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunStatisticsStatusesGetModel.md
--rw-rw-rw-   0        0        0      863 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunTestResultsPartialBulkSetModel.md
--rw-rw-rw-   0        0        0      510 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunTestResultsSelectModel.md
--rw-rw-rw-   0        0        0     1271 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunV2GetModel.md
--rw-rw-rw-   0        0        0      538 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunV2PostShortModel.md
--rw-rw-rw-   0        0        0      506 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestRunV2PutModel.md
--rw-rw-rw-   0        0        0    60531 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/TestRunsApi.md
--rw-rw-rw-   0        0        0      530 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestSuiteChangeViewModel.md
--rw-rw-rw-   0        0        0      518 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestSuiteChangeViewModelTestPlanChangedFieldViewModel.md
--rw-rw-rw-   0        0        0      442 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestSuiteV2GetModel.md
--rw-rw-rw-   0        0        0      409 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestSuiteV2PostModel.md
--rw-rw-rw-   0        0        0      398 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestSuiteV2PutModel.md
--rw-rw-rw-   0        0        0      581 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestSuiteV2TreeModel.md
--rw-rw-rw-   0        0        0      743 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestSuiteWithChildrenModel.md
--rw-rw-rw-   0        0        0     1943 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/TestSuiteWorkItemsSearchModel.md
--rw-rw-rw-   0        0        0    48014 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/TestSuitesApi.md
--rw-rw-rw-   0        0        0      581 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/UserRankModel.md
--rw-rw-rw-   0        0        0     1030 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/UserWithRankModel.md
--rw-rw-rw-   0        0        0      511 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ValidateAntiForgeryTokenAttribute.md
--rw-rw-rw-   0        0        0      777 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/docs/ValidationProblemDetails.md
--rw-rw-rw-   0        0        0      392 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WebHookEventType.md
--rw-rw-rw-   0        0        0      397 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WebHookEventTypeModel.md
--rw-rw-rw-   0        0        0     1280 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WebHookLogModel.md
--rw-rw-rw-   0        0        0     2191 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WebHookModel.md
--rw-rw-rw-   0        0        0     1464 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WebHookPostModel.md
--rw-rw-rw-   0        0        0    22565 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WebhooksApi.md
--rw-rw-rw-   0        0        0     9163 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WebhooksLogsApi.md
--rw-rw-rw-   0        0        0      693 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemChangeModel.md
--rw-rw-rw-   0        0        0      677 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemChangedAttributeViewModel.md
--rw-rw-rw-   0        0        0     2945 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemChangedFieldsViewModel.md
--rw-rw-rw-   0        0        0      666 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemCommentModel.md
--rw-rw-rw-   0        0        0      361 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemCommentPostModel.md
--rw-rw-rw-   0        0        0      393 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemCommentPutModel.md
--rw-rw-rw-   0        0        0      384 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemEntityTypes.md
--rw-rw-rw-   0        0        0     2595 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemFilterModel.md
--rw-rw-rw-   0        0        0      453 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemIdModel.md
--rw-rw-rw-   0        0        0      491 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemIdentifierModel.md
--rw-rw-rw-   0        0        0      686 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemLikeModel.md
--rw-rw-rw-   0        0        0      576 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemLinkChangeViewModel.md
--rw-rw-rw-   0        0        0      564 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemLinkChangeViewModelArrayWorkItemChangedFieldViewModel.md
--rw-rw-rw-   0        0        0     2222 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemModel.md
--rw-rw-rw-   0        0        0      475 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemMovePostModel.md
--rw-rw-rw-   0        0        0     1493 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemPostModel.md
--rw-rw-rw-   0        0        0      390 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemPriorityModel.md
--rw-rw-rw-   0        0        0     1284 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemPutModel.md
--rw-rw-rw-   0        0        0     2156 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemSearchQueryModel.md
--rw-rw-rw-   0        0        0      524 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemSelectModel.md
--rw-rw-rw-   0        0        0     1486 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemShortModel.md
--rw-rw-rw-   0        0        0      371 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemStates.md
--rw-rw-rw-   0        0        0      696 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemStepChangeViewModel.md
--rw-rw-rw-   0        0        0      564 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemStepChangeViewModelArrayWorkItemChangedFieldViewModel.md
--rw-rw-rw-   0        0        0      604 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemVersionModel.md
--rw-rw-rw-   0        0        0    91917 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemsApi.md
--rw-rw-rw-   0        0        0    12716 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemsCommentsApi.md
--rw-rw-rw-   0        0        0      605 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/docs/WorkItemsExtractionModel.md
-drwxrwxrwx   0        0        0        0 2023-03-22 12:38:23.702606 testgear-api-client-3.0.0/images/
--rw-rw-rw-   0        0        0   240535 2023-03-01 09:29:54.000000 testgear-api-client-3.0.0/images/banner.png
--rw-rw-rw-   0        0        0   482201 2023-03-01 09:29:54.000000 testgear-api-client-3.0.0/images/icon.png
--rw-rw-rw-   0        0        0       64 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-22 12:38:23.953594 testgear-api-client-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      692 2023-03-01 09:35:45.000000 testgear-api-client-3.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 12:38:23.391821 testgear-api-client-3.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-22 12:38:23.702606 testgear-api-client-3.0.0/src/testgear_api_client/
--rw-rw-rw-   0        0        0      801 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 12:38:23.736673 testgear-api-client-3.0.0/src/testgear_api_client/api/
--rw-rw-rw-   0        0        0      227 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/__init__.py
--rw-rw-rw-   0        0        0    22909 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/attachments_api.py
--rw-rw-rw-   0        0        0   120716 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/auto_tests_api.py
--rw-rw-rw-   0        0        0    28727 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/configurations_api.py
--rw-rw-rw-   0        0        0    46513 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/custom_attribute_templates_api.py
--rw-rw-rw-   0        0        0    28250 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/custom_attributes_api.py
--rw-rw-rw-   0        0        0    29065 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/notifications_api.py
--rw-rw-rw-   0        0        0    75479 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/parameters_api.py
--rw-rw-rw-   0        0        0   273080 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/projects_api.py
--rw-rw-rw-   0        0        0    40176 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/sections_api.py
--rw-rw-rw-   0        0        0    11887 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/tags_api.py
--rw-rw-rw-   0        0        0   148094 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/test_plans_api.py
--rw-rw-rw-   0        0        0    23857 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/test_points_api.py
--rw-rw-rw-   0        0        0    68539 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/test_results_api.py
--rw-rw-rw-   0        0        0    81994 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/test_runs_api.py
--rw-rw-rw-   0        0        0    68798 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/test_suites_api.py
--rw-rw-rw-   0        0        0    37242 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/webhooks_api.py
--rw-rw-rw-   0        0        0    17088 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/webhooks_logs_api.py
--rw-rw-rw-   0        0        0   129545 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/work_items_api.py
--rw-rw-rw-   0        0        0    21821 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api/work_items_comments_api.py
--rw-rw-rw-   0        0        0    39172 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/api_client.py
-drwxrwxrwx   0        0        0        0 2023-03-22 12:38:23.736673 testgear-api-client-3.0.0/src/testgear_api_client/apis/
--rw-rw-rw-   0        0        0     1730 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/apis/__init__.py
--rw-rw-rw-   0        0        0    17148 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/configuration.py
--rw-rw-rw-   0        0        0     5093 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-22 12:38:23.949592 testgear-api-client-3.0.0/src/testgear_api_client/model/
--rw-rw-rw-   0        0        0      353 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/__init__.py
--rw-rw-rw-   0        0        0    11789 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/attachment_change_view_model.py
--rw-rw-rw-   0        0        0    11941 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/attachment_change_view_model_array_work_item_changed_field_view_model.py
--rw-rw-rw-   0        0        0    13225 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/attachment_model.py
--rw-rw-rw-   0        0        0    14994 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/attachment_model_auto_test_step_results_model.py
--rw-rw-rw-   0        0        0    11268 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/attachment_put_model.py
--rw-rw-rw-   0        0        0    15034 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/attachment_put_model_auto_test_step_results_model.py
--rw-rw-rw-   0        0        0    11382 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/attachment_sub_get_model.py
--rw-rw-rw-   0        0        0    11578 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_average_duration_model.py
--rw-rw-rw-   0        0        0    11831 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_change_view_model.py
--rw-rw-rw-   0        0        0    11916 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_change_view_model_array_work_item_changed_field_view_model.py
--rw-rw-rw-   0        0        0    11153 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_id_model.py
--rw-rw-rw-   0        0        0    19927 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_model.py
--rw-rw-rw-   0        0        0    15822 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_model_v2_get_model.py
--rw-rw-rw-   0        0        0    11484 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_namespace_model.py
--rw-rw-rw-   0        0        0    16707 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_post_model.py
--rw-rw-rw-   0        0        0    16519 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_put_model.py
--rw-rw-rw-   0        0        0    18933 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_results_for_test_run_model.py
--rw-rw-rw-   0        0        0    12027 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_short_model.py
--rw-rw-rw-   0        0        0    12104 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_step_model.py
--rw-rw-rw-   0        0        0    17699 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/autotest_filter_model.py
--rw-rw-rw-   0        0        0    13533 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/autotest_historical_result_select_model.py
--rw-rw-rw-   0        0        0    14684 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/autotest_result_historical_get_model.py
--rw-rw-rw-   0        0        0    12227 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/autotest_result_outcome.py
--rw-rw-rw-   0        0        0    11721 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/autotest_result_reason_sub_get_model.py
--rw-rw-rw-   0        0        0    11881 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/autotest_select_model.py
--rw-rw-rw-   0        0        0    11418 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/autotests_extraction_model.py
--rw-rw-rw-   0        0        0    11911 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/autotests_select_model.py
--rw-rw-rw-   0        0        0    12146 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/available_test_result_outcome.py
--rw-rw-rw-   0        0        0    11548 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/boolean_nullable_test_plan_changed_field_view_model.py
--rw-rw-rw-   0        0        0    11458 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/boolean_test_plan_changed_field_view_model.py
--rw-rw-rw-   0        0        0    11458 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/boolean_work_item_changed_field_view_model.py
--rw-rw-rw-   0        0        0    11655 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/configuration_by_parameters_model.py
--rw-rw-rw-   0        0        0    14485 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/configuration_model.py
--rw-rw-rw-   0        0        0    12929 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/configuration_post_model.py
--rw-rw-rw-   0        0        0    13094 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/configuration_put_model.py
--rw-rw-rw-   0        0        0    12626 2023-03-01 09:21:11.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/configuration_select_model.py
--rw-rw-rw-   0        0        0    12533 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_change_model.py
--rw-rw-rw-   0        0        0    13706 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_get_model.py
--rw-rw-rw-   0        0        0    13980 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_model.py
--rw-rw-rw-   0        0        0    12249 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_option_model.py
--rw-rw-rw-   0        0        0    11719 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_option_post_model.py
--rw-rw-rw-   0        0        0    13501 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_post_model.py
--rw-rw-rw-   0        0        0    13983 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_put_model.py
--rw-rw-rw-   0        0        0    13592 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_search_query_model.py
--rw-rw-rw-   0        0        0    11778 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_template_model.py
--rw-rw-rw-   0        0        0    11813 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_template_post_model.py
--rw-rw-rw-   0        0        0    12050 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_template_put_model.py
--rw-rw-rw-   0        0        0    12425 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_template_search_query_model.py
--rw-rw-rw-   0        0        0    12089 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_test_plan_project_relation_put_model.py
--rw-rw-rw-   0        0        0    12260 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_types_enum.py
--rw-rw-rw-   0        0        0    11520 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/date_range_model.py
--rw-rw-rw-   0        0        0    11464 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/date_time_range_selector_model.py
--rw-rw-rw-   0        0        0    13028 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/external_link_model.py
--rw-rw-rw-   0        0        0    12278 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/failure_category_model.py
--rw-rw-rw-   0        0        0    13674 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/failure_class_model.py
--rw-rw-rw-   0        0        0    12015 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/failure_class_regex_model.py
--rw-rw-rw-   0        0        0    13718 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/filter_model.py
--rw-rw-rw-   0        0        0    11721 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/flaky_bulk_model.py
--rw-rw-rw-   0        0        0    14529 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/get_xlsx_test_points_by_test_plan_model.py
--rw-rw-rw-   0        0        0    13274 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/global_custom_attribute_post_model.py
--rw-rw-rw-   0        0        0    12834 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/global_custom_attribute_update_model.py
--rw-rw-rw-   0        0        0    11531 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/guid_extraction_model.py
--rw-rw-rw-   0        0        0    11443 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/guid_work_item_changed_field_view_model.py
--rw-rw-rw-   0        0        0    12029 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/image_resize_type.py
--rw-rw-rw-   0        0        0    11425 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/int32_range_selector_model.py
--rw-rw-rw-   0        0        0    11446 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/int32_work_item_changed_field_view_model.py
--rw-rw-rw-   0        0        0    11425 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/int64_range_selector_model.py
--rw-rw-rw-   0        0        0    11446 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/int64_work_item_changed_field_view_model.py
--rw-rw-rw-   0        0        0    11630 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/iteration_model.py
--rw-rw-rw-   0        0        0    11712 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/iteration_put_model.py
--rw-rw-rw-   0        0        0    11287 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/label_post_model.py
--rw-rw-rw-   0        0        0    11492 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/label_short_model.py
--rw-rw-rw-   0        0        0    12904 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/last_test_result_model.py
--rw-rw-rw-   0        0        0    12613 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/link_model.py
--rw-rw-rw-   0        0        0    12457 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/link_post_model.py
--rw-rw-rw-   0        0        0    12633 2023-03-01 13:28:19.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/link_put_model.py
--rw-rw-rw-   0        0        0    11402 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/link_sub_get_model.py
--rw-rw-rw-   0        0        0    12296 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/link_type.py
--rw-rw-rw-   0        0        0    11197 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/no_content_result.py
--rw-rw-rw-   0        0        0    14588 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/notification_model.py
--rw-rw-rw-   0        0        0    12213 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/notification_query_filter_model.py
--rw-rw-rw-   0        0        0    12485 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/notification_type_model.py
--rw-rw-rw-   0        0        0    11725 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/parameter_group_model.py
--rw-rw-rw-   0        0        0    11207 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/parameter_iteration_model.py
--rw-rw-rw-   0        0        0    13184 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/parameter_model.py
--rw-rw-rw-   0        0        0    11600 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/parameter_post_model.py
--rw-rw-rw-   0        0        0    11765 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/parameter_put_model.py
--rw-rw-rw-   0        0        0    12007 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/parameter_short_model.py
--rw-rw-rw-   0        0        0    11485 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/period_view_model.py
--rw-rw-rw-   0        0        0    11717 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/period_view_model_test_plan_changed_field_view_model.py
--rw-rw-rw-   0        0        0    12357 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/problem_details.py
--rw-rw-rw-   0        0        0    12982 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/project_attributes_filter_model.py
--rw-rw-rw-   0        0        0    12527 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/project_custom_attribute_template_get_model.py
--rw-rw-rw-   0        0        0    12052 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/project_custom_attributes_templates_filter_model.py
--rw-rw-rw-   0        0        0    12458 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/project_export_query_model.py
--rw-rw-rw-   0        0        0    11828 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/project_export_with_test_plans_post_model.py
--rw-rw-rw-   0        0        0    16399 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/project_model.py
--rw-rw-rw-   0        0        0    11611 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/project_post_model.py
--rw-rw-rw-   0        0        0    11826 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/project_put_model.py
--rw-rw-rw-   0        0        0    11997 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/project_shortest_model.py
--rw-rw-rw-   0        0        0    14706 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/projects_filter_model.py
--rw-rw-rw-   0        0        0    12494 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/public_test_point_model.py
--rw-rw-rw-   0        0        0    13939 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/public_test_run_model.py
--rw-rw-rw-   0        0        0    12002 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/request_type_model.py
--rw-rw-rw-   0        0        0    11937 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/search_auto_tests_query_includes_model.py
--rw-rw-rw-   0        0        0    12698 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/search_custom_attribute_template_get_model.py
--rw-rw-rw-   0        0        0    13278 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/search_webhooks_query_model.py
--rw-rw-rw-   0        0        0    13092 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/section_model.py
--rw-rw-rw-   0        0        0    12321 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/section_move_model.py
--rw-rw-rw-   0        0        0    12578 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/section_post_model.py
--rw-rw-rw-   0        0        0    12743 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/section_put_model.py
--rw-rw-rw-   0        0        0    11474 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/section_rename_model.py
--rw-rw-rw-   0        0        0    13876 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/section_with_steps_model.py
--rw-rw-rw-   0        0        0    12110 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/shared_step_change_view_model.py
--rw-rw-rw-   0        0        0    12199 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/shared_step_model.py
--rw-rw-rw-   0        0        0    15804 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/shared_step_reference_model.py
--rw-rw-rw-   0        0        0    13314 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/shared_step_reference_section_model.py
--rw-rw-rw-   0        0        0    13000 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/shared_step_reference_sections_query_filter_model.py
--rw-rw-rw-   0        0        0    15921 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/shared_step_references_query_filter_model.py
--rw-rw-rw-   0        0        0    11421 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/shared_step_result_model.py
--rw-rw-rw-   0        0        0    11373 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/short_configuration.py
--rw-rw-rw-   0        0        0    13614 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/step_comment_model.py
--rw-rw-rw-   0        0        0    12803 2023-03-01 13:29:07.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/step_model.py
--rw-rw-rw-   0        0        0    12311 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/step_put_model.py
--rw-rw-rw-   0        0        0    12239 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/step_result_model.py
--rw-rw-rw-   0        0        0    11542 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/string_array_test_plan_changed_field_view_model.py
--rw-rw-rw-   0        0        0    11542 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/string_array_work_item_changed_field_view_model.py
--rw-rw-rw-   0        0        0    11515 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/string_test_plan_changed_field_view_model.py
--rw-rw-rw-   0        0        0    11515 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/string_work_item_changed_field_view_model.py
--rw-rw-rw-   0        0        0    11290 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/tag_short_model.py
--rw-rw-rw-   0        0        0    12455 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_change_model.py
--rw-rw-rw-   0        0        0    17462 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_changed_fields_view_model.py
--rw-rw-rw-   0        0        0    11407 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_group_by_status.py
--rw-rw-rw-   0        0        0    11680 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_group_by_test_suite.py
--rw-rw-rw-   0        0        0    11411 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_group_by_tester.py
--rw-rw-rw-   0        0        0    11659 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_group_by_tester_and_status.py
--rw-rw-rw-   0        0        0    12992 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_link.py
--rw-rw-rw-   0        0        0    17636 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_model.py
--rw-rw-rw-   0        0        0    14320 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_post_model.py
--rw-rw-rw-   0        0        0    14734 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_put_model.py
--rw-rw-rw-   0        0        0    15813 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_search_query_model.py
--rw-rw-rw-   0        0        0    11580 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_short_model.py
--rw-rw-rw-   0        0        0    12137 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_status_model.py
--rw-rw-rw-   0        0        0    18090 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_with_analytic_model.py
--rw-rw-rw-   0        0        0    18180 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_with_test_suite_tree_model.py
--rw-rw-rw-   0        0        0    13577 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_analytic_result.py
--rw-rw-rw-   0        0        0    12788 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_by_test_suite_model.py
--rw-rw-rw-   0        0        0    11675 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_change_view_model.py
--rw-rw-rw-   0        0        0    11836 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_change_view_model_test_plan_changed_field_view_model.py
--rw-rw-rw-   0        0        0    17768 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_filter_model.py
--rw-rw-rw-   0        0        0    13187 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_put_model.py
--rw-rw-rw-   0        0        0    13267 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_result_model.py
--rw-rw-rw-   0        0        0    12025 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_selector.py
--rw-rw-rw-   0        0        0    18780 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_short_get_model.py
--rw-rw-rw-   0        0        0    12991 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_short_model.py
--rw-rw-rw-   0        0        0    12299 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_status.py
--rw-rw-rw-   0        0        0    17594 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_with_last_result_model.py
--rw-rw-rw-   0        0        0    11251 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_change_view_model.py
--rw-rw-rw-   0        0        0    11849 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_change_view_model_test_plan_changed_field_view_model.py
--rw-rw-rw-   0        0        0    11424 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_chronology_model.py
--rw-rw-rw-   0        0        0    20391 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_history_report_model.py
--rw-rw-rw-   0        0        0    20738 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_model.py
--rw-rw-rw-   0        0        0    12215 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_outcome.py
--rw-rw-rw-   0        0        0    15838 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_short_get_model.py
--rw-rw-rw-   0        0        0    13584 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_short_model.py
--rw-rw-rw-   0        0        0    12395 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_step_comment_put_model.py
--rw-rw-rw-   0        0        0    14847 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_update_model.py
--rw-rw-rw-   0        0        0    17228 2023-03-01 13:27:25.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_v2_get_model.py
--rw-rw-rw-   0        0        0    16310 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_v2_short_model.py
--rw-rw-rw-   0        0        0    13948 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_results_filter_model.py
--rw-rw-rw-   0        0        0    13564 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_results_local_filter_model.py
--rw-rw-rw-   0        0        0    12148 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_results_statistics_get_model.py
--rw-rw-rw-   0        0        0    12207 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_analytic_result_model.py
--rw-rw-rw-   0        0        0    13477 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_fill_by_auto_tests_post_model.py
--rw-rw-rw-   0        0        0    13594 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_fill_by_configurations_post_model.py
--rw-rw-rw-   0        0        0    13857 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_fill_by_work_items_post_model.py
--rw-rw-rw-   0        0        0    13132 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_filter_model.py
--rw-rw-rw-   0        0        0    11486 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_group_by_failure_class_model.py
--rw-rw-rw-   0        0        0    11419 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_group_by_status_model.py
--rw-rw-rw-   0        0        0    18016 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_model.py
--rw-rw-rw-   0        0        0    13132 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_search_query_model.py
--rw-rw-rw-   0        0        0    14881 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_short_get_model.py
--rw-rw-rw-   0        0        0    12795 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_short_model.py
--rw-rw-rw-   0        0        0    12164 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_state.py
--rw-rw-rw-   0        0        0    12888 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_statistics_error_categories_get_model.py
--rw-rw-rw-   0        0        0    12533 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_statistics_statuses_get_model.py
--rw-rw-rw-   0        0        0    13222 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_test_results_partial_bulk_set_model.py
--rw-rw-rw-   0        0        0    12011 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_test_results_select_model.py
--rw-rw-rw-   0        0        0    15358 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_v2_get_model.py
--rw-rw-rw-   0        0        0    12104 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_v2_post_short_model.py
--rw-rw-rw-   0        0        0    12049 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_v2_put_model.py
--rw-rw-rw-   0        0        0    12114 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_suite_change_view_model.py
--rw-rw-rw-   0        0        0    11836 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_suite_change_view_model_test_plan_changed_field_view_model.py
--rw-rw-rw-   0        0        0    11988 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_suite_v2_get_model.py
--rw-rw-rw-   0        0        0    11823 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_suite_v2_post_model.py
--rw-rw-rw-   0        0        0    11712 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_suite_v2_put_model.py
--rw-rw-rw-   0        0        0    12365 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_suite_v2_tree_model.py
--rw-rw-rw-   0        0        0    12721 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_suite_with_children_model.py
--rw-rw-rw-   0        0        0    17169 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/test_suite_work_items_search_model.py
--rw-rw-rw-   0        0        0    12402 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/user_rank_model.py
--rw-rw-rw-   0        0        0    14454 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/user_with_rank_model.py
--rw-rw-rw-   0        0        0    11870 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/validate_anti_forgery_token_attribute.py
--rw-rw-rw-   0        0        0    12644 2023-03-01 09:21:12.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/validation_problem_details.py
--rw-rw-rw-   0        0        0    12158 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/web_hook_event_type.py
--rw-rw-rw-   0        0        0    12173 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/web_hook_event_type_model.py
--rw-rw-rw-   0        0        0    15487 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/web_hook_log_model.py
--rw-rw-rw-   0        0        0    18015 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/web_hook_model.py
--rw-rw-rw-   0        0        0    16025 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/web_hook_post_model.py
--rw-rw-rw-   0        0        0    12907 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_change_model.py
--rw-rw-rw-   0        0        0    12554 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_changed_attribute_view_model.py
--rw-rw-rw-   0        0        0    20377 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_changed_fields_view_model.py
--rw-rw-rw-   0        0        0    12759 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_comment_model.py
--rw-rw-rw-   0        0        0    11601 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_comment_post_model.py
--rw-rw-rw-   0        0        0    11580 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_comment_put_model.py
--rw-rw-rw-   0        0        0    12113 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_entity_types.py
--rw-rw-rw-   0        0        0    19538 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_filter_model.py
--rw-rw-rw-   0        0        0    11418 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_id_model.py
--rw-rw-rw-   0        0        0    11611 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_identifier_model.py
--rw-rw-rw-   0        0        0    12689 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_like_model.py
--rw-rw-rw-   0        0        0    12268 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_link_change_view_model.py
--rw-rw-rw-   0        0        0    11969 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_link_change_view_model_array_work_item_changed_field_view_model.py
--rw-rw-rw-   0        0        0    20491 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_model.py
--rw-rw-rw-   0        0        0    12031 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_move_post_model.py
--rw-rw-rw-   0        0        0    17526 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_post_model.py
--rw-rw-rw-   0        0        0    12167 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_priority_model.py
--rw-rw-rw-   0        0        0    16590 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_put_model.py
--rw-rw-rw-   0        0        0    18246 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_search_query_model.py
--rw-rw-rw-   0        0        0    11883 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_select_model.py
--rw-rw-rw-   0        0        0    16737 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_short_model.py
--rw-rw-rw-   0        0        0    12050 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_states.py
--rw-rw-rw-   0        0        0    12850 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_step_change_view_model.py
--rw-rw-rw-   0        0        0    11969 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_step_change_view_model_array_work_item_changed_field_view_model.py
--rw-rw-rw-   0        0        0    12169 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_version_model.py
--rw-rw-rw-   0        0        0    11938 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model/work_items_extraction_model.py
--rw-rw-rw-   0        0        0    82625 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/model_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-22 12:38:23.951592 testgear-api-client-3.0.0/src/testgear_api_client/models/
--rw-rw-rw-   0        0        0    21703 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/models/__init__.py
--rw-rw-rw-   0        0        0    14302 2023-03-01 09:21:13.000000 testgear-api-client-3.0.0/src/testgear_api_client/rest.py
-drwxrwxrwx   0        0        0        0 2023-03-22 12:38:23.702606 testgear-api-client-3.0.0/src/testgear_api_client.egg-info/
--rw-rw-rw-   0        0        0    45982 2023-03-22 12:38:22.000000 testgear-api-client-3.0.0/src/testgear_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    24105 2023-03-22 12:38:23.000000 testgear-api-client-3.0.0/src/testgear_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 12:38:22.000000 testgear-api-client-3.0.0/src/testgear_api_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-03-22 12:38:22.000000 testgear-api-client-3.0.0/src/testgear_api_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-03-22 12:38:22.000000 testgear-api-client-3.0.0/src/testgear_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:31:41.743655 testgear-api-client-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    47971 2023-05-11 08:31:41.743655 testgear-api-client-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    47663 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 08:31:41.743655 testgear-api-client-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:31:41.671655 testgear-api-client-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:31:41.675655 testgear-api-client-3.1.0/src/testgear_api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:31:41.683655 testgear-api-client-3.1.0/src/testgear_api_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126095 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/auto_tests_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/background_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34218 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/configurations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46513 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/custom_attribute_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28250 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/custom_attributes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29065 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81825 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/parameters_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   332767 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45551 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   164728 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/test_plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23857 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/test_points_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68539 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/test_results_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81994 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/test_runs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79236 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/test_suites_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37242 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/webhooks_logs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144889 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/work_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21821 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api/work_items_comments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39172 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:31:41.683655 testgear-api-client-3.1.0/src/testgear_api_client/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:31:41.739655 testgear-api-client-3.1.0/src/testgear_api_client/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/api_v2_attachments_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/attachment_change_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/attachment_change_view_model_array_work_item_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/attachment_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/attachment_model_auto_test_step_results_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/attachment_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15034 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/attachment_put_model_auto_test_step_results_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/attachment_sub_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_average_duration_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11831 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_change_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_change_view_model_array_work_item_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11153 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15822 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_model_v2_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_namespace_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16707 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18873 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_results_for_test_run_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_step_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/autotest_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/autotest_historical_result_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/autotest_result_historical_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/autotest_result_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/autotest_result_reason_sub_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/autotest_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/autotests_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/autotests_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/available_test_result_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/background_job_attachment_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13796 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/background_job_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/background_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13745 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/background_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/boolean_nullable_test_plan_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/boolean_test_plan_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/boolean_work_item_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/configuration_by_parameters_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/configuration_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/configuration_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/configuration_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_change_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13748 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_option_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_option_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_search_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_template_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_template_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_template_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_template_search_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_test_plan_project_relation_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_types_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/date_time_range_selector_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/deletion_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/external_link_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/failure_category_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/failure_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/failure_class_regex_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/flaky_bulk_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14529 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/get_xlsx_test_points_by_test_plan_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13274 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/global_custom_attribute_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12834 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/global_custom_attribute_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/guid_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/guid_work_item_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/image_resize_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/int32_range_selector_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/int32_work_item_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/int64_range_selector_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/int64_work_item_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/iteration_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11712 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/iteration_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/label_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/label_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/last_test_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/link_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/link_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/link_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/link_sub_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/link_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/no_content_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14708 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/notification_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/notification_query_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/notification_type_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/parameter_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/parameter_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/parameter_iteration_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13184 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/parameter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/parameter_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/parameter_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/parameter_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/period_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/period_view_model_test_plan_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12357 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/project_attributes_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/project_custom_attribute_template_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/project_custom_attributes_templates_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/project_export_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/project_export_with_test_plans_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16333 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/project_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/project_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/project_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/project_shortest_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/project_test_plans_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14706 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/projects_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/public_test_point_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/public_test_run_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/request_type_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/search_auto_tests_query_includes_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/search_custom_attribute_template_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/search_webhooks_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/section_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/section_move_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/section_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/section_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/section_rename_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/section_with_steps_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/shared_step_change_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12199 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/shared_step_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/shared_step_reference_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13314 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/shared_step_reference_section_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/shared_step_reference_sections_query_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/shared_step_references_query_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/shared_step_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/short_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/step_comment_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12709 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/step_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/step_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/step_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/string_array_test_plan_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/string_array_work_item_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11515 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/string_test_plan_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11515 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/string_work_item_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/tag_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_change_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17462 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_changed_fields_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_group_by_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11680 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_group_by_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_group_by_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_group_by_tester_and_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17663 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14323 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18117 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_with_analytic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18207 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_with_test_suite_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13577 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_analytic_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_by_test_suite_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_change_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11836 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_change_view_model_test_plan_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18173 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_short_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17660 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_with_last_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_points_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_change_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11849 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_change_view_model_test_plan_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_chronology_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20361 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_history_report_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20678 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_short_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_step_comment_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17074 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_v2_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16250 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_v2_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13948 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_results_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_results_local_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_results_statistics_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_analytic_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_fill_by_auto_tests_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_fill_by_configurations_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_fill_by_work_items_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_group_by_failure_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_group_by_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18094 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_search_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_short_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12888 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_statistics_error_categories_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_statistics_statuses_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_test_results_partial_bulk_set_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12011 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_test_results_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_v2_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_v2_post_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_v2_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12114 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_change_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11836 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_change_view_model_test_plan_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_v2_get_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_v2_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_v2_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_v2_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_with_children_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17139 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_work_items_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12402 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/user_rank_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/user_with_rank_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/validate_anti_forgery_token_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/validation_problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/web_hook_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/web_hook_event_type_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15625 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/web_hook_log_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/web_hook_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15965 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/web_hook_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_change_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12554 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_changed_attribute_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20377 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_changed_fields_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_comment_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_comment_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_comment_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_entity_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19538 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_identifier_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_like_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_link_change_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_link_change_view_model_array_work_item_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12031 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_move_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_post_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_priority_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_put_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18246 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_search_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17177 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_short_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_step_change_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_step_change_view_model_array_work_item_changed_field_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_version_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model/work_items_extraction_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82625 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:31:41.739655 testgear-api-client-3.1.0/src/testgear_api_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    22519 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14302 2023-05-11 08:31:22.000000 testgear-api-client-3.1.0/src/testgear_api_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:31:41.675655 testgear-api-client-3.1.0/src/testgear_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47971 2023-05-11 08:31:41.000000 testgear-api-client-3.1.0/src/testgear_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-05-11 08:31:41.000000 testgear-api-client-3.1.0/src/testgear_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:31:41.000000 testgear-api-client-3.1.0/src/testgear_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 08:31:41.000000 testgear-api-client-3.1.0/src/testgear_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 08:31:41.000000 testgear-api-client-3.1.0/src/testgear_api_client.egg-info/top_level.txt
```

### Comparing `testgear-api-client-3.0.0/LICENSE.md` & `testgear-api-client-3.1.0/LICENSE.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2022 TestGear
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2022 TestGear
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
    limitations under the License.
```

### Comparing `testgear-api-client-3.0.0/PKG-INFO` & `testgear-api-client-3.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,312 +1,336 @@
-Metadata-Version: 2.1
-Name: testgear-api-client
-Version: 3.0.0
-Summary: API-client for Test Gear
-Home-page: https://pypi.org/project/testgear-api-client/
-Author: Integration team
-Author-email: integrations@test-gear.io
-License: UNKNOWN
-Description: # Api client for Test Gear TMS
-        ![Test Gear](https://raw.githubusercontent.com/testgear-tms/api-client-python/master/images/banner.png)
-        
-        ## Getting Started
-        
-        ### Compatibility
-        
-        | Test Gear | API Client |
-        |-----------|------------|
-        | 3.5       | 2.0        |
-        | 4.0       | 3.0        |
-        
-        ## Installation & Usage
-        ### pip install
-        
-        ```sh
-        pip install testgear-api-client
-        ```
-        
-        Then import the package:
-        
-        ```python
-        import testgear_api_client
-        ```
-        
-        ## Getting Started
-        
-        Please follow the [installation procedure](#installation--usage) and then run the following:
-        
-        ```python
-        import testgear_api_client
-        from testgear_api_client.api import attachments_api
-        from testgear_api_client.model.attachment_model import AttachmentModel
-        from testgear_api_client.model.image_resize_type import ImageResizeType
-        from testgear_api_client.model.problem_details import ProblemDetails
-        from testgear_api_client.model.validation_problem_details import ValidationProblemDetails
-        
-        configuration = testgear_api_client.Configuration(
-            host = "Your TMS address"
-        )
-        
-        with testgear_api_client.ApiClient(
-                configuration,
-                header_name='Authorization',
-                header_value='PrivateToken ' + 'Your private token') as api_client:
-            api_instance = attachments_api.AttachmentsApi(api_client)
-            id = "Attachment's guid in the TMS"
-        
-            try:
-                api_instance.api_v2_attachments_id_delete(id)
-            except testgear_api_client.ApiException as e:
-                print("Exception when calling AttachmentsApi->api_v2_attachments_id_delete: %s\n" % e)
-        ```
-        
-        ## Documentation for API Endpoints
-        
-        All URIs are relative to *http://localhost*
-        
-        Class | Method | HTTP request | Description
-        ------------ | ------------- | ------------- | -------------
-        *AttachmentsApi* | [**api_v2_attachments_id_delete**](docs/AttachmentsApi.md#api_v2_attachments_id_delete) | **DELETE** /api/v2/attachments/{id} | Delete attachment file
-        *AttachmentsApi* | [**api_v2_attachments_id_get**](docs/AttachmentsApi.md#api_v2_attachments_id_get) | **GET** /api/v2/attachments/{id} | Download attachment file
-        *AttachmentsApi* | [**api_v2_attachments_occupied_file_storage_size_get**](docs/AttachmentsApi.md#api_v2_attachments_occupied_file_storage_size_get) | **GET** /api/v2/attachments/occupiedFileStorageSize | Get size of attachments storage in bytes
-        *AttachmentsApi* | [**api_v2_attachments_post**](docs/AttachmentsApi.md#api_v2_attachments_post) | **POST** /api/v2/attachments | Upload new attachment file
-        *AutoTestsApi* | [**api_v2_auto_tests_flaky_bulk_post**](docs/AutoTestsApi.md#api_v2_auto_tests_flaky_bulk_post) | **POST** /api/v2/autoTests/flaky/bulk | Set \&quot;Flaky\&quot; status for multiple autotests
-        *AutoTestsApi* | [**api_v2_auto_tests_id_test_results_search_post**](docs/AutoTestsApi.md#api_v2_auto_tests_id_test_results_search_post) | **POST** /api/v2/autoTests/{id}/testResults/search | Get test results history for autotest
-        *AutoTestsApi* | [**api_v2_auto_tests_id_work_items_changed_id_get**](docs/AutoTestsApi.md#api_v2_auto_tests_id_work_items_changed_id_get) | **GET** /api/v2/autoTests/{id}/workItems/changed/id | Get identifiers of changed linked work items
-        *AutoTestsApi* | [**api_v2_auto_tests_id_work_items_changed_work_item_id_approve_post**](docs/AutoTestsApi.md#api_v2_auto_tests_id_work_items_changed_work_item_id_approve_post) | **POST** /api/v2/autoTests/{id}/workItems/changed/{workItemId}/approve | Approve changes to work items linked to autotest
-        *AutoTestsApi* | [**api_v2_auto_tests_search_post**](docs/AutoTestsApi.md#api_v2_auto_tests_search_post) | **POST** /api/v2/autoTests/search | Search for autotests
-        *AutoTestsApi* | [**create_auto_test**](docs/AutoTestsApi.md#create_auto_test) | **POST** /api/v2/autoTests | Create autotest
-        *AutoTestsApi* | [**create_multiple**](docs/AutoTestsApi.md#create_multiple) | **POST** /api/v2/autoTests/bulk | Create multiple autotests
-        *AutoTestsApi* | [**delete_auto_test**](docs/AutoTestsApi.md#delete_auto_test) | **DELETE** /api/v2/autoTests/{id} | Delete autotest
-        *AutoTestsApi* | [**delete_auto_test_link_from_work_item**](docs/AutoTestsApi.md#delete_auto_test_link_from_work_item) | **DELETE** /api/v2/autoTests/{id}/workItems | Unlink autotest from work item
-        *AutoTestsApi* | [**get_all_auto_tests**](docs/AutoTestsApi.md#get_all_auto_tests) | **GET** /api/v2/autoTests | 
-        *AutoTestsApi* | [**get_auto_test_average_duration**](docs/AutoTestsApi.md#get_auto_test_average_duration) | **GET** /api/v2/autoTests/{id}/averageDuration | Get average autotest duration
-        *AutoTestsApi* | [**get_auto_test_by_id**](docs/AutoTestsApi.md#get_auto_test_by_id) | **GET** /api/v2/autoTests/{id} | Get autotest by internal or global ID
-        *AutoTestsApi* | [**get_auto_test_chronology**](docs/AutoTestsApi.md#get_auto_test_chronology) | **GET** /api/v2/autoTests/{id}/chronology | Get autotest chronology
-        *AutoTestsApi* | [**get_test_runs**](docs/AutoTestsApi.md#get_test_runs) | **GET** /api/v2/autoTests/{id}/testRuns | Get completed tests runs for autotests
-        *AutoTestsApi* | [**get_work_item_results**](docs/AutoTestsApi.md#get_work_item_results) | **GET** /api/v2/autoTests/{id}/testResultHistory | 
-        *AutoTestsApi* | [**get_work_items_linked_to_auto_test**](docs/AutoTestsApi.md#get_work_items_linked_to_auto_test) | **GET** /api/v2/autoTests/{id}/workItems | Get work items linked to autotest
-        *AutoTestsApi* | [**link_auto_test_to_work_item**](docs/AutoTestsApi.md#link_auto_test_to_work_item) | **POST** /api/v2/autoTests/{id}/workItems | Link autotest with work items
-        *AutoTestsApi* | [**update_auto_test**](docs/AutoTestsApi.md#update_auto_test) | **PUT** /api/v2/autoTests | Update autotest
-        *AutoTestsApi* | [**update_multiple**](docs/AutoTestsApi.md#update_multiple) | **PUT** /api/v2/autoTests/bulk | Update multiple autotests
-        *ConfigurationsApi* | [**api_v2_configurations_create_by_parameters_post**](docs/ConfigurationsApi.md#api_v2_configurations_create_by_parameters_post) | **POST** /api/v2/configurations/createByParameters | Create Configurations by parameters
-        *ConfigurationsApi* | [**api_v2_configurations_search_post**](docs/ConfigurationsApi.md#api_v2_configurations_search_post) | **POST** /api/v2/configurations/search | Search for configurations
-        *ConfigurationsApi* | [**create_configuration**](docs/ConfigurationsApi.md#create_configuration) | **POST** /api/v2/configurations | Create Configuration
-        *ConfigurationsApi* | [**get_configuration_by_id**](docs/ConfigurationsApi.md#get_configuration_by_id) | **GET** /api/v2/configurations/{id} | Get configuration by internal or global ID
-        *ConfigurationsApi* | [**update_configuration**](docs/ConfigurationsApi.md#update_configuration) | **PUT** /api/v2/configurations | Update Configuration
-        *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_custom_attributes_exclude_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_custom_attributes_exclude_post) | **POST** /api/v2/customAttributes/templates/{id}/customAttributes/exclude | Exclude CustomAttributes from CustomAttributeTemplate
-        *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_custom_attributes_include_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_custom_attributes_include_post) | **POST** /api/v2/customAttributes/templates/{id}/customAttributes/include | Include CustomAttributes to CustomAttributeTemplate
-        *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_delete**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_delete) | **DELETE** /api/v2/customAttributes/templates/{id} | Delete CustomAttributeTemplate
-        *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_get**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_get) | **GET** /api/v2/customAttributes/templates/{id} | Get CustomAttributeTemplate by ID
-        *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_name_get**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_name_get) | **GET** /api/v2/customAttributes/templates/{name} | Get CustomAttributeTemplate by name
-        *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_post) | **POST** /api/v2/customAttributes/templates | Create CustomAttributeTemplate
-        *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_put**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_put) | **PUT** /api/v2/customAttributes/templates | Update custom attributes template
-        *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_search_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_search_post) | **POST** /api/v2/customAttributes/templates/search | Search CustomAttributeTemplates
-        *CustomAttributesApi* | [**api_v2_custom_attributes_global_id_delete**](docs/CustomAttributesApi.md#api_v2_custom_attributes_global_id_delete) | **DELETE** /api/v2/customAttributes/global/{id} | Delete global attribute
-        *CustomAttributesApi* | [**api_v2_custom_attributes_global_id_put**](docs/CustomAttributesApi.md#api_v2_custom_attributes_global_id_put) | **PUT** /api/v2/customAttributes/global/{id} | Edit global attribute
-        *CustomAttributesApi* | [**api_v2_custom_attributes_global_post**](docs/CustomAttributesApi.md#api_v2_custom_attributes_global_post) | **POST** /api/v2/customAttributes/global | Create global attribute
-        *CustomAttributesApi* | [**api_v2_custom_attributes_id_get**](docs/CustomAttributesApi.md#api_v2_custom_attributes_id_get) | **GET** /api/v2/customAttributes/{id} | Get attribute
-        *CustomAttributesApi* | [**api_v2_custom_attributes_search_post**](docs/CustomAttributesApi.md#api_v2_custom_attributes_search_post) | **POST** /api/v2/customAttributes/search | Search for attributes
-        *NotificationsApi* | [**api_v2_notifications_count_get**](docs/NotificationsApi.md#api_v2_notifications_count_get) | **GET** /api/v2/notifications/count | Get unread Notifications total in last 7 days
-        *NotificationsApi* | [**api_v2_notifications_get**](docs/NotificationsApi.md#api_v2_notifications_get) | **GET** /api/v2/notifications | Get all Notifications for current User
-        *NotificationsApi* | [**api_v2_notifications_id_read_post**](docs/NotificationsApi.md#api_v2_notifications_id_read_post) | **POST** /api/v2/notifications/{id}/read | Set Notification as read
-        *NotificationsApi* | [**api_v2_notifications_read_post**](docs/NotificationsApi.md#api_v2_notifications_read_post) | **POST** /api/v2/notifications/read | Set all Notifications as read
-        *NotificationsApi* | [**api_v2_notifications_search_post**](docs/NotificationsApi.md#api_v2_notifications_search_post) | **POST** /api/v2/notifications/search | Search Notifications for current User
-        *ParametersApi* | [**api_v2_parameters_bulk_post**](docs/ParametersApi.md#api_v2_parameters_bulk_post) | **POST** /api/v2/parameters/bulk | Create multiple parameters
-        *ParametersApi* | [**api_v2_parameters_bulk_put**](docs/ParametersApi.md#api_v2_parameters_bulk_put) | **PUT** /api/v2/parameters/bulk | Update multiple parameters
-        *ParametersApi* | [**api_v2_parameters_groups_get**](docs/ParametersApi.md#api_v2_parameters_groups_get) | **GET** /api/v2/parameters/groups | Get parameters as group
-        *ParametersApi* | [**api_v2_parameters_key_name_name_exists_get**](docs/ParametersApi.md#api_v2_parameters_key_name_name_exists_get) | **GET** /api/v2/parameters/key/name/{name}/exists | Check existence parameter key in system
-        *ParametersApi* | [**api_v2_parameters_key_values_get**](docs/ParametersApi.md#api_v2_parameters_key_values_get) | **GET** /api/v2/parameters/{key}/values | Get all parameter key values
-        *ParametersApi* | [**api_v2_parameters_keys_get**](docs/ParametersApi.md#api_v2_parameters_keys_get) | **GET** /api/v2/parameters/keys | Get all parameter keys
-        *ParametersApi* | [**create_parameter**](docs/ParametersApi.md#create_parameter) | **POST** /api/v2/parameters | Create parameter
-        *ParametersApi* | [**delete_by_name**](docs/ParametersApi.md#delete_by_name) | **DELETE** /api/v2/parameters/name/{name} | Delete parameter by name
-        *ParametersApi* | [**delete_by_parameter_key_id**](docs/ParametersApi.md#delete_by_parameter_key_id) | **DELETE** /api/v2/parameters/keyId/{keyId} | Delete parameters by parameter key identifier
-        *ParametersApi* | [**delete_parameter**](docs/ParametersApi.md#delete_parameter) | **DELETE** /api/v2/parameters/{id} | Delete parameter
-        *ParametersApi* | [**get_all_parameters**](docs/ParametersApi.md#get_all_parameters) | **GET** /api/v2/parameters | Get all parameters
-        *ParametersApi* | [**get_parameter_by_id**](docs/ParametersApi.md#get_parameter_by_id) | **GET** /api/v2/parameters/{id} | Get parameter by ID
-        *ParametersApi* | [**obsolete_delete_by_name**](docs/ParametersApi.md#obsolete_delete_by_name) | **POST** /api/v2/parameters/deleteByName | 
-        *ParametersApi* | [**update_parameter**](docs/ParametersApi.md#update_parameter) | **PUT** /api/v2/parameters | Update parameter
-        *ProjectsApi* | [**add_globa_attributes_to_project**](docs/ProjectsApi.md#add_globa_attributes_to_project) | **POST** /api/v2/projects/{id}/globalAttributes | Add global attributes to project
-        *ProjectsApi* | [**api_v2_projects_id_attributes_templates_search_post**](docs/ProjectsApi.md#api_v2_projects_id_attributes_templates_search_post) | **POST** /api/v2/projects/{id}/attributes/templates/search | Search for custom attributes templates
-        *ProjectsApi* | [**api_v2_projects_id_attributes_templates_template_id_delete**](docs/ProjectsApi.md#api_v2_projects_id_attributes_templates_template_id_delete) | **DELETE** /api/v2/projects/{id}/attributes/templates/{templateId} | Delete CustomAttributeTemplate from Project
-        *ProjectsApi* | [**api_v2_projects_id_attributes_templates_template_id_post**](docs/ProjectsApi.md#api_v2_projects_id_attributes_templates_template_id_post) | **POST** /api/v2/projects/{id}/attributes/templates/{templateId} | Add CustomAttributeTemplate to Project
-        *ProjectsApi* | [**api_v2_projects_id_failure_classes_get**](docs/ProjectsApi.md#api_v2_projects_id_failure_classes_get) | **GET** /api/v2/projects/{id}/failureClasses | Get Project FailureClasses
-        *ProjectsApi* | [**api_v2_projects_id_favorite_put**](docs/ProjectsApi.md#api_v2_projects_id_favorite_put) | **PUT** /api/v2/projects/{id}/favorite | Mark Project as favorite
-        *ProjectsApi* | [**api_v2_projects_id_filters_get**](docs/ProjectsApi.md#api_v2_projects_id_filters_get) | **GET** /api/v2/projects/{id}/filters | Get Project filters
-        *ProjectsApi* | [**api_v2_projects_id_test_plans_analytics_get**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_analytics_get) | **GET** /api/v2/projects/{id}/testPlans/analytics | Get TestPlans analytics
-        *ProjectsApi* | [**api_v2_projects_id_test_plans_name_exists_get**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_name_exists_get) | **GET** /api/v2/projects/{id}/testPlans/{name}/exists | Checks if TestPlan exists with the specified name exists for the project
-        *ProjectsApi* | [**api_v2_projects_id_test_plans_search_post**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_search_post) | **POST** /api/v2/projects/{id}/testPlans/search | Get Project TestPlans with analytics
-        *ProjectsApi* | [**api_v2_projects_id_test_runs_active_get**](docs/ProjectsApi.md#api_v2_projects_id_test_runs_active_get) | **GET** /api/v2/projects/{id}/testRuns/active | Get active Project TestRuns
-        *ProjectsApi* | [**api_v2_projects_id_test_runs_full_get**](docs/ProjectsApi.md#api_v2_projects_id_test_runs_full_get) | **GET** /api/v2/projects/{id}/testRuns/full | Get Project TestRuns full models
-        *ProjectsApi* | [**api_v2_projects_id_work_items_search_id_post**](docs/ProjectsApi.md#api_v2_projects_id_work_items_search_id_post) | **POST** /api/v2/projects/{id}/workItems/search/id | Search for work items and extract IDs only
-        *ProjectsApi* | [**api_v2_projects_id_work_items_search_post**](docs/ProjectsApi.md#api_v2_projects_id_work_items_search_post) | **POST** /api/v2/projects/{id}/workItems/search | Search for work items
-        *ProjectsApi* | [**api_v2_projects_id_work_items_tags_get**](docs/ProjectsApi.md#api_v2_projects_id_work_items_tags_get) | **GET** /api/v2/projects/{id}/workItems/tags | Get WorkItems Tags
-        *ProjectsApi* | [**api_v2_projects_name_name_exists_get**](docs/ProjectsApi.md#api_v2_projects_name_name_exists_get) | **GET** /api/v2/projects/name/{name}/exists | 
-        *ProjectsApi* | [**api_v2_projects_search_post**](docs/ProjectsApi.md#api_v2_projects_search_post) | **POST** /api/v2/projects/search | Search for projects
-        *ProjectsApi* | [**call_import**](docs/ProjectsApi.md#call_import) | **POST** /api/v2/projects/import | Import project from JSON file
-        *ProjectsApi* | [**create_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#create_custom_attribute_test_plan_project_relations) | **POST** /api/v2/projects/{id}/testPlans/attributes | Add attributes to project&#39;s test plans
-        *ProjectsApi* | [**create_project**](docs/ProjectsApi.md#create_project) | **POST** /api/v2/projects | Create project
-        *ProjectsApi* | [**create_projects_attribute**](docs/ProjectsApi.md#create_projects_attribute) | **POST** /api/v2/projects/{id}/attributes | Create project attribute
-        *ProjectsApi* | [**delete_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#delete_custom_attribute_test_plan_project_relations) | **DELETE** /api/v2/projects/{id}/testPlans/attribute/{attributeId} | Delete attribute from project&#39;s test plans
-        *ProjectsApi* | [**delete_project**](docs/ProjectsApi.md#delete_project) | **DELETE** /api/v2/projects/{id} | Delete project
-        *ProjectsApi* | [**delete_project_auto_tests**](docs/ProjectsApi.md#delete_project_auto_tests) | **DELETE** /api/v2/projects/{id}/autoTests | Delete project
-        *ProjectsApi* | [**delete_projects_attribute**](docs/ProjectsApi.md#delete_projects_attribute) | **DELETE** /api/v2/projects/{id}/attributes/{attributeId} | Delete project attribute
-        *ProjectsApi* | [**export**](docs/ProjectsApi.md#export) | **POST** /api/v2/projects/{id}/export | Export project as JSON file
-        *ProjectsApi* | [**export_with_test_plans_and_configurations**](docs/ProjectsApi.md#export_with_test_plans_and_configurations) | **POST** /api/v2/projects/{id}/export-by-testPlans | Export project with test plans, test suites and test points as JSON file
-        *ProjectsApi* | [**get_all_projects**](docs/ProjectsApi.md#get_all_projects) | **GET** /api/v2/projects | Get all projects
-        *ProjectsApi* | [**get_attribute_by_project_id**](docs/ProjectsApi.md#get_attribute_by_project_id) | **GET** /api/v2/projects/{id}/attributes/{attributeId} | Get project attribute
-        *ProjectsApi* | [**get_attributes_by_project_id**](docs/ProjectsApi.md#get_attributes_by_project_id) | **GET** /api/v2/projects/{id}/attributes | Get project attributes
-        *ProjectsApi* | [**get_auto_tests_namespaces**](docs/ProjectsApi.md#get_auto_tests_namespaces) | **GET** /api/v2/projects/{id}/autoTestsNamespaces | Get namespaces of autotests in project
-        *ProjectsApi* | [**get_configurations_by_project_id**](docs/ProjectsApi.md#get_configurations_by_project_id) | **GET** /api/v2/projects/{id}/configurations | Get project configurations
-        *ProjectsApi* | [**get_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#get_custom_attribute_test_plan_project_relations) | **GET** /api/v2/projects/{id}/testPlans/attributes | Get project&#39;s test plan attributes
-        *ProjectsApi* | [**get_project_by_id**](docs/ProjectsApi.md#get_project_by_id) | **GET** /api/v2/projects/{id} | Get project by ID
-        *ProjectsApi* | [**get_sections_by_project_id**](docs/ProjectsApi.md#get_sections_by_project_id) | **GET** /api/v2/projects/{id}/sections | Get project sections
-        *ProjectsApi* | [**get_test_plans_by_project_id**](docs/ProjectsApi.md#get_test_plans_by_project_id) | **GET** /api/v2/projects/{id}/testPlans | Get project test plans
-        *ProjectsApi* | [**get_test_runs_by_project_id**](docs/ProjectsApi.md#get_test_runs_by_project_id) | **GET** /api/v2/projects/{id}/testRuns | Get project test runs
-        *ProjectsApi* | [**get_work_items_by_project_id**](docs/ProjectsApi.md#get_work_items_by_project_id) | **GET** /api/v2/projects/{id}/workItems | Get project work items
-        *ProjectsApi* | [**import_to_existing_project**](docs/ProjectsApi.md#import_to_existing_project) | **POST** /api/v2/projects/{id}/import | Import project from JSON file into existing project
-        *ProjectsApi* | [**restore_project**](docs/ProjectsApi.md#restore_project) | **POST** /api/v2/projects/{id}/restore | Restore project
-        *ProjectsApi* | [**search_attributes_in_project**](docs/ProjectsApi.md#search_attributes_in_project) | **POST** /api/v2/projects/{id}/attributes/search | Search for attributes used in the project
-        *ProjectsApi* | [**search_test_plan_attributes_in_project**](docs/ProjectsApi.md#search_test_plan_attributes_in_project) | **POST** /api/v2/projects/{id}/testPlans/attributes/search | Search for attributes used in the project test plans
-        *ProjectsApi* | [**update_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#update_custom_attribute_test_plan_project_relations) | **PUT** /api/v2/projects/{id}/testPlans/attribute | Update attribute of project&#39;s test plans
-        *ProjectsApi* | [**update_project**](docs/ProjectsApi.md#update_project) | **PUT** /api/v2/projects | Update project
-        *ProjectsApi* | [**update_projects_attribute**](docs/ProjectsApi.md#update_projects_attribute) | **PUT** /api/v2/projects/{id}/attributes | Edit attribute of the project
-        *SectionsApi* | [**create_section**](docs/SectionsApi.md#create_section) | **POST** /api/v2/sections | Create section
-        *SectionsApi* | [**delete_section**](docs/SectionsApi.md#delete_section) | **DELETE** /api/v2/sections/{id} | Delete section
-        *SectionsApi* | [**get_section_by_id**](docs/SectionsApi.md#get_section_by_id) | **GET** /api/v2/sections/{id} | Get section
-        *SectionsApi* | [**get_work_items_by_section_id**](docs/SectionsApi.md#get_work_items_by_section_id) | **GET** /api/v2/sections/{id}/workItems | Get section work items
-        *SectionsApi* | [**move**](docs/SectionsApi.md#move) | **POST** /api/v2/sections/move | Move section with all work items into another section
-        *SectionsApi* | [**rename**](docs/SectionsApi.md#rename) | **POST** /api/v2/sections/rename | Rename section
-        *SectionsApi* | [**update_section**](docs/SectionsApi.md#update_section) | **PUT** /api/v2/sections | Update section
-        *TagsApi* | [**api_v2_tags_get**](docs/TagsApi.md#api_v2_tags_get) | **GET** /api/v2/tags | Get all Tags
-        *TagsApi* | [**api_v2_tags_test_plans_tags_get**](docs/TagsApi.md#api_v2_tags_test_plans_tags_get) | **GET** /api/v2/tags/testPlansTags | Get all Tags that are used in TestPlans
-        *TestPlansApi* | [**add_test_points_with_sections**](docs/TestPlansApi.md#add_test_points_with_sections) | **POST** /api/v2/testPlans/{id}/test-points/withSections | Add test-points to TestPlan with sections
-        *TestPlansApi* | [**add_work_items_with_sections**](docs/TestPlansApi.md#add_work_items_with_sections) | **POST** /api/v2/testPlans/{id}/workItems/withSections | Add WorkItems to TestPlan with Sections as TestSuites
-        *TestPlansApi* | [**api_v2_test_plans_id_analytics_get**](docs/TestPlansApi.md#api_v2_test_plans_id_analytics_get) | **GET** /api/v2/testPlans/{id}/analytics | Get analytics by TestPlan
-        *TestPlansApi* | [**api_v2_test_plans_id_autobalance_post**](docs/TestPlansApi.md#api_v2_test_plans_id_autobalance_post) | **POST** /api/v2/testPlans/{id}/autobalance | Distribute test points between the users
-        *TestPlansApi* | [**api_v2_test_plans_id_configurations_get**](docs/TestPlansApi.md#api_v2_test_plans_id_configurations_get) | **GET** /api/v2/testPlans/{id}/configurations | Get TestPlan configurations
-        *TestPlansApi* | [**api_v2_test_plans_id_export_test_points_xlsx_post**](docs/TestPlansApi.md#api_v2_test_plans_id_export_test_points_xlsx_post) | **POST** /api/v2/testPlans/{id}/export/testPoints/xlsx | Export TestPoints from TestPlan in xls format
-        *TestPlansApi* | [**api_v2_test_plans_id_export_test_result_history_xlsx_post**](docs/TestPlansApi.md#api_v2_test_plans_id_export_test_result_history_xlsx_post) | **POST** /api/v2/testPlans/{id}/export/testResultHistory/xlsx | Export TestResults history from TestPlan in xls format
-        *TestPlansApi* | [**api_v2_test_plans_id_history_get**](docs/TestPlansApi.md#api_v2_test_plans_id_history_get) | **GET** /api/v2/testPlans/{id}/history | Get TestPlan history
-        *TestPlansApi* | [**api_v2_test_plans_id_links_get**](docs/TestPlansApi.md#api_v2_test_plans_id_links_get) | **GET** /api/v2/testPlans/{id}/links | Get Links of TestPlan
-        *TestPlansApi* | [**api_v2_test_plans_id_test_points_last_results_get**](docs/TestPlansApi.md#api_v2_test_plans_id_test_points_last_results_get) | **GET** /api/v2/testPlans/{id}/testPoints/lastResults | Get TestPoints with last result from TestPlan
-        *TestPlansApi* | [**api_v2_test_plans_id_test_points_reset_post**](docs/TestPlansApi.md#api_v2_test_plans_id_test_points_reset_post) | **POST** /api/v2/testPlans/{id}/testPoints/reset | Reset TestPoints status of TestPlan
-        *TestPlansApi* | [**api_v2_test_plans_id_test_runs_get**](docs/TestPlansApi.md#api_v2_test_plans_id_test_runs_get) | **GET** /api/v2/testPlans/{id}/testRuns | Get TestRuns of TestPlan
-        *TestPlansApi* | [**api_v2_test_plans_id_test_runs_search_post**](docs/TestPlansApi.md#api_v2_test_plans_id_test_runs_search_post) | **POST** /api/v2/testPlans/{id}/testRuns/search | Search TestRuns of TestPlan
-        *TestPlansApi* | [**api_v2_test_plans_id_test_runs_test_results_last_modified_modified_date_get**](docs/TestPlansApi.md#api_v2_test_plans_id_test_runs_test_results_last_modified_modified_date_get) | **GET** /api/v2/testPlans/{id}/testRuns/testResults/lastModified/modifiedDate | Get last modification date of test plan&#39;s test results
-        *TestPlansApi* | [**api_v2_test_plans_id_unlock_request_post**](docs/TestPlansApi.md#api_v2_test_plans_id_unlock_request_post) | **POST** /api/v2/testPlans/{id}/unlock/request | Send unlock TestPlan notification
-        *TestPlansApi* | [**api_v2_test_plans_shorts_post**](docs/TestPlansApi.md#api_v2_test_plans_shorts_post) | **POST** /api/v2/testPlans/shorts | Get TestPlans short models by Project identifiers
-        *TestPlansApi* | [**clone**](docs/TestPlansApi.md#clone) | **POST** /api/v2/testPlans/{id}/clone | Clone TestPlan
-        *TestPlansApi* | [**complete**](docs/TestPlansApi.md#complete) | **POST** /api/v2/testPlans/{id}/complete | Complete TestPlan
-        *TestPlansApi* | [**create_test_plan**](docs/TestPlansApi.md#create_test_plan) | **POST** /api/v2/testPlans | Create TestPlan
-        *TestPlansApi* | [**delete_test_plan**](docs/TestPlansApi.md#delete_test_plan) | **DELETE** /api/v2/testPlans/{id} | Delete TestPlan
-        *TestPlansApi* | [**get_test_plan_by_id**](docs/TestPlansApi.md#get_test_plan_by_id) | **GET** /api/v2/testPlans/{id} | Get TestPlan by Id
-        *TestPlansApi* | [**get_test_suites_by_id**](docs/TestPlansApi.md#get_test_suites_by_id) | **GET** /api/v2/testPlans/{id}/testSuites | Get TestSuites Tree By Id
-        *TestPlansApi* | [**pause**](docs/TestPlansApi.md#pause) | **POST** /api/v2/testPlans/{id}/pause | Pause TestPlan
-        *TestPlansApi* | [**restore_test_plan**](docs/TestPlansApi.md#restore_test_plan) | **POST** /api/v2/testPlans/{id}/restore | Restore TestPlan
-        *TestPlansApi* | [**start**](docs/TestPlansApi.md#start) | **POST** /api/v2/testPlans/{id}/start | Start TestPlan
-        *TestPlansApi* | [**update_test_plan**](docs/TestPlansApi.md#update_test_plan) | **PUT** /api/v2/testPlans | Update TestPlan
-        *TestPointsApi* | [**api_v2_test_points_id_test_runs_get**](docs/TestPointsApi.md#api_v2_test_points_id_test_runs_get) | **GET** /api/v2/testPoints/{id}/testRuns | Get all test runs which use test point
-        *TestPointsApi* | [**api_v2_test_points_id_work_item_get**](docs/TestPointsApi.md#api_v2_test_points_id_work_item_get) | **GET** /api/v2/testPoints/{id}/workItem | Get work item represented by test point
-        *TestPointsApi* | [**api_v2_test_points_search_id_post**](docs/TestPointsApi.md#api_v2_test_points_search_id_post) | **POST** /api/v2/testPoints/search/id | Search for test points and extract IDs only
-        *TestPointsApi* | [**api_v2_test_points_search_post**](docs/TestPointsApi.md#api_v2_test_points_search_post) | **POST** /api/v2/testPoints/search | Search for test points
-        *TestResultsApi* | [**api_v2_test_results_id_aggregated_get**](docs/TestResultsApi.md#api_v2_test_results_id_aggregated_get) | **GET** /api/v2/testResults/{id}/aggregated | Get test result by ID aggregated with previous results
-        *TestResultsApi* | [**api_v2_test_results_id_attachments_attachment_id_put**](docs/TestResultsApi.md#api_v2_test_results_id_attachments_attachment_id_put) | **PUT** /api/v2/testResults/{id}/attachments/{attachmentId} | Attach file to the test result
-        *TestResultsApi* | [**api_v2_test_results_id_attachments_info_get**](docs/TestResultsApi.md#api_v2_test_results_id_attachments_info_get) | **GET** /api/v2/testResults/{id}/attachments/info | Get test result attachments meta-information
-        *TestResultsApi* | [**api_v2_test_results_id_get**](docs/TestResultsApi.md#api_v2_test_results_id_get) | **GET** /api/v2/testResults/{id} | Get test result by ID
-        *TestResultsApi* | [**api_v2_test_results_id_put**](docs/TestResultsApi.md#api_v2_test_results_id_put) | **PUT** /api/v2/testResults/{id} | Edit test result by ID
-        *TestResultsApi* | [**api_v2_test_results_search_post**](docs/TestResultsApi.md#api_v2_test_results_search_post) | **POST** /api/v2/testResults/search | Search for test results
-        *TestResultsApi* | [**api_v2_test_results_statistics_filter_post**](docs/TestResultsApi.md#api_v2_test_results_statistics_filter_post) | **POST** /api/v2/testResults/statistics/filter | Search for test results and extract statistics
-        *TestResultsApi* | [**create_attachment**](docs/TestResultsApi.md#create_attachment) | **POST** /api/v2/testResults/{id}/attachments | Upload and link attachment to TestResult
-        *TestResultsApi* | [**delete_attachment**](docs/TestResultsApi.md#delete_attachment) | **DELETE** /api/v2/testResults/{id}/attachments/{attachmentId} | Remove attachment and unlink from TestResult
-        *TestResultsApi* | [**download_attachment**](docs/TestResultsApi.md#download_attachment) | **GET** /api/v2/testResults/{id}/attachments/{attachmentId} | Get attachment of TestResult
-        *TestResultsApi* | [**get_attachment**](docs/TestResultsApi.md#get_attachment) | **GET** /api/v2/testResults/{id}/attachments/{attachmentId}/info | Get Metadata of TestResult&#39;s attachment
-        *TestResultsApi* | [**get_attachments**](docs/TestResultsApi.md#get_attachments) | **GET** /api/v2/testResults/{id}/attachments | Get all attachments of TestResult
-        *TestRunsApi* | [**api_v2_test_runs_id_statistics_filter_post**](docs/TestRunsApi.md#api_v2_test_runs_id_statistics_filter_post) | **POST** /api/v2/testRuns/{id}/statistics/filter | Search for the test run test results and build statistics
-        *TestRunsApi* | [**api_v2_test_runs_id_test_points_results_get**](docs/TestRunsApi.md#api_v2_test_runs_id_test_points_results_get) | **GET** /api/v2/testRuns/{id}/testPoints/results | Get test results from the test run grouped by test points
-        *TestRunsApi* | [**api_v2_test_runs_id_test_results_bulk_put**](docs/TestRunsApi.md#api_v2_test_runs_id_test_results_bulk_put) | **PUT** /api/v2/testRuns/{id}/testResults/bulk | Partial edit of multiple test results in the test run
-        *TestRunsApi* | [**api_v2_test_runs_id_test_results_last_modified_modification_date_get**](docs/TestRunsApi.md#api_v2_test_runs_id_test_results_last_modified_modification_date_get) | **GET** /api/v2/testRuns/{id}/testResults/lastModified/modificationDate | Get modification date of last test result of the test run
-        *TestRunsApi* | [**api_v2_test_runs_search_post**](docs/TestRunsApi.md#api_v2_test_runs_search_post) | **POST** /api/v2/testRuns/search | Search for test runs
-        *TestRunsApi* | [**complete_test_run**](docs/TestRunsApi.md#complete_test_run) | **POST** /api/v2/testRuns/{id}/complete | Complete TestRun
-        *TestRunsApi* | [**create_and_fill_by_auto_tests**](docs/TestRunsApi.md#create_and_fill_by_auto_tests) | **POST** /api/v2/testRuns/byAutoTests | Create test runs based on autotests and configurations
-        *TestRunsApi* | [**create_and_fill_by_configurations**](docs/TestRunsApi.md#create_and_fill_by_configurations) | **POST** /api/v2/testRuns/byConfigurations | Create test runs picking the needed test points
-        *TestRunsApi* | [**create_and_fill_by_work_items**](docs/TestRunsApi.md#create_and_fill_by_work_items) | **POST** /api/v2/testRuns/byWorkItems | Create test run based on configurations and work items
-        *TestRunsApi* | [**create_empty**](docs/TestRunsApi.md#create_empty) | **POST** /api/v2/testRuns | Create empty TestRun
-        *TestRunsApi* | [**get_test_run_by_id**](docs/TestRunsApi.md#get_test_run_by_id) | **GET** /api/v2/testRuns/{id} | Get TestRun by Id
-        *TestRunsApi* | [**set_auto_test_results_for_test_run**](docs/TestRunsApi.md#set_auto_test_results_for_test_run) | **POST** /api/v2/testRuns/{id}/testResults | Send test results to the test runs in the system
-        *TestRunsApi* | [**start_test_run**](docs/TestRunsApi.md#start_test_run) | **POST** /api/v2/testRuns/{id}/start | Start TestRun
-        *TestRunsApi* | [**stop_test_run**](docs/TestRunsApi.md#stop_test_run) | **POST** /api/v2/testRuns/{id}/stop | Stop TestRun
-        *TestRunsApi* | [**update_empty**](docs/TestRunsApi.md#update_empty) | **PUT** /api/v2/testRuns | Update empty TestRun
-        *TestSuitesApi* | [**add_test_points_to_test_suite**](docs/TestSuitesApi.md#add_test_points_to_test_suite) | **POST** /api/v2/testSuites/{id}/test-points | Add test-points to test suite
-        *TestSuitesApi* | [**create_test_suite**](docs/TestSuitesApi.md#create_test_suite) | **POST** /api/v2/testSuites | Create TestSuite
-        *TestSuitesApi* | [**delete_test_suite**](docs/TestSuitesApi.md#delete_test_suite) | **DELETE** /api/v2/testSuites/{id} | Delete TestSuite
-        *TestSuitesApi* | [**get_configurations_by_test_suite_id**](docs/TestSuitesApi.md#get_configurations_by_test_suite_id) | **GET** /api/v2/testSuites/{id}/configurations | Get Configurations By Id
-        *TestSuitesApi* | [**get_test_points_by_id**](docs/TestSuitesApi.md#get_test_points_by_id) | **GET** /api/v2/testSuites/{id}/testPoints | Get TestPoints By Id
-        *TestSuitesApi* | [**get_test_results_by_id**](docs/TestSuitesApi.md#get_test_results_by_id) | **GET** /api/v2/testSuites/{id}/testResults | Get TestResults By Id
-        *TestSuitesApi* | [**get_test_suite_by_id**](docs/TestSuitesApi.md#get_test_suite_by_id) | **GET** /api/v2/testSuites/{id} | Get TestSuite by Id
-        *TestSuitesApi* | [**get_work_items_by_id**](docs/TestSuitesApi.md#get_work_items_by_id) | **GET** /api/v2/testSuites/{id}/workItems | 
-        *TestSuitesApi* | [**search_work_items**](docs/TestSuitesApi.md#search_work_items) | **POST** /api/v2/testSuites/{id}/workItems/search | Search WorkItems
-        *TestSuitesApi* | [**set_configurations_by_test_suite_id**](docs/TestSuitesApi.md#set_configurations_by_test_suite_id) | **POST** /api/v2/testSuites/{id}/configurations | Set Configurations By TestSuite Id
-        *TestSuitesApi* | [**set_work_items_by_test_suite_id**](docs/TestSuitesApi.md#set_work_items_by_test_suite_id) | **POST** /api/v2/testSuites/{id}/workItems | Set WorkItems By TestSuite Id
-        *TestSuitesApi* | [**update_test_suite**](docs/TestSuitesApi.md#update_test_suite) | **PUT** /api/v2/testSuites | Update TestSuite
-        *WebhooksApi* | [**api_v2_webhooks_get**](docs/WebhooksApi.md#api_v2_webhooks_get) | **GET** /api/v2/webhooks | Get all webhooks
-        *WebhooksApi* | [**api_v2_webhooks_id_delete**](docs/WebhooksApi.md#api_v2_webhooks_id_delete) | **DELETE** /api/v2/webhooks/{id} | Delete webhook by ID
-        *WebhooksApi* | [**api_v2_webhooks_id_get**](docs/WebhooksApi.md#api_v2_webhooks_id_get) | **GET** /api/v2/webhooks/{id} | Get webhook by ID
-        *WebhooksApi* | [**api_v2_webhooks_id_put**](docs/WebhooksApi.md#api_v2_webhooks_id_put) | **PUT** /api/v2/webhooks/{id} | Edit webhook by ID
-        *WebhooksApi* | [**api_v2_webhooks_post**](docs/WebhooksApi.md#api_v2_webhooks_post) | **POST** /api/v2/webhooks | Create webhook
-        *WebhooksApi* | [**api_v2_webhooks_search_post**](docs/WebhooksApi.md#api_v2_webhooks_search_post) | **POST** /api/v2/webhooks/search | Search for webhooks
-        *WebhooksApi* | [**api_v2_webhooks_special_variables_get**](docs/WebhooksApi.md#api_v2_webhooks_special_variables_get) | **GET** /api/v2/webhooks/specialVariables | Get special variables for webhook event type
-        *WebhooksLogsApi* | [**api_v2_webhooks_logs_get**](docs/WebhooksLogsApi.md#api_v2_webhooks_logs_get) | **GET** /api/v2/webhooks/logs | Get all webhook logs
-        *WebhooksLogsApi* | [**api_v2_webhooks_logs_id_delete**](docs/WebhooksLogsApi.md#api_v2_webhooks_logs_id_delete) | **DELETE** /api/v2/webhooks/logs/{id} | Delete webhook log by ID
-        *WebhooksLogsApi* | [**api_v2_webhooks_logs_id_get**](docs/WebhooksLogsApi.md#api_v2_webhooks_logs_id_get) | **GET** /api/v2/webhooks/logs/{id} | Get webhook log by ID
-        *WorkItemsApi* | [**api_v2_work_items_id_check_list_transform_to_test_case_post**](docs/WorkItemsApi.md#api_v2_work_items_id_check_list_transform_to_test_case_post) | **POST** /api/v2/workItems/{id}/checkList/transformTo/testCase | Transform CheckList to TestCase
-        *WorkItemsApi* | [**api_v2_work_items_id_history_get**](docs/WorkItemsApi.md#api_v2_work_items_id_history_get) | **GET** /api/v2/workItems/{id}/history | Get change history of WorkItem
-        *WorkItemsApi* | [**api_v2_work_items_id_like_delete**](docs/WorkItemsApi.md#api_v2_work_items_id_like_delete) | **DELETE** /api/v2/workItems/{id}/like | Delete like from WorkItem
-        *WorkItemsApi* | [**api_v2_work_items_id_like_post**](docs/WorkItemsApi.md#api_v2_work_items_id_like_post) | **POST** /api/v2/workItems/{id}/like | Set like to WorkItem
-        *WorkItemsApi* | [**api_v2_work_items_id_likes_count_get**](docs/WorkItemsApi.md#api_v2_work_items_id_likes_count_get) | **GET** /api/v2/workItems/{id}/likes/count | Get likes count of WorkItem
-        *WorkItemsApi* | [**api_v2_work_items_id_likes_get**](docs/WorkItemsApi.md#api_v2_work_items_id_likes_get) | **GET** /api/v2/workItems/{id}/likes | Get likes of WorkItem
-        *WorkItemsApi* | [**api_v2_work_items_id_test_results_history_get**](docs/WorkItemsApi.md#api_v2_work_items_id_test_results_history_get) | **GET** /api/v2/workItems/{id}/testResults/history | Get test results history of WorkItem
-        *WorkItemsApi* | [**api_v2_work_items_id_version_version_id_actual_post**](docs/WorkItemsApi.md#api_v2_work_items_id_version_version_id_actual_post) | **POST** /api/v2/workItems/{id}/version/{versionId}/actual | Set WorkItem as actual
-        *WorkItemsApi* | [**api_v2_work_items_move_post**](docs/WorkItemsApi.md#api_v2_work_items_move_post) | **POST** /api/v2/workItems/move | Move WorkItem to another section
-        *WorkItemsApi* | [**api_v2_work_items_search_post**](docs/WorkItemsApi.md#api_v2_work_items_search_post) | **POST** /api/v2/workItems/search | Search for work items
-        *WorkItemsApi* | [**api_v2_work_items_shared_step_id_references_sections_post**](docs/WorkItemsApi.md#api_v2_work_items_shared_step_id_references_sections_post) | **POST** /api/v2/workItems/{sharedStepId}/references/sections | Get SharedStep references in sections
-        *WorkItemsApi* | [**api_v2_work_items_shared_step_id_references_work_items_post**](docs/WorkItemsApi.md#api_v2_work_items_shared_step_id_references_work_items_post) | **POST** /api/v2/workItems/{sharedStepId}/references/workItems | Get SharedStep references in workitems
-        *WorkItemsApi* | [**api_v2_work_items_shared_steps_shared_step_id_references_get**](docs/WorkItemsApi.md#api_v2_work_items_shared_steps_shared_step_id_references_get) | **GET** /api/v2/workItems/sharedSteps/{sharedStepId}/references | Get SharedStep references
-        *WorkItemsApi* | [**create_work_item**](docs/WorkItemsApi.md#create_work_item) | **POST** /api/v2/workItems | Create Test Case, Checklist or Shared Step
-        *WorkItemsApi* | [**delete_all_work_items_from_auto_test**](docs/WorkItemsApi.md#delete_all_work_items_from_auto_test) | **DELETE** /api/v2/workItems/{id}/autoTests | Delete all links AutoTests from WorkItem by Id or GlobalId
-        *WorkItemsApi* | [**delete_work_item**](docs/WorkItemsApi.md#delete_work_item) | **DELETE** /api/v2/workItems/{id} | Delete Test Case, Checklist or Shared Step by Id or GlobalId
-        *WorkItemsApi* | [**get_auto_tests_for_work_item**](docs/WorkItemsApi.md#get_auto_tests_for_work_item) | **GET** /api/v2/workItems/{id}/autoTests | Get all AutoTests linked to WorkItem by Id or GlobalId
-        *WorkItemsApi* | [**get_iterations**](docs/WorkItemsApi.md#get_iterations) | **GET** /api/v2/workItems/{id}/iterations | Get iterations by workitem Id or GlobalId
-        *WorkItemsApi* | [**get_work_item_by_id**](docs/WorkItemsApi.md#get_work_item_by_id) | **GET** /api/v2/workItems/{id} | Get Test Case, Checklist or Shared Step by Id or GlobalId
-        *WorkItemsApi* | [**get_work_item_chronology**](docs/WorkItemsApi.md#get_work_item_chronology) | **GET** /api/v2/workItems/{id}/chronology | Get WorkItem chronology by Id or GlobalId
-        *WorkItemsApi* | [**get_work_item_versions**](docs/WorkItemsApi.md#get_work_item_versions) | **GET** /api/v2/workItems/{id}/versions | Get WorkItem versions
-        *WorkItemsApi* | [**update_work_item**](docs/WorkItemsApi.md#update_work_item) | **PUT** /api/v2/workItems | Update Test Case, Checklist or Shared Step
-        *WorkItemsCommentsApi* | [**api_v2_work_items_comments_comment_id_delete**](docs/WorkItemsCommentsApi.md#api_v2_work_items_comments_comment_id_delete) | **DELETE** /api/v2/workItems/comments/{commentId} | Delete WorkItem comment
-        *WorkItemsCommentsApi* | [**api_v2_work_items_comments_post**](docs/WorkItemsCommentsApi.md#api_v2_work_items_comments_post) | **POST** /api/v2/workItems/comments | Create WorkItem comment
-        *WorkItemsCommentsApi* | [**api_v2_work_items_comments_put**](docs/WorkItemsCommentsApi.md#api_v2_work_items_comments_put) | **PUT** /api/v2/workItems/comments | Update work item comment
-        *WorkItemsCommentsApi* | [**api_v2_work_items_id_comments_get**](docs/WorkItemsCommentsApi.md#api_v2_work_items_id_comments_get) | **GET** /api/v2/workItems/{id}/comments | Get work item comments
-        
-        
-        ## Documentation For Models
-        
-         - You can see the documentation [here](docs/README.md).
-        
-        
-        # Contributing
-        
-        You can help to develop the project. Any contributions are **greatly appreciated**.
-        
-        * If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testgear-tms/api-client-python/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
-        * Please make sure you check your spelling and grammar.
-        * Create individual PR for each suggestion.
-        * Please also read through the [Code Of Conduct](https://github.com/testgear-tms/api-client-python/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
-        
-        
-        # License
-        
-        Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testgear-tms/api-client-python/blob/master/LICENSE.md) for more information.
-        
-        
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: testgear-api-client
+Version: 3.1.0
+Summary: API-client for Test Gear
+Home-page: https://pypi.org/project/testgear-api-client/
+Author: Integration team
+Author-email: integrations@test-gear.io
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# Api client for Test Gear TMS
+![Test Gear](https://raw.githubusercontent.com/testgear-tms/api-client-python/master/images/banner.png)
+
+## Getting Started
+
+### Compatibility
+
+| Test Gear | API Client |
+|-----------|------------|
+| 3.5       | 2.0        |
+| 4.0       | 3.0        |
+| 4.2       | 3.1        |
+
+## Installation & Usage
+### pip install
+
+```sh
+pip install testgear-api-client
+```
+
+Then import the package:
+
+```python
+import testgear_api_client
+```
+
+## Getting Started
+
+Please follow the [installation procedure](#installation--usage) and then run the following:
+
+```python
+import testgear_api_client
+from testgear_api_client.api import attachments_api
+from testgear_api_client.model.attachment_model import AttachmentModel
+from testgear_api_client.model.image_resize_type import ImageResizeType
+from testgear_api_client.model.problem_details import ProblemDetails
+from testgear_api_client.model.validation_problem_details import ValidationProblemDetails
+
+configuration = testgear_api_client.Configuration(
+    host = "Your TMS address"
+)
+
+with testgear_api_client.ApiClient(
+        configuration,
+        header_name='Authorization',
+        header_value='PrivateToken ' + 'Your private token') as api_client:
+    api_instance = attachments_api.AttachmentsApi(api_client)
+    id = "Attachment's guid in the TMS"
+
+    try:
+        api_instance.api_v2_attachments_id_delete(id)
+    except testgear_api_client.ApiException as e:
+        print("Exception when calling AttachmentsApi->api_v2_attachments_id_delete: %s\n" % e)
+```
+
+## Documentation for API Endpoints
+
+All URIs are relative to *http://localhost*
+
+Class | Method | HTTP request | Description
+------------ | ------------- | ------------- | -------------
+*AttachmentsApi* | [**api_v2_attachments_id_delete**](docs/AttachmentsApi.md#api_v2_attachments_id_delete) | **DELETE** /api/v2/attachments/{id} | Delete attachment file
+*AttachmentsApi* | [**api_v2_attachments_id_get**](docs/AttachmentsApi.md#api_v2_attachments_id_get) | **GET** /api/v2/attachments/{id} | Download attachment file
+*AttachmentsApi* | [**api_v2_attachments_occupied_file_storage_size_get**](docs/AttachmentsApi.md#api_v2_attachments_occupied_file_storage_size_get) | **GET** /api/v2/attachments/occupiedFileStorageSize | Get size of attachments storage in bytes
+*AttachmentsApi* | [**api_v2_attachments_post**](docs/AttachmentsApi.md#api_v2_attachments_post) | **POST** /api/v2/attachments | Upload new attachment file
+*AutoTestsApi* | [**api_v2_auto_tests_flaky_bulk_post**](docs/AutoTestsApi.md#api_v2_auto_tests_flaky_bulk_post) | **POST** /api/v2/autoTests/flaky/bulk | Set \&quot;Flaky\&quot; status for multiple autotests
+*AutoTestsApi* | [**api_v2_auto_tests_id_patch**](docs/AutoTestsApi.md#api_v2_auto_tests_id_patch) | **PATCH** /api/v2/autoTests/{id} | Patch auto test
+*AutoTestsApi* | [**api_v2_auto_tests_id_test_results_search_post**](docs/AutoTestsApi.md#api_v2_auto_tests_id_test_results_search_post) | **POST** /api/v2/autoTests/{id}/testResults/search | Get test results history for autotest
+*AutoTestsApi* | [**api_v2_auto_tests_id_work_items_changed_id_get**](docs/AutoTestsApi.md#api_v2_auto_tests_id_work_items_changed_id_get) | **GET** /api/v2/autoTests/{id}/workItems/changed/id | Get identifiers of changed linked work items
+*AutoTestsApi* | [**api_v2_auto_tests_id_work_items_changed_work_item_id_approve_post**](docs/AutoTestsApi.md#api_v2_auto_tests_id_work_items_changed_work_item_id_approve_post) | **POST** /api/v2/autoTests/{id}/workItems/changed/{workItemId}/approve | Approve changes to work items linked to autotest
+*AutoTestsApi* | [**api_v2_auto_tests_search_post**](docs/AutoTestsApi.md#api_v2_auto_tests_search_post) | **POST** /api/v2/autoTests/search | Search for autotests
+*AutoTestsApi* | [**create_auto_test**](docs/AutoTestsApi.md#create_auto_test) | **POST** /api/v2/autoTests | Create autotest
+*AutoTestsApi* | [**create_multiple**](docs/AutoTestsApi.md#create_multiple) | **POST** /api/v2/autoTests/bulk | Create multiple autotests
+*AutoTestsApi* | [**delete_auto_test**](docs/AutoTestsApi.md#delete_auto_test) | **DELETE** /api/v2/autoTests/{id} | Delete autotest
+*AutoTestsApi* | [**delete_auto_test_link_from_work_item**](docs/AutoTestsApi.md#delete_auto_test_link_from_work_item) | **DELETE** /api/v2/autoTests/{id}/workItems | Unlink autotest from work item
+*AutoTestsApi* | [**get_all_auto_tests**](docs/AutoTestsApi.md#get_all_auto_tests) | **GET** /api/v2/autoTests | 
+*AutoTestsApi* | [**get_auto_test_average_duration**](docs/AutoTestsApi.md#get_auto_test_average_duration) | **GET** /api/v2/autoTests/{id}/averageDuration | Get average autotest duration
+*AutoTestsApi* | [**get_auto_test_by_id**](docs/AutoTestsApi.md#get_auto_test_by_id) | **GET** /api/v2/autoTests/{id} | Get autotest by internal or global ID
+*AutoTestsApi* | [**get_auto_test_chronology**](docs/AutoTestsApi.md#get_auto_test_chronology) | **GET** /api/v2/autoTests/{id}/chronology | Get autotest chronology
+*AutoTestsApi* | [**get_test_runs**](docs/AutoTestsApi.md#get_test_runs) | **GET** /api/v2/autoTests/{id}/testRuns | Get completed tests runs for autotests
+*AutoTestsApi* | [**get_work_item_results**](docs/AutoTestsApi.md#get_work_item_results) | **GET** /api/v2/autoTests/{id}/testResultHistory | 
+*AutoTestsApi* | [**get_work_items_linked_to_auto_test**](docs/AutoTestsApi.md#get_work_items_linked_to_auto_test) | **GET** /api/v2/autoTests/{id}/workItems | Get work items linked to autotest
+*AutoTestsApi* | [**link_auto_test_to_work_item**](docs/AutoTestsApi.md#link_auto_test_to_work_item) | **POST** /api/v2/autoTests/{id}/workItems | Link autotest with work items
+*AutoTestsApi* | [**update_auto_test**](docs/AutoTestsApi.md#update_auto_test) | **PUT** /api/v2/autoTests | Update autotest
+*AutoTestsApi* | [**update_multiple**](docs/AutoTestsApi.md#update_multiple) | **PUT** /api/v2/autoTests/bulk | Update multiple autotests
+*BackgroundJobsApi* | [**api_v2_background_jobs_get**](docs/BackgroundJobsApi.md#api_v2_background_jobs_get) | **GET** /api/v2/backgroundJobs | Get current user background jobs
+*ConfigurationsApi* | [**api_v2_configurations_create_by_parameters_post**](docs/ConfigurationsApi.md#api_v2_configurations_create_by_parameters_post) | **POST** /api/v2/configurations/createByParameters | Create Configurations by parameters
+*ConfigurationsApi* | [**api_v2_configurations_id_patch**](docs/ConfigurationsApi.md#api_v2_configurations_id_patch) | **PATCH** /api/v2/configurations/{id} | Patch configuration
+*ConfigurationsApi* | [**api_v2_configurations_search_post**](docs/ConfigurationsApi.md#api_v2_configurations_search_post) | **POST** /api/v2/configurations/search | Search for configurations
+*ConfigurationsApi* | [**create_configuration**](docs/ConfigurationsApi.md#create_configuration) | **POST** /api/v2/configurations | Create Configuration
+*ConfigurationsApi* | [**get_configuration_by_id**](docs/ConfigurationsApi.md#get_configuration_by_id) | **GET** /api/v2/configurations/{id} | Get configuration by internal or global ID
+*ConfigurationsApi* | [**update_configuration**](docs/ConfigurationsApi.md#update_configuration) | **PUT** /api/v2/configurations | Update Configuration
+*CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_custom_attributes_exclude_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_custom_attributes_exclude_post) | **POST** /api/v2/customAttributes/templates/{id}/customAttributes/exclude | Exclude CustomAttributes from CustomAttributeTemplate
+*CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_custom_attributes_include_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_custom_attributes_include_post) | **POST** /api/v2/customAttributes/templates/{id}/customAttributes/include | Include CustomAttributes to CustomAttributeTemplate
+*CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_delete**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_delete) | **DELETE** /api/v2/customAttributes/templates/{id} | Delete CustomAttributeTemplate
+*CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_get**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_get) | **GET** /api/v2/customAttributes/templates/{id} | Get CustomAttributeTemplate by ID
+*CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_name_get**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_name_get) | **GET** /api/v2/customAttributes/templates/{name} | Get CustomAttributeTemplate by name
+*CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_post) | **POST** /api/v2/customAttributes/templates | Create CustomAttributeTemplate
+*CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_put**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_put) | **PUT** /api/v2/customAttributes/templates | Update custom attributes template
+*CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_search_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_search_post) | **POST** /api/v2/customAttributes/templates/search | Search CustomAttributeTemplates
+*CustomAttributesApi* | [**api_v2_custom_attributes_global_id_delete**](docs/CustomAttributesApi.md#api_v2_custom_attributes_global_id_delete) | **DELETE** /api/v2/customAttributes/global/{id} | Delete global attribute
+*CustomAttributesApi* | [**api_v2_custom_attributes_global_id_put**](docs/CustomAttributesApi.md#api_v2_custom_attributes_global_id_put) | **PUT** /api/v2/customAttributes/global/{id} | Edit global attribute
+*CustomAttributesApi* | [**api_v2_custom_attributes_global_post**](docs/CustomAttributesApi.md#api_v2_custom_attributes_global_post) | **POST** /api/v2/customAttributes/global | Create global attribute
+*CustomAttributesApi* | [**api_v2_custom_attributes_id_get**](docs/CustomAttributesApi.md#api_v2_custom_attributes_id_get) | **GET** /api/v2/customAttributes/{id} | Get attribute
+*CustomAttributesApi* | [**api_v2_custom_attributes_search_post**](docs/CustomAttributesApi.md#api_v2_custom_attributes_search_post) | **POST** /api/v2/customAttributes/search | Search for attributes
+*NotificationsApi* | [**api_v2_notifications_count_get**](docs/NotificationsApi.md#api_v2_notifications_count_get) | **GET** /api/v2/notifications/count | Get unread Notifications total in last 7 days
+*NotificationsApi* | [**api_v2_notifications_get**](docs/NotificationsApi.md#api_v2_notifications_get) | **GET** /api/v2/notifications | Get all Notifications for current User
+*NotificationsApi* | [**api_v2_notifications_id_read_post**](docs/NotificationsApi.md#api_v2_notifications_id_read_post) | **POST** /api/v2/notifications/{id}/read | Set Notification as read
+*NotificationsApi* | [**api_v2_notifications_read_post**](docs/NotificationsApi.md#api_v2_notifications_read_post) | **POST** /api/v2/notifications/read | Set all Notifications as read
+*NotificationsApi* | [**api_v2_notifications_search_post**](docs/NotificationsApi.md#api_v2_notifications_search_post) | **POST** /api/v2/notifications/search | Search Notifications for current User
+*ParametersApi* | [**api_v2_parameters_bulk_post**](docs/ParametersApi.md#api_v2_parameters_bulk_post) | **POST** /api/v2/parameters/bulk | Create multiple parameters
+*ParametersApi* | [**api_v2_parameters_bulk_put**](docs/ParametersApi.md#api_v2_parameters_bulk_put) | **PUT** /api/v2/parameters/bulk | Update multiple parameters
+*ParametersApi* | [**api_v2_parameters_groups_get**](docs/ParametersApi.md#api_v2_parameters_groups_get) | **GET** /api/v2/parameters/groups | Get parameters as group
+*ParametersApi* | [**api_v2_parameters_key_name_name_exists_get**](docs/ParametersApi.md#api_v2_parameters_key_name_name_exists_get) | **GET** /api/v2/parameters/key/name/{name}/exists | Check existence parameter key in system
+*ParametersApi* | [**api_v2_parameters_key_values_get**](docs/ParametersApi.md#api_v2_parameters_key_values_get) | **GET** /api/v2/parameters/{key}/values | Get all parameter key values
+*ParametersApi* | [**api_v2_parameters_keys_get**](docs/ParametersApi.md#api_v2_parameters_keys_get) | **GET** /api/v2/parameters/keys | Get all parameter keys
+*ParametersApi* | [**api_v2_parameters_search_post**](docs/ParametersApi.md#api_v2_parameters_search_post) | **POST** /api/v2/parameters/search | Search for parameters
+*ParametersApi* | [**create_parameter**](docs/ParametersApi.md#create_parameter) | **POST** /api/v2/parameters | Create parameter
+*ParametersApi* | [**delete_by_name**](docs/ParametersApi.md#delete_by_name) | **DELETE** /api/v2/parameters/name/{name} | Delete parameter by name
+*ParametersApi* | [**delete_by_parameter_key_id**](docs/ParametersApi.md#delete_by_parameter_key_id) | **DELETE** /api/v2/parameters/keyId/{keyId} | Delete parameters by parameter key identifier
+*ParametersApi* | [**delete_parameter**](docs/ParametersApi.md#delete_parameter) | **DELETE** /api/v2/parameters/{id} | Delete parameter
+*ParametersApi* | [**get_all_parameters**](docs/ParametersApi.md#get_all_parameters) | **GET** /api/v2/parameters | Get all parameters
+*ParametersApi* | [**get_parameter_by_id**](docs/ParametersApi.md#get_parameter_by_id) | **GET** /api/v2/parameters/{id} | Get parameter by ID
+*ParametersApi* | [**obsolete_delete_by_name**](docs/ParametersApi.md#obsolete_delete_by_name) | **POST** /api/v2/parameters/deleteByName | 
+*ParametersApi* | [**update_parameter**](docs/ParametersApi.md#update_parameter) | **PUT** /api/v2/parameters | Update parameter
+*ProjectsApi* | [**add_globa_attributes_to_project**](docs/ProjectsApi.md#add_globa_attributes_to_project) | **POST** /api/v2/projects/{id}/globalAttributes | Add global attributes to project
+*ProjectsApi* | [**api_v2_projects_id_attributes_templates_search_post**](docs/ProjectsApi.md#api_v2_projects_id_attributes_templates_search_post) | **POST** /api/v2/projects/{id}/attributes/templates/search | Search for custom attributes templates
+*ProjectsApi* | [**api_v2_projects_id_attributes_templates_template_id_delete**](docs/ProjectsApi.md#api_v2_projects_id_attributes_templates_template_id_delete) | **DELETE** /api/v2/projects/{id}/attributes/templates/{templateId} | Delete CustomAttributeTemplate from Project
+*ProjectsApi* | [**api_v2_projects_id_attributes_templates_template_id_post**](docs/ProjectsApi.md#api_v2_projects_id_attributes_templates_template_id_post) | **POST** /api/v2/projects/{id}/attributes/templates/{templateId} | Add CustomAttributeTemplate to Project
+*ProjectsApi* | [**api_v2_projects_id_failure_classes_get**](docs/ProjectsApi.md#api_v2_projects_id_failure_classes_get) | **GET** /api/v2/projects/{id}/failureClasses | Get Project FailureClasses
+*ProjectsApi* | [**api_v2_projects_id_favorite_put**](docs/ProjectsApi.md#api_v2_projects_id_favorite_put) | **PUT** /api/v2/projects/{id}/favorite | Mark Project as favorite
+*ProjectsApi* | [**api_v2_projects_id_filters_get**](docs/ProjectsApi.md#api_v2_projects_id_filters_get) | **GET** /api/v2/projects/{id}/filters | Get Project filters
+*ProjectsApi* | [**api_v2_projects_id_patch**](docs/ProjectsApi.md#api_v2_projects_id_patch) | **PATCH** /api/v2/projects/{id} | Patch project
+*ProjectsApi* | [**api_v2_projects_id_test_plans_analytics_get**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_analytics_get) | **GET** /api/v2/projects/{id}/testPlans/analytics | Get TestPlans analytics
+*ProjectsApi* | [**api_v2_projects_id_test_plans_delete_bulk_post**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_delete_bulk_post) | **POST** /api/v2/projects/{id}/testPlans/delete/bulk | Delete multiple test plans
+*ProjectsApi* | [**api_v2_projects_id_test_plans_name_exists_get**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_name_exists_get) | **GET** /api/v2/projects/{id}/testPlans/{name}/exists | Checks if TestPlan exists with the specified name exists for the project
+*ProjectsApi* | [**api_v2_projects_id_test_plans_restore_bulk_post**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_restore_bulk_post) | **POST** /api/v2/projects/{id}/testPlans/restore/bulk | Restore multiple test plans
+*ProjectsApi* | [**api_v2_projects_id_test_plans_search_post**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_search_post) | **POST** /api/v2/projects/{id}/testPlans/search | Get Project TestPlans with analytics
+*ProjectsApi* | [**api_v2_projects_id_test_runs_active_get**](docs/ProjectsApi.md#api_v2_projects_id_test_runs_active_get) | **GET** /api/v2/projects/{id}/testRuns/active | Get active Project TestRuns
+*ProjectsApi* | [**api_v2_projects_id_test_runs_full_get**](docs/ProjectsApi.md#api_v2_projects_id_test_runs_full_get) | **GET** /api/v2/projects/{id}/testRuns/full | Get Project TestRuns full models
+*ProjectsApi* | [**api_v2_projects_id_work_items_search_id_post**](docs/ProjectsApi.md#api_v2_projects_id_work_items_search_id_post) | **POST** /api/v2/projects/{id}/workItems/search/id | Search for work items and extract IDs only
+*ProjectsApi* | [**api_v2_projects_id_work_items_search_post**](docs/ProjectsApi.md#api_v2_projects_id_work_items_search_post) | **POST** /api/v2/projects/{id}/workItems/search | Search for work items
+*ProjectsApi* | [**api_v2_projects_id_work_items_tags_get**](docs/ProjectsApi.md#api_v2_projects_id_work_items_tags_get) | **GET** /api/v2/projects/{id}/workItems/tags | Get WorkItems Tags
+*ProjectsApi* | [**api_v2_projects_name_name_exists_get**](docs/ProjectsApi.md#api_v2_projects_name_name_exists_get) | **GET** /api/v2/projects/name/{name}/exists | 
+*ProjectsApi* | [**api_v2_projects_search_post**](docs/ProjectsApi.md#api_v2_projects_search_post) | **POST** /api/v2/projects/search | Search for projects
+*ProjectsApi* | [**background_import_project**](docs/ProjectsApi.md#background_import_project) | **POST** /api/v2/projects/import/json | Import project from JSON file in background job
+*ProjectsApi* | [**background_import_to_existing_project**](docs/ProjectsApi.md#background_import_to_existing_project) | **POST** /api/v2/projects/{id}/import/json | Import project from JSON file into existing project in background job
+*ProjectsApi* | [**background_import_zip_project**](docs/ProjectsApi.md#background_import_zip_project) | **POST** /api/v2/projects/import/zip | Import project from Zip file in background job
+*ProjectsApi* | [**background_import_zip_to_existing_project**](docs/ProjectsApi.md#background_import_zip_to_existing_project) | **POST** /api/v2/projects/{id}/import/zip | Import project from Zip file into existing project in background job
+*ProjectsApi* | [**call_import**](docs/ProjectsApi.md#call_import) | **POST** /api/v2/projects/import | Import project from JSON file
+*ProjectsApi* | [**create_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#create_custom_attribute_test_plan_project_relations) | **POST** /api/v2/projects/{id}/testPlans/attributes | Add attributes to project&#39;s test plans
+*ProjectsApi* | [**create_project**](docs/ProjectsApi.md#create_project) | **POST** /api/v2/projects | Create project
+*ProjectsApi* | [**create_projects_attribute**](docs/ProjectsApi.md#create_projects_attribute) | **POST** /api/v2/projects/{id}/attributes | Create project attribute
+*ProjectsApi* | [**delete_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#delete_custom_attribute_test_plan_project_relations) | **DELETE** /api/v2/projects/{id}/testPlans/attribute/{attributeId} | Delete attribute from project&#39;s test plans
+*ProjectsApi* | [**delete_project**](docs/ProjectsApi.md#delete_project) | **DELETE** /api/v2/projects/{id} | Delete project
+*ProjectsApi* | [**delete_project_auto_tests**](docs/ProjectsApi.md#delete_project_auto_tests) | **DELETE** /api/v2/projects/{id}/autoTests | Delete project
+*ProjectsApi* | [**delete_projects_attribute**](docs/ProjectsApi.md#delete_projects_attribute) | **DELETE** /api/v2/projects/{id}/attributes/{attributeId} | Delete project attribute
+*ProjectsApi* | [**export**](docs/ProjectsApi.md#export) | **POST** /api/v2/projects/{id}/export | Export project as JSON file
+*ProjectsApi* | [**export_project_json**](docs/ProjectsApi.md#export_project_json) | **POST** /api/v2/projects/{id}/export/json | Export project as JSON file in background job
+*ProjectsApi* | [**export_project_with_test_plans_json**](docs/ProjectsApi.md#export_project_with_test_plans_json) | **POST** /api/v2/projects/{id}/export/testPlans/json | Export project as JSON file with test plans in background job
+*ProjectsApi* | [**export_project_with_test_plans_zip**](docs/ProjectsApi.md#export_project_with_test_plans_zip) | **POST** /api/v2/projects/{id}/export/testPlans/zip | Export project as Zip file with test plans in background job
+*ProjectsApi* | [**export_project_zip**](docs/ProjectsApi.md#export_project_zip) | **POST** /api/v2/projects/{id}/export/zip | Export project as Zip file in background job
+*ProjectsApi* | [**export_with_test_plans_and_configurations**](docs/ProjectsApi.md#export_with_test_plans_and_configurations) | **POST** /api/v2/projects/{id}/export-by-testPlans | Export project with test plans, test suites and test points as JSON file
+*ProjectsApi* | [**get_all_projects**](docs/ProjectsApi.md#get_all_projects) | **GET** /api/v2/projects | Get all projects
+*ProjectsApi* | [**get_attribute_by_project_id**](docs/ProjectsApi.md#get_attribute_by_project_id) | **GET** /api/v2/projects/{id}/attributes/{attributeId} | Get project attribute
+*ProjectsApi* | [**get_attributes_by_project_id**](docs/ProjectsApi.md#get_attributes_by_project_id) | **GET** /api/v2/projects/{id}/attributes | Get project attributes
+*ProjectsApi* | [**get_auto_tests_namespaces**](docs/ProjectsApi.md#get_auto_tests_namespaces) | **GET** /api/v2/projects/{id}/autoTestsNamespaces | Get namespaces of autotests in project
+*ProjectsApi* | [**get_configurations_by_project_id**](docs/ProjectsApi.md#get_configurations_by_project_id) | **GET** /api/v2/projects/{id}/configurations | Get project configurations
+*ProjectsApi* | [**get_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#get_custom_attribute_test_plan_project_relations) | **GET** /api/v2/projects/{id}/testPlans/attributes | Get project&#39;s test plan attributes
+*ProjectsApi* | [**get_project_by_id**](docs/ProjectsApi.md#get_project_by_id) | **GET** /api/v2/projects/{id} | Get project by ID
+*ProjectsApi* | [**get_sections_by_project_id**](docs/ProjectsApi.md#get_sections_by_project_id) | **GET** /api/v2/projects/{id}/sections | Get project sections
+*ProjectsApi* | [**get_test_plans_by_project_id**](docs/ProjectsApi.md#get_test_plans_by_project_id) | **GET** /api/v2/projects/{id}/testPlans | Get project test plans
+*ProjectsApi* | [**get_test_runs_by_project_id**](docs/ProjectsApi.md#get_test_runs_by_project_id) | **GET** /api/v2/projects/{id}/testRuns | Get project test runs
+*ProjectsApi* | [**get_work_items_by_project_id**](docs/ProjectsApi.md#get_work_items_by_project_id) | **GET** /api/v2/projects/{id}/workItems | Get project work items
+*ProjectsApi* | [**import_to_existing_project**](docs/ProjectsApi.md#import_to_existing_project) | **POST** /api/v2/projects/{id}/import | Import project from JSON file into existing project
+*ProjectsApi* | [**restore_project**](docs/ProjectsApi.md#restore_project) | **POST** /api/v2/projects/{id}/restore | Restore project
+*ProjectsApi* | [**search_attributes_in_project**](docs/ProjectsApi.md#search_attributes_in_project) | **POST** /api/v2/projects/{id}/attributes/search | Search for attributes used in the project
+*ProjectsApi* | [**search_test_plan_attributes_in_project**](docs/ProjectsApi.md#search_test_plan_attributes_in_project) | **POST** /api/v2/projects/{id}/testPlans/attributes/search | Search for attributes used in the project test plans
+*ProjectsApi* | [**update_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#update_custom_attribute_test_plan_project_relations) | **PUT** /api/v2/projects/{id}/testPlans/attribute | Update attribute of project&#39;s test plans
+*ProjectsApi* | [**update_project**](docs/ProjectsApi.md#update_project) | **PUT** /api/v2/projects | Update project
+*ProjectsApi* | [**update_projects_attribute**](docs/ProjectsApi.md#update_projects_attribute) | **PUT** /api/v2/projects/{id}/attributes | Edit attribute of the project
+*SectionsApi* | [**api_v2_sections_id_patch**](docs/SectionsApi.md#api_v2_sections_id_patch) | **PATCH** /api/v2/sections/{id} | Patch section
+*SectionsApi* | [**create_section**](docs/SectionsApi.md#create_section) | **POST** /api/v2/sections | Create section
+*SectionsApi* | [**delete_section**](docs/SectionsApi.md#delete_section) | **DELETE** /api/v2/sections/{id} | Delete section
+*SectionsApi* | [**get_section_by_id**](docs/SectionsApi.md#get_section_by_id) | **GET** /api/v2/sections/{id} | Get section
+*SectionsApi* | [**get_work_items_by_section_id**](docs/SectionsApi.md#get_work_items_by_section_id) | **GET** /api/v2/sections/{id}/workItems | Get section work items
+*SectionsApi* | [**move**](docs/SectionsApi.md#move) | **POST** /api/v2/sections/move | Move section with all work items into another section
+*SectionsApi* | [**rename**](docs/SectionsApi.md#rename) | **POST** /api/v2/sections/rename | Rename section
+*SectionsApi* | [**update_section**](docs/SectionsApi.md#update_section) | **PUT** /api/v2/sections | Update section
+*TagsApi* | [**api_v2_tags_get**](docs/TagsApi.md#api_v2_tags_get) | **GET** /api/v2/tags | Get all Tags
+*TagsApi* | [**api_v2_tags_test_plans_tags_get**](docs/TagsApi.md#api_v2_tags_test_plans_tags_get) | **GET** /api/v2/tags/testPlansTags | Get all Tags that are used in TestPlans
+*TestPlansApi* | [**add_test_points_with_sections**](docs/TestPlansApi.md#add_test_points_with_sections) | **POST** /api/v2/testPlans/{id}/test-points/withSections | Add test-points to TestPlan with sections
+*TestPlansApi* | [**add_work_items_with_sections**](docs/TestPlansApi.md#add_work_items_with_sections) | **POST** /api/v2/testPlans/{id}/workItems/withSections | Add WorkItems to TestPlan with Sections as TestSuites
+*TestPlansApi* | [**api_v2_test_plans_id_analytics_get**](docs/TestPlansApi.md#api_v2_test_plans_id_analytics_get) | **GET** /api/v2/testPlans/{id}/analytics | Get analytics by TestPlan
+*TestPlansApi* | [**api_v2_test_plans_id_autobalance_post**](docs/TestPlansApi.md#api_v2_test_plans_id_autobalance_post) | **POST** /api/v2/testPlans/{id}/autobalance | Distribute test points between the users
+*TestPlansApi* | [**api_v2_test_plans_id_configurations_get**](docs/TestPlansApi.md#api_v2_test_plans_id_configurations_get) | **GET** /api/v2/testPlans/{id}/configurations | Get TestPlan configurations
+*TestPlansApi* | [**api_v2_test_plans_id_export_test_points_xlsx_post**](docs/TestPlansApi.md#api_v2_test_plans_id_export_test_points_xlsx_post) | **POST** /api/v2/testPlans/{id}/export/testPoints/xlsx | Export TestPoints from TestPlan in xls format
+*TestPlansApi* | [**api_v2_test_plans_id_export_test_result_history_xlsx_post**](docs/TestPlansApi.md#api_v2_test_plans_id_export_test_result_history_xlsx_post) | **POST** /api/v2/testPlans/{id}/export/testResultHistory/xlsx | Export TestResults history from TestPlan in xls format
+*TestPlansApi* | [**api_v2_test_plans_id_history_get**](docs/TestPlansApi.md#api_v2_test_plans_id_history_get) | **GET** /api/v2/testPlans/{id}/history | Get TestPlan history
+*TestPlansApi* | [**api_v2_test_plans_id_links_get**](docs/TestPlansApi.md#api_v2_test_plans_id_links_get) | **GET** /api/v2/testPlans/{id}/links | Get Links of TestPlan
+*TestPlansApi* | [**api_v2_test_plans_id_patch**](docs/TestPlansApi.md#api_v2_test_plans_id_patch) | **PATCH** /api/v2/testPlans/{id} | Patch test plan
+*TestPlansApi* | [**api_v2_test_plans_id_test_points_last_results_get**](docs/TestPlansApi.md#api_v2_test_plans_id_test_points_last_results_get) | **GET** /api/v2/testPlans/{id}/testPoints/lastResults | Get TestPoints with last result from TestPlan
+*TestPlansApi* | [**api_v2_test_plans_id_test_points_reset_post**](docs/TestPlansApi.md#api_v2_test_plans_id_test_points_reset_post) | **POST** /api/v2/testPlans/{id}/testPoints/reset | Reset TestPoints status of TestPlan
+*TestPlansApi* | [**api_v2_test_plans_id_test_points_tester_delete**](docs/TestPlansApi.md#api_v2_test_plans_id_test_points_tester_delete) | **DELETE** /api/v2/testPlans/{id}/testPoints/tester | Unassign users from multiple test points
+*TestPlansApi* | [**api_v2_test_plans_id_test_points_tester_user_id_post**](docs/TestPlansApi.md#api_v2_test_plans_id_test_points_tester_user_id_post) | **POST** /api/v2/testPlans/{id}/testPoints/tester/{userId} | Assign user as a tester to multiple test points
+*TestPlansApi* | [**api_v2_test_plans_id_test_runs_get**](docs/TestPlansApi.md#api_v2_test_plans_id_test_runs_get) | **GET** /api/v2/testPlans/{id}/testRuns | Get TestRuns of TestPlan
+*TestPlansApi* | [**api_v2_test_plans_id_test_runs_search_post**](docs/TestPlansApi.md#api_v2_test_plans_id_test_runs_search_post) | **POST** /api/v2/testPlans/{id}/testRuns/search | Search TestRuns of TestPlan
+*TestPlansApi* | [**api_v2_test_plans_id_test_runs_test_results_last_modified_modified_date_get**](docs/TestPlansApi.md#api_v2_test_plans_id_test_runs_test_results_last_modified_modified_date_get) | **GET** /api/v2/testPlans/{id}/testRuns/testResults/lastModified/modifiedDate | Get last modification date of test plan&#39;s test results
+*TestPlansApi* | [**api_v2_test_plans_id_unlock_request_post**](docs/TestPlansApi.md#api_v2_test_plans_id_unlock_request_post) | **POST** /api/v2/testPlans/{id}/unlock/request | Send unlock TestPlan notification
+*TestPlansApi* | [**api_v2_test_plans_shorts_post**](docs/TestPlansApi.md#api_v2_test_plans_shorts_post) | **POST** /api/v2/testPlans/shorts | Get TestPlans short models by Project identifiers
+*TestPlansApi* | [**clone**](docs/TestPlansApi.md#clone) | **POST** /api/v2/testPlans/{id}/clone | Clone TestPlan
+*TestPlansApi* | [**complete**](docs/TestPlansApi.md#complete) | **POST** /api/v2/testPlans/{id}/complete | Complete TestPlan
+*TestPlansApi* | [**create_test_plan**](docs/TestPlansApi.md#create_test_plan) | **POST** /api/v2/testPlans | Create TestPlan
+*TestPlansApi* | [**delete_test_plan**](docs/TestPlansApi.md#delete_test_plan) | **DELETE** /api/v2/testPlans/{id} | Delete TestPlan
+*TestPlansApi* | [**get_test_plan_by_id**](docs/TestPlansApi.md#get_test_plan_by_id) | **GET** /api/v2/testPlans/{id} | Get TestPlan by Id
+*TestPlansApi* | [**get_test_suites_by_id**](docs/TestPlansApi.md#get_test_suites_by_id) | **GET** /api/v2/testPlans/{id}/testSuites | Get TestSuites Tree By Id
+*TestPlansApi* | [**pause**](docs/TestPlansApi.md#pause) | **POST** /api/v2/testPlans/{id}/pause | Pause TestPlan
+*TestPlansApi* | [**restore_test_plan**](docs/TestPlansApi.md#restore_test_plan) | **POST** /api/v2/testPlans/{id}/restore | Restore TestPlan
+*TestPlansApi* | [**start**](docs/TestPlansApi.md#start) | **POST** /api/v2/testPlans/{id}/start | Start TestPlan
+*TestPlansApi* | [**update_test_plan**](docs/TestPlansApi.md#update_test_plan) | **PUT** /api/v2/testPlans | Update TestPlan
+*TestPointsApi* | [**api_v2_test_points_id_test_runs_get**](docs/TestPointsApi.md#api_v2_test_points_id_test_runs_get) | **GET** /api/v2/testPoints/{id}/testRuns | Get all test runs which use test point
+*TestPointsApi* | [**api_v2_test_points_id_work_item_get**](docs/TestPointsApi.md#api_v2_test_points_id_work_item_get) | **GET** /api/v2/testPoints/{id}/workItem | Get work item represented by test point
+*TestPointsApi* | [**api_v2_test_points_search_id_post**](docs/TestPointsApi.md#api_v2_test_points_search_id_post) | **POST** /api/v2/testPoints/search/id | Search for test points and extract IDs only
+*TestPointsApi* | [**api_v2_test_points_search_post**](docs/TestPointsApi.md#api_v2_test_points_search_post) | **POST** /api/v2/testPoints/search | Search for test points
+*TestResultsApi* | [**api_v2_test_results_id_aggregated_get**](docs/TestResultsApi.md#api_v2_test_results_id_aggregated_get) | **GET** /api/v2/testResults/{id}/aggregated | Get test result by ID aggregated with previous results
+*TestResultsApi* | [**api_v2_test_results_id_attachments_attachment_id_put**](docs/TestResultsApi.md#api_v2_test_results_id_attachments_attachment_id_put) | **PUT** /api/v2/testResults/{id}/attachments/{attachmentId} | Attach file to the test result
+*TestResultsApi* | [**api_v2_test_results_id_attachments_info_get**](docs/TestResultsApi.md#api_v2_test_results_id_attachments_info_get) | **GET** /api/v2/testResults/{id}/attachments/info | Get test result attachments meta-information
+*TestResultsApi* | [**api_v2_test_results_id_get**](docs/TestResultsApi.md#api_v2_test_results_id_get) | **GET** /api/v2/testResults/{id} | Get test result by ID
+*TestResultsApi* | [**api_v2_test_results_id_put**](docs/TestResultsApi.md#api_v2_test_results_id_put) | **PUT** /api/v2/testResults/{id} | Edit test result by ID
+*TestResultsApi* | [**api_v2_test_results_search_post**](docs/TestResultsApi.md#api_v2_test_results_search_post) | **POST** /api/v2/testResults/search | Search for test results
+*TestResultsApi* | [**api_v2_test_results_statistics_filter_post**](docs/TestResultsApi.md#api_v2_test_results_statistics_filter_post) | **POST** /api/v2/testResults/statistics/filter | Search for test results and extract statistics
+*TestResultsApi* | [**create_attachment**](docs/TestResultsApi.md#create_attachment) | **POST** /api/v2/testResults/{id}/attachments | Upload and link attachment to TestResult
+*TestResultsApi* | [**delete_attachment**](docs/TestResultsApi.md#delete_attachment) | **DELETE** /api/v2/testResults/{id}/attachments/{attachmentId} | Remove attachment and unlink from TestResult
+*TestResultsApi* | [**download_attachment**](docs/TestResultsApi.md#download_attachment) | **GET** /api/v2/testResults/{id}/attachments/{attachmentId} | Get attachment of TestResult
+*TestResultsApi* | [**get_attachment**](docs/TestResultsApi.md#get_attachment) | **GET** /api/v2/testResults/{id}/attachments/{attachmentId}/info | Get Metadata of TestResult&#39;s attachment
+*TestResultsApi* | [**get_attachments**](docs/TestResultsApi.md#get_attachments) | **GET** /api/v2/testResults/{id}/attachments | Get all attachments of TestResult
+*TestRunsApi* | [**api_v2_test_runs_id_statistics_filter_post**](docs/TestRunsApi.md#api_v2_test_runs_id_statistics_filter_post) | **POST** /api/v2/testRuns/{id}/statistics/filter | Search for the test run test results and build statistics
+*TestRunsApi* | [**api_v2_test_runs_id_test_points_results_get**](docs/TestRunsApi.md#api_v2_test_runs_id_test_points_results_get) | **GET** /api/v2/testRuns/{id}/testPoints/results | Get test results from the test run grouped by test points
+*TestRunsApi* | [**api_v2_test_runs_id_test_results_bulk_put**](docs/TestRunsApi.md#api_v2_test_runs_id_test_results_bulk_put) | **PUT** /api/v2/testRuns/{id}/testResults/bulk | Partial edit of multiple test results in the test run
+*TestRunsApi* | [**api_v2_test_runs_id_test_results_last_modified_modification_date_get**](docs/TestRunsApi.md#api_v2_test_runs_id_test_results_last_modified_modification_date_get) | **GET** /api/v2/testRuns/{id}/testResults/lastModified/modificationDate | Get modification date of last test result of the test run
+*TestRunsApi* | [**api_v2_test_runs_search_post**](docs/TestRunsApi.md#api_v2_test_runs_search_post) | **POST** /api/v2/testRuns/search | Search for test runs
+*TestRunsApi* | [**complete_test_run**](docs/TestRunsApi.md#complete_test_run) | **POST** /api/v2/testRuns/{id}/complete | Complete TestRun
+*TestRunsApi* | [**create_and_fill_by_auto_tests**](docs/TestRunsApi.md#create_and_fill_by_auto_tests) | **POST** /api/v2/testRuns/byAutoTests | Create test runs based on autotests and configurations
+*TestRunsApi* | [**create_and_fill_by_configurations**](docs/TestRunsApi.md#create_and_fill_by_configurations) | **POST** /api/v2/testRuns/byConfigurations | Create test runs picking the needed test points
+*TestRunsApi* | [**create_and_fill_by_work_items**](docs/TestRunsApi.md#create_and_fill_by_work_items) | **POST** /api/v2/testRuns/byWorkItems | Create test run based on configurations and work items
+*TestRunsApi* | [**create_empty**](docs/TestRunsApi.md#create_empty) | **POST** /api/v2/testRuns | Create empty TestRun
+*TestRunsApi* | [**get_test_run_by_id**](docs/TestRunsApi.md#get_test_run_by_id) | **GET** /api/v2/testRuns/{id} | Get TestRun by Id
+*TestRunsApi* | [**set_auto_test_results_for_test_run**](docs/TestRunsApi.md#set_auto_test_results_for_test_run) | **POST** /api/v2/testRuns/{id}/testResults | Send test results to the test runs in the system
+*TestRunsApi* | [**start_test_run**](docs/TestRunsApi.md#start_test_run) | **POST** /api/v2/testRuns/{id}/start | Start TestRun
+*TestRunsApi* | [**stop_test_run**](docs/TestRunsApi.md#stop_test_run) | **POST** /api/v2/testRuns/{id}/stop | Stop TestRun
+*TestRunsApi* | [**update_empty**](docs/TestRunsApi.md#update_empty) | **PUT** /api/v2/testRuns | Update empty TestRun
+*TestSuitesApi* | [**add_test_points_to_test_suite**](docs/TestSuitesApi.md#add_test_points_to_test_suite) | **POST** /api/v2/testSuites/{id}/test-points | Add test-points to test suite
+*TestSuitesApi* | [**api_v2_test_suites_id_patch**](docs/TestSuitesApi.md#api_v2_test_suites_id_patch) | **PATCH** /api/v2/testSuites/{id} | Patch test suite
+*TestSuitesApi* | [**api_v2_test_suites_id_refresh_post**](docs/TestSuitesApi.md#api_v2_test_suites_id_refresh_post) | **POST** /api/v2/testSuites/{id}/refresh | Refresh test suite. Only dynamic test suites are supported by this method
+*TestSuitesApi* | [**create_test_suite**](docs/TestSuitesApi.md#create_test_suite) | **POST** /api/v2/testSuites | Create TestSuite
+*TestSuitesApi* | [**delete_test_suite**](docs/TestSuitesApi.md#delete_test_suite) | **DELETE** /api/v2/testSuites/{id} | Delete TestSuite
+*TestSuitesApi* | [**get_configurations_by_test_suite_id**](docs/TestSuitesApi.md#get_configurations_by_test_suite_id) | **GET** /api/v2/testSuites/{id}/configurations | Get Configurations By Id
+*TestSuitesApi* | [**get_test_points_by_id**](docs/TestSuitesApi.md#get_test_points_by_id) | **GET** /api/v2/testSuites/{id}/testPoints | Get TestPoints By Id
+*TestSuitesApi* | [**get_test_results_by_id**](docs/TestSuitesApi.md#get_test_results_by_id) | **GET** /api/v2/testSuites/{id}/testResults | Get TestResults By Id
+*TestSuitesApi* | [**get_test_suite_by_id**](docs/TestSuitesApi.md#get_test_suite_by_id) | **GET** /api/v2/testSuites/{id} | Get TestSuite by Id
+*TestSuitesApi* | [**get_work_items_by_id**](docs/TestSuitesApi.md#get_work_items_by_id) | **GET** /api/v2/testSuites/{id}/workItems | 
+*TestSuitesApi* | [**search_work_items**](docs/TestSuitesApi.md#search_work_items) | **POST** /api/v2/testSuites/{id}/workItems/search | Search WorkItems
+*TestSuitesApi* | [**set_configurations_by_test_suite_id**](docs/TestSuitesApi.md#set_configurations_by_test_suite_id) | **POST** /api/v2/testSuites/{id}/configurations | Set Configurations By TestSuite Id
+*TestSuitesApi* | [**set_work_items_by_test_suite_id**](docs/TestSuitesApi.md#set_work_items_by_test_suite_id) | **POST** /api/v2/testSuites/{id}/workItems | Set WorkItems By TestSuite Id
+*TestSuitesApi* | [**update_test_suite**](docs/TestSuitesApi.md#update_test_suite) | **PUT** /api/v2/testSuites | Update TestSuite
+*WebhooksApi* | [**api_v2_webhooks_get**](docs/WebhooksApi.md#api_v2_webhooks_get) | **GET** /api/v2/webhooks | Get all webhooks
+*WebhooksApi* | [**api_v2_webhooks_id_delete**](docs/WebhooksApi.md#api_v2_webhooks_id_delete) | **DELETE** /api/v2/webhooks/{id} | Delete webhook by ID
+*WebhooksApi* | [**api_v2_webhooks_id_get**](docs/WebhooksApi.md#api_v2_webhooks_id_get) | **GET** /api/v2/webhooks/{id} | Get webhook by ID
+*WebhooksApi* | [**api_v2_webhooks_id_put**](docs/WebhooksApi.md#api_v2_webhooks_id_put) | **PUT** /api/v2/webhooks/{id} | Edit webhook by ID
+*WebhooksApi* | [**api_v2_webhooks_post**](docs/WebhooksApi.md#api_v2_webhooks_post) | **POST** /api/v2/webhooks | Create webhook
+*WebhooksApi* | [**api_v2_webhooks_search_post**](docs/WebhooksApi.md#api_v2_webhooks_search_post) | **POST** /api/v2/webhooks/search | Search for webhooks
+*WebhooksApi* | [**api_v2_webhooks_special_variables_get**](docs/WebhooksApi.md#api_v2_webhooks_special_variables_get) | **GET** /api/v2/webhooks/specialVariables | Get special variables for webhook event type
+*WebhooksLogsApi* | [**api_v2_webhooks_logs_get**](docs/WebhooksLogsApi.md#api_v2_webhooks_logs_get) | **GET** /api/v2/webhooks/logs | Get all webhook logs
+*WebhooksLogsApi* | [**api_v2_webhooks_logs_id_delete**](docs/WebhooksLogsApi.md#api_v2_webhooks_logs_id_delete) | **DELETE** /api/v2/webhooks/logs/{id} | Delete webhook log by ID
+*WebhooksLogsApi* | [**api_v2_webhooks_logs_id_get**](docs/WebhooksLogsApi.md#api_v2_webhooks_logs_id_get) | **GET** /api/v2/webhooks/logs/{id} | Get webhook log by ID
+*WorkItemsApi* | [**api_v2_work_items_id_attachments_post**](docs/WorkItemsApi.md#api_v2_work_items_id_attachments_post) | **POST** /api/v2/workItems/{id}/attachments | Upload and link attachment to WorkItem
+*WorkItemsApi* | [**api_v2_work_items_id_check_list_transform_to_test_case_post**](docs/WorkItemsApi.md#api_v2_work_items_id_check_list_transform_to_test_case_post) | **POST** /api/v2/workItems/{id}/checkList/transformTo/testCase | Transform CheckList to TestCase
+*WorkItemsApi* | [**api_v2_work_items_id_history_get**](docs/WorkItemsApi.md#api_v2_work_items_id_history_get) | **GET** /api/v2/workItems/{id}/history | Get change history of WorkItem
+*WorkItemsApi* | [**api_v2_work_items_id_like_delete**](docs/WorkItemsApi.md#api_v2_work_items_id_like_delete) | **DELETE** /api/v2/workItems/{id}/like | Delete like from WorkItem
+*WorkItemsApi* | [**api_v2_work_items_id_like_post**](docs/WorkItemsApi.md#api_v2_work_items_id_like_post) | **POST** /api/v2/workItems/{id}/like | Set like to WorkItem
+*WorkItemsApi* | [**api_v2_work_items_id_likes_count_get**](docs/WorkItemsApi.md#api_v2_work_items_id_likes_count_get) | **GET** /api/v2/workItems/{id}/likes/count | Get likes count of WorkItem
+*WorkItemsApi* | [**api_v2_work_items_id_likes_get**](docs/WorkItemsApi.md#api_v2_work_items_id_likes_get) | **GET** /api/v2/workItems/{id}/likes | Get likes of WorkItem
+*WorkItemsApi* | [**api_v2_work_items_id_test_results_history_get**](docs/WorkItemsApi.md#api_v2_work_items_id_test_results_history_get) | **GET** /api/v2/workItems/{id}/testResults/history | Get test results history of WorkItem
+*WorkItemsApi* | [**api_v2_work_items_id_version_version_id_actual_post**](docs/WorkItemsApi.md#api_v2_work_items_id_version_version_id_actual_post) | **POST** /api/v2/workItems/{id}/version/{versionId}/actual | Set WorkItem as actual
+*WorkItemsApi* | [**api_v2_work_items_move_post**](docs/WorkItemsApi.md#api_v2_work_items_move_post) | **POST** /api/v2/workItems/move | Move WorkItem to another section
+*WorkItemsApi* | [**api_v2_work_items_search_post**](docs/WorkItemsApi.md#api_v2_work_items_search_post) | **POST** /api/v2/workItems/search | Search for work items
+*WorkItemsApi* | [**api_v2_work_items_shared_step_id_references_sections_post**](docs/WorkItemsApi.md#api_v2_work_items_shared_step_id_references_sections_post) | **POST** /api/v2/workItems/{sharedStepId}/references/sections | Get SharedStep references in sections
+*WorkItemsApi* | [**api_v2_work_items_shared_step_id_references_work_items_post**](docs/WorkItemsApi.md#api_v2_work_items_shared_step_id_references_work_items_post) | **POST** /api/v2/workItems/{sharedStepId}/references/workItems | Get SharedStep references in workitems
+*WorkItemsApi* | [**api_v2_work_items_shared_steps_shared_step_id_references_get**](docs/WorkItemsApi.md#api_v2_work_items_shared_steps_shared_step_id_references_get) | **GET** /api/v2/workItems/sharedSteps/{sharedStepId}/references | Get SharedStep references
+*WorkItemsApi* | [**create_work_item**](docs/WorkItemsApi.md#create_work_item) | **POST** /api/v2/workItems | Create Test Case, Checklist or Shared Step
+*WorkItemsApi* | [**delete_all_work_items_from_auto_test**](docs/WorkItemsApi.md#delete_all_work_items_from_auto_test) | **DELETE** /api/v2/workItems/{id}/autoTests | Delete all links AutoTests from WorkItem by Id or GlobalId
+*WorkItemsApi* | [**delete_work_item**](docs/WorkItemsApi.md#delete_work_item) | **DELETE** /api/v2/workItems/{id} | Delete Test Case, Checklist or Shared Step by Id or GlobalId
+*WorkItemsApi* | [**get_auto_tests_for_work_item**](docs/WorkItemsApi.md#get_auto_tests_for_work_item) | **GET** /api/v2/workItems/{id}/autoTests | Get all AutoTests linked to WorkItem by Id or GlobalId
+*WorkItemsApi* | [**get_iterations**](docs/WorkItemsApi.md#get_iterations) | **GET** /api/v2/workItems/{id}/iterations | Get iterations by workitem Id or GlobalId
+*WorkItemsApi* | [**get_work_item_by_id**](docs/WorkItemsApi.md#get_work_item_by_id) | **GET** /api/v2/workItems/{id} | Get Test Case, Checklist or Shared Step by Id or GlobalId
+*WorkItemsApi* | [**get_work_item_chronology**](docs/WorkItemsApi.md#get_work_item_chronology) | **GET** /api/v2/workItems/{id}/chronology | Get WorkItem chronology by Id or GlobalId
+*WorkItemsApi* | [**get_work_item_versions**](docs/WorkItemsApi.md#get_work_item_versions) | **GET** /api/v2/workItems/{id}/versions | Get WorkItem versions
+*WorkItemsApi* | [**purge_work_item**](docs/WorkItemsApi.md#purge_work_item) | **POST** /api/v2/workItems/{id}/purge | Permanently delete test case, checklist or shared steps from archive
+*WorkItemsApi* | [**restore_work_item**](docs/WorkItemsApi.md#restore_work_item) | **POST** /api/v2/workItems/{id}/restore | Restore test case, checklist or shared steps from archive
+*WorkItemsApi* | [**update_work_item**](docs/WorkItemsApi.md#update_work_item) | **PUT** /api/v2/workItems | Update Test Case, Checklist or Shared Step
+*WorkItemsCommentsApi* | [**api_v2_work_items_comments_comment_id_delete**](docs/WorkItemsCommentsApi.md#api_v2_work_items_comments_comment_id_delete) | **DELETE** /api/v2/workItems/comments/{commentId} | Delete WorkItem comment
+*WorkItemsCommentsApi* | [**api_v2_work_items_comments_post**](docs/WorkItemsCommentsApi.md#api_v2_work_items_comments_post) | **POST** /api/v2/workItems/comments | Create WorkItem comment
+*WorkItemsCommentsApi* | [**api_v2_work_items_comments_put**](docs/WorkItemsCommentsApi.md#api_v2_work_items_comments_put) | **PUT** /api/v2/workItems/comments | Update work item comment
+*WorkItemsCommentsApi* | [**api_v2_work_items_id_comments_get**](docs/WorkItemsCommentsApi.md#api_v2_work_items_id_comments_get) | **GET** /api/v2/workItems/{id}/comments | Get work item comments
+
+
+## Documentation For Models
+
+ - You can see the documentation [here](docs/README.md).
+
+
+# Contributing
+
+You can help to develop the project. Any contributions are **greatly appreciated**.
+
+* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testgear-tms/api-client-python/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
+* Please make sure you check your spelling and grammar.
+* Create individual PR for each suggestion.
+* Please also read through the [Code Of Conduct](https://github.com/testgear-tms/api-client-python/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
+
+
+# License
+
+Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testgear-tms/api-client-python/blob/master/LICENSE.md) for more information.
+
```

### Comparing `testgear-api-client-3.0.0/README.md` & `testgear-api-client-3.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 ### Compatibility
 
 | Test Gear | API Client |
 |-----------|------------|
 | 3.5       | 2.0        |
 | 4.0       | 3.0        |
+| 4.2       | 3.1        |
 
 ## Installation & Usage
 ### pip install
 
 ```sh
 pip install testgear-api-client
 ```
@@ -59,14 +60,15 @@
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AttachmentsApi* | [**api_v2_attachments_id_delete**](docs/AttachmentsApi.md#api_v2_attachments_id_delete) | **DELETE** /api/v2/attachments/{id} | Delete attachment file
 *AttachmentsApi* | [**api_v2_attachments_id_get**](docs/AttachmentsApi.md#api_v2_attachments_id_get) | **GET** /api/v2/attachments/{id} | Download attachment file
 *AttachmentsApi* | [**api_v2_attachments_occupied_file_storage_size_get**](docs/AttachmentsApi.md#api_v2_attachments_occupied_file_storage_size_get) | **GET** /api/v2/attachments/occupiedFileStorageSize | Get size of attachments storage in bytes
 *AttachmentsApi* | [**api_v2_attachments_post**](docs/AttachmentsApi.md#api_v2_attachments_post) | **POST** /api/v2/attachments | Upload new attachment file
 *AutoTestsApi* | [**api_v2_auto_tests_flaky_bulk_post**](docs/AutoTestsApi.md#api_v2_auto_tests_flaky_bulk_post) | **POST** /api/v2/autoTests/flaky/bulk | Set \&quot;Flaky\&quot; status for multiple autotests
+*AutoTestsApi* | [**api_v2_auto_tests_id_patch**](docs/AutoTestsApi.md#api_v2_auto_tests_id_patch) | **PATCH** /api/v2/autoTests/{id} | Patch auto test
 *AutoTestsApi* | [**api_v2_auto_tests_id_test_results_search_post**](docs/AutoTestsApi.md#api_v2_auto_tests_id_test_results_search_post) | **POST** /api/v2/autoTests/{id}/testResults/search | Get test results history for autotest
 *AutoTestsApi* | [**api_v2_auto_tests_id_work_items_changed_id_get**](docs/AutoTestsApi.md#api_v2_auto_tests_id_work_items_changed_id_get) | **GET** /api/v2/autoTests/{id}/workItems/changed/id | Get identifiers of changed linked work items
 *AutoTestsApi* | [**api_v2_auto_tests_id_work_items_changed_work_item_id_approve_post**](docs/AutoTestsApi.md#api_v2_auto_tests_id_work_items_changed_work_item_id_approve_post) | **POST** /api/v2/autoTests/{id}/workItems/changed/{workItemId}/approve | Approve changes to work items linked to autotest
 *AutoTestsApi* | [**api_v2_auto_tests_search_post**](docs/AutoTestsApi.md#api_v2_auto_tests_search_post) | **POST** /api/v2/autoTests/search | Search for autotests
 *AutoTestsApi* | [**create_auto_test**](docs/AutoTestsApi.md#create_auto_test) | **POST** /api/v2/autoTests | Create autotest
 *AutoTestsApi* | [**create_multiple**](docs/AutoTestsApi.md#create_multiple) | **POST** /api/v2/autoTests/bulk | Create multiple autotests
 *AutoTestsApi* | [**delete_auto_test**](docs/AutoTestsApi.md#delete_auto_test) | **DELETE** /api/v2/autoTests/{id} | Delete autotest
@@ -77,15 +79,17 @@
 *AutoTestsApi* | [**get_auto_test_chronology**](docs/AutoTestsApi.md#get_auto_test_chronology) | **GET** /api/v2/autoTests/{id}/chronology | Get autotest chronology
 *AutoTestsApi* | [**get_test_runs**](docs/AutoTestsApi.md#get_test_runs) | **GET** /api/v2/autoTests/{id}/testRuns | Get completed tests runs for autotests
 *AutoTestsApi* | [**get_work_item_results**](docs/AutoTestsApi.md#get_work_item_results) | **GET** /api/v2/autoTests/{id}/testResultHistory | 
 *AutoTestsApi* | [**get_work_items_linked_to_auto_test**](docs/AutoTestsApi.md#get_work_items_linked_to_auto_test) | **GET** /api/v2/autoTests/{id}/workItems | Get work items linked to autotest
 *AutoTestsApi* | [**link_auto_test_to_work_item**](docs/AutoTestsApi.md#link_auto_test_to_work_item) | **POST** /api/v2/autoTests/{id}/workItems | Link autotest with work items
 *AutoTestsApi* | [**update_auto_test**](docs/AutoTestsApi.md#update_auto_test) | **PUT** /api/v2/autoTests | Update autotest
 *AutoTestsApi* | [**update_multiple**](docs/AutoTestsApi.md#update_multiple) | **PUT** /api/v2/autoTests/bulk | Update multiple autotests
+*BackgroundJobsApi* | [**api_v2_background_jobs_get**](docs/BackgroundJobsApi.md#api_v2_background_jobs_get) | **GET** /api/v2/backgroundJobs | Get current user background jobs
 *ConfigurationsApi* | [**api_v2_configurations_create_by_parameters_post**](docs/ConfigurationsApi.md#api_v2_configurations_create_by_parameters_post) | **POST** /api/v2/configurations/createByParameters | Create Configurations by parameters
+*ConfigurationsApi* | [**api_v2_configurations_id_patch**](docs/ConfigurationsApi.md#api_v2_configurations_id_patch) | **PATCH** /api/v2/configurations/{id} | Patch configuration
 *ConfigurationsApi* | [**api_v2_configurations_search_post**](docs/ConfigurationsApi.md#api_v2_configurations_search_post) | **POST** /api/v2/configurations/search | Search for configurations
 *ConfigurationsApi* | [**create_configuration**](docs/ConfigurationsApi.md#create_configuration) | **POST** /api/v2/configurations | Create Configuration
 *ConfigurationsApi* | [**get_configuration_by_id**](docs/ConfigurationsApi.md#get_configuration_by_id) | **GET** /api/v2/configurations/{id} | Get configuration by internal or global ID
 *ConfigurationsApi* | [**update_configuration**](docs/ConfigurationsApi.md#update_configuration) | **PUT** /api/v2/configurations | Update Configuration
 *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_custom_attributes_exclude_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_custom_attributes_exclude_post) | **POST** /api/v2/customAttributes/templates/{id}/customAttributes/exclude | Exclude CustomAttributes from CustomAttributeTemplate
 *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_custom_attributes_include_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_custom_attributes_include_post) | **POST** /api/v2/customAttributes/templates/{id}/customAttributes/include | Include CustomAttributes to CustomAttributeTemplate
 *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_delete**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_delete) | **DELETE** /api/v2/customAttributes/templates/{id} | Delete CustomAttributeTemplate
@@ -106,14 +110,15 @@
 *NotificationsApi* | [**api_v2_notifications_search_post**](docs/NotificationsApi.md#api_v2_notifications_search_post) | **POST** /api/v2/notifications/search | Search Notifications for current User
 *ParametersApi* | [**api_v2_parameters_bulk_post**](docs/ParametersApi.md#api_v2_parameters_bulk_post) | **POST** /api/v2/parameters/bulk | Create multiple parameters
 *ParametersApi* | [**api_v2_parameters_bulk_put**](docs/ParametersApi.md#api_v2_parameters_bulk_put) | **PUT** /api/v2/parameters/bulk | Update multiple parameters
 *ParametersApi* | [**api_v2_parameters_groups_get**](docs/ParametersApi.md#api_v2_parameters_groups_get) | **GET** /api/v2/parameters/groups | Get parameters as group
 *ParametersApi* | [**api_v2_parameters_key_name_name_exists_get**](docs/ParametersApi.md#api_v2_parameters_key_name_name_exists_get) | **GET** /api/v2/parameters/key/name/{name}/exists | Check existence parameter key in system
 *ParametersApi* | [**api_v2_parameters_key_values_get**](docs/ParametersApi.md#api_v2_parameters_key_values_get) | **GET** /api/v2/parameters/{key}/values | Get all parameter key values
 *ParametersApi* | [**api_v2_parameters_keys_get**](docs/ParametersApi.md#api_v2_parameters_keys_get) | **GET** /api/v2/parameters/keys | Get all parameter keys
+*ParametersApi* | [**api_v2_parameters_search_post**](docs/ParametersApi.md#api_v2_parameters_search_post) | **POST** /api/v2/parameters/search | Search for parameters
 *ParametersApi* | [**create_parameter**](docs/ParametersApi.md#create_parameter) | **POST** /api/v2/parameters | Create parameter
 *ParametersApi* | [**delete_by_name**](docs/ParametersApi.md#delete_by_name) | **DELETE** /api/v2/parameters/name/{name} | Delete parameter by name
 *ParametersApi* | [**delete_by_parameter_key_id**](docs/ParametersApi.md#delete_by_parameter_key_id) | **DELETE** /api/v2/parameters/keyId/{keyId} | Delete parameters by parameter key identifier
 *ParametersApi* | [**delete_parameter**](docs/ParametersApi.md#delete_parameter) | **DELETE** /api/v2/parameters/{id} | Delete parameter
 *ParametersApi* | [**get_all_parameters**](docs/ParametersApi.md#get_all_parameters) | **GET** /api/v2/parameters | Get all parameters
 *ParametersApi* | [**get_parameter_by_id**](docs/ParametersApi.md#get_parameter_by_id) | **GET** /api/v2/parameters/{id} | Get parameter by ID
 *ParametersApi* | [**obsolete_delete_by_name**](docs/ParametersApi.md#obsolete_delete_by_name) | **POST** /api/v2/parameters/deleteByName | 
@@ -121,33 +126,44 @@
 *ProjectsApi* | [**add_globa_attributes_to_project**](docs/ProjectsApi.md#add_globa_attributes_to_project) | **POST** /api/v2/projects/{id}/globalAttributes | Add global attributes to project
 *ProjectsApi* | [**api_v2_projects_id_attributes_templates_search_post**](docs/ProjectsApi.md#api_v2_projects_id_attributes_templates_search_post) | **POST** /api/v2/projects/{id}/attributes/templates/search | Search for custom attributes templates
 *ProjectsApi* | [**api_v2_projects_id_attributes_templates_template_id_delete**](docs/ProjectsApi.md#api_v2_projects_id_attributes_templates_template_id_delete) | **DELETE** /api/v2/projects/{id}/attributes/templates/{templateId} | Delete CustomAttributeTemplate from Project
 *ProjectsApi* | [**api_v2_projects_id_attributes_templates_template_id_post**](docs/ProjectsApi.md#api_v2_projects_id_attributes_templates_template_id_post) | **POST** /api/v2/projects/{id}/attributes/templates/{templateId} | Add CustomAttributeTemplate to Project
 *ProjectsApi* | [**api_v2_projects_id_failure_classes_get**](docs/ProjectsApi.md#api_v2_projects_id_failure_classes_get) | **GET** /api/v2/projects/{id}/failureClasses | Get Project FailureClasses
 *ProjectsApi* | [**api_v2_projects_id_favorite_put**](docs/ProjectsApi.md#api_v2_projects_id_favorite_put) | **PUT** /api/v2/projects/{id}/favorite | Mark Project as favorite
 *ProjectsApi* | [**api_v2_projects_id_filters_get**](docs/ProjectsApi.md#api_v2_projects_id_filters_get) | **GET** /api/v2/projects/{id}/filters | Get Project filters
+*ProjectsApi* | [**api_v2_projects_id_patch**](docs/ProjectsApi.md#api_v2_projects_id_patch) | **PATCH** /api/v2/projects/{id} | Patch project
 *ProjectsApi* | [**api_v2_projects_id_test_plans_analytics_get**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_analytics_get) | **GET** /api/v2/projects/{id}/testPlans/analytics | Get TestPlans analytics
+*ProjectsApi* | [**api_v2_projects_id_test_plans_delete_bulk_post**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_delete_bulk_post) | **POST** /api/v2/projects/{id}/testPlans/delete/bulk | Delete multiple test plans
 *ProjectsApi* | [**api_v2_projects_id_test_plans_name_exists_get**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_name_exists_get) | **GET** /api/v2/projects/{id}/testPlans/{name}/exists | Checks if TestPlan exists with the specified name exists for the project
+*ProjectsApi* | [**api_v2_projects_id_test_plans_restore_bulk_post**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_restore_bulk_post) | **POST** /api/v2/projects/{id}/testPlans/restore/bulk | Restore multiple test plans
 *ProjectsApi* | [**api_v2_projects_id_test_plans_search_post**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_search_post) | **POST** /api/v2/projects/{id}/testPlans/search | Get Project TestPlans with analytics
 *ProjectsApi* | [**api_v2_projects_id_test_runs_active_get**](docs/ProjectsApi.md#api_v2_projects_id_test_runs_active_get) | **GET** /api/v2/projects/{id}/testRuns/active | Get active Project TestRuns
 *ProjectsApi* | [**api_v2_projects_id_test_runs_full_get**](docs/ProjectsApi.md#api_v2_projects_id_test_runs_full_get) | **GET** /api/v2/projects/{id}/testRuns/full | Get Project TestRuns full models
 *ProjectsApi* | [**api_v2_projects_id_work_items_search_id_post**](docs/ProjectsApi.md#api_v2_projects_id_work_items_search_id_post) | **POST** /api/v2/projects/{id}/workItems/search/id | Search for work items and extract IDs only
 *ProjectsApi* | [**api_v2_projects_id_work_items_search_post**](docs/ProjectsApi.md#api_v2_projects_id_work_items_search_post) | **POST** /api/v2/projects/{id}/workItems/search | Search for work items
 *ProjectsApi* | [**api_v2_projects_id_work_items_tags_get**](docs/ProjectsApi.md#api_v2_projects_id_work_items_tags_get) | **GET** /api/v2/projects/{id}/workItems/tags | Get WorkItems Tags
 *ProjectsApi* | [**api_v2_projects_name_name_exists_get**](docs/ProjectsApi.md#api_v2_projects_name_name_exists_get) | **GET** /api/v2/projects/name/{name}/exists | 
 *ProjectsApi* | [**api_v2_projects_search_post**](docs/ProjectsApi.md#api_v2_projects_search_post) | **POST** /api/v2/projects/search | Search for projects
+*ProjectsApi* | [**background_import_project**](docs/ProjectsApi.md#background_import_project) | **POST** /api/v2/projects/import/json | Import project from JSON file in background job
+*ProjectsApi* | [**background_import_to_existing_project**](docs/ProjectsApi.md#background_import_to_existing_project) | **POST** /api/v2/projects/{id}/import/json | Import project from JSON file into existing project in background job
+*ProjectsApi* | [**background_import_zip_project**](docs/ProjectsApi.md#background_import_zip_project) | **POST** /api/v2/projects/import/zip | Import project from Zip file in background job
+*ProjectsApi* | [**background_import_zip_to_existing_project**](docs/ProjectsApi.md#background_import_zip_to_existing_project) | **POST** /api/v2/projects/{id}/import/zip | Import project from Zip file into existing project in background job
 *ProjectsApi* | [**call_import**](docs/ProjectsApi.md#call_import) | **POST** /api/v2/projects/import | Import project from JSON file
 *ProjectsApi* | [**create_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#create_custom_attribute_test_plan_project_relations) | **POST** /api/v2/projects/{id}/testPlans/attributes | Add attributes to project&#39;s test plans
 *ProjectsApi* | [**create_project**](docs/ProjectsApi.md#create_project) | **POST** /api/v2/projects | Create project
 *ProjectsApi* | [**create_projects_attribute**](docs/ProjectsApi.md#create_projects_attribute) | **POST** /api/v2/projects/{id}/attributes | Create project attribute
 *ProjectsApi* | [**delete_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#delete_custom_attribute_test_plan_project_relations) | **DELETE** /api/v2/projects/{id}/testPlans/attribute/{attributeId} | Delete attribute from project&#39;s test plans
 *ProjectsApi* | [**delete_project**](docs/ProjectsApi.md#delete_project) | **DELETE** /api/v2/projects/{id} | Delete project
 *ProjectsApi* | [**delete_project_auto_tests**](docs/ProjectsApi.md#delete_project_auto_tests) | **DELETE** /api/v2/projects/{id}/autoTests | Delete project
 *ProjectsApi* | [**delete_projects_attribute**](docs/ProjectsApi.md#delete_projects_attribute) | **DELETE** /api/v2/projects/{id}/attributes/{attributeId} | Delete project attribute
 *ProjectsApi* | [**export**](docs/ProjectsApi.md#export) | **POST** /api/v2/projects/{id}/export | Export project as JSON file
+*ProjectsApi* | [**export_project_json**](docs/ProjectsApi.md#export_project_json) | **POST** /api/v2/projects/{id}/export/json | Export project as JSON file in background job
+*ProjectsApi* | [**export_project_with_test_plans_json**](docs/ProjectsApi.md#export_project_with_test_plans_json) | **POST** /api/v2/projects/{id}/export/testPlans/json | Export project as JSON file with test plans in background job
+*ProjectsApi* | [**export_project_with_test_plans_zip**](docs/ProjectsApi.md#export_project_with_test_plans_zip) | **POST** /api/v2/projects/{id}/export/testPlans/zip | Export project as Zip file with test plans in background job
+*ProjectsApi* | [**export_project_zip**](docs/ProjectsApi.md#export_project_zip) | **POST** /api/v2/projects/{id}/export/zip | Export project as Zip file in background job
 *ProjectsApi* | [**export_with_test_plans_and_configurations**](docs/ProjectsApi.md#export_with_test_plans_and_configurations) | **POST** /api/v2/projects/{id}/export-by-testPlans | Export project with test plans, test suites and test points as JSON file
 *ProjectsApi* | [**get_all_projects**](docs/ProjectsApi.md#get_all_projects) | **GET** /api/v2/projects | Get all projects
 *ProjectsApi* | [**get_attribute_by_project_id**](docs/ProjectsApi.md#get_attribute_by_project_id) | **GET** /api/v2/projects/{id}/attributes/{attributeId} | Get project attribute
 *ProjectsApi* | [**get_attributes_by_project_id**](docs/ProjectsApi.md#get_attributes_by_project_id) | **GET** /api/v2/projects/{id}/attributes | Get project attributes
 *ProjectsApi* | [**get_auto_tests_namespaces**](docs/ProjectsApi.md#get_auto_tests_namespaces) | **GET** /api/v2/projects/{id}/autoTestsNamespaces | Get namespaces of autotests in project
 *ProjectsApi* | [**get_configurations_by_project_id**](docs/ProjectsApi.md#get_configurations_by_project_id) | **GET** /api/v2/projects/{id}/configurations | Get project configurations
 *ProjectsApi* | [**get_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#get_custom_attribute_test_plan_project_relations) | **GET** /api/v2/projects/{id}/testPlans/attributes | Get project&#39;s test plan attributes
@@ -159,14 +175,15 @@
 *ProjectsApi* | [**import_to_existing_project**](docs/ProjectsApi.md#import_to_existing_project) | **POST** /api/v2/projects/{id}/import | Import project from JSON file into existing project
 *ProjectsApi* | [**restore_project**](docs/ProjectsApi.md#restore_project) | **POST** /api/v2/projects/{id}/restore | Restore project
 *ProjectsApi* | [**search_attributes_in_project**](docs/ProjectsApi.md#search_attributes_in_project) | **POST** /api/v2/projects/{id}/attributes/search | Search for attributes used in the project
 *ProjectsApi* | [**search_test_plan_attributes_in_project**](docs/ProjectsApi.md#search_test_plan_attributes_in_project) | **POST** /api/v2/projects/{id}/testPlans/attributes/search | Search for attributes used in the project test plans
 *ProjectsApi* | [**update_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#update_custom_attribute_test_plan_project_relations) | **PUT** /api/v2/projects/{id}/testPlans/attribute | Update attribute of project&#39;s test plans
 *ProjectsApi* | [**update_project**](docs/ProjectsApi.md#update_project) | **PUT** /api/v2/projects | Update project
 *ProjectsApi* | [**update_projects_attribute**](docs/ProjectsApi.md#update_projects_attribute) | **PUT** /api/v2/projects/{id}/attributes | Edit attribute of the project
+*SectionsApi* | [**api_v2_sections_id_patch**](docs/SectionsApi.md#api_v2_sections_id_patch) | **PATCH** /api/v2/sections/{id} | Patch section
 *SectionsApi* | [**create_section**](docs/SectionsApi.md#create_section) | **POST** /api/v2/sections | Create section
 *SectionsApi* | [**delete_section**](docs/SectionsApi.md#delete_section) | **DELETE** /api/v2/sections/{id} | Delete section
 *SectionsApi* | [**get_section_by_id**](docs/SectionsApi.md#get_section_by_id) | **GET** /api/v2/sections/{id} | Get section
 *SectionsApi* | [**get_work_items_by_section_id**](docs/SectionsApi.md#get_work_items_by_section_id) | **GET** /api/v2/sections/{id}/workItems | Get section work items
 *SectionsApi* | [**move**](docs/SectionsApi.md#move) | **POST** /api/v2/sections/move | Move section with all work items into another section
 *SectionsApi* | [**rename**](docs/SectionsApi.md#rename) | **POST** /api/v2/sections/rename | Rename section
 *SectionsApi* | [**update_section**](docs/SectionsApi.md#update_section) | **PUT** /api/v2/sections | Update section
@@ -177,16 +194,19 @@
 *TestPlansApi* | [**api_v2_test_plans_id_analytics_get**](docs/TestPlansApi.md#api_v2_test_plans_id_analytics_get) | **GET** /api/v2/testPlans/{id}/analytics | Get analytics by TestPlan
 *TestPlansApi* | [**api_v2_test_plans_id_autobalance_post**](docs/TestPlansApi.md#api_v2_test_plans_id_autobalance_post) | **POST** /api/v2/testPlans/{id}/autobalance | Distribute test points between the users
 *TestPlansApi* | [**api_v2_test_plans_id_configurations_get**](docs/TestPlansApi.md#api_v2_test_plans_id_configurations_get) | **GET** /api/v2/testPlans/{id}/configurations | Get TestPlan configurations
 *TestPlansApi* | [**api_v2_test_plans_id_export_test_points_xlsx_post**](docs/TestPlansApi.md#api_v2_test_plans_id_export_test_points_xlsx_post) | **POST** /api/v2/testPlans/{id}/export/testPoints/xlsx | Export TestPoints from TestPlan in xls format
 *TestPlansApi* | [**api_v2_test_plans_id_export_test_result_history_xlsx_post**](docs/TestPlansApi.md#api_v2_test_plans_id_export_test_result_history_xlsx_post) | **POST** /api/v2/testPlans/{id}/export/testResultHistory/xlsx | Export TestResults history from TestPlan in xls format
 *TestPlansApi* | [**api_v2_test_plans_id_history_get**](docs/TestPlansApi.md#api_v2_test_plans_id_history_get) | **GET** /api/v2/testPlans/{id}/history | Get TestPlan history
 *TestPlansApi* | [**api_v2_test_plans_id_links_get**](docs/TestPlansApi.md#api_v2_test_plans_id_links_get) | **GET** /api/v2/testPlans/{id}/links | Get Links of TestPlan
+*TestPlansApi* | [**api_v2_test_plans_id_patch**](docs/TestPlansApi.md#api_v2_test_plans_id_patch) | **PATCH** /api/v2/testPlans/{id} | Patch test plan
 *TestPlansApi* | [**api_v2_test_plans_id_test_points_last_results_get**](docs/TestPlansApi.md#api_v2_test_plans_id_test_points_last_results_get) | **GET** /api/v2/testPlans/{id}/testPoints/lastResults | Get TestPoints with last result from TestPlan
 *TestPlansApi* | [**api_v2_test_plans_id_test_points_reset_post**](docs/TestPlansApi.md#api_v2_test_plans_id_test_points_reset_post) | **POST** /api/v2/testPlans/{id}/testPoints/reset | Reset TestPoints status of TestPlan
+*TestPlansApi* | [**api_v2_test_plans_id_test_points_tester_delete**](docs/TestPlansApi.md#api_v2_test_plans_id_test_points_tester_delete) | **DELETE** /api/v2/testPlans/{id}/testPoints/tester | Unassign users from multiple test points
+*TestPlansApi* | [**api_v2_test_plans_id_test_points_tester_user_id_post**](docs/TestPlansApi.md#api_v2_test_plans_id_test_points_tester_user_id_post) | **POST** /api/v2/testPlans/{id}/testPoints/tester/{userId} | Assign user as a tester to multiple test points
 *TestPlansApi* | [**api_v2_test_plans_id_test_runs_get**](docs/TestPlansApi.md#api_v2_test_plans_id_test_runs_get) | **GET** /api/v2/testPlans/{id}/testRuns | Get TestRuns of TestPlan
 *TestPlansApi* | [**api_v2_test_plans_id_test_runs_search_post**](docs/TestPlansApi.md#api_v2_test_plans_id_test_runs_search_post) | **POST** /api/v2/testPlans/{id}/testRuns/search | Search TestRuns of TestPlan
 *TestPlansApi* | [**api_v2_test_plans_id_test_runs_test_results_last_modified_modified_date_get**](docs/TestPlansApi.md#api_v2_test_plans_id_test_runs_test_results_last_modified_modified_date_get) | **GET** /api/v2/testPlans/{id}/testRuns/testResults/lastModified/modifiedDate | Get last modification date of test plan&#39;s test results
 *TestPlansApi* | [**api_v2_test_plans_id_unlock_request_post**](docs/TestPlansApi.md#api_v2_test_plans_id_unlock_request_post) | **POST** /api/v2/testPlans/{id}/unlock/request | Send unlock TestPlan notification
 *TestPlansApi* | [**api_v2_test_plans_shorts_post**](docs/TestPlansApi.md#api_v2_test_plans_shorts_post) | **POST** /api/v2/testPlans/shorts | Get TestPlans short models by Project identifiers
 *TestPlansApi* | [**clone**](docs/TestPlansApi.md#clone) | **POST** /api/v2/testPlans/{id}/clone | Clone TestPlan
 *TestPlansApi* | [**complete**](docs/TestPlansApi.md#complete) | **POST** /api/v2/testPlans/{id}/complete | Complete TestPlan
@@ -226,14 +246,16 @@
 *TestRunsApi* | [**create_empty**](docs/TestRunsApi.md#create_empty) | **POST** /api/v2/testRuns | Create empty TestRun
 *TestRunsApi* | [**get_test_run_by_id**](docs/TestRunsApi.md#get_test_run_by_id) | **GET** /api/v2/testRuns/{id} | Get TestRun by Id
 *TestRunsApi* | [**set_auto_test_results_for_test_run**](docs/TestRunsApi.md#set_auto_test_results_for_test_run) | **POST** /api/v2/testRuns/{id}/testResults | Send test results to the test runs in the system
 *TestRunsApi* | [**start_test_run**](docs/TestRunsApi.md#start_test_run) | **POST** /api/v2/testRuns/{id}/start | Start TestRun
 *TestRunsApi* | [**stop_test_run**](docs/TestRunsApi.md#stop_test_run) | **POST** /api/v2/testRuns/{id}/stop | Stop TestRun
 *TestRunsApi* | [**update_empty**](docs/TestRunsApi.md#update_empty) | **PUT** /api/v2/testRuns | Update empty TestRun
 *TestSuitesApi* | [**add_test_points_to_test_suite**](docs/TestSuitesApi.md#add_test_points_to_test_suite) | **POST** /api/v2/testSuites/{id}/test-points | Add test-points to test suite
+*TestSuitesApi* | [**api_v2_test_suites_id_patch**](docs/TestSuitesApi.md#api_v2_test_suites_id_patch) | **PATCH** /api/v2/testSuites/{id} | Patch test suite
+*TestSuitesApi* | [**api_v2_test_suites_id_refresh_post**](docs/TestSuitesApi.md#api_v2_test_suites_id_refresh_post) | **POST** /api/v2/testSuites/{id}/refresh | Refresh test suite. Only dynamic test suites are supported by this method
 *TestSuitesApi* | [**create_test_suite**](docs/TestSuitesApi.md#create_test_suite) | **POST** /api/v2/testSuites | Create TestSuite
 *TestSuitesApi* | [**delete_test_suite**](docs/TestSuitesApi.md#delete_test_suite) | **DELETE** /api/v2/testSuites/{id} | Delete TestSuite
 *TestSuitesApi* | [**get_configurations_by_test_suite_id**](docs/TestSuitesApi.md#get_configurations_by_test_suite_id) | **GET** /api/v2/testSuites/{id}/configurations | Get Configurations By Id
 *TestSuitesApi* | [**get_test_points_by_id**](docs/TestSuitesApi.md#get_test_points_by_id) | **GET** /api/v2/testSuites/{id}/testPoints | Get TestPoints By Id
 *TestSuitesApi* | [**get_test_results_by_id**](docs/TestSuitesApi.md#get_test_results_by_id) | **GET** /api/v2/testSuites/{id}/testResults | Get TestResults By Id
 *TestSuitesApi* | [**get_test_suite_by_id**](docs/TestSuitesApi.md#get_test_suite_by_id) | **GET** /api/v2/testSuites/{id} | Get TestSuite by Id
 *TestSuitesApi* | [**get_work_items_by_id**](docs/TestSuitesApi.md#get_work_items_by_id) | **GET** /api/v2/testSuites/{id}/workItems | 
@@ -247,14 +269,15 @@
 *WebhooksApi* | [**api_v2_webhooks_id_put**](docs/WebhooksApi.md#api_v2_webhooks_id_put) | **PUT** /api/v2/webhooks/{id} | Edit webhook by ID
 *WebhooksApi* | [**api_v2_webhooks_post**](docs/WebhooksApi.md#api_v2_webhooks_post) | **POST** /api/v2/webhooks | Create webhook
 *WebhooksApi* | [**api_v2_webhooks_search_post**](docs/WebhooksApi.md#api_v2_webhooks_search_post) | **POST** /api/v2/webhooks/search | Search for webhooks
 *WebhooksApi* | [**api_v2_webhooks_special_variables_get**](docs/WebhooksApi.md#api_v2_webhooks_special_variables_get) | **GET** /api/v2/webhooks/specialVariables | Get special variables for webhook event type
 *WebhooksLogsApi* | [**api_v2_webhooks_logs_get**](docs/WebhooksLogsApi.md#api_v2_webhooks_logs_get) | **GET** /api/v2/webhooks/logs | Get all webhook logs
 *WebhooksLogsApi* | [**api_v2_webhooks_logs_id_delete**](docs/WebhooksLogsApi.md#api_v2_webhooks_logs_id_delete) | **DELETE** /api/v2/webhooks/logs/{id} | Delete webhook log by ID
 *WebhooksLogsApi* | [**api_v2_webhooks_logs_id_get**](docs/WebhooksLogsApi.md#api_v2_webhooks_logs_id_get) | **GET** /api/v2/webhooks/logs/{id} | Get webhook log by ID
+*WorkItemsApi* | [**api_v2_work_items_id_attachments_post**](docs/WorkItemsApi.md#api_v2_work_items_id_attachments_post) | **POST** /api/v2/workItems/{id}/attachments | Upload and link attachment to WorkItem
 *WorkItemsApi* | [**api_v2_work_items_id_check_list_transform_to_test_case_post**](docs/WorkItemsApi.md#api_v2_work_items_id_check_list_transform_to_test_case_post) | **POST** /api/v2/workItems/{id}/checkList/transformTo/testCase | Transform CheckList to TestCase
 *WorkItemsApi* | [**api_v2_work_items_id_history_get**](docs/WorkItemsApi.md#api_v2_work_items_id_history_get) | **GET** /api/v2/workItems/{id}/history | Get change history of WorkItem
 *WorkItemsApi* | [**api_v2_work_items_id_like_delete**](docs/WorkItemsApi.md#api_v2_work_items_id_like_delete) | **DELETE** /api/v2/workItems/{id}/like | Delete like from WorkItem
 *WorkItemsApi* | [**api_v2_work_items_id_like_post**](docs/WorkItemsApi.md#api_v2_work_items_id_like_post) | **POST** /api/v2/workItems/{id}/like | Set like to WorkItem
 *WorkItemsApi* | [**api_v2_work_items_id_likes_count_get**](docs/WorkItemsApi.md#api_v2_work_items_id_likes_count_get) | **GET** /api/v2/workItems/{id}/likes/count | Get likes count of WorkItem
 *WorkItemsApi* | [**api_v2_work_items_id_likes_get**](docs/WorkItemsApi.md#api_v2_work_items_id_likes_get) | **GET** /api/v2/workItems/{id}/likes | Get likes of WorkItem
 *WorkItemsApi* | [**api_v2_work_items_id_test_results_history_get**](docs/WorkItemsApi.md#api_v2_work_items_id_test_results_history_get) | **GET** /api/v2/workItems/{id}/testResults/history | Get test results history of WorkItem
@@ -268,14 +291,16 @@
 *WorkItemsApi* | [**delete_all_work_items_from_auto_test**](docs/WorkItemsApi.md#delete_all_work_items_from_auto_test) | **DELETE** /api/v2/workItems/{id}/autoTests | Delete all links AutoTests from WorkItem by Id or GlobalId
 *WorkItemsApi* | [**delete_work_item**](docs/WorkItemsApi.md#delete_work_item) | **DELETE** /api/v2/workItems/{id} | Delete Test Case, Checklist or Shared Step by Id or GlobalId
 *WorkItemsApi* | [**get_auto_tests_for_work_item**](docs/WorkItemsApi.md#get_auto_tests_for_work_item) | **GET** /api/v2/workItems/{id}/autoTests | Get all AutoTests linked to WorkItem by Id or GlobalId
 *WorkItemsApi* | [**get_iterations**](docs/WorkItemsApi.md#get_iterations) | **GET** /api/v2/workItems/{id}/iterations | Get iterations by workitem Id or GlobalId
 *WorkItemsApi* | [**get_work_item_by_id**](docs/WorkItemsApi.md#get_work_item_by_id) | **GET** /api/v2/workItems/{id} | Get Test Case, Checklist or Shared Step by Id or GlobalId
 *WorkItemsApi* | [**get_work_item_chronology**](docs/WorkItemsApi.md#get_work_item_chronology) | **GET** /api/v2/workItems/{id}/chronology | Get WorkItem chronology by Id or GlobalId
 *WorkItemsApi* | [**get_work_item_versions**](docs/WorkItemsApi.md#get_work_item_versions) | **GET** /api/v2/workItems/{id}/versions | Get WorkItem versions
+*WorkItemsApi* | [**purge_work_item**](docs/WorkItemsApi.md#purge_work_item) | **POST** /api/v2/workItems/{id}/purge | Permanently delete test case, checklist or shared steps from archive
+*WorkItemsApi* | [**restore_work_item**](docs/WorkItemsApi.md#restore_work_item) | **POST** /api/v2/workItems/{id}/restore | Restore test case, checklist or shared steps from archive
 *WorkItemsApi* | [**update_work_item**](docs/WorkItemsApi.md#update_work_item) | **PUT** /api/v2/workItems | Update Test Case, Checklist or Shared Step
 *WorkItemsCommentsApi* | [**api_v2_work_items_comments_comment_id_delete**](docs/WorkItemsCommentsApi.md#api_v2_work_items_comments_comment_id_delete) | **DELETE** /api/v2/workItems/comments/{commentId} | Delete WorkItem comment
 *WorkItemsCommentsApi* | [**api_v2_work_items_comments_post**](docs/WorkItemsCommentsApi.md#api_v2_work_items_comments_post) | **POST** /api/v2/workItems/comments | Create WorkItem comment
 *WorkItemsCommentsApi* | [**api_v2_work_items_comments_put**](docs/WorkItemsCommentsApi.md#api_v2_work_items_comments_put) | **PUT** /api/v2/workItems/comments | Update work item comment
 *WorkItemsCommentsApi* | [**api_v2_work_items_id_comments_get**](docs/WorkItemsCommentsApi.md#api_v2_work_items_id_comments_get) | **GET** /api/v2/workItems/{id}/comments | Get work item comments
```

### Comparing `testgear-api-client-3.0.0/setup.py` & `testgear-api-client-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "testgear-api-client"
-VERSION = "3.0.0"
+VERSION = "3.1.0"
 REQUIRES = [
   "urllib3 >= 1.25.3",
   "python-dateutil",
 ]
 
 setup(
     name=NAME,
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/__init__.py` & `testgear-api-client-3.1.0/src/testgear_api_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: v2.0
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "3.0.0"
+__version__ = "3.1.0"
 
 # import ApiClient
 from testgear_api_client.api_client import ApiClient
 
 # import Configuration
 from testgear_api_client.configuration import Configuration
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/attachments_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/attachments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
 
     def api_v2_attachments_post(
         self,
         **kwargs
     ):
         """Upload new attachment file  # noqa: E501
 
-        File size is restricted to 1 GB (1 073 741 824 bytes)  # noqa: E501
+        File size is restricted to 50 MB (52 428 800 bytes)  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_v2_attachments_post(async_req=True)
         >>> result = thread.get()
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/auto_tests_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/auto_tests_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from testgear_api_client.model.auto_test_model import AutoTestModel
 from testgear_api_client.model.auto_test_post_model import AutoTestPostModel
 from testgear_api_client.model.auto_test_put_model import AutoTestPutModel
 from testgear_api_client.model.autotest_historical_result_select_model import AutotestHistoricalResultSelectModel
 from testgear_api_client.model.autotest_result_historical_get_model import AutotestResultHistoricalGetModel
 from testgear_api_client.model.autotests_select_model import AutotestsSelectModel
 from testgear_api_client.model.flaky_bulk_model import FlakyBulkModel
+from testgear_api_client.model.operation import Operation
 from testgear_api_client.model.problem_details import ProblemDetails
 from testgear_api_client.model.test_result_chronology_model import TestResultChronologyModel
 from testgear_api_client.model.test_result_history_report_model import TestResultHistoryReportModel
 from testgear_api_client.model.test_run_short_model import TestRunShortModel
 from testgear_api_client.model.validation_problem_details import ValidationProblemDetails
 from testgear_api_client.model.work_item_id_model import WorkItemIdModel
 from testgear_api_client.model.work_item_identifier_model import WorkItemIdentifierModel
@@ -120,14 +121,71 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.api_v2_auto_tests_id_patch_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/autoTests/{id}',
+                'operation_id': 'api_v2_auto_tests_id_patch',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'operation',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'operation':
+                        ([Operation],),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'operation': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.api_v2_auto_tests_id_test_results_search_post_endpoint = _Endpoint(
             settings={
                 'response_type': ([AutotestResultHistoricalGetModel],),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
                 'endpoint_path': '/api/v2/autoTests/{id}/testResults/search',
@@ -1395,14 +1453,98 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.api_v2_auto_tests_flaky_bulk_post_endpoint.call_with_http_info(**kwargs)
 
+    def api_v2_auto_tests_id_patch(
+        self,
+        id,
+        **kwargs
+    ):
+        """Patch auto test  # noqa: E501
+
+        See <a href=\"https://www.rfc-editor.org/rfc/rfc6902\" target=\"_blank\">RFC 6902: JavaScript Object Notation (JSON) Patch</a> for details  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_auto_tests_id_patch(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Global Id of auto test
+
+        Keyword Args:
+            operation ([Operation]): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.api_v2_auto_tests_id_patch_endpoint.call_with_http_info(**kwargs)
+
     def api_v2_auto_tests_id_test_results_search_post(
         self,
         id,
         **kwargs
     ):
         """Get test results history for autotest  # noqa: E501
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/configurations_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/configurations_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     validate_and_convert_types
 )
 from testgear_api_client.model.configuration_by_parameters_model import ConfigurationByParametersModel
 from testgear_api_client.model.configuration_model import ConfigurationModel
 from testgear_api_client.model.configuration_post_model import ConfigurationPostModel
 from testgear_api_client.model.configuration_put_model import ConfigurationPutModel
 from testgear_api_client.model.configuration_select_model import ConfigurationSelectModel
+from testgear_api_client.model.operation import Operation
 from testgear_api_client.model.problem_details import ProblemDetails
 from testgear_api_client.model.validation_problem_details import ValidationProblemDetails
 
 
 class ConfigurationsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
@@ -87,14 +88,71 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.api_v2_configurations_id_patch_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/configurations/{id}',
+                'operation_id': 'api_v2_configurations_id_patch',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'operation',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'operation':
+                        ([Operation],),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'operation': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.api_v2_configurations_search_post_endpoint = _Endpoint(
             settings={
                 'response_type': ([ConfigurationModel],),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
                 'endpoint_path': '/api/v2/configurations/search',
@@ -393,14 +451,98 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.api_v2_configurations_create_by_parameters_post_endpoint.call_with_http_info(**kwargs)
 
+    def api_v2_configurations_id_patch(
+        self,
+        id,
+        **kwargs
+    ):
+        """Patch configuration  # noqa: E501
+
+        See <a href=\"https://www.rfc-editor.org/rfc/rfc6902\" target=\"_blank\">RFC 6902: JavaScript Object Notation (JSON) Patch</a> for details  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_configurations_id_patch(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Unique ID of the configuration
+
+        Keyword Args:
+            operation ([Operation]): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.api_v2_configurations_id_patch_endpoint.call_with_http_info(**kwargs)
+
     def api_v2_configurations_search_post(
         self,
         **kwargs
     ):
         """Search for configurations  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -570,15 +712,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_configuration_by_id(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str):
+            id (str): Configuration internal (guid format) or global (integer format) identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/custom_attribute_templates_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/custom_attribute_templates_api.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/custom_attributes_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/custom_attributes_api.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/notifications_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/notifications_api.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/parameters_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/parameters_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
+from testgear_api_client.model.parameter_filter_model import ParameterFilterModel
 from testgear_api_client.model.parameter_group_model import ParameterGroupModel
 from testgear_api_client.model.parameter_model import ParameterModel
 from testgear_api_client.model.parameter_post_model import ParameterPostModel
 from testgear_api_client.model.parameter_put_model import ParameterPutModel
 from testgear_api_client.model.problem_details import ProblemDetails
 from testgear_api_client.model.validation_problem_details import ValidationProblemDetails
 
@@ -366,14 +367,89 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.api_v2_parameters_search_post_endpoint = _Endpoint(
+            settings={
+                'response_type': ([ParameterModel],),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/parameters/search',
+                'operation_id': 'api_v2_parameters_search_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'skip',
+                    'take',
+                    'order_by',
+                    'search_field',
+                    'search_value',
+                    'parameter_filter_model',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'skip':
+                        (int,),
+                    'take':
+                        (int,),
+                    'order_by':
+                        (str,),
+                    'search_field':
+                        (str,),
+                    'search_value':
+                        (str,),
+                    'parameter_filter_model':
+                        (ParameterFilterModel,),
+                },
+                'attribute_map': {
+                    'skip': 'Skip',
+                    'take': 'Take',
+                    'order_by': 'OrderBy',
+                    'search_field': 'SearchField',
+                    'search_value': 'SearchValue',
+                },
+                'location_map': {
+                    'skip': 'query',
+                    'take': 'query',
+                    'order_by': 'query',
+                    'search_field': 'query',
+                    'search_value': 'query',
+                    'parameter_filter_model': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.create_parameter_endpoint = _Endpoint(
             settings={
                 'response_type': (ParameterModel,),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
                 'endpoint_path': '/api/v2/parameters',
@@ -1284,14 +1360,97 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.api_v2_parameters_keys_get_endpoint.call_with_http_info(**kwargs)
 
+    def api_v2_parameters_search_post(
+        self,
+        **kwargs
+    ):
+        """Search for parameters  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_parameters_search_post(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            skip (int): Amount of items to be skipped (offset). [optional]
+            take (int): Amount of items to be taken (limit). [optional]
+            order_by (str): SQL-like  ORDER BY statement (column1 ASC|DESC , column2 ASC|DESC). [optional]
+            search_field (str): Property name for searching. [optional]
+            search_value (str): Value for searching. [optional]
+            parameter_filter_model (ParameterFilterModel): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [ParameterModel]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.api_v2_parameters_search_post_endpoint.call_with_http_info(**kwargs)
+
     def create_parameter(
         self,
         **kwargs
     ):
         """Create parameter  # noqa: E501
 
         <br>Use case  <br>User sets parameter model (listed in the request example)  <br>User runs method execution  <br>System creates parameter  <br>System returns parameter model  # noqa: E501
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/projects_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/projects_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,31 +24,33 @@
 from testgear_api_client.model.auto_test_namespace_model import AutoTestNamespaceModel
 from testgear_api_client.model.configuration_model import ConfigurationModel
 from testgear_api_client.model.custom_attribute_get_model import CustomAttributeGetModel
 from testgear_api_client.model.custom_attribute_model import CustomAttributeModel
 from testgear_api_client.model.custom_attribute_post_model import CustomAttributePostModel
 from testgear_api_client.model.custom_attribute_put_model import CustomAttributePutModel
 from testgear_api_client.model.custom_attribute_test_plan_project_relation_put_model import CustomAttributeTestPlanProjectRelationPutModel
+from testgear_api_client.model.deletion_state import DeletionState
 from testgear_api_client.model.failure_class_model import FailureClassModel
 from testgear_api_client.model.filter_model import FilterModel
+from testgear_api_client.model.operation import Operation
 from testgear_api_client.model.problem_details import ProblemDetails
 from testgear_api_client.model.project_attributes_filter_model import ProjectAttributesFilterModel
 from testgear_api_client.model.project_custom_attribute_template_get_model import ProjectCustomAttributeTemplateGetModel
 from testgear_api_client.model.project_custom_attributes_templates_filter_model import ProjectCustomAttributesTemplatesFilterModel
 from testgear_api_client.model.project_export_query_model import ProjectExportQueryModel
 from testgear_api_client.model.project_export_with_test_plans_post_model import ProjectExportWithTestPlansPostModel
 from testgear_api_client.model.project_model import ProjectModel
 from testgear_api_client.model.project_post_model import ProjectPostModel
 from testgear_api_client.model.project_put_model import ProjectPutModel
+from testgear_api_client.model.project_test_plans_filter_model import ProjectTestPlansFilterModel
 from testgear_api_client.model.projects_filter_model import ProjectsFilterModel
 from testgear_api_client.model.public_test_run_model import PublicTestRunModel
 from testgear_api_client.model.section_model import SectionModel
 from testgear_api_client.model.tag_short_model import TagShortModel
 from testgear_api_client.model.test_plan_model import TestPlanModel
-from testgear_api_client.model.test_plan_search_query_model import TestPlanSearchQueryModel
 from testgear_api_client.model.test_plan_with_analytic_model import TestPlanWithAnalyticModel
 from testgear_api_client.model.test_run_model import TestRunModel
 from testgear_api_client.model.test_run_v2_get_model import TestRunV2GetModel
 from testgear_api_client.model.validation_problem_details import ValidationProblemDetails
 from testgear_api_client.model.work_item_select_model import WorkItemSelectModel
 from testgear_api_client.model.work_item_short_model import WorkItemShortModel
 
@@ -475,14 +477,71 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.api_v2_projects_id_patch_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/projects/{id}',
+                'operation_id': 'api_v2_projects_id_patch',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'operation',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'operation':
+                        ([Operation],),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'operation': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.api_v2_projects_id_test_plans_analytics_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([TestPlanWithAnalyticModel],),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
                 'endpoint_path': '/api/v2/projects/{id}/testPlans/analytics',
@@ -561,14 +620,71 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.api_v2_projects_id_test_plans_delete_bulk_post_endpoint = _Endpoint(
+            settings={
+                'response_type': ([str],),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/projects/{id}/testPlans/delete/bulk',
+                'operation_id': 'api_v2_projects_id_test_plans_delete_bulk_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'project_test_plans_filter_model',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'project_test_plans_filter_model':
+                        (ProjectTestPlansFilterModel,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'project_test_plans_filter_model': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.api_v2_projects_id_test_plans_name_exists_get_endpoint = _Endpoint(
             settings={
                 'response_type': (bool,),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
                 'endpoint_path': '/api/v2/projects/{id}/testPlans/{name}/exists',
@@ -618,14 +734,71 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.api_v2_projects_id_test_plans_restore_bulk_post_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/projects/{id}/testPlans/restore/bulk',
+                'operation_id': 'api_v2_projects_id_test_plans_restore_bulk_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'project_test_plans_filter_model',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'project_test_plans_filter_model':
+                        (ProjectTestPlansFilterModel,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'project_test_plans_filter_model': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.api_v2_projects_id_test_plans_search_post_endpoint = _Endpoint(
             settings={
                 'response_type': ([TestPlanWithAnalyticModel],),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
                 'endpoint_path': '/api/v2/projects/{id}/testPlans/search',
@@ -638,15 +811,15 @@
                     'id',
                     'must_update_cache',
                     'skip',
                     'take',
                     'order_by',
                     'search_field',
                     'search_value',
-                    'test_plan_search_query_model',
+                    'project_test_plans_filter_model',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -670,16 +843,16 @@
                         (int,),
                     'order_by':
                         (str,),
                     'search_field':
                         (str,),
                     'search_value':
                         (str,),
-                    'test_plan_search_query_model':
-                        (TestPlanSearchQueryModel,),
+                    'project_test_plans_filter_model':
+                        (ProjectTestPlansFilterModel,),
                 },
                 'attribute_map': {
                     'id': 'id',
                     'must_update_cache': 'mustUpdateCache',
                     'skip': 'Skip',
                     'take': 'Take',
                     'order_by': 'OrderBy',
@@ -690,15 +863,15 @@
                     'id': 'path',
                     'must_update_cache': 'query',
                     'skip': 'query',
                     'take': 'query',
                     'order_by': 'query',
                     'search_field': 'query',
                     'search_value': 'query',
-                    'test_plan_search_query_model': 'body',
+                    'project_test_plans_filter_model': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -1223,14 +1396,234 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.background_import_project_endpoint = _Endpoint(
+            settings={
+                'response_type': (str,),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/projects/import/json',
+                'operation_id': 'background_import_project',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'file',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'file':
+                        (file_type,),
+                },
+                'attribute_map': {
+                    'file': 'file',
+                },
+                'location_map': {
+                    'file': 'form',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'multipart/form-data',
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.background_import_to_existing_project_endpoint = _Endpoint(
+            settings={
+                'response_type': (str,),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/projects/{id}/import/json',
+                'operation_id': 'background_import_to_existing_project',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'file',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'file':
+                        (file_type,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                    'file': 'file',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'file': 'form',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'multipart/form-data'
+                ]
+            },
+            api_client=api_client
+        )
+        self.background_import_zip_project_endpoint = _Endpoint(
+            settings={
+                'response_type': (str,),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/projects/import/zip',
+                'operation_id': 'background_import_zip_project',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'file',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'file':
+                        (file_type,),
+                },
+                'attribute_map': {
+                    'file': 'file',
+                },
+                'location_map': {
+                    'file': 'form',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'multipart/form-data',
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.background_import_zip_to_existing_project_endpoint = _Endpoint(
+            settings={
+                'response_type': (str,),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/projects/{id}/import/zip',
+                'operation_id': 'background_import_zip_to_existing_project',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'file',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'file':
+                        (file_type,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                    'file': 'file',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'file': 'form',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'multipart/form-data'
+                ]
+            },
+            api_client=api_client
+        )
         self.call_import_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
                 'endpoint_path': '/api/v2/projects/import',
@@ -1725,14 +2118,262 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.export_project_json_endpoint = _Endpoint(
+            settings={
+                'response_type': (str,),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/projects/{id}/export/json',
+                'operation_id': 'export_project_json',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'time_zone_offset_in_minutes',
+                    'project_export_query_model',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'time_zone_offset_in_minutes':
+                        (int,),
+                    'project_export_query_model':
+                        (ProjectExportQueryModel,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                    'time_zone_offset_in_minutes': 'time-Zone-Offset-In-Minutes',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'time_zone_offset_in_minutes': 'header',
+                    'project_export_query_model': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.export_project_with_test_plans_json_endpoint = _Endpoint(
+            settings={
+                'response_type': (str,),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/projects/{id}/export/testPlans/json',
+                'operation_id': 'export_project_with_test_plans_json',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'time_zone_offset_in_minutes',
+                    'project_export_with_test_plans_post_model',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'time_zone_offset_in_minutes':
+                        (int,),
+                    'project_export_with_test_plans_post_model':
+                        (ProjectExportWithTestPlansPostModel,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                    'time_zone_offset_in_minutes': 'time-Zone-Offset-In-Minutes',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'time_zone_offset_in_minutes': 'header',
+                    'project_export_with_test_plans_post_model': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.export_project_with_test_plans_zip_endpoint = _Endpoint(
+            settings={
+                'response_type': (str,),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/projects/{id}/export/testPlans/zip',
+                'operation_id': 'export_project_with_test_plans_zip',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'time_zone_offset_in_minutes',
+                    'project_export_with_test_plans_post_model',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'time_zone_offset_in_minutes':
+                        (int,),
+                    'project_export_with_test_plans_post_model':
+                        (ProjectExportWithTestPlansPostModel,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                    'time_zone_offset_in_minutes': 'time-Zone-Offset-In-Minutes',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'time_zone_offset_in_minutes': 'header',
+                    'project_export_with_test_plans_post_model': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.export_project_zip_endpoint = _Endpoint(
+            settings={
+                'response_type': (str,),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/projects/{id}/export/zip',
+                'operation_id': 'export_project_zip',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'time_zone_offset_in_minutes',
+                    'project_export_query_model',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'time_zone_offset_in_minutes':
+                        (int,),
+                    'project_export_query_model':
+                        (ProjectExportQueryModel,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                    'time_zone_offset_in_minutes': 'time-Zone-Offset-In-Minutes',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'time_zone_offset_in_minutes': 'header',
+                    'project_export_query_model': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.export_with_test_plans_and_configurations_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
                 'endpoint_path': '/api/v2/projects/{id}/export-by-testPlans',
@@ -1958,15 +2599,15 @@
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (str,),
                     'is_deleted':
-                        (bool,),
+                        (DeletionState,),
                 },
                 'attribute_map': {
                     'id': 'id',
                     'is_deleted': 'isDeleted',
                 },
                 'location_map': {
                     'id': 'path',
@@ -3556,14 +4197,98 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.api_v2_projects_id_filters_get_endpoint.call_with_http_info(**kwargs)
 
+    def api_v2_projects_id_patch(
+        self,
+        id,
+        **kwargs
+    ):
+        """Patch project  # noqa: E501
+
+        See <a href=\"https://www.rfc-editor.org/rfc/rfc6902\" target=\"_blank\">RFC 6902: JavaScript Object Notation (JSON) Patch</a> for details  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_projects_id_patch(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Unique or global Id of project
+
+        Keyword Args:
+            operation ([Operation]): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.api_v2_projects_id_patch_endpoint.call_with_http_info(**kwargs)
+
     def api_v2_projects_id_test_plans_analytics_get(
         self,
         id,
         **kwargs
     ):
         """Get TestPlans analytics  # noqa: E501
 
@@ -3646,14 +4371,97 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.api_v2_projects_id_test_plans_analytics_get_endpoint.call_with_http_info(**kwargs)
 
+    def api_v2_projects_id_test_plans_delete_bulk_post(
+        self,
+        id,
+        **kwargs
+    ):
+        """Delete multiple test plans  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_projects_id_test_plans_delete_bulk_post(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Unique or global ID of the project
+
+        Keyword Args:
+            project_test_plans_filter_model (ProjectTestPlansFilterModel): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [str]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.api_v2_projects_id_test_plans_delete_bulk_post_endpoint.call_with_http_info(**kwargs)
+
     def api_v2_projects_id_test_plans_name_exists_get(
         self,
         id,
         name,
         **kwargs
     ):
         """Checks if TestPlan exists with the specified name exists for the project  # noqa: E501
@@ -3733,14 +4541,97 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         kwargs['name'] = \
             name
         return self.api_v2_projects_id_test_plans_name_exists_get_endpoint.call_with_http_info(**kwargs)
 
+    def api_v2_projects_id_test_plans_restore_bulk_post(
+        self,
+        id,
+        **kwargs
+    ):
+        """Restore multiple test plans  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_projects_id_test_plans_restore_bulk_post(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Unique or global ID of the project
+
+        Keyword Args:
+            project_test_plans_filter_model (ProjectTestPlansFilterModel): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.api_v2_projects_id_test_plans_restore_bulk_post_endpoint.call_with_http_info(**kwargs)
+
     def api_v2_projects_id_test_plans_search_post(
         self,
         id,
         **kwargs
     ):
         """Get Project TestPlans with analytics  # noqa: E501
 
@@ -3757,15 +4648,15 @@
         Keyword Args:
             must_update_cache (bool): [optional] if omitted the server will use the default value of False
             skip (int): Amount of items to be skipped (offset). [optional]
             take (int): Amount of items to be taken (limit). [optional]
             order_by (str): SQL-like  ORDER BY statement (column1 ASC|DESC , column2 ASC|DESC). [optional]
             search_field (str): Property name for searching. [optional]
             search_value (str): Value for searching. [optional]
-            test_plan_search_query_model (TestPlanSearchQueryModel): [optional]
+            project_test_plans_filter_model (ProjectTestPlansFilterModel): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -4428,14 +5319,336 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.api_v2_projects_search_post_endpoint.call_with_http_info(**kwargs)
 
+    def background_import_project(
+        self,
+        **kwargs
+    ):
+        """Import project from JSON file in background job  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.background_import_project(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            file (file_type): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            str
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.background_import_project_endpoint.call_with_http_info(**kwargs)
+
+    def background_import_to_existing_project(
+        self,
+        id,
+        **kwargs
+    ):
+        """Import project from JSON file into existing project in background job  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.background_import_to_existing_project(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Project internal (UUID) or global (integer) identifier
+
+        Keyword Args:
+            file (file_type): Select file. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            str
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.background_import_to_existing_project_endpoint.call_with_http_info(**kwargs)
+
+    def background_import_zip_project(
+        self,
+        **kwargs
+    ):
+        """Import project from Zip file in background job  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.background_import_zip_project(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            file (file_type): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            str
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.background_import_zip_project_endpoint.call_with_http_info(**kwargs)
+
+    def background_import_zip_to_existing_project(
+        self,
+        id,
+        **kwargs
+    ):
+        """Import project from Zip file into existing project in background job  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.background_import_zip_to_existing_project(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Project internal (UUID) or global (integer) identifier
+
+        Keyword Args:
+            file (file_type): Select file. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            str
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.background_import_zip_to_existing_project_endpoint.call_with_http_info(**kwargs)
+
     def call_import(
         self,
         **kwargs
     ):
         """Import project from JSON file  # noqa: E501
 
         <br>    <b>A project can only be exported to another TMS instance, different from the one it was imported from.</b>    <br>This method imports a `.json` file with a project to the test management system.  <br>In the body of the request, send the `.json` file received by the `POST /api/v2/projects/export` method:  <br>    ```              curl -X POST \"http://{domain.com}/api/v2/projects/import\" \\              -H \"accept: /\" -H \"Authorization: PrivateToken {token}\" -H \"Content-Type: multipart/form-data\" \\              -F \"file=@import.txt;type=text/plain\"              ```    <br>              In the second instance, a project with the name of the imported one is created.              User attributes and the test library (along with content and structure) are imported.                <br>Test plan execution history from the first instance of TMS cannot be transferred.  # noqa: E501
@@ -5180,14 +6393,350 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.export_endpoint.call_with_http_info(**kwargs)
 
+    def export_project_json(
+        self,
+        id,
+        **kwargs
+    ):
+        """Export project as JSON file in background job  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.export_project_json(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Project internal (UUID) or global (integer) identifier
+
+        Keyword Args:
+            time_zone_offset_in_minutes (int): [optional]
+            project_export_query_model (ProjectExportQueryModel): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            str
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.export_project_json_endpoint.call_with_http_info(**kwargs)
+
+    def export_project_with_test_plans_json(
+        self,
+        id,
+        **kwargs
+    ):
+        """Export project as JSON file with test plans in background job  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.export_project_with_test_plans_json(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Project internal (UUID) or global (integer) identifier
+
+        Keyword Args:
+            time_zone_offset_in_minutes (int): [optional]
+            project_export_with_test_plans_post_model (ProjectExportWithTestPlansPostModel): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            str
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.export_project_with_test_plans_json_endpoint.call_with_http_info(**kwargs)
+
+    def export_project_with_test_plans_zip(
+        self,
+        id,
+        **kwargs
+    ):
+        """Export project as Zip file with test plans in background job  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.export_project_with_test_plans_zip(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Project internal (UUID) or global (integer) identifier
+
+        Keyword Args:
+            time_zone_offset_in_minutes (int): [optional]
+            project_export_with_test_plans_post_model (ProjectExportWithTestPlansPostModel): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            str
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.export_project_with_test_plans_zip_endpoint.call_with_http_info(**kwargs)
+
+    def export_project_zip(
+        self,
+        id,
+        **kwargs
+    ):
+        """Export project as Zip file in background job  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.export_project_zip(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Project internal (UUID) or global (integer) identifier
+
+        Keyword Args:
+            time_zone_offset_in_minutes (int): [optional]
+            project_export_query_model (ProjectExportQueryModel): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            str
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.export_project_zip_endpoint.call_with_http_info(**kwargs)
+
     def export_with_test_plans_and_configurations(
         self,
         id,
         **kwargs
     ):
         """Export project with test plans, test suites and test points as JSON file  # noqa: E501
 
@@ -5455,15 +7004,15 @@
         >>> thread = api.get_attributes_by_project_id(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): Project internal (UUID) or global (integer) identifier
 
         Keyword Args:
-            is_deleted (bool): If result must consist of only actual/deleted work items. [optional] if omitted the server will use the default value of False
+            is_deleted (DeletionState): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/sections_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/sections_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
+from testgear_api_client.model.deletion_state import DeletionState
+from testgear_api_client.model.operation import Operation
 from testgear_api_client.model.problem_details import ProblemDetails
 from testgear_api_client.model.section_move_model import SectionMoveModel
 from testgear_api_client.model.section_post_model import SectionPostModel
 from testgear_api_client.model.section_put_model import SectionPutModel
 from testgear_api_client.model.section_rename_model import SectionRenameModel
 from testgear_api_client.model.section_with_steps_model import SectionWithStepsModel
 from testgear_api_client.model.validation_problem_details import ValidationProblemDetails
@@ -38,14 +40,71 @@
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
+        self.api_v2_sections_id_patch_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/sections/{id}',
+                'operation_id': 'api_v2_sections_id_patch',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'operation',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'operation':
+                        ([Operation],),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'operation': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.create_section_endpoint = _Endpoint(
             settings={
                 'response_type': (SectionWithStepsModel,),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
                 'endpoint_path': '/api/v2/sections',
@@ -174,15 +233,15 @@
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (str,),
                     'is_deleted':
-                        (bool,),
+                        (DeletionState,),
                 },
                 'attribute_map': {
                     'id': 'id',
                     'is_deleted': 'isDeleted',
                 },
                 'location_map': {
                     'id': 'path',
@@ -438,14 +497,98 @@
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
 
+    def api_v2_sections_id_patch(
+        self,
+        id,
+        **kwargs
+    ):
+        """Patch section  # noqa: E501
+
+        See <a href=\"https://www.rfc-editor.org/rfc/rfc6902\" target=\"_blank\">RFC 6902: JavaScript Object Notation (JSON) Patch</a> for details  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_sections_id_patch(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Section internal (UUID) identifier
+
+        Keyword Args:
+            operation ([Operation]): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.api_v2_sections_id_patch_endpoint.call_with_http_info(**kwargs)
+
     def create_section(
         self,
         **kwargs
     ):
         """Create section  # noqa: E501
 
         <br>Use case  <br>User sets section properties (listed in request example)  <br>User runs method execution  <br>System creates section property values  <br>System returns section (listed in response example)  # noqa: E501
@@ -618,15 +761,15 @@
         >>> thread = api.get_section_by_id(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): Section internal (UUID) identifier
 
         Keyword Args:
-            is_deleted (bool): Requested section is deleted. [optional] if omitted the server will use the default value of False
+            is_deleted (DeletionState): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/tags_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/test_plans_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/test_plans_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,25 @@
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from testgear_api_client.model.configuration_model import ConfigurationModel
 from testgear_api_client.model.get_xlsx_test_points_by_test_plan_model import GetXlsxTestPointsByTestPlanModel
+from testgear_api_client.model.operation import Operation
 from testgear_api_client.model.problem_details import ProblemDetails
 from testgear_api_client.model.test_plan_change_model import TestPlanChangeModel
 from testgear_api_client.model.test_plan_link import TestPlanLink
 from testgear_api_client.model.test_plan_model import TestPlanModel
 from testgear_api_client.model.test_plan_post_model import TestPlanPostModel
 from testgear_api_client.model.test_plan_put_model import TestPlanPutModel
 from testgear_api_client.model.test_plan_short_model import TestPlanShortModel
 from testgear_api_client.model.test_plan_with_test_suite_tree_model import TestPlanWithTestSuiteTreeModel
 from testgear_api_client.model.test_point_analytic_result import TestPointAnalyticResult
+from testgear_api_client.model.test_point_select_model import TestPointSelectModel
 from testgear_api_client.model.test_point_with_last_result_model import TestPointWithLastResultModel
 from testgear_api_client.model.test_run_model import TestRunModel
 from testgear_api_client.model.test_run_search_query_model import TestRunSearchQueryModel
 from testgear_api_client.model.test_suite_v2_tree_model import TestSuiteV2TreeModel
 from testgear_api_client.model.validation_problem_details import ValidationProblemDetails
 from testgear_api_client.model.work_item_select_model import WorkItemSelectModel
 
@@ -605,14 +607,71 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.api_v2_test_plans_id_patch_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/testPlans/{id}',
+                'operation_id': 'api_v2_test_plans_id_patch',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'operation',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'operation':
+                        ([Operation],),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'operation': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.api_v2_test_plans_id_test_points_last_results_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([TestPointWithLastResultModel],),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
                 'endpoint_path': '/api/v2/testPlans/{id}/testPoints/lastResults',
@@ -747,14 +806,134 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.api_v2_test_plans_id_test_points_tester_delete_endpoint = _Endpoint(
+            settings={
+                'response_type': ([str],),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/testPlans/{id}/testPoints/tester',
+                'operation_id': 'api_v2_test_plans_id_test_points_tester_delete',
+                'http_method': 'DELETE',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'test_point_select_model',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'test_point_select_model':
+                        (TestPointSelectModel,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'test_point_select_model': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.api_v2_test_plans_id_test_points_tester_user_id_post_endpoint = _Endpoint(
+            settings={
+                'response_type': ([str],),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/testPlans/{id}/testPoints/tester/{userId}',
+                'operation_id': 'api_v2_test_plans_id_test_points_tester_user_id_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'user_id',
+                    'test_point_select_model',
+                ],
+                'required': [
+                    'id',
+                    'user_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'user_id':
+                        (str,),
+                    'test_point_select_model':
+                        (TestPointSelectModel,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                    'user_id': 'userId',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'user_id': 'path',
+                    'test_point_select_model': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.api_v2_test_plans_id_test_runs_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([TestRunModel],),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
                 'endpoint_path': '/api/v2/testPlans/{id}/testRuns',
@@ -2357,14 +2536,98 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.api_v2_test_plans_id_links_get_endpoint.call_with_http_info(**kwargs)
 
+    def api_v2_test_plans_id_patch(
+        self,
+        id,
+        **kwargs
+    ):
+        """Patch test plan  # noqa: E501
+
+        See <a href=\"https://www.rfc-editor.org/rfc/rfc6902\" target=\"_blank\">RFC 6902: JavaScript Object Notation (JSON) Patch</a> for details  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_test_plans_id_patch(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Unique ID of the test plan
+
+        Keyword Args:
+            operation ([Operation]): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.api_v2_test_plans_id_patch_endpoint.call_with_http_info(**kwargs)
+
     def api_v2_test_plans_id_test_points_last_results_get(
         self,
         id,
         **kwargs
     ):
         """Get TestPoints with last result from TestPlan  # noqa: E501
 
@@ -2530,14 +2793,184 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.api_v2_test_plans_id_test_points_reset_post_endpoint.call_with_http_info(**kwargs)
 
+    def api_v2_test_plans_id_test_points_tester_delete(
+        self,
+        id,
+        **kwargs
+    ):
+        """Unassign users from multiple test points  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_test_plans_id_test_points_tester_delete(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Unique or global ID of the test plan
+
+        Keyword Args:
+            test_point_select_model (TestPointSelectModel): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [str]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.api_v2_test_plans_id_test_points_tester_delete_endpoint.call_with_http_info(**kwargs)
+
+    def api_v2_test_plans_id_test_points_tester_user_id_post(
+        self,
+        id,
+        user_id,
+        **kwargs
+    ):
+        """Assign user as a tester to multiple test points  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_test_plans_id_test_points_tester_user_id_post(id, user_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Unique or global ID of the test plan
+            user_id (str): Unique ID of the user
+
+        Keyword Args:
+            test_point_select_model (TestPointSelectModel): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [str]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        kwargs['user_id'] = \
+            user_id
+        return self.api_v2_test_plans_id_test_points_tester_user_id_post_endpoint.call_with_http_info(**kwargs)
+
     def api_v2_test_plans_id_test_runs_get(
         self,
         id,
         **kwargs
     ):
         """Get TestRuns of TestPlan  # noqa: E501
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/test_points_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/test_points_api.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/test_results_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/test_results_api.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/test_runs_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/test_runs_api.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/test_suites_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/test_suites_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from testgear_api_client.model.configuration_model import ConfigurationModel
+from testgear_api_client.model.operation import Operation
 from testgear_api_client.model.problem_details import ProblemDetails
 from testgear_api_client.model.test_point_by_test_suite_model import TestPointByTestSuiteModel
 from testgear_api_client.model.test_result_v2_short_model import TestResultV2ShortModel
 from testgear_api_client.model.test_suite_v2_get_model import TestSuiteV2GetModel
 from testgear_api_client.model.test_suite_v2_post_model import TestSuiteV2PostModel
 from testgear_api_client.model.test_suite_v2_put_model import TestSuiteV2PutModel
 from testgear_api_client.model.test_suite_work_items_search_model import TestSuiteWorkItemsSearchModel
@@ -98,14 +99,122 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.api_v2_test_suites_id_patch_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/testSuites/{id}',
+                'operation_id': 'api_v2_test_suites_id_patch',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'operation',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'operation':
+                        ([Operation],),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'operation': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.api_v2_test_suites_id_refresh_post_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/testSuites/{id}/refresh',
+                'operation_id': 'api_v2_test_suites_id_refresh_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.create_test_suite_endpoint = _Endpoint(
             settings={
                 'response_type': (TestSuiteV2GetModel,),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
                 'endpoint_path': '/api/v2/testSuites',
@@ -828,14 +937,180 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.add_test_points_to_test_suite_endpoint.call_with_http_info(**kwargs)
 
+    def api_v2_test_suites_id_patch(
+        self,
+        id,
+        **kwargs
+    ):
+        """Patch test suite  # noqa: E501
+
+        See <a href=\"https://www.rfc-editor.org/rfc/rfc6902\" target=\"_blank\">RFC 6902: JavaScript Object Notation (JSON) Patch</a> for details  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_test_suites_id_patch(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Test Suite internal (UUID) identifier
+
+        Keyword Args:
+            operation ([Operation]): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.api_v2_test_suites_id_patch_endpoint.call_with_http_info(**kwargs)
+
+    def api_v2_test_suites_id_refresh_post(
+        self,
+        id,
+        **kwargs
+    ):
+        """Refresh test suite. Only dynamic test suites are supported by this method  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_test_suites_id_refresh_post(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Test Suite internal (UUID) identifier
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.api_v2_test_suites_id_refresh_post_endpoint.call_with_http_info(**kwargs)
+
     def create_test_suite(
         self,
         **kwargs
     ):
         """Create TestSuite  # noqa: E501
 
         <br>Use case  <br>User sets test suite model (listed in request parameters)  <br>User runs method execution  <br>System creates test suite  <br>System returns test suite  # noqa: E501
@@ -1418,15 +1693,15 @@
     def search_work_items(
         self,
         id,
         **kwargs
     ):
         """Search WorkItems  # noqa: E501
 
-        <br>Use case  <br>User sets test suite identifier  <br>[Optional] User sets filter  <br>User runs method execution  <br>System search test suite by identifier  <br>System search test points related to the test suite  <br>System search workitems related to the test points  <br>                      [Optional] User sets filter, system applies filter                     <br>System returns workitems array  # noqa: E501
+        <br>Use case  <br>User sets test suite identifier  <br>[Optional] User sets filter  <br>User runs method execution  <br>System search test suite by identifier  <br>System search test points related to the test suite  <br>System search work items related to the test points  <br>                      [Optional] User sets filter, system applies filter                     <br>System returns work items array  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.search_work_items(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1591,26 +1866,26 @@
     def set_work_items_by_test_suite_id(
         self,
         id,
         **kwargs
     ):
         """Set WorkItems By TestSuite Id  # noqa: E501
 
-        <br>Use case  <br>User sets test suite identifier  <br>User sets collection of workitems identifiers  <br>User runs method execution  <br>System search test suite by identifier  <br>System search test points related to the test suite  <br>System search workitems  <br>System restores(if exist) or creates test points with listed workitems  <br>System returns no content response  # noqa: E501
+        <br>Use case  <br>User sets test suite identifier  <br>User sets collection of work items identifiers  <br>User runs method execution  <br>System search test suite by identifier  <br>System search test points related to the test suite  <br>System search work items  <br>System restores(if exist) or creates test points with listed work items  <br>System returns no content response  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.set_work_items_by_test_suite_id(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): Test suite internal (guid format) identifier\"
 
         Keyword Args:
-            request_body ([str]): Collection of workitem identifiers\". [optional]
+            request_body ([str]): Collection of work item identifiers\". [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/webhooks_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/webhooks_api.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/webhooks_logs_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/webhooks_logs_api.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/work_items_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/work_items_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,72 @@
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
+        self.api_v2_work_items_id_attachments_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (str,),
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/workItems/{id}/attachments',
+                'operation_id': 'api_v2_work_items_id_attachments_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                    'file',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                    'file':
+                        (file_type,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                    'file': 'file',
+                },
+                'location_map': {
+                    'id': 'path',
+                    'file': 'form',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'multipart/form-data'
+                ]
+            },
+            api_client=api_client
+        )
         self.api_v2_work_items_id_check_list_transform_to_test_case_post_endpoint = _Endpoint(
             settings={
                 'response_type': (WorkItemModel,),
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
                 'endpoint_path': '/api/v2/workItems/{id}/checkList/transformTo/testCase',
@@ -1340,14 +1398,116 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.purge_work_item_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/workItems/{id}/purge',
+                'operation_id': 'purge_work_item',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.restore_work_item_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'Bearer or PrivateToken'
+                ],
+                'endpoint_path': '/api/v2/workItems/{id}/restore',
+                'operation_id': 'restore_work_item',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.update_work_item_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'Bearer or PrivateToken'
                 ],
                 'endpoint_path': '/api/v2/workItems',
@@ -1391,14 +1551,98 @@
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
 
+    def api_v2_work_items_id_attachments_post(
+        self,
+        id,
+        **kwargs
+    ):
+        """Upload and link attachment to WorkItem  # noqa: E501
+
+        <br>Use case  <br>User sets workItemId  <br>User attaches a file  <br>System creates attachment and links it to the work item  <br>System returns attachment identifier  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_v2_work_items_id_attachments_post(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Work item internal identifier (guid format)
+
+        Keyword Args:
+            file (file_type): Select file. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            str
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.api_v2_work_items_id_attachments_post_endpoint.call_with_http_info(**kwargs)
+
     def api_v2_work_items_id_check_list_transform_to_test_case_post(
         self,
         id,
         **kwargs
     ):
         """Transform CheckList to TestCase  # noqa: E501
 
@@ -3166,14 +3410,178 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.get_work_item_versions_endpoint.call_with_http_info(**kwargs)
 
+    def purge_work_item(
+        self,
+        id,
+        **kwargs
+    ):
+        """Permanently delete test case, checklist or shared steps from archive  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.purge_work_item(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Unique or global ID of the work item
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.purge_work_item_endpoint.call_with_http_info(**kwargs)
+
+    def restore_work_item(
+        self,
+        id,
+        **kwargs
+    ):
+        """Restore test case, checklist or shared steps from archive  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.restore_work_item(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Unique or global ID of the work item
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['id'] = \
+            id
+        return self.restore_work_item_endpoint.call_with_http_info(**kwargs)
+
     def update_work_item(
         self,
         **kwargs
     ):
         """Update Test Case, Checklist or Shared Step  # noqa: E501
 
         <br>Use case  <br>User sets workitem properties (listed in request parameters)  <br>User runs method execution  <br>System updates workitem by identifier  <br>System returns updated workitem model (listed in response parameters)  # noqa: E501
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api/work_items_comments_api.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api/work_items_comments_api.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/api_client.py` & `testgear-api-client-3.1.0/src/testgear_api_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/3.0.0/python'
+        self.user_agent = 'OpenAPI-Generator/3.1.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/apis/__init__.py` & `testgear-api-client-3.1.0/src/testgear_api_client/apis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
 from testgear_api_client.api.attachments_api import AttachmentsApi
 from testgear_api_client.api.auto_tests_api import AutoTestsApi
+from testgear_api_client.api.background_jobs_api import BackgroundJobsApi
 from testgear_api_client.api.configurations_api import ConfigurationsApi
 from testgear_api_client.api.custom_attribute_templates_api import CustomAttributeTemplatesApi
 from testgear_api_client.api.custom_attributes_api import CustomAttributesApi
 from testgear_api_client.api.notifications_api import NotificationsApi
 from testgear_api_client.api.parameters_api import ParametersApi
 from testgear_api_client.api.projects_api import ProjectsApi
 from testgear_api_client.api.sections_api import SectionsApi
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/configuration.py` & `testgear-api-client-3.1.0/src/testgear_api_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v2.0\n"\
-               "SDK Package Version: 3.0.0".\
+               "SDK Package Version: 3.1.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/exceptions.py` & `testgear-api-client-3.1.0/src/testgear_api_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/attachment_change_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/attachment_change_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/attachment_change_view_model_array_work_item_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/attachment_change_view_model_array_work_item_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/attachment_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/attachment_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/attachment_model_auto_test_step_results_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/attachment_model_auto_test_step_results_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/attachment_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/attachment_put_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/attachment_put_model_auto_test_step_results_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/attachment_put_model_auto_test_step_results_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/attachment_sub_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/attachment_sub_get_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_average_duration_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_average_duration_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_change_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_change_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_change_view_model_array_work_item_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_change_view_model_array_work_item_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_id_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_id_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_model_v2_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_model_v2_get_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_namespace_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_namespace_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_post_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_put_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_results_for_test_run_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_results_for_test_run_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,16 +101,16 @@
             'failure_reason_names': ([FailureCategoryModel], none_type,),  # noqa: E501
             'message': (str, none_type,),  # noqa: E501
             'traces': (str, none_type,),  # noqa: E501
             'started_on': (datetime, none_type,),  # noqa: E501
             'completed_on': (datetime, none_type,),  # noqa: E501
             'duration': (int, none_type,),  # noqa: E501
             'attachments': ([AttachmentPutModel], none_type,),  # noqa: E501
-            'parameters': ({str: (str, none_type)}, none_type,),  # noqa: E501
-            'properties': ({str: (str, none_type)}, none_type,),  # noqa: E501
+            'parameters': ({str: (str,)}, none_type,),  # noqa: E501
+            'properties': ({str: (str,)}, none_type,),  # noqa: E501
             'step_results': ([AttachmentPutModelAutoTestStepResultsModel], none_type,),  # noqa: E501
             'setup_results': ([AttachmentPutModelAutoTestStepResultsModel], none_type,),  # noqa: E501
             'teardown_results': ([AttachmentPutModelAutoTestStepResultsModel], none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -186,16 +186,16 @@
             failure_reason_names ([FailureCategoryModel], none_type): Specifies the cause of autotest failure.. [optional]  # noqa: E501
             message (str, none_type): A comment for the result.. [optional]  # noqa: E501
             traces (str, none_type): An extended comment or a stack trace.. [optional]  # noqa: E501
             started_on (datetime, none_type): Test run start date.. [optional]  # noqa: E501
             completed_on (datetime, none_type): Test run end date.. [optional]  # noqa: E501
             duration (int, none_type): Expected or actual duration of the test run execution in milliseconds.. [optional]  # noqa: E501
             attachments ([AttachmentPutModel], none_type): Specifies an attachment GUID. Multiple values can be sent.. [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): \"<b>parameter</b>\": \"<b>value</b>\" pair with arbitrary custom parameters. Multiple parameters can be sent.. [optional]  # noqa: E501
-            properties ({str: (str, none_type)}, none_type): \"<b>property</b>\": \"<b>value</b>\" pair with arbitrary custom properties. Multiple properties can be sent.. [optional]  # noqa: E501
+            parameters ({str: (str,)}, none_type): \"<b>parameter</b>\": \"<b>value</b>\" pair with arbitrary custom parameters. Multiple parameters can be sent.. [optional]  # noqa: E501
+            properties ({str: (str,)}, none_type): \"<b>property</b>\": \"<b>value</b>\" pair with arbitrary custom properties. Multiple properties can be sent.. [optional]  # noqa: E501
             step_results ([AttachmentPutModelAutoTestStepResultsModel], none_type): Specifies the results of individual steps.. [optional]  # noqa: E501
             setup_results ([AttachmentPutModelAutoTestStepResultsModel], none_type): Specifies the results of setup steps. For information on supported values, see the `stepResults` parameter above.. [optional]  # noqa: E501
             teardown_results ([AttachmentPutModelAutoTestStepResultsModel], none_type): Specifies the results of the teardown steps. For information on supported values, see the `stepResults` parameter above.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
@@ -292,16 +292,16 @@
             failure_reason_names ([FailureCategoryModel], none_type): Specifies the cause of autotest failure.. [optional]  # noqa: E501
             message (str, none_type): A comment for the result.. [optional]  # noqa: E501
             traces (str, none_type): An extended comment or a stack trace.. [optional]  # noqa: E501
             started_on (datetime, none_type): Test run start date.. [optional]  # noqa: E501
             completed_on (datetime, none_type): Test run end date.. [optional]  # noqa: E501
             duration (int, none_type): Expected or actual duration of the test run execution in milliseconds.. [optional]  # noqa: E501
             attachments ([AttachmentPutModel], none_type): Specifies an attachment GUID. Multiple values can be sent.. [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): \"<b>parameter</b>\": \"<b>value</b>\" pair with arbitrary custom parameters. Multiple parameters can be sent.. [optional]  # noqa: E501
-            properties ({str: (str, none_type)}, none_type): \"<b>property</b>\": \"<b>value</b>\" pair with arbitrary custom properties. Multiple properties can be sent.. [optional]  # noqa: E501
+            parameters ({str: (str,)}, none_type): \"<b>parameter</b>\": \"<b>value</b>\" pair with arbitrary custom parameters. Multiple parameters can be sent.. [optional]  # noqa: E501
+            properties ({str: (str,)}, none_type): \"<b>property</b>\": \"<b>value</b>\" pair with arbitrary custom properties. Multiple properties can be sent.. [optional]  # noqa: E501
             step_results ([AttachmentPutModelAutoTestStepResultsModel], none_type): Specifies the results of individual steps.. [optional]  # noqa: E501
             setup_results ([AttachmentPutModelAutoTestStepResultsModel], none_type): Specifies the results of setup steps. For information on supported values, see the `stepResults` parameter above.. [optional]  # noqa: E501
             teardown_results ([AttachmentPutModelAutoTestStepResultsModel], none_type): Specifies the results of the teardown steps. For information on supported values, see the `stepResults` parameter above.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_short_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_short_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/auto_test_step_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/auto_test_step_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/autotest_filter_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/autotest_filter_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/autotest_historical_result_select_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/autotest_historical_result_select_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/autotest_result_historical_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/autotest_result_historical_get_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,64 +76,67 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'outcome': (AutotestResultOutcome,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'created_by_id': (str,),  # noqa: E501
-            'modified_date': (datetime, none_type,),  # noqa: E501
-            'modified_by_id': (str, none_type,),  # noqa: E501
             'test_run_id': (str,),  # noqa: E501
             'test_run_name': (str, none_type,),  # noqa: E501
+            'configuration_id': (str,),  # noqa: E501
+            'launch_source': (str, none_type,),  # noqa: E501
+            'modified_date': (datetime, none_type,),  # noqa: E501
+            'modified_by_id': (str, none_type,),  # noqa: E501
             'test_plan_id': (str, none_type,),  # noqa: E501
             'test_plan_global_id': (int, none_type,),  # noqa: E501
             'test_plan_name': (str, none_type,),  # noqa: E501
-            'configuration_id': (str,),  # noqa: E501
-            'outcome': (AutotestResultOutcome,),  # noqa: E501
             'duration': (int, none_type,),  # noqa: E501
-            'launch_source': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'outcome': 'outcome',  # noqa: E501
         'id': 'id',  # noqa: E501
         'created_date': 'createdDate',  # noqa: E501
         'created_by_id': 'createdById',  # noqa: E501
-        'modified_date': 'modifiedDate',  # noqa: E501
-        'modified_by_id': 'modifiedById',  # noqa: E501
         'test_run_id': 'testRunId',  # noqa: E501
         'test_run_name': 'testRunName',  # noqa: E501
+        'configuration_id': 'configurationId',  # noqa: E501
+        'launch_source': 'launchSource',  # noqa: E501
+        'modified_date': 'modifiedDate',  # noqa: E501
+        'modified_by_id': 'modifiedById',  # noqa: E501
         'test_plan_id': 'testPlanId',  # noqa: E501
         'test_plan_global_id': 'testPlanGlobalId',  # noqa: E501
         'test_plan_name': 'testPlanName',  # noqa: E501
-        'configuration_id': 'configurationId',  # noqa: E501
-        'outcome': 'outcome',  # noqa: E501
         'duration': 'duration',  # noqa: E501
-        'launch_source': 'launchSource',  # noqa: E501
     }
 
     read_only_vars = {
         'modified_date',  # noqa: E501
         'modified_by_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, outcome, *args, **kwargs):  # noqa: E501
         """AutotestResultHistoricalGetModel - a model defined in OpenAPI
 
+        Args:
+            outcome (AutotestResultOutcome):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -160,25 +163,24 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
             created_date (datetime): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
-            modified_date (datetime, none_type): [optional]  # noqa: E501
-            modified_by_id (str, none_type): [optional]  # noqa: E501
             test_run_id (str): [optional]  # noqa: E501
             test_run_name (str, none_type): [optional]  # noqa: E501
+            configuration_id (str): [optional]  # noqa: E501
+            launch_source (str, none_type): [optional]  # noqa: E501
+            modified_date (datetime, none_type): [optional]  # noqa: E501
+            modified_by_id (str, none_type): [optional]  # noqa: E501
             test_plan_id (str, none_type): [optional]  # noqa: E501
             test_plan_global_id (int, none_type): [optional]  # noqa: E501
             test_plan_name (str, none_type): [optional]  # noqa: E501
-            configuration_id (str): [optional]  # noqa: E501
-            outcome (AutotestResultOutcome): [optional]  # noqa: E501
             duration (int, none_type): [optional]  # noqa: E501
-            launch_source (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -202,14 +204,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.outcome = outcome
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -222,17 +225,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, outcome, *args, **kwargs):  # noqa: E501
         """AutotestResultHistoricalGetModel - a model defined in OpenAPI
 
+        Args:
+            outcome (AutotestResultOutcome):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -259,25 +265,24 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
             created_date (datetime): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
-            modified_date (datetime, none_type): [optional]  # noqa: E501
-            modified_by_id (str, none_type): [optional]  # noqa: E501
             test_run_id (str): [optional]  # noqa: E501
             test_run_name (str, none_type): [optional]  # noqa: E501
+            configuration_id (str): [optional]  # noqa: E501
+            launch_source (str, none_type): [optional]  # noqa: E501
+            modified_date (datetime, none_type): [optional]  # noqa: E501
+            modified_by_id (str, none_type): [optional]  # noqa: E501
             test_plan_id (str, none_type): [optional]  # noqa: E501
             test_plan_global_id (int, none_type): [optional]  # noqa: E501
             test_plan_name (str, none_type): [optional]  # noqa: E501
-            configuration_id (str): [optional]  # noqa: E501
-            outcome (AutotestResultOutcome): [optional]  # noqa: E501
             duration (int, none_type): [optional]  # noqa: E501
-            launch_source (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -299,14 +304,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.outcome = outcome
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/autotest_result_outcome.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/autotest_result_outcome.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/autotest_result_reason_sub_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/autotest_result_reason_sub_get_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/autotest_select_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/autotest_select_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/autotests_extraction_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/autotests_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/autotests_select_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/autotests_select_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/available_test_result_outcome.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/available_test_result_outcome.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/boolean_nullable_test_plan_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/boolean_nullable_test_plan_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/boolean_test_plan_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/boolean_test_plan_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/boolean_work_item_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/boolean_work_item_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/configuration_by_parameters_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/configuration_by_parameters_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,38 +73,41 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
+            'parameter_ids': ([str],),  # noqa: E501
             'project_id': (str,),  # noqa: E501
-            'parameter_ids': ([str], none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'project_id': 'projectId',  # noqa: E501
         'parameter_ids': 'parameterIds',  # noqa: E501
+        'project_id': 'projectId',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, parameter_ids, *args, **kwargs):  # noqa: E501
         """ConfigurationByParametersModel - a model defined in OpenAPI
 
+        Args:
+            parameter_ids ([str]):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -129,15 +132,14 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             project_id (str): This property is used to link configuration with project. [optional]  # noqa: E501
-            parameter_ids ([str], none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -161,14 +163,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.parameter_ids = parameter_ids
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -181,17 +184,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, parameter_ids, *args, **kwargs):  # noqa: E501
         """ConfigurationByParametersModel - a model defined in OpenAPI
 
+        Args:
+            parameter_ids ([str]):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -216,15 +222,14 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             project_id (str): This property is used to link configuration with project. [optional]  # noqa: E501
-            parameter_ids ([str], none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -246,14 +251,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.parameter_ids = parameter_ids
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/configuration_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/configuration_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,16 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'description': (str, none_type,),  # noqa: E501
             'is_active': (bool,),  # noqa: E501
-            'capabilities': ({str: (str, none_type)}, none_type,),  # noqa: E501
-            'parameters': ({str: (str, none_type)}, none_type,),  # noqa: E501
+            'capabilities': ({str: (str,)}, none_type,),  # noqa: E501
+            'parameters': ({str: (str,)}, none_type,),  # noqa: E501
             'project_id': (str,),  # noqa: E501
             'is_default': (bool,),  # noqa: E501
             'name': (str, none_type,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'modified_date': (datetime, none_type,),  # noqa: E501
             'created_by_id': (str,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
@@ -152,16 +152,16 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str, none_type): [optional]  # noqa: E501
             is_active (bool): [optional]  # noqa: E501
-            capabilities ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
+            capabilities ({str: (str,)}, none_type): [optional]  # noqa: E501
+            parameters ({str: (str,)}, none_type): [optional]  # noqa: E501
             project_id (str): This property is used to link configuration with project. [optional]  # noqa: E501
             is_default (bool): [optional]  # noqa: E501
             name (str, none_type): [optional]  # noqa: E501
             created_date (datetime): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
@@ -251,16 +251,16 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str, none_type): [optional]  # noqa: E501
             is_active (bool): [optional]  # noqa: E501
-            capabilities ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
+            capabilities ({str: (str,)}, none_type): [optional]  # noqa: E501
+            parameters ({str: (str,)}, none_type): [optional]  # noqa: E501
             project_id (str): This property is used to link configuration with project. [optional]  # noqa: E501
             is_default (bool): [optional]  # noqa: E501
             name (str, none_type): [optional]  # noqa: E501
             created_date (datetime): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/configuration_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/configuration_put_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 
-class ConfigurationPostModel(ModelNormal):
+class ConfigurationPutModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -74,29 +74,31 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
+            'id': (str,),  # noqa: E501
             'project_id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'description': (str, none_type,),  # noqa: E501
             'is_active': (bool,),  # noqa: E501
-            'capabilities': ({str: (str, none_type)}, none_type,),  # noqa: E501
-            'parameters': ({str: (str, none_type)}, none_type,),  # noqa: E501
+            'capabilities': ({str: (str,)}, none_type,),  # noqa: E501
+            'parameters': ({str: (str,)}, none_type,),  # noqa: E501
             'is_default': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'id': 'id',  # noqa: E501
         'project_id': 'projectId',  # noqa: E501
         'name': 'name',  # noqa: E501
         'description': 'description',  # noqa: E501
         'is_active': 'isActive',  # noqa: E501
         'capabilities': 'capabilities',  # noqa: E501
         'parameters': 'parameters',  # noqa: E501
         'is_default': 'isDefault',  # noqa: E501
@@ -105,18 +107,19 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, project_id, name, *args, **kwargs):  # noqa: E501
-        """ConfigurationPostModel - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, project_id, name, *args, **kwargs):  # noqa: E501
+        """ConfigurationPutModel - a model defined in OpenAPI
 
         Args:
+            id (str):
             project_id (str): This property is used to link configuration with project
             name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -145,16 +148,16 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str, none_type): [optional]  # noqa: E501
             is_active (bool): [optional]  # noqa: E501
-            capabilities ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
+            capabilities ({str: (str,)}, none_type): [optional]  # noqa: E501
+            parameters ({str: (str,)}, none_type): [optional]  # noqa: E501
             is_default (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -179,14 +182,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
         self.project_id = project_id
         self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
@@ -201,18 +205,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, project_id, name, *args, **kwargs):  # noqa: E501
-        """ConfigurationPostModel - a model defined in OpenAPI
+    def __init__(self, id, project_id, name, *args, **kwargs):  # noqa: E501
+        """ConfigurationPutModel - a model defined in OpenAPI
 
         Args:
+            id (str):
             project_id (str): This property is used to link configuration with project
             name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -241,16 +246,16 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str, none_type): [optional]  # noqa: E501
             is_active (bool): [optional]  # noqa: E501
-            capabilities ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
+            capabilities ({str: (str,)}, none_type): [optional]  # noqa: E501
+            parameters ({str: (str,)}, none_type): [optional]  # noqa: E501
             is_default (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -273,14 +278,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
         self.project_id = project_id
         self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/configuration_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/link_put_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from testgear_api_client.model.link_type import LinkType
+    globals()['LinkType'] = LinkType
 
-class ConfigurationPutModel(ModelNormal):
+
+class LinkPutModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -54,15 +58,15 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('name',): {
+        ('url',): {
             'min_length': 1,
         },
     }
 
     additional_properties_type = None
 
     _nullable = False
@@ -73,55 +77,50 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
+            'url': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
-            'project_id': (str,),  # noqa: E501
-            'name': (str,),  # noqa: E501
+            'title': (str, none_type,),  # noqa: E501
             'description': (str, none_type,),  # noqa: E501
-            'is_active': (bool,),  # noqa: E501
-            'capabilities': ({str: (str, none_type)}, none_type,),  # noqa: E501
-            'parameters': ({str: (str, none_type)}, none_type,),  # noqa: E501
-            'is_default': (bool,),  # noqa: E501
+            'type': (LinkType,),  # noqa: E501
+            'has_info': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'url': 'url',  # noqa: E501
         'id': 'id',  # noqa: E501
-        'project_id': 'projectId',  # noqa: E501
-        'name': 'name',  # noqa: E501
+        'title': 'title',  # noqa: E501
         'description': 'description',  # noqa: E501
-        'is_active': 'isActive',  # noqa: E501
-        'capabilities': 'capabilities',  # noqa: E501
-        'parameters': 'parameters',  # noqa: E501
-        'is_default': 'isDefault',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'has_info': 'hasInfo',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, project_id, name, *args, **kwargs):  # noqa: E501
-        """ConfigurationPutModel - a model defined in OpenAPI
+    def _from_openapi_data(cls, url, *args, **kwargs):  # noqa: E501
+        """LinkPutModel - a model defined in OpenAPI
 
         Args:
-            id (str):
-            project_id (str): This property is used to link configuration with project
-            name (str):
+            url (str): Address can be specified without protocol, but necessarily with the domain.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -146,19 +145,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            description (str, none_type): [optional]  # noqa: E501
-            is_active (bool): [optional]  # noqa: E501
-            capabilities ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
-            is_default (bool): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            title (str, none_type): Link name.. [optional]  # noqa: E501
+            description (str, none_type): Link description.. [optional]  # noqa: E501
+            type (LinkType): [optional]  # noqa: E501
+            has_info (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -182,17 +181,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.project_id = project_id
-        self.name = name
+        self.url = url
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -205,21 +202,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, project_id, name, *args, **kwargs):  # noqa: E501
-        """ConfigurationPutModel - a model defined in OpenAPI
+    def __init__(self, url, *args, **kwargs):  # noqa: E501
+        """LinkPutModel - a model defined in OpenAPI
 
         Args:
-            id (str):
-            project_id (str): This property is used to link configuration with project
-            name (str):
+            url (str): Address can be specified without protocol, but necessarily with the domain.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,19 +239,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            description (str, none_type): [optional]  # noqa: E501
-            is_active (bool): [optional]  # noqa: E501
-            capabilities ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
-            is_default (bool): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            title (str, none_type): Link name.. [optional]  # noqa: E501
+            description (str, none_type): Link description.. [optional]  # noqa: E501
+            type (LinkType): [optional]  # noqa: E501
+            has_info (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -278,17 +273,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.project_id = project_id
-        self.name = name
+        self.url = url
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/configuration_select_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/configuration_select_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_change_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_change_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_get_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,50 +78,53 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'type': (CustomAttributeTypesEnum,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'options': ([CustomAttributeOptionModel], none_type,),  # noqa: E501
-            'type': (CustomAttributeTypesEnum,),  # noqa: E501
             'is_deleted': (bool,),  # noqa: E501
             'name': (str, none_type,),  # noqa: E501
             'is_enabled': (bool,),  # noqa: E501
             'is_required': (bool,),  # noqa: E501
             'is_global': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'type': 'type',  # noqa: E501
         'id': 'id',  # noqa: E501
         'options': 'options',  # noqa: E501
-        'type': 'type',  # noqa: E501
         'is_deleted': 'isDeleted',  # noqa: E501
         'name': 'name',  # noqa: E501
         'is_enabled': 'isEnabled',  # noqa: E501
         'is_required': 'isRequired',  # noqa: E501
         'is_global': 'isGlobal',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, type, *args, **kwargs):  # noqa: E501
         """CustomAttributeGetModel - a model defined in OpenAPI
 
+        Args:
+            type (CustomAttributeTypesEnum):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -147,15 +150,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Unique ID of the attribute. [optional]  # noqa: E501
             options ([CustomAttributeOptionModel], none_type): Collection of the attribute options. [optional]  # noqa: E501
-            type (CustomAttributeTypesEnum): [optional]  # noqa: E501
             is_deleted (bool): Indicates if the attribute is deleted. [optional]  # noqa: E501
             name (str, none_type): Name of the attribute. [optional]  # noqa: E501
             is_enabled (bool): Indicates if the attribute is enabled. [optional]  # noqa: E501
             is_required (bool): Indicates if the attribute is mandatory to specify. [optional]  # noqa: E501
             is_global (bool): Indicates if the attribute is available across all projects. [optional]  # noqa: E501
         """
 
@@ -184,14 +186,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -204,17 +207,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, type, *args, **kwargs):  # noqa: E501
         """CustomAttributeGetModel - a model defined in OpenAPI
 
+        Args:
+            type (CustomAttributeTypesEnum):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -240,15 +246,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Unique ID of the attribute. [optional]  # noqa: E501
             options ([CustomAttributeOptionModel], none_type): Collection of the attribute options. [optional]  # noqa: E501
-            type (CustomAttributeTypesEnum): [optional]  # noqa: E501
             is_deleted (bool): Indicates if the attribute is deleted. [optional]  # noqa: E501
             name (str, none_type): Name of the attribute. [optional]  # noqa: E501
             is_enabled (bool): Indicates if the attribute is enabled. [optional]  # noqa: E501
             is_required (bool): Indicates if the attribute is mandatory to specify. [optional]  # noqa: E501
             is_global (bool): Indicates if the attribute is available across all projects. [optional]  # noqa: E501
         """
 
@@ -275,14 +280,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_option_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_option_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_option_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_option_post_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_post_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_put_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_search_query_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_search_query_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_template_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_template_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_template_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_template_post_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_template_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_template_put_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_template_search_query_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_template_search_query_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_test_plan_project_relation_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_test_plan_project_relation_put_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/custom_attribute_types_enum.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/custom_attribute_types_enum.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/date_range_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/date_time_range_selector_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 
-class DateRangeModel(ModelNormal):
+class DateTimeRangeSelectorModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -93,15 +93,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DateRangeModel - a model defined in OpenAPI
+        """DateTimeRangeSelectorModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -126,16 +126,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            _from (datetime, none_type): Minimum date and time. [optional]  # noqa: E501
-            to (datetime, none_type): Maximum date and time. [optional]  # noqa: E501
+            _from (datetime, none_type): [optional]  # noqa: E501
+            to (datetime, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -180,15 +180,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DateRangeModel - a model defined in OpenAPI
+        """DateTimeRangeSelectorModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,16 +213,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            _from (datetime, none_type): Minimum date and time. [optional]  # noqa: E501
-            to (datetime, none_type): Maximum date and time. [optional]  # noqa: E501
+            _from (datetime, none_type): [optional]  # noqa: E501
+            to (datetime, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/date_time_range_selector_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/int32_range_selector_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 
-class DateTimeRangeSelectorModel(ModelNormal):
+class Int32RangeSelectorModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -71,16 +71,16 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            '_from': (datetime, none_type,),  # noqa: E501
-            'to': (datetime, none_type,),  # noqa: E501
+            '_from': (int, none_type,),  # noqa: E501
+            'to': (int, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -93,15 +93,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DateTimeRangeSelectorModel - a model defined in OpenAPI
+        """Int32RangeSelectorModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -126,16 +126,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            _from (datetime, none_type): [optional]  # noqa: E501
-            to (datetime, none_type): [optional]  # noqa: E501
+            _from (int, none_type): [optional]  # noqa: E501
+            to (int, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -180,15 +180,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DateTimeRangeSelectorModel - a model defined in OpenAPI
+        """Int32RangeSelectorModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,16 +213,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            _from (datetime, none_type): [optional]  # noqa: E501
-            to (datetime, none_type): [optional]  # noqa: E501
+            _from (int, none_type): [optional]  # noqa: E501
+            to (int, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/external_link_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/external_link_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/failure_category_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/failure_category_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/failure_class_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/failure_class_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,16 +78,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'name': (str, none_type,),  # noqa: E501
             'failure_category': (FailureCategoryModel,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'modified_date': (datetime, none_type,),  # noqa: E501
             'created_by_id': (str,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
             'failure_class_regexes': ([FailureClassRegexModel], none_type,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'is_deleted': (bool,),  # noqa: E501
@@ -95,16 +95,16 @@
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
         'failure_category': 'failureCategory',  # noqa: E501
+        'name': 'name',  # noqa: E501
         'created_date': 'createdDate',  # noqa: E501
         'modified_date': 'modifiedDate',  # noqa: E501
         'created_by_id': 'createdById',  # noqa: E501
         'modified_by_id': 'modifiedById',  # noqa: E501
         'failure_class_regexes': 'failureClassRegexes',  # noqa: E501
         'id': 'id',  # noqa: E501
         'is_deleted': 'isDeleted',  # noqa: E501
@@ -113,17 +113,20 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, failure_category, *args, **kwargs):  # noqa: E501
         """FailureClassModel - a model defined in OpenAPI
 
+        Args:
+            failure_category (FailureCategoryModel):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -148,15 +151,14 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             name (str, none_type): [optional]  # noqa: E501
-            failure_category (FailureCategoryModel): [optional]  # noqa: E501
             created_date (datetime): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             failure_class_regexes ([FailureClassRegexModel], none_type): [optional]  # noqa: E501
             id (str): Unique ID of the entity. [optional]  # noqa: E501
             is_deleted (bool): Indicates if the entity is deleted. [optional]  # noqa: E501
@@ -187,14 +189,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.failure_category = failure_category
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -207,17 +210,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, failure_category, *args, **kwargs):  # noqa: E501
         """FailureClassModel - a model defined in OpenAPI
 
+        Args:
+            failure_category (FailureCategoryModel):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -242,15 +248,14 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             name (str, none_type): [optional]  # noqa: E501
-            failure_category (FailureCategoryModel): [optional]  # noqa: E501
             created_date (datetime): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             failure_class_regexes ([FailureClassRegexModel], none_type): [optional]  # noqa: E501
             id (str): Unique ID of the entity. [optional]  # noqa: E501
             is_deleted (bool): Indicates if the entity is deleted. [optional]  # noqa: E501
@@ -279,14 +284,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.failure_category = failure_category
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/failure_class_regex_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/failure_class_regex_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/filter_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/filter_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/flaky_bulk_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/flaky_bulk_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/get_xlsx_test_points_by_test_plan_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/get_xlsx_test_points_by_test_plan_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/global_custom_attribute_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/global_custom_attribute_post_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/global_custom_attribute_update_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/global_custom_attribute_update_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/guid_extraction_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/guid_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/guid_work_item_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/guid_work_item_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/image_resize_type.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/image_resize_type.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/int32_range_selector_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/int64_range_selector_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 
-class Int32RangeSelectorModel(ModelNormal):
+class Int64RangeSelectorModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -93,15 +93,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Int32RangeSelectorModel - a model defined in OpenAPI
+        """Int64RangeSelectorModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -180,15 +180,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Int32RangeSelectorModel - a model defined in OpenAPI
+        """Int64RangeSelectorModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/int32_work_item_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/int32_work_item_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/int64_range_selector_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/shared_step_result_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 
-class Int64RangeSelectorModel(ModelNormal):
+class SharedStepResultModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -71,37 +71,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            '_from': (int, none_type,),  # noqa: E501
-            'to': (int, none_type,),  # noqa: E501
+            'step_id': (str,),  # noqa: E501
+            'outcome': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        '_from': 'from',  # noqa: E501
-        'to': 'to',  # noqa: E501
+        'step_id': 'stepId',  # noqa: E501
+        'outcome': 'outcome',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Int64RangeSelectorModel - a model defined in OpenAPI
+        """SharedStepResultModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -126,16 +126,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            _from (int, none_type): [optional]  # noqa: E501
-            to (int, none_type): [optional]  # noqa: E501
+            step_id (str): [optional]  # noqa: E501
+            outcome (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -180,15 +180,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Int64RangeSelectorModel - a model defined in OpenAPI
+        """SharedStepResultModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,16 +213,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            _from (int, none_type): [optional]  # noqa: E501
-            to (int, none_type): [optional]  # noqa: E501
+            step_id (str): [optional]  # noqa: E501
+            outcome (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/int64_work_item_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/int64_work_item_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/iteration_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/iteration_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/iteration_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/iteration_put_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/label_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/label_post_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/label_short_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/label_short_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/last_test_result_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/last_test_result_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/link_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/link_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/link_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/link_post_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/link_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_link_change_view_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from testgear_api_client.model.link_type import LinkType
-    globals()['LinkType'] = LinkType
 
-
-class LinkPutModel(ModelNormal):
+class WorkItemLinkChangeViewModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -58,17 +54,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('url',): {
-            'min_length': 1,
-        },
     }
 
     additional_properties_type = None
 
     _nullable = False
 
     @cached_property
@@ -77,50 +70,46 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'url': (str,),  # noqa: E501
-            'id': (str,),  # noqa: E501
-            'title': (str, none_type,),  # noqa: E501
             'description': (str, none_type,),  # noqa: E501
-            'type': (LinkType, none_type,),  # noqa: E501
+            'url': (str, none_type,),  # noqa: E501
+            'title': (str, none_type,),  # noqa: E501
             'has_info': (bool,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'type': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'description': 'description',  # noqa: E501
         'url': 'url',  # noqa: E501
-        'id': 'id',  # noqa: E501
         'title': 'title',  # noqa: E501
-        'description': 'description',  # noqa: E501
-        'type': 'type',  # noqa: E501
         'has_info': 'hasInfo',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, url, *args, **kwargs):  # noqa: E501
-        """LinkPutModel - a model defined in OpenAPI
-
-        Args:
-            url (str): Address can be specified without protocol, but necessarily with the domain.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """WorkItemLinkChangeViewModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -145,19 +134,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            title (str, none_type): Link name.. [optional]  # noqa: E501
-            description (str, none_type): Link description.. [optional]  # noqa: E501
-            type (LinkType): [optional]  # noqa: E501
+            description (str, none_type): [optional]  # noqa: E501
+            url (str, none_type): [optional]  # noqa: E501
+            title (str, none_type): [optional]  # noqa: E501
             has_info (bool): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            type (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -181,15 +171,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.url = url
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -202,19 +191,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, url, *args, **kwargs):  # noqa: E501
-        """LinkPutModel - a model defined in OpenAPI
-
-        Args:
-            url (str): Address can be specified without protocol, but necessarily with the domain.
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """WorkItemLinkChangeViewModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -239,19 +225,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            title (str, none_type): Link name.. [optional]  # noqa: E501
-            description (str, none_type): Link description.. [optional]  # noqa: E501
-            type (LinkType): [optional]  # noqa: E501
+            description (str, none_type): [optional]  # noqa: E501
+            url (str, none_type): [optional]  # noqa: E501
+            title (str, none_type): [optional]  # noqa: E501
             has_info (bool): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            type (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -273,15 +260,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.url = url
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/link_sub_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/link_sub_get_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/link_type.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/link_type.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/no_content_result.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/no_content_result.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/notification_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/notification_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,19 +76,19 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'notification_type': (NotificationTypeModel,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'created_date': (datetime, none_type,),  # noqa: E501
             'is_read': (bool,),  # noqa: E501
             'entity_id': (str,),  # noqa: E501
-            'notification_type': (NotificationTypeModel,),  # noqa: E501
             'project_global_id': (int, none_type,),  # noqa: E501
             'project_name': (str, none_type,),  # noqa: E501
             'test_plan_global_id': (int,),  # noqa: E501
             'test_plan_name': (str, none_type,),  # noqa: E501
             'workitem_global_id': (int, none_type,),  # noqa: E501
             'comment': (str, none_type,),  # noqa: E501
             'work_item_name': (str, none_type,),  # noqa: E501
@@ -98,19 +98,19 @@
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'notification_type': 'notificationType',  # noqa: E501
         'id': 'id',  # noqa: E501
         'created_date': 'createdDate',  # noqa: E501
         'is_read': 'isRead',  # noqa: E501
         'entity_id': 'entityId',  # noqa: E501
-        'notification_type': 'notificationType',  # noqa: E501
         'project_global_id': 'projectGlobalId',  # noqa: E501
         'project_name': 'projectName',  # noqa: E501
         'test_plan_global_id': 'testPlanGlobalId',  # noqa: E501
         'test_plan_name': 'testPlanName',  # noqa: E501
         'workitem_global_id': 'workitemGlobalId',  # noqa: E501
         'comment': 'comment',  # noqa: E501
         'work_item_name': 'workItemName',  # noqa: E501
@@ -121,17 +121,20 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, notification_type, *args, **kwargs):  # noqa: E501
         """NotificationModel - a model defined in OpenAPI
 
+        Args:
+            notification_type (NotificationTypeModel):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -159,15 +162,14 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
             created_date (datetime, none_type): [optional]  # noqa: E501
             is_read (bool): [optional]  # noqa: E501
             entity_id (str): [optional]  # noqa: E501
-            notification_type (NotificationTypeModel): [optional]  # noqa: E501
             project_global_id (int, none_type): [optional]  # noqa: E501
             project_name (str, none_type): [optional]  # noqa: E501
             test_plan_global_id (int): [optional]  # noqa: E501
             test_plan_name (str, none_type): [optional]  # noqa: E501
             workitem_global_id (int, none_type): [optional]  # noqa: E501
             comment (str, none_type): [optional]  # noqa: E501
             work_item_name (str, none_type): [optional]  # noqa: E501
@@ -200,14 +202,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.notification_type = notification_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -220,17 +223,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, notification_type, *args, **kwargs):  # noqa: E501
         """NotificationModel - a model defined in OpenAPI
 
+        Args:
+            notification_type (NotificationTypeModel):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -258,15 +264,14 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
             created_date (datetime, none_type): [optional]  # noqa: E501
             is_read (bool): [optional]  # noqa: E501
             entity_id (str): [optional]  # noqa: E501
-            notification_type (NotificationTypeModel): [optional]  # noqa: E501
             project_global_id (int, none_type): [optional]  # noqa: E501
             project_name (str, none_type): [optional]  # noqa: E501
             test_plan_global_id (int): [optional]  # noqa: E501
             test_plan_name (str, none_type): [optional]  # noqa: E501
             workitem_global_id (int, none_type): [optional]  # noqa: E501
             comment (str, none_type): [optional]  # noqa: E501
             work_item_name (str, none_type): [optional]  # noqa: E501
@@ -297,14 +302,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.notification_type = notification_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/notification_query_filter_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/notification_query_filter_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/notification_type_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/notification_type_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/parameter_group_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_group_by_tester_and_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 
-class ParameterGroupModel(ModelNormal):
+class TestPlanGroupByTesterAndStatus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -71,39 +71,39 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'name': (str, none_type,),  # noqa: E501
-            'values': ({str: (str, none_type)}, none_type,),  # noqa: E501
-            'parameter_key_id': (str,),  # noqa: E501
+            'user_id': (str, none_type,),  # noqa: E501
+            'status': (str, none_type,),  # noqa: E501
+            'value': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'values': 'values',  # noqa: E501
-        'parameter_key_id': 'parameterKeyId',  # noqa: E501
+        'user_id': 'userId',  # noqa: E501
+        'status': 'status',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ParameterGroupModel - a model defined in OpenAPI
+        """TestPlanGroupByTesterAndStatus - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -128,17 +128,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str, none_type): [optional]  # noqa: E501
-            values ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
-            parameter_key_id (str): [optional]  # noqa: E501
+            user_id (str, none_type): [optional]  # noqa: E501
+            status (str, none_type): [optional]  # noqa: E501
+            value (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ParameterGroupModel - a model defined in OpenAPI
+        """TestPlanGroupByTesterAndStatus - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,17 +216,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str, none_type): [optional]  # noqa: E501
-            values ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
-            parameter_key_id (str): [optional]  # noqa: E501
+            user_id (str, none_type): [optional]  # noqa: E501
+            status (str, none_type): [optional]  # noqa: E501
+            value (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/parameter_iteration_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/parameter_iteration_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/parameter_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/parameter_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/parameter_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/parameter_post_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/parameter_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/parameter_put_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/parameter_short_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/parameter_short_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/period_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/period_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/period_view_model_test_plan_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/period_view_model_test_plan_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/problem_details.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/problem_details.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/project_attributes_filter_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/project_attributes_filter_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/project_custom_attribute_template_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/project_custom_attribute_template_get_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/project_custom_attributes_templates_filter_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/project_custom_attributes_templates_filter_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/project_export_query_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/project_export_query_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/project_export_with_test_plans_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/project_export_with_test_plans_post_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/project_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/project_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,17 +58,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('name',): {
-            'min_length': 1,
-        },
     }
 
     additional_properties_type = None
 
     _nullable = False
 
     @cached_property
@@ -80,69 +77,65 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
-            'name': (str,),  # noqa: E501
+            'description': (str, none_type,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
+            'is_favorite': (bool,),  # noqa: E501
             'attributes_scheme': ([CustomAttributeModel], none_type,),  # noqa: E501
             'test_plans_attributes_scheme': ([CustomAttributeModel], none_type,),  # noqa: E501
             'test_cases_count': (int, none_type,),  # noqa: E501
             'shared_steps_count': (int, none_type,),  # noqa: E501
             'check_lists_count': (int, none_type,),  # noqa: E501
             'auto_tests_count': (int, none_type,),  # noqa: E501
-            'is_favorite': (bool,),  # noqa: E501
             'is_deleted': (bool,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'modified_date': (datetime, none_type,),  # noqa: E501
             'created_by_id': (str,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
             'global_id': (int,),  # noqa: E501
-            'description': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
+        'description': 'description',  # noqa: E501
         'name': 'name',  # noqa: E501
+        'is_favorite': 'isFavorite',  # noqa: E501
         'attributes_scheme': 'attributesScheme',  # noqa: E501
         'test_plans_attributes_scheme': 'testPlansAttributesScheme',  # noqa: E501
         'test_cases_count': 'testCasesCount',  # noqa: E501
         'shared_steps_count': 'sharedStepsCount',  # noqa: E501
         'check_lists_count': 'checkListsCount',  # noqa: E501
         'auto_tests_count': 'autoTestsCount',  # noqa: E501
-        'is_favorite': 'isFavorite',  # noqa: E501
         'is_deleted': 'isDeleted',  # noqa: E501
         'created_date': 'createdDate',  # noqa: E501
         'modified_date': 'modifiedDate',  # noqa: E501
         'created_by_id': 'createdById',  # noqa: E501
         'modified_by_id': 'modifiedById',  # noqa: E501
         'global_id': 'globalId',  # noqa: E501
-        'description': 'description',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """ProjectModel - a model defined in OpenAPI
 
-        Args:
-            id (str): Unique ID of the project
-            name (str): Name of the project
-
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -166,28 +159,30 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            id (str): Unique ID of the project. [optional]  # noqa: E501
+            description (str, none_type): Description of the project. [optional]  # noqa: E501
+            name (str, none_type): Name of the project. [optional]  # noqa: E501
+            is_favorite (bool): Indicates if the project is marked as favorite. [optional]  # noqa: E501
             attributes_scheme ([CustomAttributeModel], none_type): Collection of the project attributes. [optional]  # noqa: E501
             test_plans_attributes_scheme ([CustomAttributeModel], none_type): Collection of the project test plans attributes. [optional]  # noqa: E501
             test_cases_count (int, none_type): Number of test cases in the project. [optional]  # noqa: E501
             shared_steps_count (int, none_type): Number of shared steps in the project. [optional]  # noqa: E501
             check_lists_count (int, none_type): Number of checklists in the project. [optional]  # noqa: E501
             auto_tests_count (int, none_type): Number of autotests in the project. [optional]  # noqa: E501
-            is_favorite (bool): Indicates if the project is marked as favorite. [optional]  # noqa: E501
             is_deleted (bool): Indicates if the project is deleted. [optional]  # noqa: E501
             created_date (datetime): Creation date of the project. [optional]  # noqa: E501
             modified_date (datetime, none_type): Last modification date of the project. [optional]  # noqa: E501
             created_by_id (str): Unique ID of the project creator. [optional]  # noqa: E501
             modified_by_id (str, none_type): Unique ID of the project last editor. [optional]  # noqa: E501
             global_id (int): Global ID of the project. [optional]  # noqa: E501
-            description (str, none_type): Description of the project. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -211,16 +206,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -233,21 +226,17 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, *args, **kwargs):  # noqa: E501
+    def __init__(self, *args, **kwargs):  # noqa: E501
         """ProjectModel - a model defined in OpenAPI
 
-        Args:
-            id (str): Unique ID of the project
-            name (str): Name of the project
-
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -271,28 +260,30 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            id (str): Unique ID of the project. [optional]  # noqa: E501
+            description (str, none_type): Description of the project. [optional]  # noqa: E501
+            name (str, none_type): Name of the project. [optional]  # noqa: E501
+            is_favorite (bool): Indicates if the project is marked as favorite. [optional]  # noqa: E501
             attributes_scheme ([CustomAttributeModel], none_type): Collection of the project attributes. [optional]  # noqa: E501
             test_plans_attributes_scheme ([CustomAttributeModel], none_type): Collection of the project test plans attributes. [optional]  # noqa: E501
             test_cases_count (int, none_type): Number of test cases in the project. [optional]  # noqa: E501
             shared_steps_count (int, none_type): Number of shared steps in the project. [optional]  # noqa: E501
             check_lists_count (int, none_type): Number of checklists in the project. [optional]  # noqa: E501
             auto_tests_count (int, none_type): Number of autotests in the project. [optional]  # noqa: E501
-            is_favorite (bool): Indicates if the project is marked as favorite. [optional]  # noqa: E501
             is_deleted (bool): Indicates if the project is deleted. [optional]  # noqa: E501
             created_date (datetime): Creation date of the project. [optional]  # noqa: E501
             modified_date (datetime, none_type): Last modification date of the project. [optional]  # noqa: E501
             created_by_id (str): Unique ID of the project creator. [optional]  # noqa: E501
             modified_by_id (str, none_type): Unique ID of the project last editor. [optional]  # noqa: E501
             global_id (int): Global ID of the project. [optional]  # noqa: E501
-            description (str, none_type): Description of the project. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -314,16 +305,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/project_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/project_post_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,24 +76,26 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'name': (str,),  # noqa: E501
             'description': (str, none_type,),  # noqa: E501
+            'is_favorite': (bool, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'description': 'description',  # noqa: E501
+        'is_favorite': 'isFavorite',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -133,14 +135,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str, none_type): Description of the project. [optional]  # noqa: E501
+            is_favorite (bool, none_type): Indicates if the project is marked as favorite. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -223,14 +226,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str, none_type): Description of the project. [optional]  # noqa: E501
+            is_favorite (bool, none_type): Indicates if the project is marked as favorite. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/project_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/project_put_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,25 +77,27 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'description': (str, none_type,),  # noqa: E501
+            'is_favorite': (bool, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
         'description': 'description',  # noqa: E501
+        'is_favorite': 'isFavorite',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -136,14 +138,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str, none_type): Description of the project. [optional]  # noqa: E501
+            is_favorite (bool, none_type): Indicates if the project is marked as favorite. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -228,14 +231,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str, none_type): Description of the project. [optional]  # noqa: E501
+            is_favorite (bool, none_type): Indicates if the project is marked as favorite. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/project_shortest_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/project_shortest_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/projects_filter_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/projects_filter_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/public_test_point_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/public_test_point_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/public_test_run_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/public_test_run_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/request_type_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/request_type_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/search_auto_tests_query_includes_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/search_auto_tests_query_includes_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/search_custom_attribute_template_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/search_custom_attribute_template_get_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/search_webhooks_query_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/search_webhooks_query_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/section_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/section_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/section_move_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/section_move_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/section_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/section_post_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/section_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/section_put_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/section_rename_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/section_rename_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/section_with_steps_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/section_with_steps_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/shared_step_change_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/shared_step_change_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/shared_step_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/shared_step_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/shared_step_reference_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/shared_step_reference_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,70 +78,73 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'priority': (WorkItemPriorityModel,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'global_id': (int,),  # noqa: E501
             'name': (str, none_type,),  # noqa: E501
             'entity_type_name': (str, none_type,),  # noqa: E501
             'has_this_shared_step_as_step': (bool,),  # noqa: E501
             'has_this_shared_step_as_precondition': (bool,),  # noqa: E501
             'has_this_shared_step_as_postcondition': (bool,),  # noqa: E501
             'created_by_id': (str,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
             'created_date': (datetime, none_type,),  # noqa: E501
             'modified_date': (datetime, none_type,),  # noqa: E501
             'state': (str, none_type,),  # noqa: E501
-            'priority': (WorkItemPriorityModel,),  # noqa: E501
             'is_deleted': (bool,),  # noqa: E501
             'version_id': (str,),  # noqa: E501
             'is_automated': (bool,),  # noqa: E501
             'section_id': (str,),  # noqa: E501
             'tags': ([TagShortModel], none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'priority': 'priority',  # noqa: E501
         'id': 'id',  # noqa: E501
         'global_id': 'globalId',  # noqa: E501
         'name': 'name',  # noqa: E501
         'entity_type_name': 'entityTypeName',  # noqa: E501
         'has_this_shared_step_as_step': 'hasThisSharedStepAsStep',  # noqa: E501
         'has_this_shared_step_as_precondition': 'hasThisSharedStepAsPrecondition',  # noqa: E501
         'has_this_shared_step_as_postcondition': 'hasThisSharedStepAsPostcondition',  # noqa: E501
         'created_by_id': 'createdById',  # noqa: E501
         'modified_by_id': 'modifiedById',  # noqa: E501
         'created_date': 'createdDate',  # noqa: E501
         'modified_date': 'modifiedDate',  # noqa: E501
         'state': 'state',  # noqa: E501
-        'priority': 'priority',  # noqa: E501
         'is_deleted': 'isDeleted',  # noqa: E501
         'version_id': 'versionId',  # noqa: E501
         'is_automated': 'isAutomated',  # noqa: E501
         'section_id': 'sectionId',  # noqa: E501
         'tags': 'tags',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, priority, *args, **kwargs):  # noqa: E501
         """SharedStepReferenceModel - a model defined in OpenAPI
 
+        Args:
+            priority (WorkItemPriorityModel):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -177,15 +180,14 @@
             has_this_shared_step_as_precondition (bool): [optional]  # noqa: E501
             has_this_shared_step_as_postcondition (bool): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             created_date (datetime, none_type): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             state (str, none_type): [optional]  # noqa: E501
-            priority (WorkItemPriorityModel): [optional]  # noqa: E501
             is_deleted (bool): [optional]  # noqa: E501
             version_id (str): used for versioning changes in workitem. [optional]  # noqa: E501
             is_automated (bool): [optional]  # noqa: E501
             section_id (str): [optional]  # noqa: E501
             tags ([TagShortModel], none_type): [optional]  # noqa: E501
         """
 
@@ -214,14 +216,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.priority = priority
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -234,17 +237,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, priority, *args, **kwargs):  # noqa: E501
         """SharedStepReferenceModel - a model defined in OpenAPI
 
+        Args:
+            priority (WorkItemPriorityModel):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -280,15 +286,14 @@
             has_this_shared_step_as_precondition (bool): [optional]  # noqa: E501
             has_this_shared_step_as_postcondition (bool): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             created_date (datetime, none_type): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             state (str, none_type): [optional]  # noqa: E501
-            priority (WorkItemPriorityModel): [optional]  # noqa: E501
             is_deleted (bool): [optional]  # noqa: E501
             version_id (str): used for versioning changes in workitem. [optional]  # noqa: E501
             is_automated (bool): [optional]  # noqa: E501
             section_id (str): [optional]  # noqa: E501
             tags ([TagShortModel], none_type): [optional]  # noqa: E501
         """
 
@@ -315,14 +320,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.priority = priority
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/shared_step_reference_section_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/shared_step_reference_section_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/shared_step_reference_sections_query_filter_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/shared_step_reference_sections_query_filter_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/shared_step_references_query_filter_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/shared_step_references_query_filter_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/shared_step_result_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_group_by_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 
-class SharedStepResultModel(ModelNormal):
+class TestPlanGroupByStatus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -71,37 +71,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'step_id': (str,),  # noqa: E501
-            'outcome': (str, none_type,),  # noqa: E501
+            'status': (str, none_type,),  # noqa: E501
+            'value': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'step_id': 'stepId',  # noqa: E501
-        'outcome': 'outcome',  # noqa: E501
+        'status': 'status',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SharedStepResultModel - a model defined in OpenAPI
+        """TestPlanGroupByStatus - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -126,16 +126,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            step_id (str): [optional]  # noqa: E501
-            outcome (str, none_type): [optional]  # noqa: E501
+            status (str, none_type): [optional]  # noqa: E501
+            value (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -180,15 +180,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SharedStepResultModel - a model defined in OpenAPI
+        """TestPlanGroupByStatus - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,16 +213,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            step_id (str): [optional]  # noqa: E501
-            outcome (str, none_type): [optional]  # noqa: E501
+            status (str, none_type): [optional]  # noqa: E501
+            value (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/short_configuration.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/short_configuration.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/step_comment_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/step_comment_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/step_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/step_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,16 +183,15 @@
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None or \
-                        var_value is None:
+                        self.additional_properties_type is None:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
         return self
 
     required_properties = set([
         '_data_store',
@@ -274,15 +273,14 @@
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None or \
-                        var_value is None:
+                        self.additional_properties_type is None:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
                                      f"class with read only attributes.")
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/step_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/step_put_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/step_result_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/step_result_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from testgear_api_client.model.shared_step_result_model import SharedStepResultModel
+    from testgear_api_client.model.step_comment_model import StepCommentModel
     globals()['SharedStepResultModel'] = SharedStepResultModel
+    globals()['StepCommentModel'] = StepCommentModel
 
 
 class StepResultModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -80,26 +82,28 @@
         """
         lazy_import()
         return {
             'step_id': (str,),  # noqa: E501
             'outcome': (str, none_type,),  # noqa: E501
             'shared_step_version_id': (str, none_type,),  # noqa: E501
             'shared_step_results': ([SharedStepResultModel], none_type,),  # noqa: E501
+            'comment': (StepCommentModel,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'step_id': 'stepId',  # noqa: E501
         'outcome': 'outcome',  # noqa: E501
         'shared_step_version_id': 'sharedStepVersionId',  # noqa: E501
         'shared_step_results': 'sharedStepResults',  # noqa: E501
+        'comment': 'comment',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -139,14 +143,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             step_id (str): [optional]  # noqa: E501
             outcome (str, none_type): [optional]  # noqa: E501
             shared_step_version_id (str, none_type): [optional]  # noqa: E501
             shared_step_results ([SharedStepResultModel], none_type): [optional]  # noqa: E501
+            comment (StepCommentModel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -228,14 +233,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             step_id (str): [optional]  # noqa: E501
             outcome (str, none_type): [optional]  # noqa: E501
             shared_step_version_id (str, none_type): [optional]  # noqa: E501
             shared_step_results ([SharedStepResultModel], none_type): [optional]  # noqa: E501
+            comment (StepCommentModel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/string_array_test_plan_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/string_array_test_plan_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/string_array_work_item_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/string_array_work_item_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/string_test_plan_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/string_test_plan_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/string_work_item_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/string_work_item_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/tag_short_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/tag_short_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_change_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_change_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_changed_fields_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_changed_fields_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_group_by_status.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_group_by_tester.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 
-class TestPlanGroupByStatus(ModelNormal):
+class TestPlanGroupByTester(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -71,37 +71,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'status': (str, none_type,),  # noqa: E501
+            'user_id': (str, none_type,),  # noqa: E501
             'value': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'status': 'status',  # noqa: E501
+        'user_id': 'userId',  # noqa: E501
         'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TestPlanGroupByStatus - a model defined in OpenAPI
+        """TestPlanGroupByTester - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -126,15 +126,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (str, none_type): [optional]  # noqa: E501
+            user_id (str, none_type): [optional]  # noqa: E501
             value (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -180,15 +180,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TestPlanGroupByStatus - a model defined in OpenAPI
+        """TestPlanGroupByTester - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,15 +213,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (str, none_type): [optional]  # noqa: E501
+            user_id (str, none_type): [optional]  # noqa: E501
             value (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_group_by_test_suite.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_group_by_test_suite.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_group_by_tester.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_chronology_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 
-class TestPlanGroupByTester(ModelNormal):
+class TestResultChronologyModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -71,37 +71,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'user_id': (str, none_type,),  # noqa: E501
-            'value': (int,),  # noqa: E501
+            'outcome': (str, none_type,),  # noqa: E501
+            'count': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'user_id': 'userId',  # noqa: E501
-        'value': 'value',  # noqa: E501
+        'outcome': 'outcome',  # noqa: E501
+        'count': 'count',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TestPlanGroupByTester - a model defined in OpenAPI
+        """TestResultChronologyModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -126,16 +126,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            user_id (str, none_type): [optional]  # noqa: E501
-            value (int): [optional]  # noqa: E501
+            outcome (str, none_type): [optional]  # noqa: E501
+            count (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -180,15 +180,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TestPlanGroupByTester - a model defined in OpenAPI
+        """TestResultChronologyModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,16 +213,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            user_id (str, none_type): [optional]  # noqa: E501
-            value (int): [optional]  # noqa: E501
+            outcome (str, none_type): [optional]  # noqa: E501
+            count (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_group_by_tester_and_status.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/background_job_attachment_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 
-class TestPlanGroupByTesterAndStatus(ModelNormal):
+class BackgroundJobAttachmentModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -71,39 +71,39 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'user_id': (str, none_type,),  # noqa: E501
-            'status': (str, none_type,),  # noqa: E501
-            'value': (int,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
+            'type': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'user_id': 'userId',  # noqa: E501
-        'status': 'status',  # noqa: E501
-        'value': 'value',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TestPlanGroupByTesterAndStatus - a model defined in OpenAPI
+        """BackgroundJobAttachmentModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -128,17 +128,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            user_id (str, none_type): [optional]  # noqa: E501
-            status (str, none_type): [optional]  # noqa: E501
-            value (int): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            name (str, none_type): [optional]  # noqa: E501
+            type (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TestPlanGroupByTesterAndStatus - a model defined in OpenAPI
+        """BackgroundJobAttachmentModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,17 +216,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            user_id (str, none_type): [optional]  # noqa: E501
-            status (str, none_type): [optional]  # noqa: E501
-            value (int): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            name (str, none_type): [optional]  # noqa: E501
+            type (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_link.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_link.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     validations = {
         ('name',): {
             'max_length': 450,
             'min_length': 0,
         },
         ('description',): {
-            'max_length': 999,
+            'max_length': 100000,
             'min_length': 0,
         },
         ('build',): {
             'max_length': 450,
             'min_length': 0,
         },
         ('product_name',): {
@@ -94,18 +94,18 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'status': (TestPlanStatusModel,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'project_id': (str,),  # noqa: E501
-            'status': (TestPlanStatusModel,),  # noqa: E501
             'started_on': (datetime, none_type,),  # noqa: E501
             'completed_on': (datetime, none_type,),  # noqa: E501
             'created_date': (datetime, none_type,),  # noqa: E501
             'modified_date': (datetime, none_type,),  # noqa: E501
             'created_by_id': (str,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
             'global_id': (int,),  # noqa: E501
@@ -124,18 +124,18 @@
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'status': 'status',  # noqa: E501
         'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
         'project_id': 'projectId',  # noqa: E501
-        'status': 'status',  # noqa: E501
         'started_on': 'startedOn',  # noqa: E501
         'completed_on': 'completedOn',  # noqa: E501
         'created_date': 'createdDate',  # noqa: E501
         'modified_date': 'modifiedDate',  # noqa: E501
         'created_by_id': 'createdById',  # noqa: E501
         'modified_by_id': 'modifiedById',  # noqa: E501
         'global_id': 'globalId',  # noqa: E501
@@ -155,18 +155,19 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, project_id, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, status, id, name, project_id, *args, **kwargs):  # noqa: E501
         """TestPlanModel - a model defined in OpenAPI
 
         Args:
+            status (TestPlanStatusModel):
             id (str):
             name (str):
             project_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -194,15 +195,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (TestPlanStatusModel): [optional]  # noqa: E501
             started_on (datetime, none_type): Set when test plan is starter (status changed to: In Progress). [optional]  # noqa: E501
             completed_on (datetime, none_type): set when test plan status is completed (status changed to: Completed). [optional]  # noqa: E501
             created_date (datetime, none_type): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             global_id (int): Used for search Test plan. [optional]  # noqa: E501
@@ -244,14 +244,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.status = status
         self.id = id
         self.name = name
         self.project_id = project_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
@@ -267,18 +268,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, project_id, *args, **kwargs):  # noqa: E501
+    def __init__(self, status, id, name, project_id, *args, **kwargs):  # noqa: E501
         """TestPlanModel - a model defined in OpenAPI
 
         Args:
+            status (TestPlanStatusModel):
             id (str):
             name (str):
             project_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -306,15 +308,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (TestPlanStatusModel): [optional]  # noqa: E501
             started_on (datetime, none_type): Set when test plan is starter (status changed to: In Progress). [optional]  # noqa: E501
             completed_on (datetime, none_type): set when test plan status is completed (status changed to: Completed). [optional]  # noqa: E501
             created_date (datetime, none_type): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             global_id (int): Used for search Test plan. [optional]  # noqa: E501
@@ -354,14 +355,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.status = status
         self.id = id
         self.name = name
         self.project_id = project_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_post_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     validations = {
         ('name',): {
             'max_length': 450,
             'min_length': 0,
         },
         ('description',): {
-            'max_length': 999,
+            'max_length': 100000,
             'min_length': 0,
         },
         ('build',): {
             'max_length': 450,
             'min_length': 0,
         },
         ('product_name',): {
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_put_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     validations = {
         ('name',): {
             'max_length': 450,
             'min_length': 0,
         },
         ('description',): {
-            'max_length': 999,
+            'max_length': 100000,
             'min_length': 0,
         },
         ('build',): {
             'max_length': 450,
             'min_length': 0,
         },
         ('product_name',): {
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_search_query_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/project_test_plans_filter_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from testgear_api_client.model.date_range_model import DateRangeModel
+    from testgear_api_client.model.date_time_range_selector_model import DateTimeRangeSelectorModel
     from testgear_api_client.model.test_plan_status_model import TestPlanStatusModel
-    globals()['DateRangeModel'] = DateRangeModel
+    globals()['DateTimeRangeSelectorModel'] = DateTimeRangeSelectorModel
     globals()['TestPlanStatusModel'] = TestPlanStatusModel
 
 
-class TestPlanSearchQueryModel(ModelNormal):
+class ProjectTestPlansFilterModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,23 +62,27 @@
 
     allowed_values = {
     }
 
     validations = {
         ('name',): {
             'max_length': 255,
+            'min_length': 0,
         },
         ('description',): {
             'max_length': 255,
+            'min_length': 0,
         },
         ('build',): {
             'max_length': 255,
+            'min_length': 0,
         },
         ('product_name',): {
             'max_length': 255,
+            'min_length': 0,
         },
         ('status',): {
         },
         ('global_ids',): {
         },
         ('automatic_duration_timer',): {
         },
@@ -107,20 +111,20 @@
             'name': (str, none_type,),  # noqa: E501
             'description': (str, none_type,),  # noqa: E501
             'build': (str, none_type,),  # noqa: E501
             'product_name': (str, none_type,),  # noqa: E501
             'status': ([TestPlanStatusModel], none_type,),  # noqa: E501
             'global_ids': ([int], none_type,),  # noqa: E501
             'is_locked': (bool, none_type,),  # noqa: E501
-            'locked_date': (DateRangeModel,),  # noqa: E501
+            'locked_date': (DateTimeRangeSelectorModel,),  # noqa: E501
             'automatic_duration_timer': ([bool], none_type,),  # noqa: E501
             'created_by_ids': ([str], none_type,),  # noqa: E501
-            'created_date': (DateRangeModel,),  # noqa: E501
-            'start_date': (DateRangeModel,),  # noqa: E501
-            'end_date': (DateRangeModel,),  # noqa: E501
+            'created_date': (DateTimeRangeSelectorModel,),  # noqa: E501
+            'start_date': (DateTimeRangeSelectorModel,),  # noqa: E501
+            'end_date': (DateTimeRangeSelectorModel,),  # noqa: E501
             'tag_names': ([str], none_type,),  # noqa: E501
             'attributes': ({str: ([str], none_type)}, none_type,),  # noqa: E501
             'is_deleted': (bool, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -150,15 +154,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TestPlanSearchQueryModel - a model defined in OpenAPI
+        """ProjectTestPlansFilterModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -190,20 +194,20 @@
             name (str, none_type): [optional]  # noqa: E501
             description (str, none_type): [optional]  # noqa: E501
             build (str, none_type): [optional]  # noqa: E501
             product_name (str, none_type): [optional]  # noqa: E501
             status ([TestPlanStatusModel], none_type): [optional]  # noqa: E501
             global_ids ([int], none_type): [optional]  # noqa: E501
             is_locked (bool, none_type): [optional]  # noqa: E501
-            locked_date (DateRangeModel): [optional]  # noqa: E501
+            locked_date (DateTimeRangeSelectorModel): [optional]  # noqa: E501
             automatic_duration_timer ([bool], none_type): [optional]  # noqa: E501
             created_by_ids ([str], none_type): [optional]  # noqa: E501
-            created_date (DateRangeModel): [optional]  # noqa: E501
-            start_date (DateRangeModel): [optional]  # noqa: E501
-            end_date (DateRangeModel): [optional]  # noqa: E501
+            created_date (DateTimeRangeSelectorModel): [optional]  # noqa: E501
+            start_date (DateTimeRangeSelectorModel): [optional]  # noqa: E501
+            end_date (DateTimeRangeSelectorModel): [optional]  # noqa: E501
             tag_names ([str], none_type): [optional]  # noqa: E501
             attributes ({str: ([str], none_type)}, none_type): [optional]  # noqa: E501
             is_deleted (bool, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
@@ -251,15 +255,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TestPlanSearchQueryModel - a model defined in OpenAPI
+        """ProjectTestPlansFilterModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -291,20 +295,20 @@
             name (str, none_type): [optional]  # noqa: E501
             description (str, none_type): [optional]  # noqa: E501
             build (str, none_type): [optional]  # noqa: E501
             product_name (str, none_type): [optional]  # noqa: E501
             status ([TestPlanStatusModel], none_type): [optional]  # noqa: E501
             global_ids ([int], none_type): [optional]  # noqa: E501
             is_locked (bool, none_type): [optional]  # noqa: E501
-            locked_date (DateRangeModel): [optional]  # noqa: E501
+            locked_date (DateTimeRangeSelectorModel): [optional]  # noqa: E501
             automatic_duration_timer ([bool], none_type): [optional]  # noqa: E501
             created_by_ids ([str], none_type): [optional]  # noqa: E501
-            created_date (DateRangeModel): [optional]  # noqa: E501
-            start_date (DateRangeModel): [optional]  # noqa: E501
-            end_date (DateRangeModel): [optional]  # noqa: E501
+            created_date (DateTimeRangeSelectorModel): [optional]  # noqa: E501
+            start_date (DateTimeRangeSelectorModel): [optional]  # noqa: E501
+            end_date (DateTimeRangeSelectorModel): [optional]  # noqa: E501
             tag_names ([str], none_type): [optional]  # noqa: E501
             attributes ({str: ([str], none_type)}, none_type): [optional]  # noqa: E501
             is_deleted (bool, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_short_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_short_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_status_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_status_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_with_analytic_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_with_analytic_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     validations = {
         ('name',): {
             'max_length': 450,
             'min_length': 0,
         },
         ('description',): {
-            'max_length': 999,
+            'max_length': 100000,
             'min_length': 0,
         },
         ('build',): {
             'max_length': 450,
             'min_length': 0,
         },
         ('product_name',): {
@@ -96,19 +96,19 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'status': (TestPlanStatusModel,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'project_id': (str,),  # noqa: E501
             'analytic': (TestPointAnalyticResult,),  # noqa: E501
-            'status': (TestPlanStatusModel,),  # noqa: E501
             'started_on': (datetime, none_type,),  # noqa: E501
             'completed_on': (datetime, none_type,),  # noqa: E501
             'created_date': (datetime, none_type,),  # noqa: E501
             'modified_date': (datetime, none_type,),  # noqa: E501
             'created_by_id': (str,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
             'global_id': (int,),  # noqa: E501
@@ -127,19 +127,19 @@
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'status': 'status',  # noqa: E501
         'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
         'project_id': 'projectId',  # noqa: E501
         'analytic': 'analytic',  # noqa: E501
-        'status': 'status',  # noqa: E501
         'started_on': 'startedOn',  # noqa: E501
         'completed_on': 'completedOn',  # noqa: E501
         'created_date': 'createdDate',  # noqa: E501
         'modified_date': 'modifiedDate',  # noqa: E501
         'created_by_id': 'createdById',  # noqa: E501
         'modified_by_id': 'modifiedById',  # noqa: E501
         'global_id': 'globalId',  # noqa: E501
@@ -159,18 +159,19 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, project_id, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, status, id, name, project_id, *args, **kwargs):  # noqa: E501
         """TestPlanWithAnalyticModel - a model defined in OpenAPI
 
         Args:
+            status (TestPlanStatusModel):
             id (str):
             name (str):
             project_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -199,15 +200,14 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             analytic (TestPointAnalyticResult): [optional]  # noqa: E501
-            status (TestPlanStatusModel): [optional]  # noqa: E501
             started_on (datetime, none_type): Set when test plan is starter (status changed to: In Progress). [optional]  # noqa: E501
             completed_on (datetime, none_type): set when test plan status is completed (status changed to: Completed). [optional]  # noqa: E501
             created_date (datetime, none_type): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             global_id (int): Used for search Test plan. [optional]  # noqa: E501
@@ -249,14 +249,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.status = status
         self.id = id
         self.name = name
         self.project_id = project_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
@@ -272,18 +273,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, project_id, *args, **kwargs):  # noqa: E501
+    def __init__(self, status, id, name, project_id, *args, **kwargs):  # noqa: E501
         """TestPlanWithAnalyticModel - a model defined in OpenAPI
 
         Args:
+            status (TestPlanStatusModel):
             id (str):
             name (str):
             project_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -312,15 +314,14 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             analytic (TestPointAnalyticResult): [optional]  # noqa: E501
-            status (TestPlanStatusModel): [optional]  # noqa: E501
             started_on (datetime, none_type): Set when test plan is starter (status changed to: In Progress). [optional]  # noqa: E501
             completed_on (datetime, none_type): set when test plan status is completed (status changed to: Completed). [optional]  # noqa: E501
             created_date (datetime, none_type): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             global_id (int): Used for search Test plan. [optional]  # noqa: E501
@@ -360,14 +361,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.status = status
         self.id = id
         self.name = name
         self.project_id = project_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_plan_with_test_suite_tree_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_plan_with_test_suite_tree_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     validations = {
         ('name',): {
             'max_length': 450,
             'min_length': 0,
         },
         ('description',): {
-            'max_length': 999,
+            'max_length': 100000,
             'min_length': 0,
         },
         ('build',): {
             'max_length': 450,
             'min_length': 0,
         },
         ('product_name',): {
@@ -96,19 +96,19 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'status': (TestPlanStatusModel,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'project_id': (str,),  # noqa: E501
             'test_suites': ([TestSuiteWithChildrenModel], none_type,),  # noqa: E501
-            'status': (TestPlanStatusModel,),  # noqa: E501
             'started_on': (datetime, none_type,),  # noqa: E501
             'completed_on': (datetime, none_type,),  # noqa: E501
             'created_date': (datetime, none_type,),  # noqa: E501
             'modified_date': (datetime, none_type,),  # noqa: E501
             'created_by_id': (str,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
             'global_id': (int,),  # noqa: E501
@@ -127,19 +127,19 @@
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'status': 'status',  # noqa: E501
         'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
         'project_id': 'projectId',  # noqa: E501
         'test_suites': 'testSuites',  # noqa: E501
-        'status': 'status',  # noqa: E501
         'started_on': 'startedOn',  # noqa: E501
         'completed_on': 'completedOn',  # noqa: E501
         'created_date': 'createdDate',  # noqa: E501
         'modified_date': 'modifiedDate',  # noqa: E501
         'created_by_id': 'createdById',  # noqa: E501
         'modified_by_id': 'modifiedById',  # noqa: E501
         'global_id': 'globalId',  # noqa: E501
@@ -159,18 +159,19 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, project_id, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, status, id, name, project_id, *args, **kwargs):  # noqa: E501
         """TestPlanWithTestSuiteTreeModel - a model defined in OpenAPI
 
         Args:
+            status (TestPlanStatusModel):
             id (str):
             name (str):
             project_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -199,15 +200,14 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             test_suites ([TestSuiteWithChildrenModel], none_type): [optional]  # noqa: E501
-            status (TestPlanStatusModel): [optional]  # noqa: E501
             started_on (datetime, none_type): Set when test plan is starter (status changed to: In Progress). [optional]  # noqa: E501
             completed_on (datetime, none_type): set when test plan status is completed (status changed to: Completed). [optional]  # noqa: E501
             created_date (datetime, none_type): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             global_id (int): Used for search Test plan. [optional]  # noqa: E501
@@ -249,14 +249,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.status = status
         self.id = id
         self.name = name
         self.project_id = project_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
@@ -272,18 +273,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, project_id, *args, **kwargs):  # noqa: E501
+    def __init__(self, status, id, name, project_id, *args, **kwargs):  # noqa: E501
         """TestPlanWithTestSuiteTreeModel - a model defined in OpenAPI
 
         Args:
+            status (TestPlanStatusModel):
             id (str):
             name (str):
             project_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -312,15 +314,14 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             test_suites ([TestSuiteWithChildrenModel], none_type): [optional]  # noqa: E501
-            status (TestPlanStatusModel): [optional]  # noqa: E501
             started_on (datetime, none_type): Set when test plan is starter (status changed to: In Progress). [optional]  # noqa: E501
             completed_on (datetime, none_type): set when test plan status is completed (status changed to: Completed). [optional]  # noqa: E501
             created_date (datetime, none_type): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             global_id (int): Used for search Test plan. [optional]  # noqa: E501
@@ -360,14 +361,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.status = status
         self.id = id
         self.name = name
         self.project_id = project_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_analytic_result.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_analytic_result.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_by_test_suite_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_by_test_suite_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_change_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_change_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_change_view_model_test_plan_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_change_view_model_test_plan_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_filter_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_filter_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,16 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('test_plan_ids',): {
+        },
         ('test_suite_ids',): {
         },
         ('work_item_global_ids',): {
         },
         ('statuses',): {
         },
         ('priorities',): {
@@ -106,14 +108,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'test_plan_ids': ([str], none_type,),  # noqa: E501
             'test_suite_ids': ([str], none_type,),  # noqa: E501
             'work_item_global_ids': ([int], none_type,),  # noqa: E501
             'statuses': ([TestPointStatus], none_type,),  # noqa: E501
             'priorities': ([WorkItemPriorityModel], none_type,),  # noqa: E501
             'is_automated': (bool, none_type,),  # noqa: E501
             'name': (str, none_type,),  # noqa: E501
             'configuration_ids': ([str], none_type,),  # noqa: E501
@@ -130,14 +133,15 @@
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'test_plan_ids': 'testPlanIds',  # noqa: E501
         'test_suite_ids': 'testSuiteIds',  # noqa: E501
         'work_item_global_ids': 'workItemGlobalIds',  # noqa: E501
         'statuses': 'statuses',  # noqa: E501
         'priorities': 'priorities',  # noqa: E501
         'is_automated': 'isAutomated',  # noqa: E501
         'name': 'name',  # noqa: E501
         'configuration_ids': 'configurationIds',  # noqa: E501
@@ -189,14 +193,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            test_plan_ids ([str], none_type): Specifies a test point test plan IDS to search for. [optional]  # noqa: E501
             test_suite_ids ([str], none_type): Specifies a test point test suite IDs to search for. [optional]  # noqa: E501
             work_item_global_ids ([int], none_type): Specifies a test point work item global IDs to search for. [optional]  # noqa: E501
             statuses ([TestPointStatus], none_type): Specifies a test point statuses to search for. [optional]  # noqa: E501
             priorities ([WorkItemPriorityModel], none_type): Specifies a test point priorities to search for. [optional]  # noqa: E501
             is_automated (bool, none_type): Specifies a test point automation status to search for. [optional]  # noqa: E501
             name (str, none_type): Specifies a test point name to search for. [optional]  # noqa: E501
             configuration_ids ([str], none_type): Specifies a test point configuration IDs to search for. [optional]  # noqa: E501
@@ -290,14 +295,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            test_plan_ids ([str], none_type): Specifies a test point test plan IDS to search for. [optional]  # noqa: E501
             test_suite_ids ([str], none_type): Specifies a test point test suite IDs to search for. [optional]  # noqa: E501
             work_item_global_ids ([int], none_type): Specifies a test point work item global IDs to search for. [optional]  # noqa: E501
             statuses ([TestPointStatus], none_type): Specifies a test point statuses to search for. [optional]  # noqa: E501
             priorities ([WorkItemPriorityModel], none_type): Specifies a test point priorities to search for. [optional]  # noqa: E501
             is_automated (bool, none_type): Specifies a test point automation status to search for. [optional]  # noqa: E501
             name (str, none_type): Specifies a test point name to search for. [optional]  # noqa: E501
             configuration_ids ([str], none_type): Specifies a test point configuration IDs to search for. [optional]  # noqa: E501
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_put_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_result_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_result_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_selector.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,40 +72,40 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'configuration_id': (str,),  # noqa: E501
-            'workitem_ids': ([str],),  # noqa: E501
+            'work_item_ids': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'configuration_id': 'configurationId',  # noqa: E501
-        'workitem_ids': 'workitemIds',  # noqa: E501
+        'work_item_ids': 'workItemIds',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, configuration_id, workitem_ids, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, configuration_id, work_item_ids, *args, **kwargs):  # noqa: E501
         """TestPointSelector - a model defined in OpenAPI
 
         Args:
             configuration_id (str): Specifies the configuration GUIDs, from which test points are created. You can specify several GUIDs.
-            workitem_ids ([str]): Specifies the work item GUIDs, from which test points are created. You can specify several GUIDs.
+            work_item_ids ([str]): Specifies the work item GUIDs, from which test points are created. You can specify several GUIDs.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -162,15 +162,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.configuration_id = configuration_id
-        self.workitem_ids = workitem_ids
+        self.work_item_ids = work_item_ids
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -183,20 +183,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, configuration_id, workitem_ids, *args, **kwargs):  # noqa: E501
+    def __init__(self, configuration_id, work_item_ids, *args, **kwargs):  # noqa: E501
         """TestPointSelector - a model defined in OpenAPI
 
         Args:
             configuration_id (str): Specifies the configuration GUIDs, from which test points are created. You can specify several GUIDs.
-            workitem_ids ([str]): Specifies the work item GUIDs, from which test points are created. You can specify several GUIDs.
+            work_item_ids ([str]): Specifies the work item GUIDs, from which test points are created. You can specify several GUIDs.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -251,15 +251,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.configuration_id = configuration_id
-        self.workitem_ids = workitem_ids
+        self.work_item_ids = work_item_ids
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_short_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_short_get_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,80 +80,89 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'status': (TestPointStatus,),  # noqa: E501
+            'priority': (WorkItemPriorityModel,),  # noqa: E501
+            'last_test_result': (LastTestResultModel,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'created_by_id': (str,),  # noqa: E501
             'modified_date': (datetime, none_type,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
             'tester_id': (str, none_type,),  # noqa: E501
-            'parameters': ({str: (str, none_type)}, none_type,),  # noqa: E501
+            'parameters': ({str: (str,)}, none_type,),  # noqa: E501
             'attributes': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'tags': ([str], none_type,),  # noqa: E501
             'links': ([str], none_type,),  # noqa: E501
             'test_suite_id': (str,),  # noqa: E501
+            'work_item_id': (str,),  # noqa: E501
             'work_item_global_id': (int,),  # noqa: E501
             'work_item_version_id': (str,),  # noqa: E501
-            'status': (TestPointStatus,),  # noqa: E501
-            'priority': (WorkItemPriorityModel,),  # noqa: E501
             'is_automated': (bool,),  # noqa: E501
             'name': (str, none_type,),  # noqa: E501
             'configuration_id': (str,),  # noqa: E501
             'duration': (int,),  # noqa: E501
             'section_id': (str,),  # noqa: E501
+            'section_name': (str, none_type,),  # noqa: E501
             'project_id': (str,),  # noqa: E501
-            'last_test_result': (LastTestResultModel,),  # noqa: E501
             'iteration_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'status': 'status',  # noqa: E501
+        'priority': 'priority',  # noqa: E501
+        'last_test_result': 'lastTestResult',  # noqa: E501
         'id': 'id',  # noqa: E501
         'created_date': 'createdDate',  # noqa: E501
         'created_by_id': 'createdById',  # noqa: E501
         'modified_date': 'modifiedDate',  # noqa: E501
         'modified_by_id': 'modifiedById',  # noqa: E501
         'tester_id': 'testerId',  # noqa: E501
         'parameters': 'parameters',  # noqa: E501
         'attributes': 'attributes',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'links': 'links',  # noqa: E501
         'test_suite_id': 'testSuiteId',  # noqa: E501
+        'work_item_id': 'workItemId',  # noqa: E501
         'work_item_global_id': 'workItemGlobalId',  # noqa: E501
         'work_item_version_id': 'workItemVersionId',  # noqa: E501
-        'status': 'status',  # noqa: E501
-        'priority': 'priority',  # noqa: E501
         'is_automated': 'isAutomated',  # noqa: E501
         'name': 'name',  # noqa: E501
         'configuration_id': 'configurationId',  # noqa: E501
         'duration': 'duration',  # noqa: E501
         'section_id': 'sectionId',  # noqa: E501
+        'section_name': 'sectionName',  # noqa: E501
         'project_id': 'projectId',  # noqa: E501
-        'last_test_result': 'lastTestResult',  # noqa: E501
         'iteration_id': 'iterationId',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, status, priority, last_test_result, *args, **kwargs):  # noqa: E501
         """TestPointShortGetModel - a model defined in OpenAPI
 
+        Args:
+            status (TestPointStatus):
+            priority (WorkItemPriorityModel):
+            last_test_result (LastTestResultModel):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -183,30 +192,29 @@
                                 _visited_composed_classes = (Animal,)
             id (str): Unique ID of the test point. [optional]  # noqa: E501
             created_date (datetime): Creation date of the test point. [optional]  # noqa: E501
             created_by_id (str): Unique ID of the test point creator. [optional]  # noqa: E501
             modified_date (datetime, none_type): Last modification date of the test point. [optional]  # noqa: E501
             modified_by_id (str, none_type): Unique ID of the test point last editor. [optional]  # noqa: E501
             tester_id (str, none_type): Unique ID of the test point assigned user. [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): Collection of the test point parameters. [optional]  # noqa: E501
+            parameters ({str: (str,)}, none_type): Collection of the test point parameters. [optional]  # noqa: E501
             attributes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Collection of attributes of work item the test point represents. [optional]  # noqa: E501
             tags ([str], none_type): Collection of the test point tags. [optional]  # noqa: E501
             links ([str], none_type): Collection of the test point links. [optional]  # noqa: E501
             test_suite_id (str): Unique ID of test suite the test point assigned to. [optional]  # noqa: E501
+            work_item_id (str): Unique ID of work item the test point represents. [optional]  # noqa: E501
             work_item_global_id (int): Global ID of work item the test point represents. [optional]  # noqa: E501
             work_item_version_id (str): Unique ID of work item version the test point represents. [optional]  # noqa: E501
-            status (TestPointStatus): [optional]  # noqa: E501
-            priority (WorkItemPriorityModel): [optional]  # noqa: E501
             is_automated (bool): Indicates if the test point represents an autotest. [optional]  # noqa: E501
             name (str, none_type): Name of the test point. [optional]  # noqa: E501
             configuration_id (str): Unique ID of the test point configuration. [optional]  # noqa: E501
             duration (int): Duration of the test point. [optional]  # noqa: E501
             section_id (str): Unique ID of section where work item the test point represents is located. [optional]  # noqa: E501
+            section_name (str, none_type): Name of section where work item the test point represents is located. [optional]  # noqa: E501
             project_id (str): Unique ID of the test point project. [optional]  # noqa: E501
-            last_test_result (LastTestResultModel): [optional]  # noqa: E501
             iteration_id (str): Unique ID of work item iteration the test point represents. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -231,14 +239,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.status = status
+        self.priority = priority
+        self.last_test_result = last_test_result
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -251,17 +262,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, status, priority, last_test_result, *args, **kwargs):  # noqa: E501
         """TestPointShortGetModel - a model defined in OpenAPI
 
+        Args:
+            status (TestPointStatus):
+            priority (WorkItemPriorityModel):
+            last_test_result (LastTestResultModel):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -291,30 +307,29 @@
                                 _visited_composed_classes = (Animal,)
             id (str): Unique ID of the test point. [optional]  # noqa: E501
             created_date (datetime): Creation date of the test point. [optional]  # noqa: E501
             created_by_id (str): Unique ID of the test point creator. [optional]  # noqa: E501
             modified_date (datetime, none_type): Last modification date of the test point. [optional]  # noqa: E501
             modified_by_id (str, none_type): Unique ID of the test point last editor. [optional]  # noqa: E501
             tester_id (str, none_type): Unique ID of the test point assigned user. [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): Collection of the test point parameters. [optional]  # noqa: E501
+            parameters ({str: (str,)}, none_type): Collection of the test point parameters. [optional]  # noqa: E501
             attributes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Collection of attributes of work item the test point represents. [optional]  # noqa: E501
             tags ([str], none_type): Collection of the test point tags. [optional]  # noqa: E501
             links ([str], none_type): Collection of the test point links. [optional]  # noqa: E501
             test_suite_id (str): Unique ID of test suite the test point assigned to. [optional]  # noqa: E501
+            work_item_id (str): Unique ID of work item the test point represents. [optional]  # noqa: E501
             work_item_global_id (int): Global ID of work item the test point represents. [optional]  # noqa: E501
             work_item_version_id (str): Unique ID of work item version the test point represents. [optional]  # noqa: E501
-            status (TestPointStatus): [optional]  # noqa: E501
-            priority (WorkItemPriorityModel): [optional]  # noqa: E501
             is_automated (bool): Indicates if the test point represents an autotest. [optional]  # noqa: E501
             name (str, none_type): Name of the test point. [optional]  # noqa: E501
             configuration_id (str): Unique ID of the test point configuration. [optional]  # noqa: E501
             duration (int): Duration of the test point. [optional]  # noqa: E501
             section_id (str): Unique ID of section where work item the test point represents is located. [optional]  # noqa: E501
+            section_name (str, none_type): Name of section where work item the test point represents is located. [optional]  # noqa: E501
             project_id (str): Unique ID of the test point project. [optional]  # noqa: E501
-            last_test_result (LastTestResultModel): [optional]  # noqa: E501
             iteration_id (str): Unique ID of work item iteration the test point represents. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -337,14 +352,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.status = status
+        self.priority = priority
+        self.last_test_result = last_test_result
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_short_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_short_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_status.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_status.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_point_with_last_result_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_point_with_last_result_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'priority': (WorkItemPriorityModel,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'work_item_name': (str, none_type,),  # noqa: E501
             'is_automated': (bool,),  # noqa: E501
             'tester_id': (str, none_type,),  # noqa: E501
             'work_item_id': (str,),  # noqa: E501
             'configuration_id': (str, none_type,),  # noqa: E501
             'test_suite_id': (str,),  # noqa: E501
@@ -100,26 +101,26 @@
             'created_date': (datetime, none_type,),  # noqa: E501
             'modified_date': (datetime, none_type,),  # noqa: E501
             'created_by_id': (str,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
             'attributes': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'tag_names': ([str], none_type,),  # noqa: E501
             'duration': (int,),  # noqa: E501
-            'priority': (WorkItemPriorityModel,),  # noqa: E501
             'test_suite_name_bread_crumbs': ([str], none_type,),  # noqa: E501
             'group_count': (int, none_type,),  # noqa: E501
             'iteration': (IterationModel,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'priority': 'priority',  # noqa: E501
         'id': 'id',  # noqa: E501
         'work_item_name': 'workItemName',  # noqa: E501
         'is_automated': 'isAutomated',  # noqa: E501
         'tester_id': 'testerId',  # noqa: E501
         'work_item_id': 'workItemId',  # noqa: E501
         'configuration_id': 'configurationId',  # noqa: E501
         'test_suite_id': 'testSuiteId',  # noqa: E501
@@ -132,30 +133,32 @@
         'created_date': 'createdDate',  # noqa: E501
         'modified_date': 'modifiedDate',  # noqa: E501
         'created_by_id': 'createdById',  # noqa: E501
         'modified_by_id': 'modifiedById',  # noqa: E501
         'attributes': 'attributes',  # noqa: E501
         'tag_names': 'tagNames',  # noqa: E501
         'duration': 'duration',  # noqa: E501
-        'priority': 'priority',  # noqa: E501
         'test_suite_name_bread_crumbs': 'testSuiteNameBreadCrumbs',  # noqa: E501
         'group_count': 'groupCount',  # noqa: E501
         'iteration': 'iteration',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, priority, *args, **kwargs):  # noqa: E501
         """TestPointWithLastResultModel - a model defined in OpenAPI
 
+        Args:
+            priority (WorkItemPriorityModel):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -199,15 +202,14 @@
             created_date (datetime, none_type): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             attributes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
             tag_names ([str], none_type): [optional]  # noqa: E501
             duration (int): [optional]  # noqa: E501
-            priority (WorkItemPriorityModel): [optional]  # noqa: E501
             test_suite_name_bread_crumbs ([str], none_type): [optional]  # noqa: E501
             group_count (int, none_type): [optional]  # noqa: E501
             iteration (IterationModel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
@@ -234,14 +236,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.priority = priority
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -254,17 +257,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, priority, *args, **kwargs):  # noqa: E501
         """TestPointWithLastResultModel - a model defined in OpenAPI
 
+        Args:
+            priority (WorkItemPriorityModel):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -308,15 +314,14 @@
             created_date (datetime, none_type): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             attributes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
             tag_names ([str], none_type): [optional]  # noqa: E501
             duration (int): [optional]  # noqa: E501
-            priority (WorkItemPriorityModel): [optional]  # noqa: E501
             test_suite_name_bread_crumbs ([str], none_type): [optional]  # noqa: E501
             group_count (int, none_type): [optional]  # noqa: E501
             iteration (IterationModel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -341,14 +346,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.priority = priority
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_change_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_change_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_change_view_model_test_plan_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_change_view_model_test_plan_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_chronology_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_v2_put_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 
-class TestResultChronologyModel(ModelNormal):
+class TestSuiteV2PutModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -54,14 +54,18 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('name',): {
+            'max_length': 255,
+            'min_length': 0,
+        },
     }
 
     additional_properties_type = None
 
     _nullable = False
 
     @cached_property
@@ -71,37 +75,45 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'outcome': (str, none_type,),  # noqa: E501
-            'count': (int,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'parent_id': (str, none_type,),  # noqa: E501
+            'is_deleted': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'outcome': 'outcome',  # noqa: E501
-        'count': 'count',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'parent_id': 'parentId',  # noqa: E501
+        'is_deleted': 'isDeleted',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TestResultChronologyModel - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, name, *args, **kwargs):  # noqa: E501
+        """TestSuiteV2PutModel - a model defined in OpenAPI
+
+        Args:
+            id (str):
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -126,16 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            outcome (str, none_type): [optional]  # noqa: E501
-            count (int): [optional]  # noqa: E501
+            parent_id (str, none_type): [optional]  # noqa: E501
+            is_deleted (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -159,14 +171,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -179,16 +193,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """TestResultChronologyModel - a model defined in OpenAPI
+    def __init__(self, id, name, *args, **kwargs):  # noqa: E501
+        """TestSuiteV2PutModel - a model defined in OpenAPI
+
+        Args:
+            id (str):
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,16 +231,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            outcome (str, none_type): [optional]  # noqa: E501
-            count (int): [optional]  # noqa: E501
+            parent_id (str, none_type): [optional]  # noqa: E501
+            is_deleted (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -244,14 +262,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_history_report_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_history_report_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             'created_by_id': (str,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
             'attachments': ([AttachmentModel], none_type,),  # noqa: E501
             'work_item_version_id': (str, none_type,),  # noqa: E501
             'work_item_version_number': (int, none_type,),  # noqa: E501
             'launch_source': (str, none_type,),  # noqa: E501
             'failure_class_ids': ([str], none_type,),  # noqa: E501
-            'parameters': ({str: (str, none_type)}, none_type,),  # noqa: E501
+            'parameters': ({str: (str,)}, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -206,15 +206,15 @@
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             attachments ([AttachmentModel], none_type): If any test result related to the test run is linked with autotest, attachments will be equal to the attachments of last modified test result.Otherwise, the attachments equals to the attachments of first created test result in the test run. [optional]  # noqa: E501
             work_item_version_id (str, none_type): [optional]  # noqa: E501
             work_item_version_number (int, none_type): [optional]  # noqa: E501
             launch_source (str, none_type): [optional]  # noqa: E501
             failure_class_ids ([str], none_type): [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
+            parameters ({str: (str,)}, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -317,15 +317,15 @@
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             attachments ([AttachmentModel], none_type): If any test result related to the test run is linked with autotest, attachments will be equal to the attachments of last modified test result.Otherwise, the attachments equals to the attachments of first created test result in the test run. [optional]  # noqa: E501
             work_item_version_id (str, none_type): [optional]  # noqa: E501
             work_item_version_number (int, none_type): [optional]  # noqa: E501
             launch_source (str, none_type): [optional]  # noqa: E501
             failure_class_ids ([str], none_type): [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
+            parameters ({str: (str,)}, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,16 +107,16 @@
             'test_point': (TestPointPutModel,),  # noqa: E501
             'auto_test': (AutoTestModel,),  # noqa: E501
             'auto_test_step_results': ([AttachmentModelAutoTestStepResultsModel], none_type,),  # noqa: E501
             'setup_results': ([AttachmentModelAutoTestStepResultsModel], none_type,),  # noqa: E501
             'teardown_results': ([AttachmentModelAutoTestStepResultsModel], none_type,),  # noqa: E501
             'work_item_version_id': (str,),  # noqa: E501
             'work_item_version_number': (int, none_type,),  # noqa: E501
-            'parameters': ({str: (str, none_type)}, none_type,),  # noqa: E501
-            'properties': ({str: (str, none_type)}, none_type,),  # noqa: E501
+            'parameters': ({str: (str,)}, none_type,),  # noqa: E501
+            'properties': ({str: (str,)}, none_type,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'modified_date': (datetime, none_type,),  # noqa: E501
             'created_by_id': (str,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
             'step_comments': ([StepCommentModel], none_type,),  # noqa: E501
             'failure_class_ids': ([str], none_type,),  # noqa: E501
@@ -224,16 +224,16 @@
             test_point (TestPointPutModel): [optional]  # noqa: E501
             auto_test (AutoTestModel): [optional]  # noqa: E501
             auto_test_step_results ([AttachmentModelAutoTestStepResultsModel], none_type): [optional]  # noqa: E501
             setup_results ([AttachmentModelAutoTestStepResultsModel], none_type): [optional]  # noqa: E501
             teardown_results ([AttachmentModelAutoTestStepResultsModel], none_type): [optional]  # noqa: E501
             work_item_version_id (str): [optional]  # noqa: E501
             work_item_version_number (int, none_type): [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
-            properties ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
+            parameters ({str: (str,)}, none_type): [optional]  # noqa: E501
+            properties ({str: (str,)}, none_type): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             created_date (datetime): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             step_comments ([StepCommentModel], none_type): [optional]  # noqa: E501
             failure_class_ids ([str], none_type): [optional]  # noqa: E501
@@ -342,16 +342,16 @@
             test_point (TestPointPutModel): [optional]  # noqa: E501
             auto_test (AutoTestModel): [optional]  # noqa: E501
             auto_test_step_results ([AttachmentModelAutoTestStepResultsModel], none_type): [optional]  # noqa: E501
             setup_results ([AttachmentModelAutoTestStepResultsModel], none_type): [optional]  # noqa: E501
             teardown_results ([AttachmentModelAutoTestStepResultsModel], none_type): [optional]  # noqa: E501
             work_item_version_id (str): [optional]  # noqa: E501
             work_item_version_number (int, none_type): [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
-            properties ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
+            parameters ({str: (str,)}, none_type): [optional]  # noqa: E501
+            properties ({str: (str,)}, none_type): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             created_date (datetime): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             step_comments ([StepCommentModel], none_type): [optional]  # noqa: E501
             failure_class_ids ([str], none_type): [optional]  # noqa: E501
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_outcome.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_outcome.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_short_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_short_get_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,42 +82,42 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'outcome': (TestResultOutcome,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'name': (str, none_type,),  # noqa: E501
             'autotest_global_id': (int,),  # noqa: E501
             'test_run_id': (str,),  # noqa: E501
             'configuration_id': (str,),  # noqa: E501
             'configuration_name': (str, none_type,),  # noqa: E501
-            'outcome': (TestResultOutcome,),  # noqa: E501
             'result_reasons': ([AutotestResultReasonSubGetModel], none_type,),  # noqa: E501
             'comment': (str, none_type,),  # noqa: E501
             'date': (datetime,),  # noqa: E501
             'duration': (int, none_type,),  # noqa: E501
             'links': ([LinkSubGetModel], none_type,),  # noqa: E501
             'attachments': ([AttachmentSubGetModel], none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'outcome': 'outcome',  # noqa: E501
         'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
         'autotest_global_id': 'autotestGlobalId',  # noqa: E501
         'test_run_id': 'testRunId',  # noqa: E501
         'configuration_id': 'configurationId',  # noqa: E501
         'configuration_name': 'configurationName',  # noqa: E501
-        'outcome': 'outcome',  # noqa: E501
         'result_reasons': 'resultReasons',  # noqa: E501
         'comment': 'comment',  # noqa: E501
         'date': 'date',  # noqa: E501
         'duration': 'duration',  # noqa: E501
         'links': 'links',  # noqa: E501
         'attachments': 'attachments',  # noqa: E501
     }
@@ -125,17 +125,20 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, outcome, *args, **kwargs):  # noqa: E501
         """TestResultShortGetModel - a model defined in OpenAPI
 
+        Args:
+            outcome (TestResultOutcome):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -165,15 +168,14 @@
                                 _visited_composed_classes = (Animal,)
             id (str): Unique ID of test result. [optional]  # noqa: E501
             name (str, none_type): Name of autotest represented by the test result. [optional]  # noqa: E501
             autotest_global_id (int): Global ID of autotest represented by test result. [optional]  # noqa: E501
             test_run_id (str): Unique ID of test run where test result is located. [optional]  # noqa: E501
             configuration_id (str): Unique ID of configuration which test result uses. [optional]  # noqa: E501
             configuration_name (str, none_type): Name of configuration which test result uses. [optional]  # noqa: E501
-            outcome (TestResultOutcome): [optional]  # noqa: E501
             result_reasons ([AutotestResultReasonSubGetModel], none_type): Collection of result reasons which test result have. [optional]  # noqa: E501
             comment (str, none_type): Comment to test result. [optional]  # noqa: E501
             date (datetime): Date when test result has been set. [optional]  # noqa: E501
             duration (int, none_type): Time which it took to run the test. [optional]  # noqa: E501
             links ([LinkSubGetModel], none_type): Collection of links attached to test result. [optional]  # noqa: E501
             attachments ([AttachmentSubGetModel], none_type): Collection of files attached to test result. [optional]  # noqa: E501
         """
@@ -203,14 +205,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.outcome = outcome
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -223,17 +226,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, outcome, *args, **kwargs):  # noqa: E501
         """TestResultShortGetModel - a model defined in OpenAPI
 
+        Args:
+            outcome (TestResultOutcome):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -263,15 +269,14 @@
                                 _visited_composed_classes = (Animal,)
             id (str): Unique ID of test result. [optional]  # noqa: E501
             name (str, none_type): Name of autotest represented by the test result. [optional]  # noqa: E501
             autotest_global_id (int): Global ID of autotest represented by test result. [optional]  # noqa: E501
             test_run_id (str): Unique ID of test run where test result is located. [optional]  # noqa: E501
             configuration_id (str): Unique ID of configuration which test result uses. [optional]  # noqa: E501
             configuration_name (str, none_type): Name of configuration which test result uses. [optional]  # noqa: E501
-            outcome (TestResultOutcome): [optional]  # noqa: E501
             result_reasons ([AutotestResultReasonSubGetModel], none_type): Collection of result reasons which test result have. [optional]  # noqa: E501
             comment (str, none_type): Comment to test result. [optional]  # noqa: E501
             date (datetime): Date when test result has been set. [optional]  # noqa: E501
             duration (int, none_type): Time which it took to run the test. [optional]  # noqa: E501
             links ([LinkSubGetModel], none_type): Collection of links attached to test result. [optional]  # noqa: E501
             attachments ([AttachmentSubGetModel], none_type): Collection of files attached to test result. [optional]  # noqa: E501
         """
@@ -299,14 +304,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.outcome = outcome
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_short_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_short_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_step_comment_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_step_comment_put_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_update_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_update_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_v2_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_v2_get_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,16 +103,16 @@
             'test_point_id': (str, none_type,),  # noqa: E501
             'test_point': (TestPointShortModel,),  # noqa: E501
             'test_run_id': (str,),  # noqa: E501
             'outcome': (str, none_type,),  # noqa: E501
             'comment': (str, none_type,),  # noqa: E501
             'links': ([LinkModel], none_type,),  # noqa: E501
             'attachments': ([AttachmentModel], none_type,),  # noqa: E501
-            'parameters': ({str: (str, none_type)}, none_type,),  # noqa: E501
-            'properties': ({str: (str, none_type)}, none_type,),  # noqa: E501
+            'parameters': ({str: (str,)}, none_type,),  # noqa: E501
+            'properties': ({str: (str,)}, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -196,16 +196,16 @@
             test_point_id (str, none_type): [optional]  # noqa: E501
             test_point (TestPointShortModel): [optional]  # noqa: E501
             test_run_id (str): [optional]  # noqa: E501
             outcome (str, none_type): Property can contain one of these values: Passed, Failed, InProgress, Blocked, Skipped. [optional]  # noqa: E501
             comment (str, none_type): [optional]  # noqa: E501
             links ([LinkModel], none_type): [optional]  # noqa: E501
             attachments ([AttachmentModel], none_type): [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
-            properties ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
+            parameters ({str: (str,)}, none_type): [optional]  # noqa: E501
+            properties ({str: (str,)}, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -233,16 +233,15 @@
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None or \
-                        var_value is None:
+                        self.additional_properties_type is None:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
         return self
 
     required_properties = set([
         '_data_store',
@@ -303,16 +302,16 @@
             test_point_id (str, none_type): [optional]  # noqa: E501
             test_point (TestPointShortModel): [optional]  # noqa: E501
             test_run_id (str): [optional]  # noqa: E501
             outcome (str, none_type): Property can contain one of these values: Passed, Failed, InProgress, Blocked, Skipped. [optional]  # noqa: E501
             comment (str, none_type): [optional]  # noqa: E501
             links ([LinkModel], none_type): [optional]  # noqa: E501
             attachments ([AttachmentModel], none_type): [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
-            properties ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
+            parameters ({str: (str,)}, none_type): [optional]  # noqa: E501
+            properties ({str: (str,)}, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -338,15 +337,14 @@
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None or \
-                        var_value is None:
+                        self.additional_properties_type is None:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
                                      f"class with read only attributes.")
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_result_v2_short_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_result_v2_short_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,16 +97,16 @@
             'test_point_id': (str, none_type,),  # noqa: E501
             'test_point': (TestPointShortModel,),  # noqa: E501
             'test_run_id': (str,),  # noqa: E501
             'outcome': (str, none_type,),  # noqa: E501
             'comment': (str, none_type,),  # noqa: E501
             'links': ([LinkModel], none_type,),  # noqa: E501
             'attachments': ([AttachmentModel], none_type,),  # noqa: E501
-            'parameters': ({str: (str, none_type)}, none_type,),  # noqa: E501
-            'properties': ({str: (str, none_type)}, none_type,),  # noqa: E501
+            'parameters': ({str: (str,)}, none_type,),  # noqa: E501
+            'properties': ({str: (str,)}, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -186,16 +186,16 @@
             test_point_id (str, none_type): [optional]  # noqa: E501
             test_point (TestPointShortModel): [optional]  # noqa: E501
             test_run_id (str): [optional]  # noqa: E501
             outcome (str, none_type): Property can contain one of these values: Passed, Failed, InProgress, Blocked, Skipped. [optional]  # noqa: E501
             comment (str, none_type): [optional]  # noqa: E501
             links ([LinkModel], none_type): [optional]  # noqa: E501
             attachments ([AttachmentModel], none_type): [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
-            properties ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
+            parameters ({str: (str,)}, none_type): [optional]  # noqa: E501
+            properties ({str: (str,)}, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -290,16 +290,16 @@
             test_point_id (str, none_type): [optional]  # noqa: E501
             test_point (TestPointShortModel): [optional]  # noqa: E501
             test_run_id (str): [optional]  # noqa: E501
             outcome (str, none_type): Property can contain one of these values: Passed, Failed, InProgress, Blocked, Skipped. [optional]  # noqa: E501
             comment (str, none_type): [optional]  # noqa: E501
             links ([LinkModel], none_type): [optional]  # noqa: E501
             attachments ([AttachmentModel], none_type): [optional]  # noqa: E501
-            parameters ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
-            properties ({str: (str, none_type)}, none_type): [optional]  # noqa: E501
+            parameters ({str: (str,)}, none_type): [optional]  # noqa: E501
+            properties ({str: (str,)}, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_results_filter_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_results_filter_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_results_local_filter_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_results_local_filter_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_results_statistics_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_results_statistics_get_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_analytic_result_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_analytic_result_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_fill_by_auto_tests_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_fill_by_auto_tests_post_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_fill_by_configurations_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_fill_by_configurations_post_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_fill_by_work_items_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_fill_by_work_items_post_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,50 +72,50 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'configuration_ids': ([str],),  # noqa: E501
-            'workitem_ids': ([str],),  # noqa: E501
+            'work_item_ids': ([str],),  # noqa: E501
             'project_id': (str,),  # noqa: E501
             'test_plan_id': (str,),  # noqa: E501
             'name': (str, none_type,),  # noqa: E501
             'description': (str, none_type,),  # noqa: E501
             'launch_source': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'configuration_ids': 'configurationIds',  # noqa: E501
-        'workitem_ids': 'workitemIds',  # noqa: E501
+        'work_item_ids': 'workItemIds',  # noqa: E501
         'project_id': 'projectId',  # noqa: E501
         'test_plan_id': 'testPlanId',  # noqa: E501
         'name': 'name',  # noqa: E501
         'description': 'description',  # noqa: E501
         'launch_source': 'launchSource',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, configuration_ids, workitem_ids, project_id, test_plan_id, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, configuration_ids, work_item_ids, project_id, test_plan_id, *args, **kwargs):  # noqa: E501
         """TestRunFillByWorkItemsPostModel - a model defined in OpenAPI
 
         Args:
             configuration_ids ([str]): Specifies the configuration GUIDs, from which test points are created. You can specify several GUIDs.
-            workitem_ids ([str]): Specifies the work item GUIDs, from which test points are created. You can specify several GUIDs.
+            work_item_ids ([str]): Specifies the work item GUIDs, from which test points are created. You can specify several GUIDs.
             project_id (str): Specifies the GUID of the project, in which a test run will be created.
             test_plan_id (str): Specifies the GUID of the test plan, within which the test run will be created.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -177,15 +177,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.configuration_ids = configuration_ids
-        self.workitem_ids = workitem_ids
+        self.work_item_ids = work_item_ids
         self.project_id = project_id
         self.test_plan_id = test_plan_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
@@ -200,20 +200,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, configuration_ids, workitem_ids, project_id, test_plan_id, *args, **kwargs):  # noqa: E501
+    def __init__(self, configuration_ids, work_item_ids, project_id, test_plan_id, *args, **kwargs):  # noqa: E501
         """TestRunFillByWorkItemsPostModel - a model defined in OpenAPI
 
         Args:
             configuration_ids ([str]): Specifies the configuration GUIDs, from which test points are created. You can specify several GUIDs.
-            workitem_ids ([str]): Specifies the work item GUIDs, from which test points are created. You can specify several GUIDs.
+            work_item_ids ([str]): Specifies the work item GUIDs, from which test points are created. You can specify several GUIDs.
             project_id (str): Specifies the GUID of the project, in which a test run will be created.
             test_plan_id (str): Specifies the GUID of the test plan, within which the test run will be created.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -273,15 +273,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.configuration_ids = configuration_ids
-        self.workitem_ids = workitem_ids
+        self.work_item_ids = work_item_ids
         self.project_id = project_id
         self.test_plan_id = test_plan_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_filter_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_filter_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_group_by_failure_class_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_group_by_failure_class_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_group_by_status_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_group_by_status_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'state_name': (TestRunState,),  # noqa: E501
             'auto_tests': ([AutoTestModel], none_type,),  # noqa: E501
             'auto_tests_count': (int,),  # noqa: E501
             'test_suite_ids': ([str], none_type,),  # noqa: E501
             'is_automated': (bool,),  # noqa: E501
             'analytic': (TestRunAnalyticResultModel,),  # noqa: E501
             'test_results': ([TestResultModel], none_type,),  # noqa: E501
             'test_plan': (TestPlanModel,),  # noqa: E501
@@ -104,15 +105,14 @@
             'created_by_id': (str,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
             'created_by_user_name': (str, none_type,),  # noqa: E501
             'started_date': (datetime, none_type,),  # noqa: E501
             'completed_date': (datetime, none_type,),  # noqa: E501
             'build': (str, none_type,),  # noqa: E501
             'description': (str, none_type,),  # noqa: E501
-            'state_name': (TestRunState,),  # noqa: E501
             'project_id': (str,),  # noqa: E501
             'test_plan_id': (str, none_type,),  # noqa: E501
             'run_by_user_id': (str, none_type,),  # noqa: E501
             'stopped_by_user_id': (str, none_type,),  # noqa: E501
             'name': (str, none_type,),  # noqa: E501
             'launch_source': (str, none_type,),  # noqa: E501
             'id': (str,),  # noqa: E501
@@ -121,14 +121,15 @@
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'state_name': 'stateName',  # noqa: E501
         'auto_tests': 'autoTests',  # noqa: E501
         'auto_tests_count': 'autoTestsCount',  # noqa: E501
         'test_suite_ids': 'testSuiteIds',  # noqa: E501
         'is_automated': 'isAutomated',  # noqa: E501
         'analytic': 'analytic',  # noqa: E501
         'test_results': 'testResults',  # noqa: E501
         'test_plan': 'testPlan',  # noqa: E501
@@ -137,15 +138,14 @@
         'created_by_id': 'createdById',  # noqa: E501
         'modified_by_id': 'modifiedById',  # noqa: E501
         'created_by_user_name': 'createdByUserName',  # noqa: E501
         'started_date': 'startedDate',  # noqa: E501
         'completed_date': 'completedDate',  # noqa: E501
         'build': 'build',  # noqa: E501
         'description': 'description',  # noqa: E501
-        'state_name': 'stateName',  # noqa: E501
         'project_id': 'projectId',  # noqa: E501
         'test_plan_id': 'testPlanId',  # noqa: E501
         'run_by_user_id': 'runByUserId',  # noqa: E501
         'stopped_by_user_id': 'stoppedByUserId',  # noqa: E501
         'name': 'name',  # noqa: E501
         'launch_source': 'launchSource',  # noqa: E501
         'id': 'id',  # noqa: E501
@@ -155,17 +155,20 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, state_name, *args, **kwargs):  # noqa: E501
         """TestRunModel - a model defined in OpenAPI
 
+        Args:
+            state_name (TestRunState):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -205,15 +208,14 @@
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             created_by_user_name (str, none_type): [optional]  # noqa: E501
             started_date (datetime, none_type): [optional]  # noqa: E501
             completed_date (datetime, none_type): [optional]  # noqa: E501
             build (str, none_type): [optional]  # noqa: E501
             description (str, none_type): [optional]  # noqa: E501
-            state_name (TestRunState): [optional]  # noqa: E501
             project_id (str): [optional]  # noqa: E501
             test_plan_id (str, none_type): [optional]  # noqa: E501
             run_by_user_id (str, none_type): [optional]  # noqa: E501
             stopped_by_user_id (str, none_type): [optional]  # noqa: E501
             name (str, none_type): [optional]  # noqa: E501
             launch_source (str, none_type): [optional]  # noqa: E501
             id (str): Unique ID of the entity. [optional]  # noqa: E501
@@ -245,14 +247,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.state_name = state_name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -265,17 +268,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, state_name, *args, **kwargs):  # noqa: E501
         """TestRunModel - a model defined in OpenAPI
 
+        Args:
+            state_name (TestRunState):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -315,15 +321,14 @@
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             created_by_user_name (str, none_type): [optional]  # noqa: E501
             started_date (datetime, none_type): [optional]  # noqa: E501
             completed_date (datetime, none_type): [optional]  # noqa: E501
             build (str, none_type): [optional]  # noqa: E501
             description (str, none_type): [optional]  # noqa: E501
-            state_name (TestRunState): [optional]  # noqa: E501
             project_id (str): [optional]  # noqa: E501
             test_plan_id (str, none_type): [optional]  # noqa: E501
             run_by_user_id (str, none_type): [optional]  # noqa: E501
             stopped_by_user_id (str, none_type): [optional]  # noqa: E501
             name (str, none_type): [optional]  # noqa: E501
             launch_source (str, none_type): [optional]  # noqa: E501
             id (str): Unique ID of the entity. [optional]  # noqa: E501
@@ -353,14 +358,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.state_name = state_name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_search_query_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_search_query_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_short_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_v2_get_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from testgear_api_client.model.test_results_statistics_get_model import TestResultsStatisticsGetModel
+    from testgear_api_client.model.test_result_v2_get_model import TestResultV2GetModel
     from testgear_api_client.model.test_run_state import TestRunState
-    globals()['TestResultsStatisticsGetModel'] = TestResultsStatisticsGetModel
+    globals()['TestResultV2GetModel'] = TestResultV2GetModel
     globals()['TestRunState'] = TestRunState
 
 
-class TestRunShortGetModel(ModelNormal):
+class TestRunV2GetModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -60,14 +60,17 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('name',): {
+            'min_length': 1,
+        },
     }
 
     additional_properties_type = None
 
     _nullable = False
 
     @cached_property
@@ -78,57 +81,68 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'state_name': (TestRunState,),  # noqa: E501
             'id': (str,),  # noqa: E501
-            'name': (str, none_type,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'started_on': (datetime, none_type,),  # noqa: E501
+            'completed_on': (datetime, none_type,),  # noqa: E501
             'project_id': (str,),  # noqa: E501
+            'test_plan_id': (str, none_type,),  # noqa: E501
+            'test_results': ([TestResultV2GetModel], none_type,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
-            'created_by_id': (str,),  # noqa: E501
             'modified_date': (datetime, none_type,),  # noqa: E501
+            'created_by_id': (str,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
-            'is_deleted': (bool,),  # noqa: E501
-            'state': (TestRunState,),  # noqa: E501
-            'started_date': (datetime, none_type,),  # noqa: E501
-            'autotests_count': (int,),  # noqa: E501
-            'statistics': (TestResultsStatisticsGetModel,),  # noqa: E501
+            'created_by_user_name': (str, none_type,),  # noqa: E501
+            'description': (str, none_type,),  # noqa: E501
+            'launch_source': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'state_name': 'stateName',  # noqa: E501
         'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
+        'started_on': 'startedOn',  # noqa: E501
+        'completed_on': 'completedOn',  # noqa: E501
         'project_id': 'projectId',  # noqa: E501
+        'test_plan_id': 'testPlanId',  # noqa: E501
+        'test_results': 'testResults',  # noqa: E501
         'created_date': 'createdDate',  # noqa: E501
-        'created_by_id': 'createdById',  # noqa: E501
         'modified_date': 'modifiedDate',  # noqa: E501
+        'created_by_id': 'createdById',  # noqa: E501
         'modified_by_id': 'modifiedById',  # noqa: E501
-        'is_deleted': 'isDeleted',  # noqa: E501
-        'state': 'state',  # noqa: E501
-        'started_date': 'startedDate',  # noqa: E501
-        'autotests_count': 'autotestsCount',  # noqa: E501
-        'statistics': 'statistics',  # noqa: E501
+        'created_by_user_name': 'createdByUserName',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'launch_source': 'launchSource',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TestRunShortGetModel - a model defined in OpenAPI
+    def _from_openapi_data(cls, state_name, id, name, *args, **kwargs):  # noqa: E501
+        """TestRunV2GetModel - a model defined in OpenAPI
+
+        Args:
+            state_name (TestRunState):
+            id (str):
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -153,26 +167,26 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): Unique ID of the test run. [optional]  # noqa: E501
-            name (str, none_type): Name of the test run. [optional]  # noqa: E501
-            project_id (str): Unique ID of project where test run is located. [optional]  # noqa: E501
-            created_date (datetime): Date when the test run was created. [optional]  # noqa: E501
-            created_by_id (str): Unique ID of user who created the test run. [optional]  # noqa: E501
-            modified_date (datetime, none_type): Date when the test run was modified last time. [optional]  # noqa: E501
-            modified_by_id (str, none_type): Unique ID of user who modified the test run last time. [optional]  # noqa: E501
-            is_deleted (bool): Is the test run is deleted. [optional]  # noqa: E501
-            state (TestRunState): [optional]  # noqa: E501
-            started_date (datetime, none_type): Date when the test run was started. [optional]  # noqa: E501
-            autotests_count (int): Number of autotests run in the test run. [optional]  # noqa: E501
-            statistics (TestResultsStatisticsGetModel): [optional]  # noqa: E501
+            started_on (datetime, none_type): [optional]  # noqa: E501
+            completed_on (datetime, none_type): [optional]  # noqa: E501
+            project_id (str): This property is used to link test run with project. [optional]  # noqa: E501
+            test_plan_id (str, none_type): This property is used to link test run with test plan. [optional]  # noqa: E501
+            test_results ([TestResultV2GetModel], none_type): [optional]  # noqa: E501
+            created_date (datetime): [optional]  # noqa: E501
+            modified_date (datetime, none_type): [optional]  # noqa: E501
+            created_by_id (str): [optional]  # noqa: E501
+            modified_by_id (str, none_type): [optional]  # noqa: E501
+            created_by_user_name (str, none_type): [optional]  # noqa: E501
+            description (str, none_type): [optional]  # noqa: E501
+            launch_source (str, none_type): Once launch source is specified it cannot be updated. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -196,14 +210,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.state_name = state_name
+        self.id = id
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -216,16 +233,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """TestRunShortGetModel - a model defined in OpenAPI
+    def __init__(self, state_name, id, name, *args, **kwargs):  # noqa: E501
+        """TestRunV2GetModel - a model defined in OpenAPI
+
+        Args:
+            state_name (TestRunState):
+            id (str):
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -250,26 +272,26 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): Unique ID of the test run. [optional]  # noqa: E501
-            name (str, none_type): Name of the test run. [optional]  # noqa: E501
-            project_id (str): Unique ID of project where test run is located. [optional]  # noqa: E501
-            created_date (datetime): Date when the test run was created. [optional]  # noqa: E501
-            created_by_id (str): Unique ID of user who created the test run. [optional]  # noqa: E501
-            modified_date (datetime, none_type): Date when the test run was modified last time. [optional]  # noqa: E501
-            modified_by_id (str, none_type): Unique ID of user who modified the test run last time. [optional]  # noqa: E501
-            is_deleted (bool): Is the test run is deleted. [optional]  # noqa: E501
-            state (TestRunState): [optional]  # noqa: E501
-            started_date (datetime, none_type): Date when the test run was started. [optional]  # noqa: E501
-            autotests_count (int): Number of autotests run in the test run. [optional]  # noqa: E501
-            statistics (TestResultsStatisticsGetModel): [optional]  # noqa: E501
+            started_on (datetime, none_type): [optional]  # noqa: E501
+            completed_on (datetime, none_type): [optional]  # noqa: E501
+            project_id (str): This property is used to link test run with project. [optional]  # noqa: E501
+            test_plan_id (str, none_type): This property is used to link test run with test plan. [optional]  # noqa: E501
+            test_results ([TestResultV2GetModel], none_type): [optional]  # noqa: E501
+            created_date (datetime): [optional]  # noqa: E501
+            modified_date (datetime, none_type): [optional]  # noqa: E501
+            created_by_id (str): [optional]  # noqa: E501
+            modified_by_id (str, none_type): [optional]  # noqa: E501
+            created_by_user_name (str, none_type): [optional]  # noqa: E501
+            description (str, none_type): [optional]  # noqa: E501
+            launch_source (str, none_type): Once launch source is specified it cannot be updated. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -291,14 +313,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.state_name = state_name
+        self.id = id
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_short_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_short_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,17 +107,20 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, state_name, *args, **kwargs):  # noqa: E501
         """TestRunShortModel - a model defined in OpenAPI
 
+        Args:
+            state_name (TestRunState):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -141,15 +144,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            state_name (TestRunState): [optional]  # noqa: E501
             project_id (str): [optional]  # noqa: E501
             test_plan_id (str, none_type): [optional]  # noqa: E501
             name (str, none_type): [optional]  # noqa: E501
             description (str, none_type): [optional]  # noqa: E501
             id (str): Unique ID of the entity. [optional]  # noqa: E501
             is_deleted (bool): Indicates if the entity is deleted. [optional]  # noqa: E501
         """
@@ -179,14 +181,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.state_name = state_name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -199,17 +202,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, state_name, *args, **kwargs):  # noqa: E501
         """TestRunShortModel - a model defined in OpenAPI
 
+        Args:
+            state_name (TestRunState):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -233,15 +239,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            state_name (TestRunState): [optional]  # noqa: E501
             project_id (str): [optional]  # noqa: E501
             test_plan_id (str, none_type): [optional]  # noqa: E501
             name (str, none_type): [optional]  # noqa: E501
             description (str, none_type): [optional]  # noqa: E501
             id (str): Unique ID of the entity. [optional]  # noqa: E501
             is_deleted (bool): Indicates if the entity is deleted. [optional]  # noqa: E501
         """
@@ -269,14 +274,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.state_name = state_name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_state.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_state.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_statistics_error_categories_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_statistics_error_categories_get_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_statistics_statuses_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_statistics_statuses_get_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_test_results_partial_bulk_set_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_test_results_partial_bulk_set_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_test_results_select_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_test_results_select_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_v2_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_short_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,21 +26,23 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from testgear_api_client.model.test_result_v2_get_model import TestResultV2GetModel
-    from testgear_api_client.model.test_run_state import TestRunState
-    globals()['TestResultV2GetModel'] = TestResultV2GetModel
-    globals()['TestRunState'] = TestRunState
+    from testgear_api_client.model.iteration_model import IterationModel
+    from testgear_api_client.model.work_item_priority_model import WorkItemPriorityModel
+    from testgear_api_client.model.work_item_states import WorkItemStates
+    globals()['IterationModel'] = IterationModel
+    globals()['WorkItemPriorityModel'] = WorkItemPriorityModel
+    globals()['WorkItemStates'] = WorkItemStates
 
 
-class TestRunV2GetModel(ModelNormal):
+class WorkItemShortModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +65,20 @@
     allowed_values = {
     }
 
     validations = {
         ('name',): {
             'min_length': 1,
         },
+        ('entity_type_name',): {
+            'min_length': 1,
+        },
+        ('section_name',): {
+            'min_length': 1,
+        },
     }
 
     additional_properties_type = None
 
     _nullable = False
 
     @cached_property
@@ -81,67 +89,82 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
-            'started_on': (datetime, none_type,),  # noqa: E501
-            'completed_on': (datetime, none_type,),  # noqa: E501
-            'state_name': (TestRunState,),  # noqa: E501
+            'entity_type_name': (str,),  # noqa: E501
             'project_id': (str,),  # noqa: E501
-            'test_plan_id': (str, none_type,),  # noqa: E501
-            'test_results': ([TestResultV2GetModel], none_type,),  # noqa: E501
-            'created_date': (datetime,),  # noqa: E501
-            'modified_date': (datetime, none_type,),  # noqa: E501
+            'section_id': (str,),  # noqa: E501
+            'section_name': (str,),  # noqa: E501
+            'state': (WorkItemStates,),  # noqa: E501
+            'priority': (WorkItemPriorityModel,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'version_id': (str,),  # noqa: E501
+            'is_automated': (bool,),  # noqa: E501
+            'global_id': (int,),  # noqa: E501
+            'duration': (int,),  # noqa: E501
+            'attributes': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'created_by_id': (str,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
-            'created_by_user_name': (str, none_type,),  # noqa: E501
-            'description': (str, none_type,),  # noqa: E501
-            'launch_source': (str, none_type,),  # noqa: E501
+            'created_date': (datetime, none_type,),  # noqa: E501
+            'modified_date': (datetime, none_type,),  # noqa: E501
+            'is_deleted': (bool,),  # noqa: E501
+            'tag_names': ([str], none_type,),  # noqa: E501
+            'iterations': ([IterationModel], none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'started_on': 'startedOn',  # noqa: E501
-        'completed_on': 'completedOn',  # noqa: E501
-        'state_name': 'stateName',  # noqa: E501
+        'entity_type_name': 'entityTypeName',  # noqa: E501
         'project_id': 'projectId',  # noqa: E501
-        'test_plan_id': 'testPlanId',  # noqa: E501
-        'test_results': 'testResults',  # noqa: E501
-        'created_date': 'createdDate',  # noqa: E501
-        'modified_date': 'modifiedDate',  # noqa: E501
+        'section_id': 'sectionId',  # noqa: E501
+        'section_name': 'sectionName',  # noqa: E501
+        'state': 'state',  # noqa: E501
+        'priority': 'priority',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'version_id': 'versionId',  # noqa: E501
+        'is_automated': 'isAutomated',  # noqa: E501
+        'global_id': 'globalId',  # noqa: E501
+        'duration': 'duration',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
         'created_by_id': 'createdById',  # noqa: E501
         'modified_by_id': 'modifiedById',  # noqa: E501
-        'created_by_user_name': 'createdByUserName',  # noqa: E501
-        'description': 'description',  # noqa: E501
-        'launch_source': 'launchSource',  # noqa: E501
+        'created_date': 'createdDate',  # noqa: E501
+        'modified_date': 'modifiedDate',  # noqa: E501
+        'is_deleted': 'isDeleted',  # noqa: E501
+        'tag_names': 'tagNames',  # noqa: E501
+        'iterations': 'iterations',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, *args, **kwargs):  # noqa: E501
-        """TestRunV2GetModel - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, entity_type_name, project_id, section_id, section_name, state, priority, *args, **kwargs):  # noqa: E501
+        """WorkItemShortModel - a model defined in OpenAPI
 
         Args:
-            id (str):
             name (str):
+            entity_type_name (str): Property can have one of these values: CheckLists, SharedSteps, TestCases
+            project_id (str): This property is used to link autotest with project
+            section_id (str): This property links workitem with section
+            section_name (str): Name of the section where work item is located
+            state (WorkItemStates):
+            priority (WorkItemPriorityModel):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -166,27 +189,27 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            started_on (datetime, none_type): [optional]  # noqa: E501
-            completed_on (datetime, none_type): [optional]  # noqa: E501
-            state_name (TestRunState): [optional]  # noqa: E501
-            project_id (str): This property is used to link test run with project. [optional]  # noqa: E501
-            test_plan_id (str, none_type): This property is used to link test run with test plan. [optional]  # noqa: E501
-            test_results ([TestResultV2GetModel], none_type): [optional]  # noqa: E501
-            created_date (datetime): [optional]  # noqa: E501
-            modified_date (datetime, none_type): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            version_id (str): used for versioning changes in workitem. [optional]  # noqa: E501
+            is_automated (bool): [optional]  # noqa: E501
+            global_id (int): [optional]  # noqa: E501
+            duration (int): [optional]  # noqa: E501
+            attributes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
-            created_by_user_name (str, none_type): [optional]  # noqa: E501
-            description (str, none_type): [optional]  # noqa: E501
-            launch_source (str, none_type): Once launch source is specified it cannot be updated. [optional]  # noqa: E501
+            created_date (datetime, none_type): [optional]  # noqa: E501
+            modified_date (datetime, none_type): [optional]  # noqa: E501
+            is_deleted (bool): [optional]  # noqa: E501
+            tag_names ([str], none_type): [optional]  # noqa: E501
+            iterations ([IterationModel], none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -210,16 +233,21 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
         self.name = name
+        self.entity_type_name = entity_type_name
+        self.project_id = project_id
+        self.section_id = section_id
+        self.section_name = section_name
+        self.state = state
+        self.priority = priority
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -232,20 +260,25 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, *args, **kwargs):  # noqa: E501
-        """TestRunV2GetModel - a model defined in OpenAPI
+    def __init__(self, name, entity_type_name, project_id, section_id, section_name, state, priority, *args, **kwargs):  # noqa: E501
+        """WorkItemShortModel - a model defined in OpenAPI
 
         Args:
-            id (str):
             name (str):
+            entity_type_name (str): Property can have one of these values: CheckLists, SharedSteps, TestCases
+            project_id (str): This property is used to link autotest with project
+            section_id (str): This property links workitem with section
+            section_name (str): Name of the section where work item is located
+            state (WorkItemStates):
+            priority (WorkItemPriorityModel):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -270,27 +303,27 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            started_on (datetime, none_type): [optional]  # noqa: E501
-            completed_on (datetime, none_type): [optional]  # noqa: E501
-            state_name (TestRunState): [optional]  # noqa: E501
-            project_id (str): This property is used to link test run with project. [optional]  # noqa: E501
-            test_plan_id (str, none_type): This property is used to link test run with test plan. [optional]  # noqa: E501
-            test_results ([TestResultV2GetModel], none_type): [optional]  # noqa: E501
-            created_date (datetime): [optional]  # noqa: E501
-            modified_date (datetime, none_type): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            version_id (str): used for versioning changes in workitem. [optional]  # noqa: E501
+            is_automated (bool): [optional]  # noqa: E501
+            global_id (int): [optional]  # noqa: E501
+            duration (int): [optional]  # noqa: E501
+            attributes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
-            created_by_user_name (str, none_type): [optional]  # noqa: E501
-            description (str, none_type): [optional]  # noqa: E501
-            launch_source (str, none_type): Once launch source is specified it cannot be updated. [optional]  # noqa: E501
+            created_date (datetime, none_type): [optional]  # noqa: E501
+            modified_date (datetime, none_type): [optional]  # noqa: E501
+            is_deleted (bool): [optional]  # noqa: E501
+            tag_names ([str], none_type): [optional]  # noqa: E501
+            iterations ([IterationModel], none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -312,16 +345,21 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
         self.name = name
+        self.entity_type_name = entity_type_name
+        self.project_id = project_id
+        self.section_id = section_id
+        self.section_name = section_name
+        self.state = state
+        self.priority = priority
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_v2_post_short_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_v2_post_short_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_run_v2_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_run_v2_put_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_suite_change_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_change_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_suite_change_view_model_test_plan_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_change_view_model_test_plan_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_suite_v2_get_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_v2_get_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,18 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from testgear_api_client.model.test_suite_type import TestSuiteType
+    globals()['TestSuiteType'] = TestSuiteType
+
 
 class TestSuiteV2GetModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
@@ -74,31 +78,36 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
             'test_plan_id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'parent_id': (str, none_type,),  # noqa: E501
+            'type': (TestSuiteType,),  # noqa: E501
+            'save_structure': (bool, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'test_plan_id': 'testPlanId',  # noqa: E501
         'name': 'name',  # noqa: E501
         'id': 'id',  # noqa: E501
         'parent_id': 'parentId',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'save_structure': 'saveStructure',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -140,14 +149,16 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
             parent_id (str, none_type): [optional]  # noqa: E501
+            type (TestSuiteType): [optional]  # noqa: E501
+            save_structure (bool, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -233,14 +244,16 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
             parent_id (str, none_type): [optional]  # noqa: E501
+            type (TestSuiteType): [optional]  # noqa: E501
+            save_structure (bool, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_suite_v2_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/api_v2_attachments_post_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 
-class TestSuiteV2PostModel(ModelNormal):
+class ApiV2AttachmentsPostRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -54,64 +54,58 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('name',): {
-            'max_length': 255,
-            'min_length': 0,
-        },
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'test_plan_id': (str,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'parent_id': (str, none_type,),  # noqa: E501
+            'file': (file_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'test_plan_id': 'testPlanId',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'parent_id': 'parentId',  # noqa: E501
+        'file': 'file',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, test_plan_id, name, *args, **kwargs):  # noqa: E501
-        """TestSuiteV2PostModel - a model defined in OpenAPI
-
-        Args:
-            test_plan_id (str):
-            name (str):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """ApiV2AttachmentsPostRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +130,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            parent_id (str, none_type): [optional]  # noqa: E501
+            file (file_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -168,16 +162,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.test_plan_id = test_plan_id
-        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,20 +182,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, test_plan_id, name, *args, **kwargs):  # noqa: E501
-        """TestSuiteV2PostModel - a model defined in OpenAPI
-
-        Args:
-            test_plan_id (str):
-            name (str):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """ApiV2AttachmentsPostRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            parent_id (str, none_type): [optional]  # noqa: E501
+            file (file_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -258,16 +246,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.test_plan_id = test_plan_id
-        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_suite_v2_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/parameter_group_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 
-class TestSuiteV2PutModel(ModelNormal):
+class ParameterGroupModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -54,18 +54,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('name',): {
-            'max_length': 255,
-            'min_length': 0,
-        },
     }
 
     additional_properties_type = None
 
     _nullable = False
 
     @cached_property
@@ -75,43 +71,39 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'parent_id': (str, none_type,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
+            'values': ({str: (str,)}, none_type,),  # noqa: E501
+            'parameter_key_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'parent_id': 'parentId',  # noqa: E501
+        'values': 'values',  # noqa: E501
+        'parameter_key_id': 'parameterKeyId',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, *args, **kwargs):  # noqa: E501
-        """TestSuiteV2PutModel - a model defined in OpenAPI
-
-        Args:
-            id (str):
-            name (str):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """ParameterGroupModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +128,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            parent_id (str, none_type): [optional]  # noqa: E501
+            name (str, none_type): [optional]  # noqa: E501
+            values ({str: (str,)}, none_type): [optional]  # noqa: E501
+            parameter_key_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -168,16 +162,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,20 +182,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, *args, **kwargs):  # noqa: E501
-        """TestSuiteV2PutModel - a model defined in OpenAPI
-
-        Args:
-            id (str):
-            name (str):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """ParameterGroupModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,15 +216,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            parent_id (str, none_type): [optional]  # noqa: E501
+            name (str, none_type): [optional]  # noqa: E501
+            values ({str: (str,)}, none_type): [optional]  # noqa: E501
+            parameter_key_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -258,16 +248,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_suite_v2_tree_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_v2_post_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from testgear_api_client.model.test_suite_type import TestSuiteType
+    globals()['TestSuiteType'] = TestSuiteType
 
-class TestSuiteV2TreeModel(ModelNormal):
+
+class TestSuiteV2PostModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -74,44 +78,45 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
             'test_plan_id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
-            'children': ([TestSuiteV2TreeModel], none_type,),  # noqa: E501
-            'id': (str,),  # noqa: E501
             'parent_id': (str, none_type,),  # noqa: E501
+            'type': (TestSuiteType,),  # noqa: E501
+            'save_structure': (bool, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'test_plan_id': 'testPlanId',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'children': 'children',  # noqa: E501
-        'id': 'id',  # noqa: E501
         'parent_id': 'parentId',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'save_structure': 'saveStructure',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, test_plan_id, name, *args, **kwargs):  # noqa: E501
-        """TestSuiteV2TreeModel - a model defined in OpenAPI
+        """TestSuiteV2PostModel - a model defined in OpenAPI
 
         Args:
             test_plan_id (str):
             name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -140,17 +145,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            children ([TestSuiteV2TreeModel], none_type): nested enumeration of children is allowed. [optional]  # noqa: E501
-            id (str): [optional]  # noqa: E501
             parent_id (str, none_type): [optional]  # noqa: E501
+            type (TestSuiteType): [optional]  # noqa: E501
+            save_structure (bool, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -197,15 +202,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, test_plan_id, name, *args, **kwargs):  # noqa: E501
-        """TestSuiteV2TreeModel - a model defined in OpenAPI
+        """TestSuiteV2PostModel - a model defined in OpenAPI
 
         Args:
             test_plan_id (str):
             name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -234,17 +239,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            children ([TestSuiteV2TreeModel], none_type): nested enumeration of children is allowed. [optional]  # noqa: E501
-            id (str): [optional]  # noqa: E501
             parent_id (str, none_type): [optional]  # noqa: E501
+            type (TestSuiteType): [optional]  # noqa: E501
+            save_structure (bool, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_suite_with_children_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_with_children_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/test_suite_work_items_search_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_work_items_search_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             'is_automated': (bool, none_type,),  # noqa: E501
             'states': ([WorkItemStates], none_type,),  # noqa: E501
             'duration': (Int32RangeSelectorModel,),  # noqa: E501
             'created_date': (DateTimeRangeSelectorModel,),  # noqa: E501
             'modified_date': (DateTimeRangeSelectorModel,),  # noqa: E501
             'created_by_ids': ([str], none_type,),  # noqa: E501
             'modified_by_ids': ([str], none_type,),  # noqa: E501
-            'attributes': ({str: ([str], none_type)}, none_type,),  # noqa: E501
+            'attributes': ({str: ([str],)}, none_type,),  # noqa: E501
             'is_deleted': (bool, none_type,),  # noqa: E501
             'tag_names': ([str], none_type,),  # noqa: E501
             'entity_types': ([str], none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -194,15 +194,15 @@
             is_automated (bool, none_type): Is result must consist of only manual/automated work items. [optional]  # noqa: E501
             states ([WorkItemStates], none_type): Collection of states of work item. [optional]  # noqa: E501
             duration (Int32RangeSelectorModel): [optional]  # noqa: E501
             created_date (DateTimeRangeSelectorModel): [optional]  # noqa: E501
             modified_date (DateTimeRangeSelectorModel): [optional]  # noqa: E501
             created_by_ids ([str], none_type): Collection of identifiers of users who created work item. [optional]  # noqa: E501
             modified_by_ids ([str], none_type): Collection of identifiers of users who applied last modification to work item. [optional]  # noqa: E501
-            attributes ({str: ([str], none_type)}, none_type): Custom attributes of work item. [optional]  # noqa: E501
+            attributes ({str: ([str],)}, none_type): Custom attributes of work item. [optional]  # noqa: E501
             is_deleted (bool, none_type): Is result must consist of only actual/deleted work items. [optional]  # noqa: E501
             tag_names ([str], none_type): Collection of tags. [optional]  # noqa: E501
             entity_types ([str], none_type): Collection of types of work item  <br>Allowed values: `TestCases`, `CheckLists`, `SharedSteps`. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
@@ -294,15 +294,15 @@
             is_automated (bool, none_type): Is result must consist of only manual/automated work items. [optional]  # noqa: E501
             states ([WorkItemStates], none_type): Collection of states of work item. [optional]  # noqa: E501
             duration (Int32RangeSelectorModel): [optional]  # noqa: E501
             created_date (DateTimeRangeSelectorModel): [optional]  # noqa: E501
             modified_date (DateTimeRangeSelectorModel): [optional]  # noqa: E501
             created_by_ids ([str], none_type): Collection of identifiers of users who created work item. [optional]  # noqa: E501
             modified_by_ids ([str], none_type): Collection of identifiers of users who applied last modification to work item. [optional]  # noqa: E501
-            attributes ({str: ([str], none_type)}, none_type): Custom attributes of work item. [optional]  # noqa: E501
+            attributes ({str: ([str],)}, none_type): Custom attributes of work item. [optional]  # noqa: E501
             is_deleted (bool, none_type): Is result must consist of only actual/deleted work items. [optional]  # noqa: E501
             tag_names ([str], none_type): Collection of tags. [optional]  # noqa: E501
             entity_types ([str], none_type): Collection of types of work item  <br>Allowed values: `TestCases`, `CheckLists`, `SharedSteps`. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/user_rank_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/user_rank_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/user_with_rank_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/user_with_rank_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/validate_anti_forgery_token_attribute.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/validate_anti_forgery_token_attribute.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/validation_problem_details.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/web_hook_event_type.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/web_hook_event_type.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/web_hook_event_type_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/web_hook_event_type_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/web_hook_log_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/web_hook_log_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,50 +78,50 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'web_hook_name': (str, none_type,),  # noqa: E501
             'event_type': (WebHookEventTypeModel,),  # noqa: E501
+            'request_type': (RequestTypeModel,),  # noqa: E501
+            'web_hook_name': (str, none_type,),  # noqa: E501
             'web_hook_id': (str,),  # noqa: E501
             'request_body': (str, none_type,),  # noqa: E501
             'request_meta': (str, none_type,),  # noqa: E501
             'response_status_code': (int,),  # noqa: E501
             'response_body': (str, none_type,),  # noqa: E501
             'response_meta': (str, none_type,),  # noqa: E501
             'project_id': (str,),  # noqa: E501
             'url': (str, none_type,),  # noqa: E501
-            'request_type': (RequestTypeModel,),  # noqa: E501
             'created_date': (datetime, none_type,),  # noqa: E501
             'modified_date': (datetime, none_type,),  # noqa: E501
             'created_by_id': (str,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'is_deleted': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'web_hook_name': 'webHookName',  # noqa: E501
         'event_type': 'eventType',  # noqa: E501
+        'request_type': 'requestType',  # noqa: E501
+        'web_hook_name': 'webHookName',  # noqa: E501
         'web_hook_id': 'webHookId',  # noqa: E501
         'request_body': 'requestBody',  # noqa: E501
         'request_meta': 'requestMeta',  # noqa: E501
         'response_status_code': 'responseStatusCode',  # noqa: E501
         'response_body': 'responseBody',  # noqa: E501
         'response_meta': 'responseMeta',  # noqa: E501
         'project_id': 'projectId',  # noqa: E501
         'url': 'url',  # noqa: E501
-        'request_type': 'requestType',  # noqa: E501
         'created_date': 'createdDate',  # noqa: E501
         'modified_date': 'modifiedDate',  # noqa: E501
         'created_by_id': 'createdById',  # noqa: E501
         'modified_by_id': 'modifiedById',  # noqa: E501
         'id': 'id',  # noqa: E501
         'is_deleted': 'isDeleted',  # noqa: E501
     }
@@ -129,17 +129,21 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, event_type, request_type, *args, **kwargs):  # noqa: E501
         """WebHookLogModel - a model defined in OpenAPI
 
+        Args:
+            event_type (WebHookEventTypeModel):
+            request_type (RequestTypeModel):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -164,24 +168,22 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             web_hook_name (str, none_type): [optional]  # noqa: E501
-            event_type (WebHookEventTypeModel): [optional]  # noqa: E501
             web_hook_id (str): [optional]  # noqa: E501
             request_body (str, none_type): [optional]  # noqa: E501
             request_meta (str, none_type): [optional]  # noqa: E501
             response_status_code (int): [optional]  # noqa: E501
             response_body (str, none_type): [optional]  # noqa: E501
             response_meta (str, none_type): [optional]  # noqa: E501
             project_id (str): [optional]  # noqa: E501
             url (str, none_type): [optional]  # noqa: E501
-            request_type (RequestTypeModel): [optional]  # noqa: E501
             created_date (datetime, none_type): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             id (str): Unique ID of the entity. [optional]  # noqa: E501
             is_deleted (bool): Indicates if the entity is deleted. [optional]  # noqa: E501
         """
@@ -211,14 +213,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.event_type = event_type
+        self.request_type = request_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -231,17 +235,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, event_type, request_type, *args, **kwargs):  # noqa: E501
         """WebHookLogModel - a model defined in OpenAPI
 
+        Args:
+            event_type (WebHookEventTypeModel):
+            request_type (RequestTypeModel):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -266,24 +274,22 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             web_hook_name (str, none_type): [optional]  # noqa: E501
-            event_type (WebHookEventTypeModel): [optional]  # noqa: E501
             web_hook_id (str): [optional]  # noqa: E501
             request_body (str, none_type): [optional]  # noqa: E501
             request_meta (str, none_type): [optional]  # noqa: E501
             response_status_code (int): [optional]  # noqa: E501
             response_body (str, none_type): [optional]  # noqa: E501
             response_meta (str, none_type): [optional]  # noqa: E501
             project_id (str): [optional]  # noqa: E501
             url (str, none_type): [optional]  # noqa: E501
-            request_type (RequestTypeModel): [optional]  # noqa: E501
             created_date (datetime, none_type): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             id (str): Unique ID of the entity. [optional]  # noqa: E501
             is_deleted (bool): Indicates if the entity is deleted. [optional]  # noqa: E501
         """
@@ -311,14 +317,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.event_type = event_type
+        self.request_type = request_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/web_hook_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/web_hook_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,22 +78,22 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'name': (str, none_type,),  # noqa: E501
             'event_type': (WebHookEventTypeModel,),  # noqa: E501
+            'request_type': (RequestTypeModel,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
             'description': (str, none_type,),  # noqa: E501
             'url': (str, none_type,),  # noqa: E501
-            'request_type': (RequestTypeModel,),  # noqa: E501
             'should_send_body': (bool,),  # noqa: E501
-            'headers': ({str: (str, none_type)}, none_type,),  # noqa: E501
-            'query_parameters': ({str: (str, none_type)}, none_type,),  # noqa: E501
+            'headers': ({str: (str,)}, none_type,),  # noqa: E501
+            'query_parameters': ({str: (str,)}, none_type,),  # noqa: E501
             'is_enabled': (bool,),  # noqa: E501
             'should_send_custom_body': (bool,),  # noqa: E501
             'custom_body': (str, none_type,),  # noqa: E501
             'custom_body_media_type': (str, none_type,),  # noqa: E501
             'should_replace_parameters': (bool,),  # noqa: E501
             'should_escape_parameters': (bool,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
@@ -107,19 +107,19 @@
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
         'event_type': 'eventType',  # noqa: E501
+        'request_type': 'requestType',  # noqa: E501
+        'name': 'name',  # noqa: E501
         'description': 'description',  # noqa: E501
         'url': 'url',  # noqa: E501
-        'request_type': 'requestType',  # noqa: E501
         'should_send_body': 'shouldSendBody',  # noqa: E501
         'headers': 'headers',  # noqa: E501
         'query_parameters': 'queryParameters',  # noqa: E501
         'is_enabled': 'isEnabled',  # noqa: E501
         'should_send_custom_body': 'shouldSendCustomBody',  # noqa: E501
         'custom_body': 'customBody',  # noqa: E501
         'custom_body_media_type': 'customBodyMediaType',  # noqa: E501
@@ -137,17 +137,21 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, event_type, request_type, *args, **kwargs):  # noqa: E501
         """WebHookModel - a model defined in OpenAPI
 
+        Args:
+            event_type (WebHookEventTypeModel):
+            request_type (RequestTypeModel):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -172,21 +176,19 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             name (str, none_type): Name of the webhook. [optional]  # noqa: E501
-            event_type (WebHookEventTypeModel): [optional]  # noqa: E501
             description (str, none_type): Description of the webhook. [optional]  # noqa: E501
             url (str, none_type): Url to which the webhook sends request. [optional]  # noqa: E501
-            request_type (RequestTypeModel): [optional]  # noqa: E501
             should_send_body (bool): Indicates if the webhook sends body. [optional]  # noqa: E501
-            headers ({str: (str, none_type)}, none_type): Collection of headers which the webhook sends. [optional]  # noqa: E501
-            query_parameters ({str: (str, none_type)}, none_type): Collection of query parameters which the webhook sends. [optional]  # noqa: E501
+            headers ({str: (str,)}, none_type): Collection of headers which the webhook sends. [optional]  # noqa: E501
+            query_parameters ({str: (str,)}, none_type): Collection of query parameters which the webhook sends. [optional]  # noqa: E501
             is_enabled (bool): Indicates if the webhook is active. [optional]  # noqa: E501
             should_send_custom_body (bool): Indicates if the webhook sends custom body. [optional]  # noqa: E501
             custom_body (str, none_type): Custom body of the webhook. [optional]  # noqa: E501
             custom_body_media_type (str, none_type): MIME type of body of the webhook. [optional]  # noqa: E501
             should_replace_parameters (bool): Indicates if the webhook injects parameters. [optional]  # noqa: E501
             should_escape_parameters (bool): Indicates if the webhook escapes invalid characters in parameters. [optional]  # noqa: E501
             created_date (datetime): Creation date of the webhook. [optional]  # noqa: E501
@@ -223,14 +225,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.event_type = event_type
+        self.request_type = request_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -243,17 +247,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, event_type, request_type, *args, **kwargs):  # noqa: E501
         """WebHookModel - a model defined in OpenAPI
 
+        Args:
+            event_type (WebHookEventTypeModel):
+            request_type (RequestTypeModel):
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -278,21 +286,19 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             name (str, none_type): Name of the webhook. [optional]  # noqa: E501
-            event_type (WebHookEventTypeModel): [optional]  # noqa: E501
             description (str, none_type): Description of the webhook. [optional]  # noqa: E501
             url (str, none_type): Url to which the webhook sends request. [optional]  # noqa: E501
-            request_type (RequestTypeModel): [optional]  # noqa: E501
             should_send_body (bool): Indicates if the webhook sends body. [optional]  # noqa: E501
-            headers ({str: (str, none_type)}, none_type): Collection of headers which the webhook sends. [optional]  # noqa: E501
-            query_parameters ({str: (str, none_type)}, none_type): Collection of query parameters which the webhook sends. [optional]  # noqa: E501
+            headers ({str: (str,)}, none_type): Collection of headers which the webhook sends. [optional]  # noqa: E501
+            query_parameters ({str: (str,)}, none_type): Collection of query parameters which the webhook sends. [optional]  # noqa: E501
             is_enabled (bool): Indicates if the webhook is active. [optional]  # noqa: E501
             should_send_custom_body (bool): Indicates if the webhook sends custom body. [optional]  # noqa: E501
             custom_body (str, none_type): Custom body of the webhook. [optional]  # noqa: E501
             custom_body_media_type (str, none_type): MIME type of body of the webhook. [optional]  # noqa: E501
             should_replace_parameters (bool): Indicates if the webhook injects parameters. [optional]  # noqa: E501
             should_escape_parameters (bool): Indicates if the webhook escapes invalid characters in parameters. [optional]  # noqa: E501
             created_date (datetime): Creation date of the webhook. [optional]  # noqa: E501
@@ -327,14 +333,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.event_type = event_type
+        self.request_type = request_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/web_hook_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/web_hook_post_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,16 +92,16 @@
             'project_id': (str,),  # noqa: E501
             'event_type': (WebHookEventTypeModel,),  # noqa: E501
             'url': (str,),  # noqa: E501
             'request_type': (RequestTypeModel,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'description': (str, none_type,),  # noqa: E501
             'should_send_body': (bool,),  # noqa: E501
-            'headers': ({str: (str, none_type)}, none_type,),  # noqa: E501
-            'query_parameters': ({str: (str, none_type)}, none_type,),  # noqa: E501
+            'headers': ({str: (str,)}, none_type,),  # noqa: E501
+            'query_parameters': ({str: (str,)}, none_type,),  # noqa: E501
             'is_enabled': (bool,),  # noqa: E501
             'should_send_custom_body': (bool,),  # noqa: E501
             'custom_body': (str, none_type,),  # noqa: E501
             'should_replace_parameters': (bool,),  # noqa: E501
             'should_escape_parameters': (bool,),  # noqa: E501
         }
 
@@ -173,16 +173,16 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str, none_type): Description of the webhook. [optional]  # noqa: E501
             should_send_body (bool): Indicates if the webhook sends body. [optional]  # noqa: E501
-            headers ({str: (str, none_type)}, none_type): Collection of the webhook headers. [optional]  # noqa: E501
-            query_parameters ({str: (str, none_type)}, none_type): Collection of the webhook query parameters. [optional]  # noqa: E501
+            headers ({str: (str,)}, none_type): Collection of the webhook headers. [optional]  # noqa: E501
+            query_parameters ({str: (str,)}, none_type): Collection of the webhook query parameters. [optional]  # noqa: E501
             is_enabled (bool): Indicates if the webhook is active. [optional]  # noqa: E501
             should_send_custom_body (bool): Indicates if the webhook sends custom body. [optional]  # noqa: E501
             custom_body (str, none_type): Custom body of the webhook. [optional]  # noqa: E501
             should_replace_parameters (bool): Indicates if the webhook injects parameters. [optional]  # noqa: E501
             should_escape_parameters (bool): Indicates if the webhook escapes invalid characters in parameters. [optional]  # noqa: E501
         """
 
@@ -279,16 +279,16 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str, none_type): Description of the webhook. [optional]  # noqa: E501
             should_send_body (bool): Indicates if the webhook sends body. [optional]  # noqa: E501
-            headers ({str: (str, none_type)}, none_type): Collection of the webhook headers. [optional]  # noqa: E501
-            query_parameters ({str: (str, none_type)}, none_type): Collection of the webhook query parameters. [optional]  # noqa: E501
+            headers ({str: (str,)}, none_type): Collection of the webhook headers. [optional]  # noqa: E501
+            query_parameters ({str: (str,)}, none_type): Collection of the webhook query parameters. [optional]  # noqa: E501
             is_enabled (bool): Indicates if the webhook is active. [optional]  # noqa: E501
             should_send_custom_body (bool): Indicates if the webhook sends custom body. [optional]  # noqa: E501
             custom_body (str, none_type): Custom body of the webhook. [optional]  # noqa: E501
             should_replace_parameters (bool): Indicates if the webhook injects parameters. [optional]  # noqa: E501
             should_escape_parameters (bool): Indicates if the webhook escapes invalid characters in parameters. [optional]  # noqa: E501
         """
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_change_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_change_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_changed_attribute_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_changed_attribute_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_changed_fields_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_changed_fields_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_comment_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_comment_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_comment_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_comment_post_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_comment_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_comment_put_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_entity_types.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_entity_types.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_filter_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_filter_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_id_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_id_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,17 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('id',): {
+            'min_length': 1,
+        },
     }
 
     additional_properties_type = None
 
     _nullable = False
 
     @cached_property
@@ -71,15 +74,15 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str, none_type,),  # noqa: E501
+            'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -90,17 +93,20 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
         """WorkItemIdModel - a model defined in OpenAPI
 
+        Args:
+            id (str): Used for search WorkItem. Internal identifier has a Guid data format. Global identifier has an integer data format
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -124,15 +130,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str, none_type): Used for search WorkItem. Internal identifier has a Guid data format. Global identifier has an integer data format. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -156,14 +161,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -176,17 +182,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, *args, **kwargs):  # noqa: E501
         """WorkItemIdModel - a model defined in OpenAPI
 
+        Args:
+            id (str): Used for search WorkItem. Internal identifier has a Guid data format. Global identifier has an integer data format
+
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -210,15 +219,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str, none_type): Used for search WorkItem. Internal identifier has a Guid data format. Global identifier has an integer data format. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -240,14 +248,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_identifier_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_identifier_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_like_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_like_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_link_change_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/test_suite_v2_tree_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from testgear_api_client.model.test_suite_type import TestSuiteType
+    globals()['TestSuiteType'] = TestSuiteType
 
-class WorkItemLinkChangeViewModel(ModelNormal):
+
+class TestSuiteV2TreeModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -54,14 +58,18 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('name',): {
+            'max_length': 255,
+            'min_length': 0,
+        },
     }
 
     additional_properties_type = None
 
     _nullable = False
 
     @cached_property
@@ -70,46 +78,53 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'description': (str, none_type,),  # noqa: E501
-            'url': (str, none_type,),  # noqa: E501
-            'title': (str, none_type,),  # noqa: E501
-            'has_info': (bool,),  # noqa: E501
+            'test_plan_id': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'children': ([TestSuiteV2TreeModel], none_type,),  # noqa: E501
             'id': (str,),  # noqa: E501
-            'type': (str, none_type,),  # noqa: E501
+            'parent_id': (str, none_type,),  # noqa: E501
+            'type': (TestSuiteType,),  # noqa: E501
+            'save_structure': (bool, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'description': 'description',  # noqa: E501
-        'url': 'url',  # noqa: E501
-        'title': 'title',  # noqa: E501
-        'has_info': 'hasInfo',  # noqa: E501
+        'test_plan_id': 'testPlanId',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'children': 'children',  # noqa: E501
         'id': 'id',  # noqa: E501
+        'parent_id': 'parentId',  # noqa: E501
         'type': 'type',  # noqa: E501
+        'save_structure': 'saveStructure',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WorkItemLinkChangeViewModel - a model defined in OpenAPI
+    def _from_openapi_data(cls, test_plan_id, name, *args, **kwargs):  # noqa: E501
+        """TestSuiteV2TreeModel - a model defined in OpenAPI
+
+        Args:
+            test_plan_id (str):
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,20 +149,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            description (str, none_type): [optional]  # noqa: E501
-            url (str, none_type): [optional]  # noqa: E501
-            title (str, none_type): [optional]  # noqa: E501
-            has_info (bool): [optional]  # noqa: E501
+            children ([TestSuiteV2TreeModel], none_type): nested enumeration of children is allowed. [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
-            type (str, none_type): [optional]  # noqa: E501
+            parent_id (str, none_type): [optional]  # noqa: E501
+            type (TestSuiteType): [optional]  # noqa: E501
+            save_structure (bool, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -171,14 +185,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.test_plan_id = test_plan_id
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -191,16 +207,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """WorkItemLinkChangeViewModel - a model defined in OpenAPI
+    def __init__(self, test_plan_id, name, *args, **kwargs):  # noqa: E501
+        """TestSuiteV2TreeModel - a model defined in OpenAPI
+
+        Args:
+            test_plan_id (str):
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -225,20 +245,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            description (str, none_type): [optional]  # noqa: E501
-            url (str, none_type): [optional]  # noqa: E501
-            title (str, none_type): [optional]  # noqa: E501
-            has_info (bool): [optional]  # noqa: E501
+            children ([TestSuiteV2TreeModel], none_type): nested enumeration of children is allowed. [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
-            type (str, none_type): [optional]  # noqa: E501
+            parent_id (str, none_type): [optional]  # noqa: E501
+            type (TestSuiteType): [optional]  # noqa: E501
+            save_structure (bool, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -260,14 +279,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.test_plan_id = test_plan_id
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_link_change_view_model_array_work_item_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_link_change_view_model_array_work_item_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'entity_type_name': (WorkItemEntityTypes,),  # noqa: E501
+            'id': (str,),  # noqa: E501
             'state': (WorkItemStates,),  # noqa: E501
             'priority': (WorkItemPriorityModel,),  # noqa: E501
             'steps': ([StepModel],),  # noqa: E501
             'precondition_steps': ([StepModel],),  # noqa: E501
             'postcondition_steps': ([StepModel],),  # noqa: E501
             'attributes': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'tags': ([TagShortModel],),  # noqa: E501
@@ -125,27 +126,27 @@
             'version_number': (int,),  # noqa: E501
             'iterations': ([IterationModel], none_type,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'modified_date': (datetime, none_type,),  # noqa: E501
             'created_by_id': (str,),  # noqa: E501
             'modified_by_id': (str, none_type,),  # noqa: E501
             'global_id': (int,),  # noqa: E501
-            'id': (str,),  # noqa: E501
             'section_id': (str,),  # noqa: E501
             'description': (str, none_type,),  # noqa: E501
             'duration': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'entity_type_name': 'entityTypeName',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'state': 'state',  # noqa: E501
         'priority': 'priority',  # noqa: E501
         'steps': 'steps',  # noqa: E501
         'precondition_steps': 'preconditionSteps',  # noqa: E501
         'postcondition_steps': 'postconditionSteps',  # noqa: E501
         'attributes': 'attributes',  # noqa: E501
         'tags': 'tags',  # noqa: E501
@@ -163,32 +164,32 @@
         'version_number': 'versionNumber',  # noqa: E501
         'iterations': 'iterations',  # noqa: E501
         'created_date': 'createdDate',  # noqa: E501
         'modified_date': 'modifiedDate',  # noqa: E501
         'created_by_id': 'createdById',  # noqa: E501
         'modified_by_id': 'modifiedById',  # noqa: E501
         'global_id': 'globalId',  # noqa: E501
-        'id': 'id',  # noqa: E501
         'section_id': 'sectionId',  # noqa: E501
         'description': 'description',  # noqa: E501
         'duration': 'duration',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, entity_type_name, state, priority, steps, precondition_steps, postcondition_steps, attributes, tags, links, name, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, entity_type_name, id, state, priority, steps, precondition_steps, postcondition_steps, attributes, tags, links, name, *args, **kwargs):  # noqa: E501
         """WorkItemModel - a model defined in OpenAPI
 
         Args:
             entity_type_name (WorkItemEntityTypes):
+            id (str):
             state (WorkItemStates):
             priority (WorkItemPriorityModel):
             steps ([StepModel]):
             precondition_steps ([StepModel]):
             postcondition_steps ([StepModel]):
             attributes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
             tags ([TagShortModel]):
@@ -238,15 +239,14 @@
             version_number (int): used for define chronology of workitem state in each version. [optional]  # noqa: E501
             iterations ([IterationModel], none_type): [optional]  # noqa: E501
             created_date (datetime): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             global_id (int): [optional]  # noqa: E501
-            id (str): [optional]  # noqa: E501
             section_id (str): [optional]  # noqa: E501
             description (str, none_type): [optional]  # noqa: E501
             duration (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
@@ -274,14 +274,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.entity_type_name = entity_type_name
+        self.id = id
         self.state = state
         self.priority = priority
         self.steps = steps
         self.precondition_steps = precondition_steps
         self.postcondition_steps = postcondition_steps
         self.attributes = attributes
         self.tags = tags
@@ -303,19 +304,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, entity_type_name, state, priority, steps, precondition_steps, postcondition_steps, attributes, tags, links, name, *args, **kwargs):  # noqa: E501
+    def __init__(self, entity_type_name, id, state, priority, steps, precondition_steps, postcondition_steps, attributes, tags, links, name, *args, **kwargs):  # noqa: E501
         """WorkItemModel - a model defined in OpenAPI
 
         Args:
             entity_type_name (WorkItemEntityTypes):
+            id (str):
             state (WorkItemStates):
             priority (WorkItemPriorityModel):
             steps ([StepModel]):
             precondition_steps ([StepModel]):
             postcondition_steps ([StepModel]):
             attributes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
             tags ([TagShortModel]):
@@ -365,15 +367,14 @@
             version_number (int): used for define chronology of workitem state in each version. [optional]  # noqa: E501
             iterations ([IterationModel], none_type): [optional]  # noqa: E501
             created_date (datetime): [optional]  # noqa: E501
             modified_date (datetime, none_type): [optional]  # noqa: E501
             created_by_id (str): [optional]  # noqa: E501
             modified_by_id (str, none_type): [optional]  # noqa: E501
             global_id (int): [optional]  # noqa: E501
-            id (str): [optional]  # noqa: E501
             section_id (str): [optional]  # noqa: E501
             description (str, none_type): [optional]  # noqa: E501
             duration (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -399,14 +400,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.entity_type_name = entity_type_name
+        self.id = id
         self.state = state
         self.priority = priority
         self.steps = steps
         self.precondition_steps = precondition_steps
         self.postcondition_steps = postcondition_steps
         self.attributes = attributes
         self.tags = tags
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_move_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_move_post_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_post_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_post_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_priority_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_priority_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_put_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_put_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,67 +98,68 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'attachments': ([AttachmentPutModel],),  # noqa: E501
+            'id': (str,),  # noqa: E501
             'state': (WorkItemStates,),  # noqa: E501
             'priority': (WorkItemPriorityModel,),  # noqa: E501
             'steps': ([StepPutModel],),  # noqa: E501
             'precondition_steps': ([StepPutModel],),  # noqa: E501
             'postcondition_steps': ([StepPutModel],),  # noqa: E501
             'attributes': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'tags': ([TagShortModel],),  # noqa: E501
             'links': ([LinkPutModel],),  # noqa: E501
             'name': (str,),  # noqa: E501
             'iterations': ([IterationPutModel], none_type,),  # noqa: E501
             'auto_tests': ([AutoTestIdModel], none_type,),  # noqa: E501
-            'id': (str,),  # noqa: E501
             'section_id': (str,),  # noqa: E501
             'description': (str, none_type,),  # noqa: E501
             'duration': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'attachments': 'attachments',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'state': 'state',  # noqa: E501
         'priority': 'priority',  # noqa: E501
         'steps': 'steps',  # noqa: E501
         'precondition_steps': 'preconditionSteps',  # noqa: E501
         'postcondition_steps': 'postconditionSteps',  # noqa: E501
         'attributes': 'attributes',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'links': 'links',  # noqa: E501
         'name': 'name',  # noqa: E501
         'iterations': 'iterations',  # noqa: E501
         'auto_tests': 'autoTests',  # noqa: E501
-        'id': 'id',  # noqa: E501
         'section_id': 'sectionId',  # noqa: E501
         'description': 'description',  # noqa: E501
         'duration': 'duration',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, attachments, state, priority, steps, precondition_steps, postcondition_steps, attributes, tags, links, name, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, attachments, id, state, priority, steps, precondition_steps, postcondition_steps, attributes, tags, links, name, *args, **kwargs):  # noqa: E501
         """WorkItemPutModel - a model defined in OpenAPI
 
         Args:
             attachments ([AttachmentPutModel]):
+            id (str):
             state (WorkItemStates):
             priority (WorkItemPriorityModel):
             steps ([StepPutModel]):
             precondition_steps ([StepPutModel]):
             postcondition_steps ([StepPutModel]):
             attributes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
             tags ([TagShortModel]):
@@ -194,15 +195,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             iterations ([IterationPutModel], none_type): [optional]  # noqa: E501
             auto_tests ([AutoTestIdModel], none_type): [optional]  # noqa: E501
-            id (str): [optional]  # noqa: E501
             section_id (str): [optional]  # noqa: E501
             description (str, none_type): [optional]  # noqa: E501
             duration (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
@@ -230,14 +230,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.attachments = attachments
+        self.id = id
         self.state = state
         self.priority = priority
         self.steps = steps
         self.precondition_steps = precondition_steps
         self.postcondition_steps = postcondition_steps
         self.attributes = attributes
         self.tags = tags
@@ -259,19 +260,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, attachments, state, priority, steps, precondition_steps, postcondition_steps, attributes, tags, links, name, *args, **kwargs):  # noqa: E501
+    def __init__(self, attachments, id, state, priority, steps, precondition_steps, postcondition_steps, attributes, tags, links, name, *args, **kwargs):  # noqa: E501
         """WorkItemPutModel - a model defined in OpenAPI
 
         Args:
             attachments ([AttachmentPutModel]):
+            id (str):
             state (WorkItemStates):
             priority (WorkItemPriorityModel):
             steps ([StepPutModel]):
             precondition_steps ([StepPutModel]):
             postcondition_steps ([StepPutModel]):
             attributes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
             tags ([TagShortModel]):
@@ -307,15 +309,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             iterations ([IterationPutModel], none_type): [optional]  # noqa: E501
             auto_tests ([AutoTestIdModel], none_type): [optional]  # noqa: E501
-            id (str): [optional]  # noqa: E501
             section_id (str): [optional]  # noqa: E501
             description (str, none_type): [optional]  # noqa: E501
             duration (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -341,14 +342,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.attachments = attachments
+        self.id = id
         self.state = state
         self.priority = priority
         self.steps = steps
         self.precondition_steps = precondition_steps
         self.postcondition_steps = postcondition_steps
         self.attributes = attributes
         self.tags = tags
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_search_query_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_search_query_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_select_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_select_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_short_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/background_job_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,23 +26,23 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from testgear_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from testgear_api_client.model.iteration_model import IterationModel
-    from testgear_api_client.model.work_item_priority_model import WorkItemPriorityModel
-    from testgear_api_client.model.work_item_states import WorkItemStates
-    globals()['IterationModel'] = IterationModel
-    globals()['WorkItemPriorityModel'] = WorkItemPriorityModel
-    globals()['WorkItemStates'] = WorkItemStates
+    from testgear_api_client.model.background_job_attachment_model import BackgroundJobAttachmentModel
+    from testgear_api_client.model.background_job_state import BackgroundJobState
+    from testgear_api_client.model.background_job_type import BackgroundJobType
+    globals()['BackgroundJobAttachmentModel'] = BackgroundJobAttachmentModel
+    globals()['BackgroundJobState'] = BackgroundJobState
+    globals()['BackgroundJobType'] = BackgroundJobType
 
 
-class WorkItemShortModel(ModelNormal):
+class BackgroundJobModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,20 +62,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('name',): {
-            'min_length': 1,
-        },
-        ('entity_type_name',): {
-            'min_length': 1,
-        },
     }
 
     additional_properties_type = None
 
     _nullable = False
 
     @cached_property
@@ -86,79 +80,53 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'name': (str,),  # noqa: E501
-            'entity_type_name': (str,),  # noqa: E501
-            'project_id': (str,),  # noqa: E501
-            'section_id': (str,),  # noqa: E501
-            'state': (WorkItemStates,),  # noqa: E501
-            'priority': (WorkItemPriorityModel,),  # noqa: E501
             'id': (str,),  # noqa: E501
-            'version_id': (str,),  # noqa: E501
-            'is_automated': (bool,),  # noqa: E501
-            'global_id': (int,),  # noqa: E501
-            'duration': (int,),  # noqa: E501
-            'attributes': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
-            'created_by_id': (str,),  # noqa: E501
-            'modified_by_id': (str, none_type,),  # noqa: E501
-            'created_date': (datetime, none_type,),  # noqa: E501
-            'modified_date': (datetime, none_type,),  # noqa: E501
+            'job_id': (str, none_type,),  # noqa: E501
+            'job_type': (BackgroundJobType,),  # noqa: E501
+            'state': (BackgroundJobState,),  # noqa: E501
             'is_deleted': (bool,),  # noqa: E501
-            'tag_names': ([str], none_type,),  # noqa: E501
-            'iterations': ([IterationModel], none_type,),  # noqa: E501
+            'progress': (int,),  # noqa: E501
+            'start_date': (datetime, none_type,),  # noqa: E501
+            'end_date': (datetime, none_type,),  # noqa: E501
+            'error': (str, none_type,),  # noqa: E501
+            'attachments': ([BackgroundJobAttachmentModel], none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'entity_type_name': 'entityTypeName',  # noqa: E501
-        'project_id': 'projectId',  # noqa: E501
-        'section_id': 'sectionId',  # noqa: E501
-        'state': 'state',  # noqa: E501
-        'priority': 'priority',  # noqa: E501
         'id': 'id',  # noqa: E501
-        'version_id': 'versionId',  # noqa: E501
-        'is_automated': 'isAutomated',  # noqa: E501
-        'global_id': 'globalId',  # noqa: E501
-        'duration': 'duration',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
-        'created_by_id': 'createdById',  # noqa: E501
-        'modified_by_id': 'modifiedById',  # noqa: E501
-        'created_date': 'createdDate',  # noqa: E501
-        'modified_date': 'modifiedDate',  # noqa: E501
+        'job_id': 'jobId',  # noqa: E501
+        'job_type': 'jobType',  # noqa: E501
+        'state': 'state',  # noqa: E501
         'is_deleted': 'isDeleted',  # noqa: E501
-        'tag_names': 'tagNames',  # noqa: E501
-        'iterations': 'iterations',  # noqa: E501
+        'progress': 'progress',  # noqa: E501
+        'start_date': 'startDate',  # noqa: E501
+        'end_date': 'endDate',  # noqa: E501
+        'error': 'error',  # noqa: E501
+        'attachments': 'attachments',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, entity_type_name, project_id, section_id, state, priority, *args, **kwargs):  # noqa: E501
-        """WorkItemShortModel - a model defined in OpenAPI
-
-        Args:
-            name (str):
-            entity_type_name (str): Property can have one of these values: CheckLists, SharedSteps, TestCases
-            project_id (str): This property is used to link autotest with project
-            section_id (str): This property links workitem with section
-            state (WorkItemStates):
-            priority (WorkItemPriorityModel):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """BackgroundJobModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -184,26 +152,23 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
-            version_id (str): used for versioning changes in workitem. [optional]  # noqa: E501
-            is_automated (bool): [optional]  # noqa: E501
-            global_id (int): [optional]  # noqa: E501
-            duration (int): [optional]  # noqa: E501
-            attributes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
-            created_by_id (str): [optional]  # noqa: E501
-            modified_by_id (str, none_type): [optional]  # noqa: E501
-            created_date (datetime, none_type): [optional]  # noqa: E501
-            modified_date (datetime, none_type): [optional]  # noqa: E501
+            job_id (str, none_type): [optional]  # noqa: E501
+            job_type (BackgroundJobType): [optional]  # noqa: E501
+            state (BackgroundJobState): [optional]  # noqa: E501
             is_deleted (bool): [optional]  # noqa: E501
-            tag_names ([str], none_type): [optional]  # noqa: E501
-            iterations ([IterationModel], none_type): [optional]  # noqa: E501
+            progress (int): [optional]  # noqa: E501
+            start_date (datetime, none_type): [optional]  # noqa: E501
+            end_date (datetime, none_type): [optional]  # noqa: E501
+            error (str, none_type): [optional]  # noqa: E501
+            attachments ([BackgroundJobAttachmentModel], none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -227,20 +192,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.entity_type_name = entity_type_name
-        self.project_id = project_id
-        self.section_id = section_id
-        self.state = state
-        self.priority = priority
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -253,24 +212,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, entity_type_name, project_id, section_id, state, priority, *args, **kwargs):  # noqa: E501
-        """WorkItemShortModel - a model defined in OpenAPI
-
-        Args:
-            name (str):
-            entity_type_name (str): Property can have one of these values: CheckLists, SharedSteps, TestCases
-            project_id (str): This property is used to link autotest with project
-            section_id (str): This property links workitem with section
-            state (WorkItemStates):
-            priority (WorkItemPriorityModel):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """BackgroundJobModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -296,26 +247,23 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
-            version_id (str): used for versioning changes in workitem. [optional]  # noqa: E501
-            is_automated (bool): [optional]  # noqa: E501
-            global_id (int): [optional]  # noqa: E501
-            duration (int): [optional]  # noqa: E501
-            attributes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
-            created_by_id (str): [optional]  # noqa: E501
-            modified_by_id (str, none_type): [optional]  # noqa: E501
-            created_date (datetime, none_type): [optional]  # noqa: E501
-            modified_date (datetime, none_type): [optional]  # noqa: E501
+            job_id (str, none_type): [optional]  # noqa: E501
+            job_type (BackgroundJobType): [optional]  # noqa: E501
+            state (BackgroundJobState): [optional]  # noqa: E501
             is_deleted (bool): [optional]  # noqa: E501
-            tag_names ([str], none_type): [optional]  # noqa: E501
-            iterations ([IterationModel], none_type): [optional]  # noqa: E501
+            progress (int): [optional]  # noqa: E501
+            start_date (datetime, none_type): [optional]  # noqa: E501
+            end_date (datetime, none_type): [optional]  # noqa: E501
+            error (str, none_type): [optional]  # noqa: E501
+            attachments ([BackgroundJobAttachmentModel], none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -337,20 +285,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.entity_type_name = entity_type_name
-        self.project_id = project_id
-        self.section_id = section_id
-        self.state = state
-        self.priority = priority
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_states.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_states.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_step_change_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_step_change_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_step_change_view_model_array_work_item_changed_field_view_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_step_change_view_model_array_work_item_changed_field_view_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_item_version_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_item_version_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model/work_items_extraction_model.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model/work_items_extraction_model.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/model_utils.py` & `testgear-api-client-3.1.0/src/testgear_api_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/models/__init__.py` & `testgear-api-client-3.1.0/src/testgear_api_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
 # from from testgear_api_client.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
+from testgear_api_client.model.api_v2_attachments_post_request import ApiV2AttachmentsPostRequest
 from testgear_api_client.model.attachment_change_view_model import AttachmentChangeViewModel
 from testgear_api_client.model.attachment_change_view_model_array_work_item_changed_field_view_model import AttachmentChangeViewModelArrayWorkItemChangedFieldViewModel
 from testgear_api_client.model.attachment_model import AttachmentModel
 from testgear_api_client.model.attachment_model_auto_test_step_results_model import AttachmentModelAutoTestStepResultsModel
 from testgear_api_client.model.attachment_put_model import AttachmentPutModel
 from testgear_api_client.model.attachment_put_model_auto_test_step_results_model import AttachmentPutModelAutoTestStepResultsModel
 from testgear_api_client.model.attachment_sub_get_model import AttachmentSubGetModel
@@ -33,14 +34,18 @@
 from testgear_api_client.model.autotest_result_historical_get_model import AutotestResultHistoricalGetModel
 from testgear_api_client.model.autotest_result_outcome import AutotestResultOutcome
 from testgear_api_client.model.autotest_result_reason_sub_get_model import AutotestResultReasonSubGetModel
 from testgear_api_client.model.autotest_select_model import AutotestSelectModel
 from testgear_api_client.model.autotests_extraction_model import AutotestsExtractionModel
 from testgear_api_client.model.autotests_select_model import AutotestsSelectModel
 from testgear_api_client.model.available_test_result_outcome import AvailableTestResultOutcome
+from testgear_api_client.model.background_job_attachment_model import BackgroundJobAttachmentModel
+from testgear_api_client.model.background_job_model import BackgroundJobModel
+from testgear_api_client.model.background_job_state import BackgroundJobState
+from testgear_api_client.model.background_job_type import BackgroundJobType
 from testgear_api_client.model.boolean_nullable_test_plan_changed_field_view_model import BooleanNullableTestPlanChangedFieldViewModel
 from testgear_api_client.model.boolean_test_plan_changed_field_view_model import BooleanTestPlanChangedFieldViewModel
 from testgear_api_client.model.boolean_work_item_changed_field_view_model import BooleanWorkItemChangedFieldViewModel
 from testgear_api_client.model.configuration_by_parameters_model import ConfigurationByParametersModel
 from testgear_api_client.model.configuration_model import ConfigurationModel
 from testgear_api_client.model.configuration_post_model import ConfigurationPostModel
 from testgear_api_client.model.configuration_put_model import ConfigurationPutModel
@@ -55,16 +60,16 @@
 from testgear_api_client.model.custom_attribute_search_query_model import CustomAttributeSearchQueryModel
 from testgear_api_client.model.custom_attribute_template_model import CustomAttributeTemplateModel
 from testgear_api_client.model.custom_attribute_template_post_model import CustomAttributeTemplatePostModel
 from testgear_api_client.model.custom_attribute_template_put_model import CustomAttributeTemplatePutModel
 from testgear_api_client.model.custom_attribute_template_search_query_model import CustomAttributeTemplateSearchQueryModel
 from testgear_api_client.model.custom_attribute_test_plan_project_relation_put_model import CustomAttributeTestPlanProjectRelationPutModel
 from testgear_api_client.model.custom_attribute_types_enum import CustomAttributeTypesEnum
-from testgear_api_client.model.date_range_model import DateRangeModel
 from testgear_api_client.model.date_time_range_selector_model import DateTimeRangeSelectorModel
+from testgear_api_client.model.deletion_state import DeletionState
 from testgear_api_client.model.external_link_model import ExternalLinkModel
 from testgear_api_client.model.failure_category_model import FailureCategoryModel
 from testgear_api_client.model.failure_class_model import FailureClassModel
 from testgear_api_client.model.failure_class_regex_model import FailureClassRegexModel
 from testgear_api_client.model.filter_model import FilterModel
 from testgear_api_client.model.flaky_bulk_model import FlakyBulkModel
 from testgear_api_client.model.get_xlsx_test_points_by_test_plan_model import GetXlsxTestPointsByTestPlanModel
@@ -87,14 +92,16 @@
 from testgear_api_client.model.link_put_model import LinkPutModel
 from testgear_api_client.model.link_sub_get_model import LinkSubGetModel
 from testgear_api_client.model.link_type import LinkType
 from testgear_api_client.model.no_content_result import NoContentResult
 from testgear_api_client.model.notification_model import NotificationModel
 from testgear_api_client.model.notification_query_filter_model import NotificationQueryFilterModel
 from testgear_api_client.model.notification_type_model import NotificationTypeModel
+from testgear_api_client.model.operation import Operation
+from testgear_api_client.model.parameter_filter_model import ParameterFilterModel
 from testgear_api_client.model.parameter_group_model import ParameterGroupModel
 from testgear_api_client.model.parameter_iteration_model import ParameterIterationModel
 from testgear_api_client.model.parameter_model import ParameterModel
 from testgear_api_client.model.parameter_post_model import ParameterPostModel
 from testgear_api_client.model.parameter_put_model import ParameterPutModel
 from testgear_api_client.model.parameter_short_model import ParameterShortModel
 from testgear_api_client.model.period_view_model import PeriodViewModel
@@ -105,14 +112,15 @@
 from testgear_api_client.model.project_custom_attributes_templates_filter_model import ProjectCustomAttributesTemplatesFilterModel
 from testgear_api_client.model.project_export_query_model import ProjectExportQueryModel
 from testgear_api_client.model.project_export_with_test_plans_post_model import ProjectExportWithTestPlansPostModel
 from testgear_api_client.model.project_model import ProjectModel
 from testgear_api_client.model.project_post_model import ProjectPostModel
 from testgear_api_client.model.project_put_model import ProjectPutModel
 from testgear_api_client.model.project_shortest_model import ProjectShortestModel
+from testgear_api_client.model.project_test_plans_filter_model import ProjectTestPlansFilterModel
 from testgear_api_client.model.projects_filter_model import ProjectsFilterModel
 from testgear_api_client.model.public_test_point_model import PublicTestPointModel
 from testgear_api_client.model.public_test_run_model import PublicTestRunModel
 from testgear_api_client.model.request_type_model import RequestTypeModel
 from testgear_api_client.model.search_auto_tests_query_includes_model import SearchAutoTestsQueryIncludesModel
 from testgear_api_client.model.search_custom_attribute_template_get_model import SearchCustomAttributeTemplateGetModel
 from testgear_api_client.model.search_webhooks_query_model import SearchWebhooksQueryModel
@@ -145,31 +153,32 @@
 from testgear_api_client.model.test_plan_group_by_test_suite import TestPlanGroupByTestSuite
 from testgear_api_client.model.test_plan_group_by_tester import TestPlanGroupByTester
 from testgear_api_client.model.test_plan_group_by_tester_and_status import TestPlanGroupByTesterAndStatus
 from testgear_api_client.model.test_plan_link import TestPlanLink
 from testgear_api_client.model.test_plan_model import TestPlanModel
 from testgear_api_client.model.test_plan_post_model import TestPlanPostModel
 from testgear_api_client.model.test_plan_put_model import TestPlanPutModel
-from testgear_api_client.model.test_plan_search_query_model import TestPlanSearchQueryModel
 from testgear_api_client.model.test_plan_short_model import TestPlanShortModel
 from testgear_api_client.model.test_plan_status_model import TestPlanStatusModel
 from testgear_api_client.model.test_plan_with_analytic_model import TestPlanWithAnalyticModel
 from testgear_api_client.model.test_plan_with_test_suite_tree_model import TestPlanWithTestSuiteTreeModel
 from testgear_api_client.model.test_point_analytic_result import TestPointAnalyticResult
 from testgear_api_client.model.test_point_by_test_suite_model import TestPointByTestSuiteModel
 from testgear_api_client.model.test_point_change_view_model import TestPointChangeViewModel
 from testgear_api_client.model.test_point_change_view_model_test_plan_changed_field_view_model import TestPointChangeViewModelTestPlanChangedFieldViewModel
 from testgear_api_client.model.test_point_filter_model import TestPointFilterModel
 from testgear_api_client.model.test_point_put_model import TestPointPutModel
 from testgear_api_client.model.test_point_result_model import TestPointResultModel
+from testgear_api_client.model.test_point_select_model import TestPointSelectModel
 from testgear_api_client.model.test_point_selector import TestPointSelector
 from testgear_api_client.model.test_point_short_get_model import TestPointShortGetModel
 from testgear_api_client.model.test_point_short_model import TestPointShortModel
 from testgear_api_client.model.test_point_status import TestPointStatus
 from testgear_api_client.model.test_point_with_last_result_model import TestPointWithLastResultModel
+from testgear_api_client.model.test_points_extraction_model import TestPointsExtractionModel
 from testgear_api_client.model.test_result_change_view_model import TestResultChangeViewModel
 from testgear_api_client.model.test_result_change_view_model_test_plan_changed_field_view_model import TestResultChangeViewModelTestPlanChangedFieldViewModel
 from testgear_api_client.model.test_result_chronology_model import TestResultChronologyModel
 from testgear_api_client.model.test_result_history_report_model import TestResultHistoryReportModel
 from testgear_api_client.model.test_result_model import TestResultModel
 from testgear_api_client.model.test_result_outcome import TestResultOutcome
 from testgear_api_client.model.test_result_short_get_model import TestResultShortGetModel
@@ -198,14 +207,15 @@
 from testgear_api_client.model.test_run_test_results_partial_bulk_set_model import TestRunTestResultsPartialBulkSetModel
 from testgear_api_client.model.test_run_test_results_select_model import TestRunTestResultsSelectModel
 from testgear_api_client.model.test_run_v2_get_model import TestRunV2GetModel
 from testgear_api_client.model.test_run_v2_post_short_model import TestRunV2PostShortModel
 from testgear_api_client.model.test_run_v2_put_model import TestRunV2PutModel
 from testgear_api_client.model.test_suite_change_view_model import TestSuiteChangeViewModel
 from testgear_api_client.model.test_suite_change_view_model_test_plan_changed_field_view_model import TestSuiteChangeViewModelTestPlanChangedFieldViewModel
+from testgear_api_client.model.test_suite_type import TestSuiteType
 from testgear_api_client.model.test_suite_v2_get_model import TestSuiteV2GetModel
 from testgear_api_client.model.test_suite_v2_post_model import TestSuiteV2PostModel
 from testgear_api_client.model.test_suite_v2_put_model import TestSuiteV2PutModel
 from testgear_api_client.model.test_suite_v2_tree_model import TestSuiteV2TreeModel
 from testgear_api_client.model.test_suite_with_children_model import TestSuiteWithChildrenModel
 from testgear_api_client.model.test_suite_work_items_search_model import TestSuiteWorkItemsSearchModel
 from testgear_api_client.model.user_rank_model import UserRankModel
```

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client/rest.py` & `testgear-api-client-3.1.0/src/testgear_api_client/rest.py`

 * *Files identical despite different names*

### Comparing `testgear-api-client-3.0.0/src/testgear_api_client.egg-info/PKG-INFO` & `testgear-api-client-3.1.0/src/testgear_api_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,312 +1,336 @@
-Metadata-Version: 2.1
-Name: testgear-api-client
-Version: 3.0.0
-Summary: API-client for Test Gear
-Home-page: https://pypi.org/project/testgear-api-client/
-Author: Integration team
-Author-email: integrations@test-gear.io
-License: UNKNOWN
-Description: # Api client for Test Gear TMS
-        ![Test Gear](https://raw.githubusercontent.com/testgear-tms/api-client-python/master/images/banner.png)
-        
-        ## Getting Started
-        
-        ### Compatibility
-        
-        | Test Gear | API Client |
-        |-----------|------------|
-        | 3.5       | 2.0        |
-        | 4.0       | 3.0        |
-        
-        ## Installation & Usage
-        ### pip install
-        
-        ```sh
-        pip install testgear-api-client
-        ```
-        
-        Then import the package:
-        
-        ```python
-        import testgear_api_client
-        ```
-        
-        ## Getting Started
-        
-        Please follow the [installation procedure](#installation--usage) and then run the following:
-        
-        ```python
-        import testgear_api_client
-        from testgear_api_client.api import attachments_api
-        from testgear_api_client.model.attachment_model import AttachmentModel
-        from testgear_api_client.model.image_resize_type import ImageResizeType
-        from testgear_api_client.model.problem_details import ProblemDetails
-        from testgear_api_client.model.validation_problem_details import ValidationProblemDetails
-        
-        configuration = testgear_api_client.Configuration(
-            host = "Your TMS address"
-        )
-        
-        with testgear_api_client.ApiClient(
-                configuration,
-                header_name='Authorization',
-                header_value='PrivateToken ' + 'Your private token') as api_client:
-            api_instance = attachments_api.AttachmentsApi(api_client)
-            id = "Attachment's guid in the TMS"
-        
-            try:
-                api_instance.api_v2_attachments_id_delete(id)
-            except testgear_api_client.ApiException as e:
-                print("Exception when calling AttachmentsApi->api_v2_attachments_id_delete: %s\n" % e)
-        ```
-        
-        ## Documentation for API Endpoints
-        
-        All URIs are relative to *http://localhost*
-        
-        Class | Method | HTTP request | Description
-        ------------ | ------------- | ------------- | -------------
-        *AttachmentsApi* | [**api_v2_attachments_id_delete**](docs/AttachmentsApi.md#api_v2_attachments_id_delete) | **DELETE** /api/v2/attachments/{id} | Delete attachment file
-        *AttachmentsApi* | [**api_v2_attachments_id_get**](docs/AttachmentsApi.md#api_v2_attachments_id_get) | **GET** /api/v2/attachments/{id} | Download attachment file
-        *AttachmentsApi* | [**api_v2_attachments_occupied_file_storage_size_get**](docs/AttachmentsApi.md#api_v2_attachments_occupied_file_storage_size_get) | **GET** /api/v2/attachments/occupiedFileStorageSize | Get size of attachments storage in bytes
-        *AttachmentsApi* | [**api_v2_attachments_post**](docs/AttachmentsApi.md#api_v2_attachments_post) | **POST** /api/v2/attachments | Upload new attachment file
-        *AutoTestsApi* | [**api_v2_auto_tests_flaky_bulk_post**](docs/AutoTestsApi.md#api_v2_auto_tests_flaky_bulk_post) | **POST** /api/v2/autoTests/flaky/bulk | Set \&quot;Flaky\&quot; status for multiple autotests
-        *AutoTestsApi* | [**api_v2_auto_tests_id_test_results_search_post**](docs/AutoTestsApi.md#api_v2_auto_tests_id_test_results_search_post) | **POST** /api/v2/autoTests/{id}/testResults/search | Get test results history for autotest
-        *AutoTestsApi* | [**api_v2_auto_tests_id_work_items_changed_id_get**](docs/AutoTestsApi.md#api_v2_auto_tests_id_work_items_changed_id_get) | **GET** /api/v2/autoTests/{id}/workItems/changed/id | Get identifiers of changed linked work items
-        *AutoTestsApi* | [**api_v2_auto_tests_id_work_items_changed_work_item_id_approve_post**](docs/AutoTestsApi.md#api_v2_auto_tests_id_work_items_changed_work_item_id_approve_post) | **POST** /api/v2/autoTests/{id}/workItems/changed/{workItemId}/approve | Approve changes to work items linked to autotest
-        *AutoTestsApi* | [**api_v2_auto_tests_search_post**](docs/AutoTestsApi.md#api_v2_auto_tests_search_post) | **POST** /api/v2/autoTests/search | Search for autotests
-        *AutoTestsApi* | [**create_auto_test**](docs/AutoTestsApi.md#create_auto_test) | **POST** /api/v2/autoTests | Create autotest
-        *AutoTestsApi* | [**create_multiple**](docs/AutoTestsApi.md#create_multiple) | **POST** /api/v2/autoTests/bulk | Create multiple autotests
-        *AutoTestsApi* | [**delete_auto_test**](docs/AutoTestsApi.md#delete_auto_test) | **DELETE** /api/v2/autoTests/{id} | Delete autotest
-        *AutoTestsApi* | [**delete_auto_test_link_from_work_item**](docs/AutoTestsApi.md#delete_auto_test_link_from_work_item) | **DELETE** /api/v2/autoTests/{id}/workItems | Unlink autotest from work item
-        *AutoTestsApi* | [**get_all_auto_tests**](docs/AutoTestsApi.md#get_all_auto_tests) | **GET** /api/v2/autoTests | 
-        *AutoTestsApi* | [**get_auto_test_average_duration**](docs/AutoTestsApi.md#get_auto_test_average_duration) | **GET** /api/v2/autoTests/{id}/averageDuration | Get average autotest duration
-        *AutoTestsApi* | [**get_auto_test_by_id**](docs/AutoTestsApi.md#get_auto_test_by_id) | **GET** /api/v2/autoTests/{id} | Get autotest by internal or global ID
-        *AutoTestsApi* | [**get_auto_test_chronology**](docs/AutoTestsApi.md#get_auto_test_chronology) | **GET** /api/v2/autoTests/{id}/chronology | Get autotest chronology
-        *AutoTestsApi* | [**get_test_runs**](docs/AutoTestsApi.md#get_test_runs) | **GET** /api/v2/autoTests/{id}/testRuns | Get completed tests runs for autotests
-        *AutoTestsApi* | [**get_work_item_results**](docs/AutoTestsApi.md#get_work_item_results) | **GET** /api/v2/autoTests/{id}/testResultHistory | 
-        *AutoTestsApi* | [**get_work_items_linked_to_auto_test**](docs/AutoTestsApi.md#get_work_items_linked_to_auto_test) | **GET** /api/v2/autoTests/{id}/workItems | Get work items linked to autotest
-        *AutoTestsApi* | [**link_auto_test_to_work_item**](docs/AutoTestsApi.md#link_auto_test_to_work_item) | **POST** /api/v2/autoTests/{id}/workItems | Link autotest with work items
-        *AutoTestsApi* | [**update_auto_test**](docs/AutoTestsApi.md#update_auto_test) | **PUT** /api/v2/autoTests | Update autotest
-        *AutoTestsApi* | [**update_multiple**](docs/AutoTestsApi.md#update_multiple) | **PUT** /api/v2/autoTests/bulk | Update multiple autotests
-        *ConfigurationsApi* | [**api_v2_configurations_create_by_parameters_post**](docs/ConfigurationsApi.md#api_v2_configurations_create_by_parameters_post) | **POST** /api/v2/configurations/createByParameters | Create Configurations by parameters
-        *ConfigurationsApi* | [**api_v2_configurations_search_post**](docs/ConfigurationsApi.md#api_v2_configurations_search_post) | **POST** /api/v2/configurations/search | Search for configurations
-        *ConfigurationsApi* | [**create_configuration**](docs/ConfigurationsApi.md#create_configuration) | **POST** /api/v2/configurations | Create Configuration
-        *ConfigurationsApi* | [**get_configuration_by_id**](docs/ConfigurationsApi.md#get_configuration_by_id) | **GET** /api/v2/configurations/{id} | Get configuration by internal or global ID
-        *ConfigurationsApi* | [**update_configuration**](docs/ConfigurationsApi.md#update_configuration) | **PUT** /api/v2/configurations | Update Configuration
-        *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_custom_attributes_exclude_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_custom_attributes_exclude_post) | **POST** /api/v2/customAttributes/templates/{id}/customAttributes/exclude | Exclude CustomAttributes from CustomAttributeTemplate
-        *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_custom_attributes_include_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_custom_attributes_include_post) | **POST** /api/v2/customAttributes/templates/{id}/customAttributes/include | Include CustomAttributes to CustomAttributeTemplate
-        *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_delete**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_delete) | **DELETE** /api/v2/customAttributes/templates/{id} | Delete CustomAttributeTemplate
-        *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_get**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_get) | **GET** /api/v2/customAttributes/templates/{id} | Get CustomAttributeTemplate by ID
-        *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_name_get**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_name_get) | **GET** /api/v2/customAttributes/templates/{name} | Get CustomAttributeTemplate by name
-        *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_post) | **POST** /api/v2/customAttributes/templates | Create CustomAttributeTemplate
-        *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_put**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_put) | **PUT** /api/v2/customAttributes/templates | Update custom attributes template
-        *CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_search_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_search_post) | **POST** /api/v2/customAttributes/templates/search | Search CustomAttributeTemplates
-        *CustomAttributesApi* | [**api_v2_custom_attributes_global_id_delete**](docs/CustomAttributesApi.md#api_v2_custom_attributes_global_id_delete) | **DELETE** /api/v2/customAttributes/global/{id} | Delete global attribute
-        *CustomAttributesApi* | [**api_v2_custom_attributes_global_id_put**](docs/CustomAttributesApi.md#api_v2_custom_attributes_global_id_put) | **PUT** /api/v2/customAttributes/global/{id} | Edit global attribute
-        *CustomAttributesApi* | [**api_v2_custom_attributes_global_post**](docs/CustomAttributesApi.md#api_v2_custom_attributes_global_post) | **POST** /api/v2/customAttributes/global | Create global attribute
-        *CustomAttributesApi* | [**api_v2_custom_attributes_id_get**](docs/CustomAttributesApi.md#api_v2_custom_attributes_id_get) | **GET** /api/v2/customAttributes/{id} | Get attribute
-        *CustomAttributesApi* | [**api_v2_custom_attributes_search_post**](docs/CustomAttributesApi.md#api_v2_custom_attributes_search_post) | **POST** /api/v2/customAttributes/search | Search for attributes
-        *NotificationsApi* | [**api_v2_notifications_count_get**](docs/NotificationsApi.md#api_v2_notifications_count_get) | **GET** /api/v2/notifications/count | Get unread Notifications total in last 7 days
-        *NotificationsApi* | [**api_v2_notifications_get**](docs/NotificationsApi.md#api_v2_notifications_get) | **GET** /api/v2/notifications | Get all Notifications for current User
-        *NotificationsApi* | [**api_v2_notifications_id_read_post**](docs/NotificationsApi.md#api_v2_notifications_id_read_post) | **POST** /api/v2/notifications/{id}/read | Set Notification as read
-        *NotificationsApi* | [**api_v2_notifications_read_post**](docs/NotificationsApi.md#api_v2_notifications_read_post) | **POST** /api/v2/notifications/read | Set all Notifications as read
-        *NotificationsApi* | [**api_v2_notifications_search_post**](docs/NotificationsApi.md#api_v2_notifications_search_post) | **POST** /api/v2/notifications/search | Search Notifications for current User
-        *ParametersApi* | [**api_v2_parameters_bulk_post**](docs/ParametersApi.md#api_v2_parameters_bulk_post) | **POST** /api/v2/parameters/bulk | Create multiple parameters
-        *ParametersApi* | [**api_v2_parameters_bulk_put**](docs/ParametersApi.md#api_v2_parameters_bulk_put) | **PUT** /api/v2/parameters/bulk | Update multiple parameters
-        *ParametersApi* | [**api_v2_parameters_groups_get**](docs/ParametersApi.md#api_v2_parameters_groups_get) | **GET** /api/v2/parameters/groups | Get parameters as group
-        *ParametersApi* | [**api_v2_parameters_key_name_name_exists_get**](docs/ParametersApi.md#api_v2_parameters_key_name_name_exists_get) | **GET** /api/v2/parameters/key/name/{name}/exists | Check existence parameter key in system
-        *ParametersApi* | [**api_v2_parameters_key_values_get**](docs/ParametersApi.md#api_v2_parameters_key_values_get) | **GET** /api/v2/parameters/{key}/values | Get all parameter key values
-        *ParametersApi* | [**api_v2_parameters_keys_get**](docs/ParametersApi.md#api_v2_parameters_keys_get) | **GET** /api/v2/parameters/keys | Get all parameter keys
-        *ParametersApi* | [**create_parameter**](docs/ParametersApi.md#create_parameter) | **POST** /api/v2/parameters | Create parameter
-        *ParametersApi* | [**delete_by_name**](docs/ParametersApi.md#delete_by_name) | **DELETE** /api/v2/parameters/name/{name} | Delete parameter by name
-        *ParametersApi* | [**delete_by_parameter_key_id**](docs/ParametersApi.md#delete_by_parameter_key_id) | **DELETE** /api/v2/parameters/keyId/{keyId} | Delete parameters by parameter key identifier
-        *ParametersApi* | [**delete_parameter**](docs/ParametersApi.md#delete_parameter) | **DELETE** /api/v2/parameters/{id} | Delete parameter
-        *ParametersApi* | [**get_all_parameters**](docs/ParametersApi.md#get_all_parameters) | **GET** /api/v2/parameters | Get all parameters
-        *ParametersApi* | [**get_parameter_by_id**](docs/ParametersApi.md#get_parameter_by_id) | **GET** /api/v2/parameters/{id} | Get parameter by ID
-        *ParametersApi* | [**obsolete_delete_by_name**](docs/ParametersApi.md#obsolete_delete_by_name) | **POST** /api/v2/parameters/deleteByName | 
-        *ParametersApi* | [**update_parameter**](docs/ParametersApi.md#update_parameter) | **PUT** /api/v2/parameters | Update parameter
-        *ProjectsApi* | [**add_globa_attributes_to_project**](docs/ProjectsApi.md#add_globa_attributes_to_project) | **POST** /api/v2/projects/{id}/globalAttributes | Add global attributes to project
-        *ProjectsApi* | [**api_v2_projects_id_attributes_templates_search_post**](docs/ProjectsApi.md#api_v2_projects_id_attributes_templates_search_post) | **POST** /api/v2/projects/{id}/attributes/templates/search | Search for custom attributes templates
-        *ProjectsApi* | [**api_v2_projects_id_attributes_templates_template_id_delete**](docs/ProjectsApi.md#api_v2_projects_id_attributes_templates_template_id_delete) | **DELETE** /api/v2/projects/{id}/attributes/templates/{templateId} | Delete CustomAttributeTemplate from Project
-        *ProjectsApi* | [**api_v2_projects_id_attributes_templates_template_id_post**](docs/ProjectsApi.md#api_v2_projects_id_attributes_templates_template_id_post) | **POST** /api/v2/projects/{id}/attributes/templates/{templateId} | Add CustomAttributeTemplate to Project
-        *ProjectsApi* | [**api_v2_projects_id_failure_classes_get**](docs/ProjectsApi.md#api_v2_projects_id_failure_classes_get) | **GET** /api/v2/projects/{id}/failureClasses | Get Project FailureClasses
-        *ProjectsApi* | [**api_v2_projects_id_favorite_put**](docs/ProjectsApi.md#api_v2_projects_id_favorite_put) | **PUT** /api/v2/projects/{id}/favorite | Mark Project as favorite
-        *ProjectsApi* | [**api_v2_projects_id_filters_get**](docs/ProjectsApi.md#api_v2_projects_id_filters_get) | **GET** /api/v2/projects/{id}/filters | Get Project filters
-        *ProjectsApi* | [**api_v2_projects_id_test_plans_analytics_get**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_analytics_get) | **GET** /api/v2/projects/{id}/testPlans/analytics | Get TestPlans analytics
-        *ProjectsApi* | [**api_v2_projects_id_test_plans_name_exists_get**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_name_exists_get) | **GET** /api/v2/projects/{id}/testPlans/{name}/exists | Checks if TestPlan exists with the specified name exists for the project
-        *ProjectsApi* | [**api_v2_projects_id_test_plans_search_post**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_search_post) | **POST** /api/v2/projects/{id}/testPlans/search | Get Project TestPlans with analytics
-        *ProjectsApi* | [**api_v2_projects_id_test_runs_active_get**](docs/ProjectsApi.md#api_v2_projects_id_test_runs_active_get) | **GET** /api/v2/projects/{id}/testRuns/active | Get active Project TestRuns
-        *ProjectsApi* | [**api_v2_projects_id_test_runs_full_get**](docs/ProjectsApi.md#api_v2_projects_id_test_runs_full_get) | **GET** /api/v2/projects/{id}/testRuns/full | Get Project TestRuns full models
-        *ProjectsApi* | [**api_v2_projects_id_work_items_search_id_post**](docs/ProjectsApi.md#api_v2_projects_id_work_items_search_id_post) | **POST** /api/v2/projects/{id}/workItems/search/id | Search for work items and extract IDs only
-        *ProjectsApi* | [**api_v2_projects_id_work_items_search_post**](docs/ProjectsApi.md#api_v2_projects_id_work_items_search_post) | **POST** /api/v2/projects/{id}/workItems/search | Search for work items
-        *ProjectsApi* | [**api_v2_projects_id_work_items_tags_get**](docs/ProjectsApi.md#api_v2_projects_id_work_items_tags_get) | **GET** /api/v2/projects/{id}/workItems/tags | Get WorkItems Tags
-        *ProjectsApi* | [**api_v2_projects_name_name_exists_get**](docs/ProjectsApi.md#api_v2_projects_name_name_exists_get) | **GET** /api/v2/projects/name/{name}/exists | 
-        *ProjectsApi* | [**api_v2_projects_search_post**](docs/ProjectsApi.md#api_v2_projects_search_post) | **POST** /api/v2/projects/search | Search for projects
-        *ProjectsApi* | [**call_import**](docs/ProjectsApi.md#call_import) | **POST** /api/v2/projects/import | Import project from JSON file
-        *ProjectsApi* | [**create_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#create_custom_attribute_test_plan_project_relations) | **POST** /api/v2/projects/{id}/testPlans/attributes | Add attributes to project&#39;s test plans
-        *ProjectsApi* | [**create_project**](docs/ProjectsApi.md#create_project) | **POST** /api/v2/projects | Create project
-        *ProjectsApi* | [**create_projects_attribute**](docs/ProjectsApi.md#create_projects_attribute) | **POST** /api/v2/projects/{id}/attributes | Create project attribute
-        *ProjectsApi* | [**delete_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#delete_custom_attribute_test_plan_project_relations) | **DELETE** /api/v2/projects/{id}/testPlans/attribute/{attributeId} | Delete attribute from project&#39;s test plans
-        *ProjectsApi* | [**delete_project**](docs/ProjectsApi.md#delete_project) | **DELETE** /api/v2/projects/{id} | Delete project
-        *ProjectsApi* | [**delete_project_auto_tests**](docs/ProjectsApi.md#delete_project_auto_tests) | **DELETE** /api/v2/projects/{id}/autoTests | Delete project
-        *ProjectsApi* | [**delete_projects_attribute**](docs/ProjectsApi.md#delete_projects_attribute) | **DELETE** /api/v2/projects/{id}/attributes/{attributeId} | Delete project attribute
-        *ProjectsApi* | [**export**](docs/ProjectsApi.md#export) | **POST** /api/v2/projects/{id}/export | Export project as JSON file
-        *ProjectsApi* | [**export_with_test_plans_and_configurations**](docs/ProjectsApi.md#export_with_test_plans_and_configurations) | **POST** /api/v2/projects/{id}/export-by-testPlans | Export project with test plans, test suites and test points as JSON file
-        *ProjectsApi* | [**get_all_projects**](docs/ProjectsApi.md#get_all_projects) | **GET** /api/v2/projects | Get all projects
-        *ProjectsApi* | [**get_attribute_by_project_id**](docs/ProjectsApi.md#get_attribute_by_project_id) | **GET** /api/v2/projects/{id}/attributes/{attributeId} | Get project attribute
-        *ProjectsApi* | [**get_attributes_by_project_id**](docs/ProjectsApi.md#get_attributes_by_project_id) | **GET** /api/v2/projects/{id}/attributes | Get project attributes
-        *ProjectsApi* | [**get_auto_tests_namespaces**](docs/ProjectsApi.md#get_auto_tests_namespaces) | **GET** /api/v2/projects/{id}/autoTestsNamespaces | Get namespaces of autotests in project
-        *ProjectsApi* | [**get_configurations_by_project_id**](docs/ProjectsApi.md#get_configurations_by_project_id) | **GET** /api/v2/projects/{id}/configurations | Get project configurations
-        *ProjectsApi* | [**get_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#get_custom_attribute_test_plan_project_relations) | **GET** /api/v2/projects/{id}/testPlans/attributes | Get project&#39;s test plan attributes
-        *ProjectsApi* | [**get_project_by_id**](docs/ProjectsApi.md#get_project_by_id) | **GET** /api/v2/projects/{id} | Get project by ID
-        *ProjectsApi* | [**get_sections_by_project_id**](docs/ProjectsApi.md#get_sections_by_project_id) | **GET** /api/v2/projects/{id}/sections | Get project sections
-        *ProjectsApi* | [**get_test_plans_by_project_id**](docs/ProjectsApi.md#get_test_plans_by_project_id) | **GET** /api/v2/projects/{id}/testPlans | Get project test plans
-        *ProjectsApi* | [**get_test_runs_by_project_id**](docs/ProjectsApi.md#get_test_runs_by_project_id) | **GET** /api/v2/projects/{id}/testRuns | Get project test runs
-        *ProjectsApi* | [**get_work_items_by_project_id**](docs/ProjectsApi.md#get_work_items_by_project_id) | **GET** /api/v2/projects/{id}/workItems | Get project work items
-        *ProjectsApi* | [**import_to_existing_project**](docs/ProjectsApi.md#import_to_existing_project) | **POST** /api/v2/projects/{id}/import | Import project from JSON file into existing project
-        *ProjectsApi* | [**restore_project**](docs/ProjectsApi.md#restore_project) | **POST** /api/v2/projects/{id}/restore | Restore project
-        *ProjectsApi* | [**search_attributes_in_project**](docs/ProjectsApi.md#search_attributes_in_project) | **POST** /api/v2/projects/{id}/attributes/search | Search for attributes used in the project
-        *ProjectsApi* | [**search_test_plan_attributes_in_project**](docs/ProjectsApi.md#search_test_plan_attributes_in_project) | **POST** /api/v2/projects/{id}/testPlans/attributes/search | Search for attributes used in the project test plans
-        *ProjectsApi* | [**update_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#update_custom_attribute_test_plan_project_relations) | **PUT** /api/v2/projects/{id}/testPlans/attribute | Update attribute of project&#39;s test plans
-        *ProjectsApi* | [**update_project**](docs/ProjectsApi.md#update_project) | **PUT** /api/v2/projects | Update project
-        *ProjectsApi* | [**update_projects_attribute**](docs/ProjectsApi.md#update_projects_attribute) | **PUT** /api/v2/projects/{id}/attributes | Edit attribute of the project
-        *SectionsApi* | [**create_section**](docs/SectionsApi.md#create_section) | **POST** /api/v2/sections | Create section
-        *SectionsApi* | [**delete_section**](docs/SectionsApi.md#delete_section) | **DELETE** /api/v2/sections/{id} | Delete section
-        *SectionsApi* | [**get_section_by_id**](docs/SectionsApi.md#get_section_by_id) | **GET** /api/v2/sections/{id} | Get section
-        *SectionsApi* | [**get_work_items_by_section_id**](docs/SectionsApi.md#get_work_items_by_section_id) | **GET** /api/v2/sections/{id}/workItems | Get section work items
-        *SectionsApi* | [**move**](docs/SectionsApi.md#move) | **POST** /api/v2/sections/move | Move section with all work items into another section
-        *SectionsApi* | [**rename**](docs/SectionsApi.md#rename) | **POST** /api/v2/sections/rename | Rename section
-        *SectionsApi* | [**update_section**](docs/SectionsApi.md#update_section) | **PUT** /api/v2/sections | Update section
-        *TagsApi* | [**api_v2_tags_get**](docs/TagsApi.md#api_v2_tags_get) | **GET** /api/v2/tags | Get all Tags
-        *TagsApi* | [**api_v2_tags_test_plans_tags_get**](docs/TagsApi.md#api_v2_tags_test_plans_tags_get) | **GET** /api/v2/tags/testPlansTags | Get all Tags that are used in TestPlans
-        *TestPlansApi* | [**add_test_points_with_sections**](docs/TestPlansApi.md#add_test_points_with_sections) | **POST** /api/v2/testPlans/{id}/test-points/withSections | Add test-points to TestPlan with sections
-        *TestPlansApi* | [**add_work_items_with_sections**](docs/TestPlansApi.md#add_work_items_with_sections) | **POST** /api/v2/testPlans/{id}/workItems/withSections | Add WorkItems to TestPlan with Sections as TestSuites
-        *TestPlansApi* | [**api_v2_test_plans_id_analytics_get**](docs/TestPlansApi.md#api_v2_test_plans_id_analytics_get) | **GET** /api/v2/testPlans/{id}/analytics | Get analytics by TestPlan
-        *TestPlansApi* | [**api_v2_test_plans_id_autobalance_post**](docs/TestPlansApi.md#api_v2_test_plans_id_autobalance_post) | **POST** /api/v2/testPlans/{id}/autobalance | Distribute test points between the users
-        *TestPlansApi* | [**api_v2_test_plans_id_configurations_get**](docs/TestPlansApi.md#api_v2_test_plans_id_configurations_get) | **GET** /api/v2/testPlans/{id}/configurations | Get TestPlan configurations
-        *TestPlansApi* | [**api_v2_test_plans_id_export_test_points_xlsx_post**](docs/TestPlansApi.md#api_v2_test_plans_id_export_test_points_xlsx_post) | **POST** /api/v2/testPlans/{id}/export/testPoints/xlsx | Export TestPoints from TestPlan in xls format
-        *TestPlansApi* | [**api_v2_test_plans_id_export_test_result_history_xlsx_post**](docs/TestPlansApi.md#api_v2_test_plans_id_export_test_result_history_xlsx_post) | **POST** /api/v2/testPlans/{id}/export/testResultHistory/xlsx | Export TestResults history from TestPlan in xls format
-        *TestPlansApi* | [**api_v2_test_plans_id_history_get**](docs/TestPlansApi.md#api_v2_test_plans_id_history_get) | **GET** /api/v2/testPlans/{id}/history | Get TestPlan history
-        *TestPlansApi* | [**api_v2_test_plans_id_links_get**](docs/TestPlansApi.md#api_v2_test_plans_id_links_get) | **GET** /api/v2/testPlans/{id}/links | Get Links of TestPlan
-        *TestPlansApi* | [**api_v2_test_plans_id_test_points_last_results_get**](docs/TestPlansApi.md#api_v2_test_plans_id_test_points_last_results_get) | **GET** /api/v2/testPlans/{id}/testPoints/lastResults | Get TestPoints with last result from TestPlan
-        *TestPlansApi* | [**api_v2_test_plans_id_test_points_reset_post**](docs/TestPlansApi.md#api_v2_test_plans_id_test_points_reset_post) | **POST** /api/v2/testPlans/{id}/testPoints/reset | Reset TestPoints status of TestPlan
-        *TestPlansApi* | [**api_v2_test_plans_id_test_runs_get**](docs/TestPlansApi.md#api_v2_test_plans_id_test_runs_get) | **GET** /api/v2/testPlans/{id}/testRuns | Get TestRuns of TestPlan
-        *TestPlansApi* | [**api_v2_test_plans_id_test_runs_search_post**](docs/TestPlansApi.md#api_v2_test_plans_id_test_runs_search_post) | **POST** /api/v2/testPlans/{id}/testRuns/search | Search TestRuns of TestPlan
-        *TestPlansApi* | [**api_v2_test_plans_id_test_runs_test_results_last_modified_modified_date_get**](docs/TestPlansApi.md#api_v2_test_plans_id_test_runs_test_results_last_modified_modified_date_get) | **GET** /api/v2/testPlans/{id}/testRuns/testResults/lastModified/modifiedDate | Get last modification date of test plan&#39;s test results
-        *TestPlansApi* | [**api_v2_test_plans_id_unlock_request_post**](docs/TestPlansApi.md#api_v2_test_plans_id_unlock_request_post) | **POST** /api/v2/testPlans/{id}/unlock/request | Send unlock TestPlan notification
-        *TestPlansApi* | [**api_v2_test_plans_shorts_post**](docs/TestPlansApi.md#api_v2_test_plans_shorts_post) | **POST** /api/v2/testPlans/shorts | Get TestPlans short models by Project identifiers
-        *TestPlansApi* | [**clone**](docs/TestPlansApi.md#clone) | **POST** /api/v2/testPlans/{id}/clone | Clone TestPlan
-        *TestPlansApi* | [**complete**](docs/TestPlansApi.md#complete) | **POST** /api/v2/testPlans/{id}/complete | Complete TestPlan
-        *TestPlansApi* | [**create_test_plan**](docs/TestPlansApi.md#create_test_plan) | **POST** /api/v2/testPlans | Create TestPlan
-        *TestPlansApi* | [**delete_test_plan**](docs/TestPlansApi.md#delete_test_plan) | **DELETE** /api/v2/testPlans/{id} | Delete TestPlan
-        *TestPlansApi* | [**get_test_plan_by_id**](docs/TestPlansApi.md#get_test_plan_by_id) | **GET** /api/v2/testPlans/{id} | Get TestPlan by Id
-        *TestPlansApi* | [**get_test_suites_by_id**](docs/TestPlansApi.md#get_test_suites_by_id) | **GET** /api/v2/testPlans/{id}/testSuites | Get TestSuites Tree By Id
-        *TestPlansApi* | [**pause**](docs/TestPlansApi.md#pause) | **POST** /api/v2/testPlans/{id}/pause | Pause TestPlan
-        *TestPlansApi* | [**restore_test_plan**](docs/TestPlansApi.md#restore_test_plan) | **POST** /api/v2/testPlans/{id}/restore | Restore TestPlan
-        *TestPlansApi* | [**start**](docs/TestPlansApi.md#start) | **POST** /api/v2/testPlans/{id}/start | Start TestPlan
-        *TestPlansApi* | [**update_test_plan**](docs/TestPlansApi.md#update_test_plan) | **PUT** /api/v2/testPlans | Update TestPlan
-        *TestPointsApi* | [**api_v2_test_points_id_test_runs_get**](docs/TestPointsApi.md#api_v2_test_points_id_test_runs_get) | **GET** /api/v2/testPoints/{id}/testRuns | Get all test runs which use test point
-        *TestPointsApi* | [**api_v2_test_points_id_work_item_get**](docs/TestPointsApi.md#api_v2_test_points_id_work_item_get) | **GET** /api/v2/testPoints/{id}/workItem | Get work item represented by test point
-        *TestPointsApi* | [**api_v2_test_points_search_id_post**](docs/TestPointsApi.md#api_v2_test_points_search_id_post) | **POST** /api/v2/testPoints/search/id | Search for test points and extract IDs only
-        *TestPointsApi* | [**api_v2_test_points_search_post**](docs/TestPointsApi.md#api_v2_test_points_search_post) | **POST** /api/v2/testPoints/search | Search for test points
-        *TestResultsApi* | [**api_v2_test_results_id_aggregated_get**](docs/TestResultsApi.md#api_v2_test_results_id_aggregated_get) | **GET** /api/v2/testResults/{id}/aggregated | Get test result by ID aggregated with previous results
-        *TestResultsApi* | [**api_v2_test_results_id_attachments_attachment_id_put**](docs/TestResultsApi.md#api_v2_test_results_id_attachments_attachment_id_put) | **PUT** /api/v2/testResults/{id}/attachments/{attachmentId} | Attach file to the test result
-        *TestResultsApi* | [**api_v2_test_results_id_attachments_info_get**](docs/TestResultsApi.md#api_v2_test_results_id_attachments_info_get) | **GET** /api/v2/testResults/{id}/attachments/info | Get test result attachments meta-information
-        *TestResultsApi* | [**api_v2_test_results_id_get**](docs/TestResultsApi.md#api_v2_test_results_id_get) | **GET** /api/v2/testResults/{id} | Get test result by ID
-        *TestResultsApi* | [**api_v2_test_results_id_put**](docs/TestResultsApi.md#api_v2_test_results_id_put) | **PUT** /api/v2/testResults/{id} | Edit test result by ID
-        *TestResultsApi* | [**api_v2_test_results_search_post**](docs/TestResultsApi.md#api_v2_test_results_search_post) | **POST** /api/v2/testResults/search | Search for test results
-        *TestResultsApi* | [**api_v2_test_results_statistics_filter_post**](docs/TestResultsApi.md#api_v2_test_results_statistics_filter_post) | **POST** /api/v2/testResults/statistics/filter | Search for test results and extract statistics
-        *TestResultsApi* | [**create_attachment**](docs/TestResultsApi.md#create_attachment) | **POST** /api/v2/testResults/{id}/attachments | Upload and link attachment to TestResult
-        *TestResultsApi* | [**delete_attachment**](docs/TestResultsApi.md#delete_attachment) | **DELETE** /api/v2/testResults/{id}/attachments/{attachmentId} | Remove attachment and unlink from TestResult
-        *TestResultsApi* | [**download_attachment**](docs/TestResultsApi.md#download_attachment) | **GET** /api/v2/testResults/{id}/attachments/{attachmentId} | Get attachment of TestResult
-        *TestResultsApi* | [**get_attachment**](docs/TestResultsApi.md#get_attachment) | **GET** /api/v2/testResults/{id}/attachments/{attachmentId}/info | Get Metadata of TestResult&#39;s attachment
-        *TestResultsApi* | [**get_attachments**](docs/TestResultsApi.md#get_attachments) | **GET** /api/v2/testResults/{id}/attachments | Get all attachments of TestResult
-        *TestRunsApi* | [**api_v2_test_runs_id_statistics_filter_post**](docs/TestRunsApi.md#api_v2_test_runs_id_statistics_filter_post) | **POST** /api/v2/testRuns/{id}/statistics/filter | Search for the test run test results and build statistics
-        *TestRunsApi* | [**api_v2_test_runs_id_test_points_results_get**](docs/TestRunsApi.md#api_v2_test_runs_id_test_points_results_get) | **GET** /api/v2/testRuns/{id}/testPoints/results | Get test results from the test run grouped by test points
-        *TestRunsApi* | [**api_v2_test_runs_id_test_results_bulk_put**](docs/TestRunsApi.md#api_v2_test_runs_id_test_results_bulk_put) | **PUT** /api/v2/testRuns/{id}/testResults/bulk | Partial edit of multiple test results in the test run
-        *TestRunsApi* | [**api_v2_test_runs_id_test_results_last_modified_modification_date_get**](docs/TestRunsApi.md#api_v2_test_runs_id_test_results_last_modified_modification_date_get) | **GET** /api/v2/testRuns/{id}/testResults/lastModified/modificationDate | Get modification date of last test result of the test run
-        *TestRunsApi* | [**api_v2_test_runs_search_post**](docs/TestRunsApi.md#api_v2_test_runs_search_post) | **POST** /api/v2/testRuns/search | Search for test runs
-        *TestRunsApi* | [**complete_test_run**](docs/TestRunsApi.md#complete_test_run) | **POST** /api/v2/testRuns/{id}/complete | Complete TestRun
-        *TestRunsApi* | [**create_and_fill_by_auto_tests**](docs/TestRunsApi.md#create_and_fill_by_auto_tests) | **POST** /api/v2/testRuns/byAutoTests | Create test runs based on autotests and configurations
-        *TestRunsApi* | [**create_and_fill_by_configurations**](docs/TestRunsApi.md#create_and_fill_by_configurations) | **POST** /api/v2/testRuns/byConfigurations | Create test runs picking the needed test points
-        *TestRunsApi* | [**create_and_fill_by_work_items**](docs/TestRunsApi.md#create_and_fill_by_work_items) | **POST** /api/v2/testRuns/byWorkItems | Create test run based on configurations and work items
-        *TestRunsApi* | [**create_empty**](docs/TestRunsApi.md#create_empty) | **POST** /api/v2/testRuns | Create empty TestRun
-        *TestRunsApi* | [**get_test_run_by_id**](docs/TestRunsApi.md#get_test_run_by_id) | **GET** /api/v2/testRuns/{id} | Get TestRun by Id
-        *TestRunsApi* | [**set_auto_test_results_for_test_run**](docs/TestRunsApi.md#set_auto_test_results_for_test_run) | **POST** /api/v2/testRuns/{id}/testResults | Send test results to the test runs in the system
-        *TestRunsApi* | [**start_test_run**](docs/TestRunsApi.md#start_test_run) | **POST** /api/v2/testRuns/{id}/start | Start TestRun
-        *TestRunsApi* | [**stop_test_run**](docs/TestRunsApi.md#stop_test_run) | **POST** /api/v2/testRuns/{id}/stop | Stop TestRun
-        *TestRunsApi* | [**update_empty**](docs/TestRunsApi.md#update_empty) | **PUT** /api/v2/testRuns | Update empty TestRun
-        *TestSuitesApi* | [**add_test_points_to_test_suite**](docs/TestSuitesApi.md#add_test_points_to_test_suite) | **POST** /api/v2/testSuites/{id}/test-points | Add test-points to test suite
-        *TestSuitesApi* | [**create_test_suite**](docs/TestSuitesApi.md#create_test_suite) | **POST** /api/v2/testSuites | Create TestSuite
-        *TestSuitesApi* | [**delete_test_suite**](docs/TestSuitesApi.md#delete_test_suite) | **DELETE** /api/v2/testSuites/{id} | Delete TestSuite
-        *TestSuitesApi* | [**get_configurations_by_test_suite_id**](docs/TestSuitesApi.md#get_configurations_by_test_suite_id) | **GET** /api/v2/testSuites/{id}/configurations | Get Configurations By Id
-        *TestSuitesApi* | [**get_test_points_by_id**](docs/TestSuitesApi.md#get_test_points_by_id) | **GET** /api/v2/testSuites/{id}/testPoints | Get TestPoints By Id
-        *TestSuitesApi* | [**get_test_results_by_id**](docs/TestSuitesApi.md#get_test_results_by_id) | **GET** /api/v2/testSuites/{id}/testResults | Get TestResults By Id
-        *TestSuitesApi* | [**get_test_suite_by_id**](docs/TestSuitesApi.md#get_test_suite_by_id) | **GET** /api/v2/testSuites/{id} | Get TestSuite by Id
-        *TestSuitesApi* | [**get_work_items_by_id**](docs/TestSuitesApi.md#get_work_items_by_id) | **GET** /api/v2/testSuites/{id}/workItems | 
-        *TestSuitesApi* | [**search_work_items**](docs/TestSuitesApi.md#search_work_items) | **POST** /api/v2/testSuites/{id}/workItems/search | Search WorkItems
-        *TestSuitesApi* | [**set_configurations_by_test_suite_id**](docs/TestSuitesApi.md#set_configurations_by_test_suite_id) | **POST** /api/v2/testSuites/{id}/configurations | Set Configurations By TestSuite Id
-        *TestSuitesApi* | [**set_work_items_by_test_suite_id**](docs/TestSuitesApi.md#set_work_items_by_test_suite_id) | **POST** /api/v2/testSuites/{id}/workItems | Set WorkItems By TestSuite Id
-        *TestSuitesApi* | [**update_test_suite**](docs/TestSuitesApi.md#update_test_suite) | **PUT** /api/v2/testSuites | Update TestSuite
-        *WebhooksApi* | [**api_v2_webhooks_get**](docs/WebhooksApi.md#api_v2_webhooks_get) | **GET** /api/v2/webhooks | Get all webhooks
-        *WebhooksApi* | [**api_v2_webhooks_id_delete**](docs/WebhooksApi.md#api_v2_webhooks_id_delete) | **DELETE** /api/v2/webhooks/{id} | Delete webhook by ID
-        *WebhooksApi* | [**api_v2_webhooks_id_get**](docs/WebhooksApi.md#api_v2_webhooks_id_get) | **GET** /api/v2/webhooks/{id} | Get webhook by ID
-        *WebhooksApi* | [**api_v2_webhooks_id_put**](docs/WebhooksApi.md#api_v2_webhooks_id_put) | **PUT** /api/v2/webhooks/{id} | Edit webhook by ID
-        *WebhooksApi* | [**api_v2_webhooks_post**](docs/WebhooksApi.md#api_v2_webhooks_post) | **POST** /api/v2/webhooks | Create webhook
-        *WebhooksApi* | [**api_v2_webhooks_search_post**](docs/WebhooksApi.md#api_v2_webhooks_search_post) | **POST** /api/v2/webhooks/search | Search for webhooks
-        *WebhooksApi* | [**api_v2_webhooks_special_variables_get**](docs/WebhooksApi.md#api_v2_webhooks_special_variables_get) | **GET** /api/v2/webhooks/specialVariables | Get special variables for webhook event type
-        *WebhooksLogsApi* | [**api_v2_webhooks_logs_get**](docs/WebhooksLogsApi.md#api_v2_webhooks_logs_get) | **GET** /api/v2/webhooks/logs | Get all webhook logs
-        *WebhooksLogsApi* | [**api_v2_webhooks_logs_id_delete**](docs/WebhooksLogsApi.md#api_v2_webhooks_logs_id_delete) | **DELETE** /api/v2/webhooks/logs/{id} | Delete webhook log by ID
-        *WebhooksLogsApi* | [**api_v2_webhooks_logs_id_get**](docs/WebhooksLogsApi.md#api_v2_webhooks_logs_id_get) | **GET** /api/v2/webhooks/logs/{id} | Get webhook log by ID
-        *WorkItemsApi* | [**api_v2_work_items_id_check_list_transform_to_test_case_post**](docs/WorkItemsApi.md#api_v2_work_items_id_check_list_transform_to_test_case_post) | **POST** /api/v2/workItems/{id}/checkList/transformTo/testCase | Transform CheckList to TestCase
-        *WorkItemsApi* | [**api_v2_work_items_id_history_get**](docs/WorkItemsApi.md#api_v2_work_items_id_history_get) | **GET** /api/v2/workItems/{id}/history | Get change history of WorkItem
-        *WorkItemsApi* | [**api_v2_work_items_id_like_delete**](docs/WorkItemsApi.md#api_v2_work_items_id_like_delete) | **DELETE** /api/v2/workItems/{id}/like | Delete like from WorkItem
-        *WorkItemsApi* | [**api_v2_work_items_id_like_post**](docs/WorkItemsApi.md#api_v2_work_items_id_like_post) | **POST** /api/v2/workItems/{id}/like | Set like to WorkItem
-        *WorkItemsApi* | [**api_v2_work_items_id_likes_count_get**](docs/WorkItemsApi.md#api_v2_work_items_id_likes_count_get) | **GET** /api/v2/workItems/{id}/likes/count | Get likes count of WorkItem
-        *WorkItemsApi* | [**api_v2_work_items_id_likes_get**](docs/WorkItemsApi.md#api_v2_work_items_id_likes_get) | **GET** /api/v2/workItems/{id}/likes | Get likes of WorkItem
-        *WorkItemsApi* | [**api_v2_work_items_id_test_results_history_get**](docs/WorkItemsApi.md#api_v2_work_items_id_test_results_history_get) | **GET** /api/v2/workItems/{id}/testResults/history | Get test results history of WorkItem
-        *WorkItemsApi* | [**api_v2_work_items_id_version_version_id_actual_post**](docs/WorkItemsApi.md#api_v2_work_items_id_version_version_id_actual_post) | **POST** /api/v2/workItems/{id}/version/{versionId}/actual | Set WorkItem as actual
-        *WorkItemsApi* | [**api_v2_work_items_move_post**](docs/WorkItemsApi.md#api_v2_work_items_move_post) | **POST** /api/v2/workItems/move | Move WorkItem to another section
-        *WorkItemsApi* | [**api_v2_work_items_search_post**](docs/WorkItemsApi.md#api_v2_work_items_search_post) | **POST** /api/v2/workItems/search | Search for work items
-        *WorkItemsApi* | [**api_v2_work_items_shared_step_id_references_sections_post**](docs/WorkItemsApi.md#api_v2_work_items_shared_step_id_references_sections_post) | **POST** /api/v2/workItems/{sharedStepId}/references/sections | Get SharedStep references in sections
-        *WorkItemsApi* | [**api_v2_work_items_shared_step_id_references_work_items_post**](docs/WorkItemsApi.md#api_v2_work_items_shared_step_id_references_work_items_post) | **POST** /api/v2/workItems/{sharedStepId}/references/workItems | Get SharedStep references in workitems
-        *WorkItemsApi* | [**api_v2_work_items_shared_steps_shared_step_id_references_get**](docs/WorkItemsApi.md#api_v2_work_items_shared_steps_shared_step_id_references_get) | **GET** /api/v2/workItems/sharedSteps/{sharedStepId}/references | Get SharedStep references
-        *WorkItemsApi* | [**create_work_item**](docs/WorkItemsApi.md#create_work_item) | **POST** /api/v2/workItems | Create Test Case, Checklist or Shared Step
-        *WorkItemsApi* | [**delete_all_work_items_from_auto_test**](docs/WorkItemsApi.md#delete_all_work_items_from_auto_test) | **DELETE** /api/v2/workItems/{id}/autoTests | Delete all links AutoTests from WorkItem by Id or GlobalId
-        *WorkItemsApi* | [**delete_work_item**](docs/WorkItemsApi.md#delete_work_item) | **DELETE** /api/v2/workItems/{id} | Delete Test Case, Checklist or Shared Step by Id or GlobalId
-        *WorkItemsApi* | [**get_auto_tests_for_work_item**](docs/WorkItemsApi.md#get_auto_tests_for_work_item) | **GET** /api/v2/workItems/{id}/autoTests | Get all AutoTests linked to WorkItem by Id or GlobalId
-        *WorkItemsApi* | [**get_iterations**](docs/WorkItemsApi.md#get_iterations) | **GET** /api/v2/workItems/{id}/iterations | Get iterations by workitem Id or GlobalId
-        *WorkItemsApi* | [**get_work_item_by_id**](docs/WorkItemsApi.md#get_work_item_by_id) | **GET** /api/v2/workItems/{id} | Get Test Case, Checklist or Shared Step by Id or GlobalId
-        *WorkItemsApi* | [**get_work_item_chronology**](docs/WorkItemsApi.md#get_work_item_chronology) | **GET** /api/v2/workItems/{id}/chronology | Get WorkItem chronology by Id or GlobalId
-        *WorkItemsApi* | [**get_work_item_versions**](docs/WorkItemsApi.md#get_work_item_versions) | **GET** /api/v2/workItems/{id}/versions | Get WorkItem versions
-        *WorkItemsApi* | [**update_work_item**](docs/WorkItemsApi.md#update_work_item) | **PUT** /api/v2/workItems | Update Test Case, Checklist or Shared Step
-        *WorkItemsCommentsApi* | [**api_v2_work_items_comments_comment_id_delete**](docs/WorkItemsCommentsApi.md#api_v2_work_items_comments_comment_id_delete) | **DELETE** /api/v2/workItems/comments/{commentId} | Delete WorkItem comment
-        *WorkItemsCommentsApi* | [**api_v2_work_items_comments_post**](docs/WorkItemsCommentsApi.md#api_v2_work_items_comments_post) | **POST** /api/v2/workItems/comments | Create WorkItem comment
-        *WorkItemsCommentsApi* | [**api_v2_work_items_comments_put**](docs/WorkItemsCommentsApi.md#api_v2_work_items_comments_put) | **PUT** /api/v2/workItems/comments | Update work item comment
-        *WorkItemsCommentsApi* | [**api_v2_work_items_id_comments_get**](docs/WorkItemsCommentsApi.md#api_v2_work_items_id_comments_get) | **GET** /api/v2/workItems/{id}/comments | Get work item comments
-        
-        
-        ## Documentation For Models
-        
-         - You can see the documentation [here](docs/README.md).
-        
-        
-        # Contributing
-        
-        You can help to develop the project. Any contributions are **greatly appreciated**.
-        
-        * If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testgear-tms/api-client-python/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
-        * Please make sure you check your spelling and grammar.
-        * Create individual PR for each suggestion.
-        * Please also read through the [Code Of Conduct](https://github.com/testgear-tms/api-client-python/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
-        
-        
-        # License
-        
-        Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testgear-tms/api-client-python/blob/master/LICENSE.md) for more information.
-        
-        
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: testgear-api-client
+Version: 3.1.0
+Summary: API-client for Test Gear
+Home-page: https://pypi.org/project/testgear-api-client/
+Author: Integration team
+Author-email: integrations@test-gear.io
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# Api client for Test Gear TMS
+![Test Gear](https://raw.githubusercontent.com/testgear-tms/api-client-python/master/images/banner.png)
+
+## Getting Started
+
+### Compatibility
+
+| Test Gear | API Client |
+|-----------|------------|
+| 3.5       | 2.0        |
+| 4.0       | 3.0        |
+| 4.2       | 3.1        |
+
+## Installation & Usage
+### pip install
+
+```sh
+pip install testgear-api-client
+```
+
+Then import the package:
+
+```python
+import testgear_api_client
+```
+
+## Getting Started
+
+Please follow the [installation procedure](#installation--usage) and then run the following:
+
+```python
+import testgear_api_client
+from testgear_api_client.api import attachments_api
+from testgear_api_client.model.attachment_model import AttachmentModel
+from testgear_api_client.model.image_resize_type import ImageResizeType
+from testgear_api_client.model.problem_details import ProblemDetails
+from testgear_api_client.model.validation_problem_details import ValidationProblemDetails
+
+configuration = testgear_api_client.Configuration(
+    host = "Your TMS address"
+)
+
+with testgear_api_client.ApiClient(
+        configuration,
+        header_name='Authorization',
+        header_value='PrivateToken ' + 'Your private token') as api_client:
+    api_instance = attachments_api.AttachmentsApi(api_client)
+    id = "Attachment's guid in the TMS"
+
+    try:
+        api_instance.api_v2_attachments_id_delete(id)
+    except testgear_api_client.ApiException as e:
+        print("Exception when calling AttachmentsApi->api_v2_attachments_id_delete: %s\n" % e)
+```
+
+## Documentation for API Endpoints
+
+All URIs are relative to *http://localhost*
+
+Class | Method | HTTP request | Description
+------------ | ------------- | ------------- | -------------
+*AttachmentsApi* | [**api_v2_attachments_id_delete**](docs/AttachmentsApi.md#api_v2_attachments_id_delete) | **DELETE** /api/v2/attachments/{id} | Delete attachment file
+*AttachmentsApi* | [**api_v2_attachments_id_get**](docs/AttachmentsApi.md#api_v2_attachments_id_get) | **GET** /api/v2/attachments/{id} | Download attachment file
+*AttachmentsApi* | [**api_v2_attachments_occupied_file_storage_size_get**](docs/AttachmentsApi.md#api_v2_attachments_occupied_file_storage_size_get) | **GET** /api/v2/attachments/occupiedFileStorageSize | Get size of attachments storage in bytes
+*AttachmentsApi* | [**api_v2_attachments_post**](docs/AttachmentsApi.md#api_v2_attachments_post) | **POST** /api/v2/attachments | Upload new attachment file
+*AutoTestsApi* | [**api_v2_auto_tests_flaky_bulk_post**](docs/AutoTestsApi.md#api_v2_auto_tests_flaky_bulk_post) | **POST** /api/v2/autoTests/flaky/bulk | Set \&quot;Flaky\&quot; status for multiple autotests
+*AutoTestsApi* | [**api_v2_auto_tests_id_patch**](docs/AutoTestsApi.md#api_v2_auto_tests_id_patch) | **PATCH** /api/v2/autoTests/{id} | Patch auto test
+*AutoTestsApi* | [**api_v2_auto_tests_id_test_results_search_post**](docs/AutoTestsApi.md#api_v2_auto_tests_id_test_results_search_post) | **POST** /api/v2/autoTests/{id}/testResults/search | Get test results history for autotest
+*AutoTestsApi* | [**api_v2_auto_tests_id_work_items_changed_id_get**](docs/AutoTestsApi.md#api_v2_auto_tests_id_work_items_changed_id_get) | **GET** /api/v2/autoTests/{id}/workItems/changed/id | Get identifiers of changed linked work items
+*AutoTestsApi* | [**api_v2_auto_tests_id_work_items_changed_work_item_id_approve_post**](docs/AutoTestsApi.md#api_v2_auto_tests_id_work_items_changed_work_item_id_approve_post) | **POST** /api/v2/autoTests/{id}/workItems/changed/{workItemId}/approve | Approve changes to work items linked to autotest
+*AutoTestsApi* | [**api_v2_auto_tests_search_post**](docs/AutoTestsApi.md#api_v2_auto_tests_search_post) | **POST** /api/v2/autoTests/search | Search for autotests
+*AutoTestsApi* | [**create_auto_test**](docs/AutoTestsApi.md#create_auto_test) | **POST** /api/v2/autoTests | Create autotest
+*AutoTestsApi* | [**create_multiple**](docs/AutoTestsApi.md#create_multiple) | **POST** /api/v2/autoTests/bulk | Create multiple autotests
+*AutoTestsApi* | [**delete_auto_test**](docs/AutoTestsApi.md#delete_auto_test) | **DELETE** /api/v2/autoTests/{id} | Delete autotest
+*AutoTestsApi* | [**delete_auto_test_link_from_work_item**](docs/AutoTestsApi.md#delete_auto_test_link_from_work_item) | **DELETE** /api/v2/autoTests/{id}/workItems | Unlink autotest from work item
+*AutoTestsApi* | [**get_all_auto_tests**](docs/AutoTestsApi.md#get_all_auto_tests) | **GET** /api/v2/autoTests | 
+*AutoTestsApi* | [**get_auto_test_average_duration**](docs/AutoTestsApi.md#get_auto_test_average_duration) | **GET** /api/v2/autoTests/{id}/averageDuration | Get average autotest duration
+*AutoTestsApi* | [**get_auto_test_by_id**](docs/AutoTestsApi.md#get_auto_test_by_id) | **GET** /api/v2/autoTests/{id} | Get autotest by internal or global ID
+*AutoTestsApi* | [**get_auto_test_chronology**](docs/AutoTestsApi.md#get_auto_test_chronology) | **GET** /api/v2/autoTests/{id}/chronology | Get autotest chronology
+*AutoTestsApi* | [**get_test_runs**](docs/AutoTestsApi.md#get_test_runs) | **GET** /api/v2/autoTests/{id}/testRuns | Get completed tests runs for autotests
+*AutoTestsApi* | [**get_work_item_results**](docs/AutoTestsApi.md#get_work_item_results) | **GET** /api/v2/autoTests/{id}/testResultHistory | 
+*AutoTestsApi* | [**get_work_items_linked_to_auto_test**](docs/AutoTestsApi.md#get_work_items_linked_to_auto_test) | **GET** /api/v2/autoTests/{id}/workItems | Get work items linked to autotest
+*AutoTestsApi* | [**link_auto_test_to_work_item**](docs/AutoTestsApi.md#link_auto_test_to_work_item) | **POST** /api/v2/autoTests/{id}/workItems | Link autotest with work items
+*AutoTestsApi* | [**update_auto_test**](docs/AutoTestsApi.md#update_auto_test) | **PUT** /api/v2/autoTests | Update autotest
+*AutoTestsApi* | [**update_multiple**](docs/AutoTestsApi.md#update_multiple) | **PUT** /api/v2/autoTests/bulk | Update multiple autotests
+*BackgroundJobsApi* | [**api_v2_background_jobs_get**](docs/BackgroundJobsApi.md#api_v2_background_jobs_get) | **GET** /api/v2/backgroundJobs | Get current user background jobs
+*ConfigurationsApi* | [**api_v2_configurations_create_by_parameters_post**](docs/ConfigurationsApi.md#api_v2_configurations_create_by_parameters_post) | **POST** /api/v2/configurations/createByParameters | Create Configurations by parameters
+*ConfigurationsApi* | [**api_v2_configurations_id_patch**](docs/ConfigurationsApi.md#api_v2_configurations_id_patch) | **PATCH** /api/v2/configurations/{id} | Patch configuration
+*ConfigurationsApi* | [**api_v2_configurations_search_post**](docs/ConfigurationsApi.md#api_v2_configurations_search_post) | **POST** /api/v2/configurations/search | Search for configurations
+*ConfigurationsApi* | [**create_configuration**](docs/ConfigurationsApi.md#create_configuration) | **POST** /api/v2/configurations | Create Configuration
+*ConfigurationsApi* | [**get_configuration_by_id**](docs/ConfigurationsApi.md#get_configuration_by_id) | **GET** /api/v2/configurations/{id} | Get configuration by internal or global ID
+*ConfigurationsApi* | [**update_configuration**](docs/ConfigurationsApi.md#update_configuration) | **PUT** /api/v2/configurations | Update Configuration
+*CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_custom_attributes_exclude_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_custom_attributes_exclude_post) | **POST** /api/v2/customAttributes/templates/{id}/customAttributes/exclude | Exclude CustomAttributes from CustomAttributeTemplate
+*CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_custom_attributes_include_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_custom_attributes_include_post) | **POST** /api/v2/customAttributes/templates/{id}/customAttributes/include | Include CustomAttributes to CustomAttributeTemplate
+*CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_delete**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_delete) | **DELETE** /api/v2/customAttributes/templates/{id} | Delete CustomAttributeTemplate
+*CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_id_get**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_id_get) | **GET** /api/v2/customAttributes/templates/{id} | Get CustomAttributeTemplate by ID
+*CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_name_get**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_name_get) | **GET** /api/v2/customAttributes/templates/{name} | Get CustomAttributeTemplate by name
+*CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_post) | **POST** /api/v2/customAttributes/templates | Create CustomAttributeTemplate
+*CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_put**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_put) | **PUT** /api/v2/customAttributes/templates | Update custom attributes template
+*CustomAttributeTemplatesApi* | [**api_v2_custom_attributes_templates_search_post**](docs/CustomAttributeTemplatesApi.md#api_v2_custom_attributes_templates_search_post) | **POST** /api/v2/customAttributes/templates/search | Search CustomAttributeTemplates
+*CustomAttributesApi* | [**api_v2_custom_attributes_global_id_delete**](docs/CustomAttributesApi.md#api_v2_custom_attributes_global_id_delete) | **DELETE** /api/v2/customAttributes/global/{id} | Delete global attribute
+*CustomAttributesApi* | [**api_v2_custom_attributes_global_id_put**](docs/CustomAttributesApi.md#api_v2_custom_attributes_global_id_put) | **PUT** /api/v2/customAttributes/global/{id} | Edit global attribute
+*CustomAttributesApi* | [**api_v2_custom_attributes_global_post**](docs/CustomAttributesApi.md#api_v2_custom_attributes_global_post) | **POST** /api/v2/customAttributes/global | Create global attribute
+*CustomAttributesApi* | [**api_v2_custom_attributes_id_get**](docs/CustomAttributesApi.md#api_v2_custom_attributes_id_get) | **GET** /api/v2/customAttributes/{id} | Get attribute
+*CustomAttributesApi* | [**api_v2_custom_attributes_search_post**](docs/CustomAttributesApi.md#api_v2_custom_attributes_search_post) | **POST** /api/v2/customAttributes/search | Search for attributes
+*NotificationsApi* | [**api_v2_notifications_count_get**](docs/NotificationsApi.md#api_v2_notifications_count_get) | **GET** /api/v2/notifications/count | Get unread Notifications total in last 7 days
+*NotificationsApi* | [**api_v2_notifications_get**](docs/NotificationsApi.md#api_v2_notifications_get) | **GET** /api/v2/notifications | Get all Notifications for current User
+*NotificationsApi* | [**api_v2_notifications_id_read_post**](docs/NotificationsApi.md#api_v2_notifications_id_read_post) | **POST** /api/v2/notifications/{id}/read | Set Notification as read
+*NotificationsApi* | [**api_v2_notifications_read_post**](docs/NotificationsApi.md#api_v2_notifications_read_post) | **POST** /api/v2/notifications/read | Set all Notifications as read
+*NotificationsApi* | [**api_v2_notifications_search_post**](docs/NotificationsApi.md#api_v2_notifications_search_post) | **POST** /api/v2/notifications/search | Search Notifications for current User
+*ParametersApi* | [**api_v2_parameters_bulk_post**](docs/ParametersApi.md#api_v2_parameters_bulk_post) | **POST** /api/v2/parameters/bulk | Create multiple parameters
+*ParametersApi* | [**api_v2_parameters_bulk_put**](docs/ParametersApi.md#api_v2_parameters_bulk_put) | **PUT** /api/v2/parameters/bulk | Update multiple parameters
+*ParametersApi* | [**api_v2_parameters_groups_get**](docs/ParametersApi.md#api_v2_parameters_groups_get) | **GET** /api/v2/parameters/groups | Get parameters as group
+*ParametersApi* | [**api_v2_parameters_key_name_name_exists_get**](docs/ParametersApi.md#api_v2_parameters_key_name_name_exists_get) | **GET** /api/v2/parameters/key/name/{name}/exists | Check existence parameter key in system
+*ParametersApi* | [**api_v2_parameters_key_values_get**](docs/ParametersApi.md#api_v2_parameters_key_values_get) | **GET** /api/v2/parameters/{key}/values | Get all parameter key values
+*ParametersApi* | [**api_v2_parameters_keys_get**](docs/ParametersApi.md#api_v2_parameters_keys_get) | **GET** /api/v2/parameters/keys | Get all parameter keys
+*ParametersApi* | [**api_v2_parameters_search_post**](docs/ParametersApi.md#api_v2_parameters_search_post) | **POST** /api/v2/parameters/search | Search for parameters
+*ParametersApi* | [**create_parameter**](docs/ParametersApi.md#create_parameter) | **POST** /api/v2/parameters | Create parameter
+*ParametersApi* | [**delete_by_name**](docs/ParametersApi.md#delete_by_name) | **DELETE** /api/v2/parameters/name/{name} | Delete parameter by name
+*ParametersApi* | [**delete_by_parameter_key_id**](docs/ParametersApi.md#delete_by_parameter_key_id) | **DELETE** /api/v2/parameters/keyId/{keyId} | Delete parameters by parameter key identifier
+*ParametersApi* | [**delete_parameter**](docs/ParametersApi.md#delete_parameter) | **DELETE** /api/v2/parameters/{id} | Delete parameter
+*ParametersApi* | [**get_all_parameters**](docs/ParametersApi.md#get_all_parameters) | **GET** /api/v2/parameters | Get all parameters
+*ParametersApi* | [**get_parameter_by_id**](docs/ParametersApi.md#get_parameter_by_id) | **GET** /api/v2/parameters/{id} | Get parameter by ID
+*ParametersApi* | [**obsolete_delete_by_name**](docs/ParametersApi.md#obsolete_delete_by_name) | **POST** /api/v2/parameters/deleteByName | 
+*ParametersApi* | [**update_parameter**](docs/ParametersApi.md#update_parameter) | **PUT** /api/v2/parameters | Update parameter
+*ProjectsApi* | [**add_globa_attributes_to_project**](docs/ProjectsApi.md#add_globa_attributes_to_project) | **POST** /api/v2/projects/{id}/globalAttributes | Add global attributes to project
+*ProjectsApi* | [**api_v2_projects_id_attributes_templates_search_post**](docs/ProjectsApi.md#api_v2_projects_id_attributes_templates_search_post) | **POST** /api/v2/projects/{id}/attributes/templates/search | Search for custom attributes templates
+*ProjectsApi* | [**api_v2_projects_id_attributes_templates_template_id_delete**](docs/ProjectsApi.md#api_v2_projects_id_attributes_templates_template_id_delete) | **DELETE** /api/v2/projects/{id}/attributes/templates/{templateId} | Delete CustomAttributeTemplate from Project
+*ProjectsApi* | [**api_v2_projects_id_attributes_templates_template_id_post**](docs/ProjectsApi.md#api_v2_projects_id_attributes_templates_template_id_post) | **POST** /api/v2/projects/{id}/attributes/templates/{templateId} | Add CustomAttributeTemplate to Project
+*ProjectsApi* | [**api_v2_projects_id_failure_classes_get**](docs/ProjectsApi.md#api_v2_projects_id_failure_classes_get) | **GET** /api/v2/projects/{id}/failureClasses | Get Project FailureClasses
+*ProjectsApi* | [**api_v2_projects_id_favorite_put**](docs/ProjectsApi.md#api_v2_projects_id_favorite_put) | **PUT** /api/v2/projects/{id}/favorite | Mark Project as favorite
+*ProjectsApi* | [**api_v2_projects_id_filters_get**](docs/ProjectsApi.md#api_v2_projects_id_filters_get) | **GET** /api/v2/projects/{id}/filters | Get Project filters
+*ProjectsApi* | [**api_v2_projects_id_patch**](docs/ProjectsApi.md#api_v2_projects_id_patch) | **PATCH** /api/v2/projects/{id} | Patch project
+*ProjectsApi* | [**api_v2_projects_id_test_plans_analytics_get**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_analytics_get) | **GET** /api/v2/projects/{id}/testPlans/analytics | Get TestPlans analytics
+*ProjectsApi* | [**api_v2_projects_id_test_plans_delete_bulk_post**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_delete_bulk_post) | **POST** /api/v2/projects/{id}/testPlans/delete/bulk | Delete multiple test plans
+*ProjectsApi* | [**api_v2_projects_id_test_plans_name_exists_get**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_name_exists_get) | **GET** /api/v2/projects/{id}/testPlans/{name}/exists | Checks if TestPlan exists with the specified name exists for the project
+*ProjectsApi* | [**api_v2_projects_id_test_plans_restore_bulk_post**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_restore_bulk_post) | **POST** /api/v2/projects/{id}/testPlans/restore/bulk | Restore multiple test plans
+*ProjectsApi* | [**api_v2_projects_id_test_plans_search_post**](docs/ProjectsApi.md#api_v2_projects_id_test_plans_search_post) | **POST** /api/v2/projects/{id}/testPlans/search | Get Project TestPlans with analytics
+*ProjectsApi* | [**api_v2_projects_id_test_runs_active_get**](docs/ProjectsApi.md#api_v2_projects_id_test_runs_active_get) | **GET** /api/v2/projects/{id}/testRuns/active | Get active Project TestRuns
+*ProjectsApi* | [**api_v2_projects_id_test_runs_full_get**](docs/ProjectsApi.md#api_v2_projects_id_test_runs_full_get) | **GET** /api/v2/projects/{id}/testRuns/full | Get Project TestRuns full models
+*ProjectsApi* | [**api_v2_projects_id_work_items_search_id_post**](docs/ProjectsApi.md#api_v2_projects_id_work_items_search_id_post) | **POST** /api/v2/projects/{id}/workItems/search/id | Search for work items and extract IDs only
+*ProjectsApi* | [**api_v2_projects_id_work_items_search_post**](docs/ProjectsApi.md#api_v2_projects_id_work_items_search_post) | **POST** /api/v2/projects/{id}/workItems/search | Search for work items
+*ProjectsApi* | [**api_v2_projects_id_work_items_tags_get**](docs/ProjectsApi.md#api_v2_projects_id_work_items_tags_get) | **GET** /api/v2/projects/{id}/workItems/tags | Get WorkItems Tags
+*ProjectsApi* | [**api_v2_projects_name_name_exists_get**](docs/ProjectsApi.md#api_v2_projects_name_name_exists_get) | **GET** /api/v2/projects/name/{name}/exists | 
+*ProjectsApi* | [**api_v2_projects_search_post**](docs/ProjectsApi.md#api_v2_projects_search_post) | **POST** /api/v2/projects/search | Search for projects
+*ProjectsApi* | [**background_import_project**](docs/ProjectsApi.md#background_import_project) | **POST** /api/v2/projects/import/json | Import project from JSON file in background job
+*ProjectsApi* | [**background_import_to_existing_project**](docs/ProjectsApi.md#background_import_to_existing_project) | **POST** /api/v2/projects/{id}/import/json | Import project from JSON file into existing project in background job
+*ProjectsApi* | [**background_import_zip_project**](docs/ProjectsApi.md#background_import_zip_project) | **POST** /api/v2/projects/import/zip | Import project from Zip file in background job
+*ProjectsApi* | [**background_import_zip_to_existing_project**](docs/ProjectsApi.md#background_import_zip_to_existing_project) | **POST** /api/v2/projects/{id}/import/zip | Import project from Zip file into existing project in background job
+*ProjectsApi* | [**call_import**](docs/ProjectsApi.md#call_import) | **POST** /api/v2/projects/import | Import project from JSON file
+*ProjectsApi* | [**create_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#create_custom_attribute_test_plan_project_relations) | **POST** /api/v2/projects/{id}/testPlans/attributes | Add attributes to project&#39;s test plans
+*ProjectsApi* | [**create_project**](docs/ProjectsApi.md#create_project) | **POST** /api/v2/projects | Create project
+*ProjectsApi* | [**create_projects_attribute**](docs/ProjectsApi.md#create_projects_attribute) | **POST** /api/v2/projects/{id}/attributes | Create project attribute
+*ProjectsApi* | [**delete_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#delete_custom_attribute_test_plan_project_relations) | **DELETE** /api/v2/projects/{id}/testPlans/attribute/{attributeId} | Delete attribute from project&#39;s test plans
+*ProjectsApi* | [**delete_project**](docs/ProjectsApi.md#delete_project) | **DELETE** /api/v2/projects/{id} | Delete project
+*ProjectsApi* | [**delete_project_auto_tests**](docs/ProjectsApi.md#delete_project_auto_tests) | **DELETE** /api/v2/projects/{id}/autoTests | Delete project
+*ProjectsApi* | [**delete_projects_attribute**](docs/ProjectsApi.md#delete_projects_attribute) | **DELETE** /api/v2/projects/{id}/attributes/{attributeId} | Delete project attribute
+*ProjectsApi* | [**export**](docs/ProjectsApi.md#export) | **POST** /api/v2/projects/{id}/export | Export project as JSON file
+*ProjectsApi* | [**export_project_json**](docs/ProjectsApi.md#export_project_json) | **POST** /api/v2/projects/{id}/export/json | Export project as JSON file in background job
+*ProjectsApi* | [**export_project_with_test_plans_json**](docs/ProjectsApi.md#export_project_with_test_plans_json) | **POST** /api/v2/projects/{id}/export/testPlans/json | Export project as JSON file with test plans in background job
+*ProjectsApi* | [**export_project_with_test_plans_zip**](docs/ProjectsApi.md#export_project_with_test_plans_zip) | **POST** /api/v2/projects/{id}/export/testPlans/zip | Export project as Zip file with test plans in background job
+*ProjectsApi* | [**export_project_zip**](docs/ProjectsApi.md#export_project_zip) | **POST** /api/v2/projects/{id}/export/zip | Export project as Zip file in background job
+*ProjectsApi* | [**export_with_test_plans_and_configurations**](docs/ProjectsApi.md#export_with_test_plans_and_configurations) | **POST** /api/v2/projects/{id}/export-by-testPlans | Export project with test plans, test suites and test points as JSON file
+*ProjectsApi* | [**get_all_projects**](docs/ProjectsApi.md#get_all_projects) | **GET** /api/v2/projects | Get all projects
+*ProjectsApi* | [**get_attribute_by_project_id**](docs/ProjectsApi.md#get_attribute_by_project_id) | **GET** /api/v2/projects/{id}/attributes/{attributeId} | Get project attribute
+*ProjectsApi* | [**get_attributes_by_project_id**](docs/ProjectsApi.md#get_attributes_by_project_id) | **GET** /api/v2/projects/{id}/attributes | Get project attributes
+*ProjectsApi* | [**get_auto_tests_namespaces**](docs/ProjectsApi.md#get_auto_tests_namespaces) | **GET** /api/v2/projects/{id}/autoTestsNamespaces | Get namespaces of autotests in project
+*ProjectsApi* | [**get_configurations_by_project_id**](docs/ProjectsApi.md#get_configurations_by_project_id) | **GET** /api/v2/projects/{id}/configurations | Get project configurations
+*ProjectsApi* | [**get_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#get_custom_attribute_test_plan_project_relations) | **GET** /api/v2/projects/{id}/testPlans/attributes | Get project&#39;s test plan attributes
+*ProjectsApi* | [**get_project_by_id**](docs/ProjectsApi.md#get_project_by_id) | **GET** /api/v2/projects/{id} | Get project by ID
+*ProjectsApi* | [**get_sections_by_project_id**](docs/ProjectsApi.md#get_sections_by_project_id) | **GET** /api/v2/projects/{id}/sections | Get project sections
+*ProjectsApi* | [**get_test_plans_by_project_id**](docs/ProjectsApi.md#get_test_plans_by_project_id) | **GET** /api/v2/projects/{id}/testPlans | Get project test plans
+*ProjectsApi* | [**get_test_runs_by_project_id**](docs/ProjectsApi.md#get_test_runs_by_project_id) | **GET** /api/v2/projects/{id}/testRuns | Get project test runs
+*ProjectsApi* | [**get_work_items_by_project_id**](docs/ProjectsApi.md#get_work_items_by_project_id) | **GET** /api/v2/projects/{id}/workItems | Get project work items
+*ProjectsApi* | [**import_to_existing_project**](docs/ProjectsApi.md#import_to_existing_project) | **POST** /api/v2/projects/{id}/import | Import project from JSON file into existing project
+*ProjectsApi* | [**restore_project**](docs/ProjectsApi.md#restore_project) | **POST** /api/v2/projects/{id}/restore | Restore project
+*ProjectsApi* | [**search_attributes_in_project**](docs/ProjectsApi.md#search_attributes_in_project) | **POST** /api/v2/projects/{id}/attributes/search | Search for attributes used in the project
+*ProjectsApi* | [**search_test_plan_attributes_in_project**](docs/ProjectsApi.md#search_test_plan_attributes_in_project) | **POST** /api/v2/projects/{id}/testPlans/attributes/search | Search for attributes used in the project test plans
+*ProjectsApi* | [**update_custom_attribute_test_plan_project_relations**](docs/ProjectsApi.md#update_custom_attribute_test_plan_project_relations) | **PUT** /api/v2/projects/{id}/testPlans/attribute | Update attribute of project&#39;s test plans
+*ProjectsApi* | [**update_project**](docs/ProjectsApi.md#update_project) | **PUT** /api/v2/projects | Update project
+*ProjectsApi* | [**update_projects_attribute**](docs/ProjectsApi.md#update_projects_attribute) | **PUT** /api/v2/projects/{id}/attributes | Edit attribute of the project
+*SectionsApi* | [**api_v2_sections_id_patch**](docs/SectionsApi.md#api_v2_sections_id_patch) | **PATCH** /api/v2/sections/{id} | Patch section
+*SectionsApi* | [**create_section**](docs/SectionsApi.md#create_section) | **POST** /api/v2/sections | Create section
+*SectionsApi* | [**delete_section**](docs/SectionsApi.md#delete_section) | **DELETE** /api/v2/sections/{id} | Delete section
+*SectionsApi* | [**get_section_by_id**](docs/SectionsApi.md#get_section_by_id) | **GET** /api/v2/sections/{id} | Get section
+*SectionsApi* | [**get_work_items_by_section_id**](docs/SectionsApi.md#get_work_items_by_section_id) | **GET** /api/v2/sections/{id}/workItems | Get section work items
+*SectionsApi* | [**move**](docs/SectionsApi.md#move) | **POST** /api/v2/sections/move | Move section with all work items into another section
+*SectionsApi* | [**rename**](docs/SectionsApi.md#rename) | **POST** /api/v2/sections/rename | Rename section
+*SectionsApi* | [**update_section**](docs/SectionsApi.md#update_section) | **PUT** /api/v2/sections | Update section
+*TagsApi* | [**api_v2_tags_get**](docs/TagsApi.md#api_v2_tags_get) | **GET** /api/v2/tags | Get all Tags
+*TagsApi* | [**api_v2_tags_test_plans_tags_get**](docs/TagsApi.md#api_v2_tags_test_plans_tags_get) | **GET** /api/v2/tags/testPlansTags | Get all Tags that are used in TestPlans
+*TestPlansApi* | [**add_test_points_with_sections**](docs/TestPlansApi.md#add_test_points_with_sections) | **POST** /api/v2/testPlans/{id}/test-points/withSections | Add test-points to TestPlan with sections
+*TestPlansApi* | [**add_work_items_with_sections**](docs/TestPlansApi.md#add_work_items_with_sections) | **POST** /api/v2/testPlans/{id}/workItems/withSections | Add WorkItems to TestPlan with Sections as TestSuites
+*TestPlansApi* | [**api_v2_test_plans_id_analytics_get**](docs/TestPlansApi.md#api_v2_test_plans_id_analytics_get) | **GET** /api/v2/testPlans/{id}/analytics | Get analytics by TestPlan
+*TestPlansApi* | [**api_v2_test_plans_id_autobalance_post**](docs/TestPlansApi.md#api_v2_test_plans_id_autobalance_post) | **POST** /api/v2/testPlans/{id}/autobalance | Distribute test points between the users
+*TestPlansApi* | [**api_v2_test_plans_id_configurations_get**](docs/TestPlansApi.md#api_v2_test_plans_id_configurations_get) | **GET** /api/v2/testPlans/{id}/configurations | Get TestPlan configurations
+*TestPlansApi* | [**api_v2_test_plans_id_export_test_points_xlsx_post**](docs/TestPlansApi.md#api_v2_test_plans_id_export_test_points_xlsx_post) | **POST** /api/v2/testPlans/{id}/export/testPoints/xlsx | Export TestPoints from TestPlan in xls format
+*TestPlansApi* | [**api_v2_test_plans_id_export_test_result_history_xlsx_post**](docs/TestPlansApi.md#api_v2_test_plans_id_export_test_result_history_xlsx_post) | **POST** /api/v2/testPlans/{id}/export/testResultHistory/xlsx | Export TestResults history from TestPlan in xls format
+*TestPlansApi* | [**api_v2_test_plans_id_history_get**](docs/TestPlansApi.md#api_v2_test_plans_id_history_get) | **GET** /api/v2/testPlans/{id}/history | Get TestPlan history
+*TestPlansApi* | [**api_v2_test_plans_id_links_get**](docs/TestPlansApi.md#api_v2_test_plans_id_links_get) | **GET** /api/v2/testPlans/{id}/links | Get Links of TestPlan
+*TestPlansApi* | [**api_v2_test_plans_id_patch**](docs/TestPlansApi.md#api_v2_test_plans_id_patch) | **PATCH** /api/v2/testPlans/{id} | Patch test plan
+*TestPlansApi* | [**api_v2_test_plans_id_test_points_last_results_get**](docs/TestPlansApi.md#api_v2_test_plans_id_test_points_last_results_get) | **GET** /api/v2/testPlans/{id}/testPoints/lastResults | Get TestPoints with last result from TestPlan
+*TestPlansApi* | [**api_v2_test_plans_id_test_points_reset_post**](docs/TestPlansApi.md#api_v2_test_plans_id_test_points_reset_post) | **POST** /api/v2/testPlans/{id}/testPoints/reset | Reset TestPoints status of TestPlan
+*TestPlansApi* | [**api_v2_test_plans_id_test_points_tester_delete**](docs/TestPlansApi.md#api_v2_test_plans_id_test_points_tester_delete) | **DELETE** /api/v2/testPlans/{id}/testPoints/tester | Unassign users from multiple test points
+*TestPlansApi* | [**api_v2_test_plans_id_test_points_tester_user_id_post**](docs/TestPlansApi.md#api_v2_test_plans_id_test_points_tester_user_id_post) | **POST** /api/v2/testPlans/{id}/testPoints/tester/{userId} | Assign user as a tester to multiple test points
+*TestPlansApi* | [**api_v2_test_plans_id_test_runs_get**](docs/TestPlansApi.md#api_v2_test_plans_id_test_runs_get) | **GET** /api/v2/testPlans/{id}/testRuns | Get TestRuns of TestPlan
+*TestPlansApi* | [**api_v2_test_plans_id_test_runs_search_post**](docs/TestPlansApi.md#api_v2_test_plans_id_test_runs_search_post) | **POST** /api/v2/testPlans/{id}/testRuns/search | Search TestRuns of TestPlan
+*TestPlansApi* | [**api_v2_test_plans_id_test_runs_test_results_last_modified_modified_date_get**](docs/TestPlansApi.md#api_v2_test_plans_id_test_runs_test_results_last_modified_modified_date_get) | **GET** /api/v2/testPlans/{id}/testRuns/testResults/lastModified/modifiedDate | Get last modification date of test plan&#39;s test results
+*TestPlansApi* | [**api_v2_test_plans_id_unlock_request_post**](docs/TestPlansApi.md#api_v2_test_plans_id_unlock_request_post) | **POST** /api/v2/testPlans/{id}/unlock/request | Send unlock TestPlan notification
+*TestPlansApi* | [**api_v2_test_plans_shorts_post**](docs/TestPlansApi.md#api_v2_test_plans_shorts_post) | **POST** /api/v2/testPlans/shorts | Get TestPlans short models by Project identifiers
+*TestPlansApi* | [**clone**](docs/TestPlansApi.md#clone) | **POST** /api/v2/testPlans/{id}/clone | Clone TestPlan
+*TestPlansApi* | [**complete**](docs/TestPlansApi.md#complete) | **POST** /api/v2/testPlans/{id}/complete | Complete TestPlan
+*TestPlansApi* | [**create_test_plan**](docs/TestPlansApi.md#create_test_plan) | **POST** /api/v2/testPlans | Create TestPlan
+*TestPlansApi* | [**delete_test_plan**](docs/TestPlansApi.md#delete_test_plan) | **DELETE** /api/v2/testPlans/{id} | Delete TestPlan
+*TestPlansApi* | [**get_test_plan_by_id**](docs/TestPlansApi.md#get_test_plan_by_id) | **GET** /api/v2/testPlans/{id} | Get TestPlan by Id
+*TestPlansApi* | [**get_test_suites_by_id**](docs/TestPlansApi.md#get_test_suites_by_id) | **GET** /api/v2/testPlans/{id}/testSuites | Get TestSuites Tree By Id
+*TestPlansApi* | [**pause**](docs/TestPlansApi.md#pause) | **POST** /api/v2/testPlans/{id}/pause | Pause TestPlan
+*TestPlansApi* | [**restore_test_plan**](docs/TestPlansApi.md#restore_test_plan) | **POST** /api/v2/testPlans/{id}/restore | Restore TestPlan
+*TestPlansApi* | [**start**](docs/TestPlansApi.md#start) | **POST** /api/v2/testPlans/{id}/start | Start TestPlan
+*TestPlansApi* | [**update_test_plan**](docs/TestPlansApi.md#update_test_plan) | **PUT** /api/v2/testPlans | Update TestPlan
+*TestPointsApi* | [**api_v2_test_points_id_test_runs_get**](docs/TestPointsApi.md#api_v2_test_points_id_test_runs_get) | **GET** /api/v2/testPoints/{id}/testRuns | Get all test runs which use test point
+*TestPointsApi* | [**api_v2_test_points_id_work_item_get**](docs/TestPointsApi.md#api_v2_test_points_id_work_item_get) | **GET** /api/v2/testPoints/{id}/workItem | Get work item represented by test point
+*TestPointsApi* | [**api_v2_test_points_search_id_post**](docs/TestPointsApi.md#api_v2_test_points_search_id_post) | **POST** /api/v2/testPoints/search/id | Search for test points and extract IDs only
+*TestPointsApi* | [**api_v2_test_points_search_post**](docs/TestPointsApi.md#api_v2_test_points_search_post) | **POST** /api/v2/testPoints/search | Search for test points
+*TestResultsApi* | [**api_v2_test_results_id_aggregated_get**](docs/TestResultsApi.md#api_v2_test_results_id_aggregated_get) | **GET** /api/v2/testResults/{id}/aggregated | Get test result by ID aggregated with previous results
+*TestResultsApi* | [**api_v2_test_results_id_attachments_attachment_id_put**](docs/TestResultsApi.md#api_v2_test_results_id_attachments_attachment_id_put) | **PUT** /api/v2/testResults/{id}/attachments/{attachmentId} | Attach file to the test result
+*TestResultsApi* | [**api_v2_test_results_id_attachments_info_get**](docs/TestResultsApi.md#api_v2_test_results_id_attachments_info_get) | **GET** /api/v2/testResults/{id}/attachments/info | Get test result attachments meta-information
+*TestResultsApi* | [**api_v2_test_results_id_get**](docs/TestResultsApi.md#api_v2_test_results_id_get) | **GET** /api/v2/testResults/{id} | Get test result by ID
+*TestResultsApi* | [**api_v2_test_results_id_put**](docs/TestResultsApi.md#api_v2_test_results_id_put) | **PUT** /api/v2/testResults/{id} | Edit test result by ID
+*TestResultsApi* | [**api_v2_test_results_search_post**](docs/TestResultsApi.md#api_v2_test_results_search_post) | **POST** /api/v2/testResults/search | Search for test results
+*TestResultsApi* | [**api_v2_test_results_statistics_filter_post**](docs/TestResultsApi.md#api_v2_test_results_statistics_filter_post) | **POST** /api/v2/testResults/statistics/filter | Search for test results and extract statistics
+*TestResultsApi* | [**create_attachment**](docs/TestResultsApi.md#create_attachment) | **POST** /api/v2/testResults/{id}/attachments | Upload and link attachment to TestResult
+*TestResultsApi* | [**delete_attachment**](docs/TestResultsApi.md#delete_attachment) | **DELETE** /api/v2/testResults/{id}/attachments/{attachmentId} | Remove attachment and unlink from TestResult
+*TestResultsApi* | [**download_attachment**](docs/TestResultsApi.md#download_attachment) | **GET** /api/v2/testResults/{id}/attachments/{attachmentId} | Get attachment of TestResult
+*TestResultsApi* | [**get_attachment**](docs/TestResultsApi.md#get_attachment) | **GET** /api/v2/testResults/{id}/attachments/{attachmentId}/info | Get Metadata of TestResult&#39;s attachment
+*TestResultsApi* | [**get_attachments**](docs/TestResultsApi.md#get_attachments) | **GET** /api/v2/testResults/{id}/attachments | Get all attachments of TestResult
+*TestRunsApi* | [**api_v2_test_runs_id_statistics_filter_post**](docs/TestRunsApi.md#api_v2_test_runs_id_statistics_filter_post) | **POST** /api/v2/testRuns/{id}/statistics/filter | Search for the test run test results and build statistics
+*TestRunsApi* | [**api_v2_test_runs_id_test_points_results_get**](docs/TestRunsApi.md#api_v2_test_runs_id_test_points_results_get) | **GET** /api/v2/testRuns/{id}/testPoints/results | Get test results from the test run grouped by test points
+*TestRunsApi* | [**api_v2_test_runs_id_test_results_bulk_put**](docs/TestRunsApi.md#api_v2_test_runs_id_test_results_bulk_put) | **PUT** /api/v2/testRuns/{id}/testResults/bulk | Partial edit of multiple test results in the test run
+*TestRunsApi* | [**api_v2_test_runs_id_test_results_last_modified_modification_date_get**](docs/TestRunsApi.md#api_v2_test_runs_id_test_results_last_modified_modification_date_get) | **GET** /api/v2/testRuns/{id}/testResults/lastModified/modificationDate | Get modification date of last test result of the test run
+*TestRunsApi* | [**api_v2_test_runs_search_post**](docs/TestRunsApi.md#api_v2_test_runs_search_post) | **POST** /api/v2/testRuns/search | Search for test runs
+*TestRunsApi* | [**complete_test_run**](docs/TestRunsApi.md#complete_test_run) | **POST** /api/v2/testRuns/{id}/complete | Complete TestRun
+*TestRunsApi* | [**create_and_fill_by_auto_tests**](docs/TestRunsApi.md#create_and_fill_by_auto_tests) | **POST** /api/v2/testRuns/byAutoTests | Create test runs based on autotests and configurations
+*TestRunsApi* | [**create_and_fill_by_configurations**](docs/TestRunsApi.md#create_and_fill_by_configurations) | **POST** /api/v2/testRuns/byConfigurations | Create test runs picking the needed test points
+*TestRunsApi* | [**create_and_fill_by_work_items**](docs/TestRunsApi.md#create_and_fill_by_work_items) | **POST** /api/v2/testRuns/byWorkItems | Create test run based on configurations and work items
+*TestRunsApi* | [**create_empty**](docs/TestRunsApi.md#create_empty) | **POST** /api/v2/testRuns | Create empty TestRun
+*TestRunsApi* | [**get_test_run_by_id**](docs/TestRunsApi.md#get_test_run_by_id) | **GET** /api/v2/testRuns/{id} | Get TestRun by Id
+*TestRunsApi* | [**set_auto_test_results_for_test_run**](docs/TestRunsApi.md#set_auto_test_results_for_test_run) | **POST** /api/v2/testRuns/{id}/testResults | Send test results to the test runs in the system
+*TestRunsApi* | [**start_test_run**](docs/TestRunsApi.md#start_test_run) | **POST** /api/v2/testRuns/{id}/start | Start TestRun
+*TestRunsApi* | [**stop_test_run**](docs/TestRunsApi.md#stop_test_run) | **POST** /api/v2/testRuns/{id}/stop | Stop TestRun
+*TestRunsApi* | [**update_empty**](docs/TestRunsApi.md#update_empty) | **PUT** /api/v2/testRuns | Update empty TestRun
+*TestSuitesApi* | [**add_test_points_to_test_suite**](docs/TestSuitesApi.md#add_test_points_to_test_suite) | **POST** /api/v2/testSuites/{id}/test-points | Add test-points to test suite
+*TestSuitesApi* | [**api_v2_test_suites_id_patch**](docs/TestSuitesApi.md#api_v2_test_suites_id_patch) | **PATCH** /api/v2/testSuites/{id} | Patch test suite
+*TestSuitesApi* | [**api_v2_test_suites_id_refresh_post**](docs/TestSuitesApi.md#api_v2_test_suites_id_refresh_post) | **POST** /api/v2/testSuites/{id}/refresh | Refresh test suite. Only dynamic test suites are supported by this method
+*TestSuitesApi* | [**create_test_suite**](docs/TestSuitesApi.md#create_test_suite) | **POST** /api/v2/testSuites | Create TestSuite
+*TestSuitesApi* | [**delete_test_suite**](docs/TestSuitesApi.md#delete_test_suite) | **DELETE** /api/v2/testSuites/{id} | Delete TestSuite
+*TestSuitesApi* | [**get_configurations_by_test_suite_id**](docs/TestSuitesApi.md#get_configurations_by_test_suite_id) | **GET** /api/v2/testSuites/{id}/configurations | Get Configurations By Id
+*TestSuitesApi* | [**get_test_points_by_id**](docs/TestSuitesApi.md#get_test_points_by_id) | **GET** /api/v2/testSuites/{id}/testPoints | Get TestPoints By Id
+*TestSuitesApi* | [**get_test_results_by_id**](docs/TestSuitesApi.md#get_test_results_by_id) | **GET** /api/v2/testSuites/{id}/testResults | Get TestResults By Id
+*TestSuitesApi* | [**get_test_suite_by_id**](docs/TestSuitesApi.md#get_test_suite_by_id) | **GET** /api/v2/testSuites/{id} | Get TestSuite by Id
+*TestSuitesApi* | [**get_work_items_by_id**](docs/TestSuitesApi.md#get_work_items_by_id) | **GET** /api/v2/testSuites/{id}/workItems | 
+*TestSuitesApi* | [**search_work_items**](docs/TestSuitesApi.md#search_work_items) | **POST** /api/v2/testSuites/{id}/workItems/search | Search WorkItems
+*TestSuitesApi* | [**set_configurations_by_test_suite_id**](docs/TestSuitesApi.md#set_configurations_by_test_suite_id) | **POST** /api/v2/testSuites/{id}/configurations | Set Configurations By TestSuite Id
+*TestSuitesApi* | [**set_work_items_by_test_suite_id**](docs/TestSuitesApi.md#set_work_items_by_test_suite_id) | **POST** /api/v2/testSuites/{id}/workItems | Set WorkItems By TestSuite Id
+*TestSuitesApi* | [**update_test_suite**](docs/TestSuitesApi.md#update_test_suite) | **PUT** /api/v2/testSuites | Update TestSuite
+*WebhooksApi* | [**api_v2_webhooks_get**](docs/WebhooksApi.md#api_v2_webhooks_get) | **GET** /api/v2/webhooks | Get all webhooks
+*WebhooksApi* | [**api_v2_webhooks_id_delete**](docs/WebhooksApi.md#api_v2_webhooks_id_delete) | **DELETE** /api/v2/webhooks/{id} | Delete webhook by ID
+*WebhooksApi* | [**api_v2_webhooks_id_get**](docs/WebhooksApi.md#api_v2_webhooks_id_get) | **GET** /api/v2/webhooks/{id} | Get webhook by ID
+*WebhooksApi* | [**api_v2_webhooks_id_put**](docs/WebhooksApi.md#api_v2_webhooks_id_put) | **PUT** /api/v2/webhooks/{id} | Edit webhook by ID
+*WebhooksApi* | [**api_v2_webhooks_post**](docs/WebhooksApi.md#api_v2_webhooks_post) | **POST** /api/v2/webhooks | Create webhook
+*WebhooksApi* | [**api_v2_webhooks_search_post**](docs/WebhooksApi.md#api_v2_webhooks_search_post) | **POST** /api/v2/webhooks/search | Search for webhooks
+*WebhooksApi* | [**api_v2_webhooks_special_variables_get**](docs/WebhooksApi.md#api_v2_webhooks_special_variables_get) | **GET** /api/v2/webhooks/specialVariables | Get special variables for webhook event type
+*WebhooksLogsApi* | [**api_v2_webhooks_logs_get**](docs/WebhooksLogsApi.md#api_v2_webhooks_logs_get) | **GET** /api/v2/webhooks/logs | Get all webhook logs
+*WebhooksLogsApi* | [**api_v2_webhooks_logs_id_delete**](docs/WebhooksLogsApi.md#api_v2_webhooks_logs_id_delete) | **DELETE** /api/v2/webhooks/logs/{id} | Delete webhook log by ID
+*WebhooksLogsApi* | [**api_v2_webhooks_logs_id_get**](docs/WebhooksLogsApi.md#api_v2_webhooks_logs_id_get) | **GET** /api/v2/webhooks/logs/{id} | Get webhook log by ID
+*WorkItemsApi* | [**api_v2_work_items_id_attachments_post**](docs/WorkItemsApi.md#api_v2_work_items_id_attachments_post) | **POST** /api/v2/workItems/{id}/attachments | Upload and link attachment to WorkItem
+*WorkItemsApi* | [**api_v2_work_items_id_check_list_transform_to_test_case_post**](docs/WorkItemsApi.md#api_v2_work_items_id_check_list_transform_to_test_case_post) | **POST** /api/v2/workItems/{id}/checkList/transformTo/testCase | Transform CheckList to TestCase
+*WorkItemsApi* | [**api_v2_work_items_id_history_get**](docs/WorkItemsApi.md#api_v2_work_items_id_history_get) | **GET** /api/v2/workItems/{id}/history | Get change history of WorkItem
+*WorkItemsApi* | [**api_v2_work_items_id_like_delete**](docs/WorkItemsApi.md#api_v2_work_items_id_like_delete) | **DELETE** /api/v2/workItems/{id}/like | Delete like from WorkItem
+*WorkItemsApi* | [**api_v2_work_items_id_like_post**](docs/WorkItemsApi.md#api_v2_work_items_id_like_post) | **POST** /api/v2/workItems/{id}/like | Set like to WorkItem
+*WorkItemsApi* | [**api_v2_work_items_id_likes_count_get**](docs/WorkItemsApi.md#api_v2_work_items_id_likes_count_get) | **GET** /api/v2/workItems/{id}/likes/count | Get likes count of WorkItem
+*WorkItemsApi* | [**api_v2_work_items_id_likes_get**](docs/WorkItemsApi.md#api_v2_work_items_id_likes_get) | **GET** /api/v2/workItems/{id}/likes | Get likes of WorkItem
+*WorkItemsApi* | [**api_v2_work_items_id_test_results_history_get**](docs/WorkItemsApi.md#api_v2_work_items_id_test_results_history_get) | **GET** /api/v2/workItems/{id}/testResults/history | Get test results history of WorkItem
+*WorkItemsApi* | [**api_v2_work_items_id_version_version_id_actual_post**](docs/WorkItemsApi.md#api_v2_work_items_id_version_version_id_actual_post) | **POST** /api/v2/workItems/{id}/version/{versionId}/actual | Set WorkItem as actual
+*WorkItemsApi* | [**api_v2_work_items_move_post**](docs/WorkItemsApi.md#api_v2_work_items_move_post) | **POST** /api/v2/workItems/move | Move WorkItem to another section
+*WorkItemsApi* | [**api_v2_work_items_search_post**](docs/WorkItemsApi.md#api_v2_work_items_search_post) | **POST** /api/v2/workItems/search | Search for work items
+*WorkItemsApi* | [**api_v2_work_items_shared_step_id_references_sections_post**](docs/WorkItemsApi.md#api_v2_work_items_shared_step_id_references_sections_post) | **POST** /api/v2/workItems/{sharedStepId}/references/sections | Get SharedStep references in sections
+*WorkItemsApi* | [**api_v2_work_items_shared_step_id_references_work_items_post**](docs/WorkItemsApi.md#api_v2_work_items_shared_step_id_references_work_items_post) | **POST** /api/v2/workItems/{sharedStepId}/references/workItems | Get SharedStep references in workitems
+*WorkItemsApi* | [**api_v2_work_items_shared_steps_shared_step_id_references_get**](docs/WorkItemsApi.md#api_v2_work_items_shared_steps_shared_step_id_references_get) | **GET** /api/v2/workItems/sharedSteps/{sharedStepId}/references | Get SharedStep references
+*WorkItemsApi* | [**create_work_item**](docs/WorkItemsApi.md#create_work_item) | **POST** /api/v2/workItems | Create Test Case, Checklist or Shared Step
+*WorkItemsApi* | [**delete_all_work_items_from_auto_test**](docs/WorkItemsApi.md#delete_all_work_items_from_auto_test) | **DELETE** /api/v2/workItems/{id}/autoTests | Delete all links AutoTests from WorkItem by Id or GlobalId
+*WorkItemsApi* | [**delete_work_item**](docs/WorkItemsApi.md#delete_work_item) | **DELETE** /api/v2/workItems/{id} | Delete Test Case, Checklist or Shared Step by Id or GlobalId
+*WorkItemsApi* | [**get_auto_tests_for_work_item**](docs/WorkItemsApi.md#get_auto_tests_for_work_item) | **GET** /api/v2/workItems/{id}/autoTests | Get all AutoTests linked to WorkItem by Id or GlobalId
+*WorkItemsApi* | [**get_iterations**](docs/WorkItemsApi.md#get_iterations) | **GET** /api/v2/workItems/{id}/iterations | Get iterations by workitem Id or GlobalId
+*WorkItemsApi* | [**get_work_item_by_id**](docs/WorkItemsApi.md#get_work_item_by_id) | **GET** /api/v2/workItems/{id} | Get Test Case, Checklist or Shared Step by Id or GlobalId
+*WorkItemsApi* | [**get_work_item_chronology**](docs/WorkItemsApi.md#get_work_item_chronology) | **GET** /api/v2/workItems/{id}/chronology | Get WorkItem chronology by Id or GlobalId
+*WorkItemsApi* | [**get_work_item_versions**](docs/WorkItemsApi.md#get_work_item_versions) | **GET** /api/v2/workItems/{id}/versions | Get WorkItem versions
+*WorkItemsApi* | [**purge_work_item**](docs/WorkItemsApi.md#purge_work_item) | **POST** /api/v2/workItems/{id}/purge | Permanently delete test case, checklist or shared steps from archive
+*WorkItemsApi* | [**restore_work_item**](docs/WorkItemsApi.md#restore_work_item) | **POST** /api/v2/workItems/{id}/restore | Restore test case, checklist or shared steps from archive
+*WorkItemsApi* | [**update_work_item**](docs/WorkItemsApi.md#update_work_item) | **PUT** /api/v2/workItems | Update Test Case, Checklist or Shared Step
+*WorkItemsCommentsApi* | [**api_v2_work_items_comments_comment_id_delete**](docs/WorkItemsCommentsApi.md#api_v2_work_items_comments_comment_id_delete) | **DELETE** /api/v2/workItems/comments/{commentId} | Delete WorkItem comment
+*WorkItemsCommentsApi* | [**api_v2_work_items_comments_post**](docs/WorkItemsCommentsApi.md#api_v2_work_items_comments_post) | **POST** /api/v2/workItems/comments | Create WorkItem comment
+*WorkItemsCommentsApi* | [**api_v2_work_items_comments_put**](docs/WorkItemsCommentsApi.md#api_v2_work_items_comments_put) | **PUT** /api/v2/workItems/comments | Update work item comment
+*WorkItemsCommentsApi* | [**api_v2_work_items_id_comments_get**](docs/WorkItemsCommentsApi.md#api_v2_work_items_id_comments_get) | **GET** /api/v2/workItems/{id}/comments | Get work item comments
+
+
+## Documentation For Models
+
+ - You can see the documentation [here](docs/README.md).
+
+
+# Contributing
+
+You can help to develop the project. Any contributions are **greatly appreciated**.
+
+* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testgear-tms/api-client-python/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
+* Please make sure you check your spelling and grammar.
+* Create individual PR for each suggestion.
+* Please also read through the [Code Of Conduct](https://github.com/testgear-tms/api-client-python/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
+
+
+# License
+
+Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testgear-tms/api-client-python/blob/master/LICENSE.md) for more information.
+
```

