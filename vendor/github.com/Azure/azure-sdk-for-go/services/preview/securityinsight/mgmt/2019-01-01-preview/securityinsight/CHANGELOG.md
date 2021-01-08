Generated from https://github.com/Azure/azure-rest-api-specs/tree/3c764635e7d442b3e74caf593029fcd440b3ef82

Code generator @microsoft.azure/autorest.go@~2.1.161

## Breaking Changes

- Function `NewBookmarkListPage` parameter(s) have been changed from `(func(context.Context, BookmarkList) (BookmarkList, error))` to `(BookmarkList, func(context.Context, BookmarkList) (BookmarkList, error))`
- Function `NewCaseRelationListPage` parameter(s) have been changed from `(func(context.Context, CaseRelationList) (CaseRelationList, error))` to `(CaseRelationList, func(context.Context, CaseRelationList) (CaseRelationList, error))`
- Function `NewCaseCommentListPage` parameter(s) have been changed from `(func(context.Context, CaseCommentList) (CaseCommentList, error))` to `(CaseCommentList, func(context.Context, CaseCommentList) (CaseCommentList, error))`
- Function `NewIncidentCommentListPage` parameter(s) have been changed from `(func(context.Context, IncidentCommentList) (IncidentCommentList, error))` to `(IncidentCommentList, func(context.Context, IncidentCommentList) (IncidentCommentList, error))`
- Function `NewOperationsListPage` parameter(s) have been changed from `(func(context.Context, OperationsList) (OperationsList, error))` to `(OperationsList, func(context.Context, OperationsList) (OperationsList, error))`
- Function `NewAlertRuleTemplatesListPage` parameter(s) have been changed from `(func(context.Context, AlertRuleTemplatesList) (AlertRuleTemplatesList, error))` to `(AlertRuleTemplatesList, func(context.Context, AlertRuleTemplatesList) (AlertRuleTemplatesList, error))`
- Function `NewEntityQueryListPage` parameter(s) have been changed from `(func(context.Context, EntityQueryList) (EntityQueryList, error))` to `(EntityQueryList, func(context.Context, EntityQueryList) (EntityQueryList, error))`
- Function `NewRelationListPage` parameter(s) have been changed from `(func(context.Context, RelationList) (RelationList, error))` to `(RelationList, func(context.Context, RelationList) (RelationList, error))`
- Function `NewEntityListPage` parameter(s) have been changed from `(func(context.Context, EntityList) (EntityList, error))` to `(EntityList, func(context.Context, EntityList) (EntityList, error))`
- Function `NewDataConnectorListPage` parameter(s) have been changed from `(func(context.Context, DataConnectorList) (DataConnectorList, error))` to `(DataConnectorList, func(context.Context, DataConnectorList) (DataConnectorList, error))`
- Function `NewCaseListPage` parameter(s) have been changed from `(func(context.Context, CaseList) (CaseList, error))` to `(CaseList, func(context.Context, CaseList) (CaseList, error))`
- Function `NewOfficeConsentListPage` parameter(s) have been changed from `(func(context.Context, OfficeConsentList) (OfficeConsentList, error))` to `(OfficeConsentList, func(context.Context, OfficeConsentList) (OfficeConsentList, error))`
- Function `NewActionsListPage` parameter(s) have been changed from `(func(context.Context, ActionsList) (ActionsList, error))` to `(ActionsList, func(context.Context, ActionsList) (ActionsList, error))`
- Function `NewAlertRulesListPage` parameter(s) have been changed from `(func(context.Context, AlertRulesList) (AlertRulesList, error))` to `(AlertRulesList, func(context.Context, AlertRulesList) (AlertRulesList, error))`
- Function `NewIncidentListPage` parameter(s) have been changed from `(func(context.Context, IncidentList) (IncidentList, error))` to `(IncidentList, func(context.Context, IncidentList) (IncidentList, error))`
- Type of `SettingsKind.Kind` has been changed from `*string` to `SettingKind`

## New Content

- New const `SingleAlert`
- New const `PreAttack`
- New const `EntityTimelineKindSecurityAlert`
- New const `KindOfficeATP`
- New const `DataConnectorKindOfficeATP`
- New const `AuditLogs`
- New const `SecurityEvent`
- New const `KindBasicEntityTimelineItemKindActivity`
- New const `SettingKindEyesOn`
- New const `AzureActivity`
- New const `SettingKindUeba`
- New const `Office365AdvancedThreatProtection`
- New const `KindBookmark`
- New const `KindBasicEntityTimelineItemKindSecurityAlert`
- New const `Localfile`
- New const `Unsorted`
- New const `EntityTimelineKindActivity`
- New const `AlertPerResult`
- New const `Descending`
- New const `Remotestorage`
- New const `SigninLogs`
- New const `KindUeba`
- New const `EntityTimelineKindBookmark`
- New const `KindEntityAnalytics`
- New const `KindBasicEntityTimelineItemKindBookmark`
- New const `SettingKindEntityAnalytics`
- New const `Indicator`
- New const `Ascending`
- New const `KindThreatIntelligenceInformation`
- New const `KindBasicDataConnectorsCheckRequirementsKindOfficeATP`
- New const `KindBasicEntityTimelineItemKindEntityTimelineItem`
- New const `MicrosoftDefenderAdvancedThreatProtection`
- New const `KindIndicator`
- New function `EntityAnalytics.AsUeba() (*Ueba, bool)`
- New function `PossibleUebaDataSourcesValues() []UebaDataSources`
- New function `ThreatIntelligenceIndicatorModelForRequestBody.MarshalJSON() ([]byte, error)`
- New function `WatchlistsClient.DeletePreparer(context.Context, string, string, string, string) (*http.Request, error)`
- New function `ThreatIntelligenceIndicatorClient.ReplaceTagsSender(*http.Request) (*http.Response, error)`
- New function `RegistryValueEntity.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `IncidentsClient.ListOfBookmarksSender(*http.Request) (*http.Response, error)`
- New function `*ThreatIntelligenceInformationListPage.Next() error`
- New function `IncidentsClient.ListOfAlertsSender(*http.Request) (*http.Response, error)`
- New function `*ThreatIntelligenceInformationListIterator.Next() error`
- New function `ThreatIntelligenceInformationList.IsEmpty() bool`
- New function `OfficeATPCheckRequirements.AsTICheckRequirements() (*TICheckRequirements, bool)`
- New function `WatchlistsClient.ListPreparer(context.Context, string, string, string) (*http.Request, error)`
- New function `HuntingBookmark.AsURLEntity() (*URLEntity, bool)`
- New function `HuntingBookmark.AsProcessEntity() (*ProcessEntity, bool)`
- New function `ThreatIntelligenceIndicatorModel.AsThreatIntelligenceInformation() (*ThreatIntelligenceInformation, bool)`
- New function `*ThreatIntelligenceIndicatorModelForRequestBody.UnmarshalJSON([]byte) error`
- New function `EntitiesGetTimelineClient.ListPreparer(context.Context, string, string, string, string, EntityTimelineParameters) (*http.Request, error)`
- New function `NewThreatIntelligenceIndicatorClientWithBaseURI(string, string) ThreatIntelligenceIndicatorClient`
- New function `EyesOn.AsEntityAnalytics() (*EntityAnalytics, bool)`
- New function `ThreatIntelligenceIndicatorsClient.List(context.Context, string, string, string, string, *int32, string, string) (ThreatIntelligenceInformationListPage, error)`
- New function `IncidentCommentsClient.DeleteComment(context.Context, string, string, string, string, string) (autorest.Response, error)`
- New function `HuntingBookmark.MarshalJSON() ([]byte, error)`
- New function `*EntityAnalytics.UnmarshalJSON([]byte) error`
- New function `OfficeATPCheckRequirements.AsMCASCheckRequirements() (*MCASCheckRequirements, bool)`
- New function `HuntingBookmark.AsFileHashEntity() (*FileHashEntity, bool)`
- New function `ThreatIntelligenceInformationListIterator.Response() ThreatIntelligenceInformationList`
- New function `WatchlistsClient.Delete(context.Context, string, string, string, string) (autorest.Response, error)`
- New function `ProcessEntity.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `WatchlistsClient.DeleteSender(*http.Request) (*http.Response, error)`
- New function `*Ueba.UnmarshalJSON([]byte) error`
- New function `WatchlistListPage.Response() WatchlistList`
- New function `ThreatIntelligenceIndicatorClient.GetResponder(*http.Response) (ThreatIntelligenceInformationModel, error)`
- New function `BookmarkTimelineItem.AsBookmarkTimelineItem() (*BookmarkTimelineItem, bool)`
- New function `HuntingBookmark.AsFileEntity() (*FileEntity, bool)`
- New function `ThreatIntelligenceIndicatorClient.CreateSender(*http.Request) (*http.Response, error)`
- New function `HuntingBookmark.AsAzureResourceEntity() (*AzureResourceEntity, bool)`
- New function `ActivityTimelineItem.MarshalJSON() ([]byte, error)`
- New function `ActivityTimelineItem.AsSecurityAlertTimelineItem() (*SecurityAlertTimelineItem, bool)`
- New function `ThreatIntelligenceIndicatorClient.DeletePreparer(context.Context, string, string, string, string) (*http.Request, error)`
- New function `EntityAnalytics.AsEntityAnalytics() (*EntityAnalytics, bool)`
- New function `MCASDataConnector.AsOfficeATPDataConnector() (*OfficeATPDataConnector, bool)`
- New function `*WatchlistListPage.NextWithContext(context.Context) error`
- New function `ThreatIntelligenceIndicatorClient.ReplaceTagsPreparer(context.Context, string, string, string, string, ThreatIntelligenceIndicatorModelForRequestBody) (*http.Request, error)`
- New function `PossibleKindBasicThreatIntelligenceInformationValues() []KindBasicThreatIntelligenceInformation`
- New function `WatchlistList.IsEmpty() bool`
- New function `Ueba.AsEyesOn() (*EyesOn, bool)`
- New function `HuntingBookmark.AsIPEntity() (*IPEntity, bool)`
- New function `ThreatIntelligenceIndicatorClient.QueryIndicatorsPreparer(context.Context, string, string, string, ThreatIntelligenceFilteringCriteria) (*http.Request, error)`
- New function `HuntingBookmarkProperties.MarshalJSON() ([]byte, error)`
- New function `IncidentCommentsClient.DeleteCommentResponder(*http.Response) (autorest.Response, error)`
- New function `MDATPCheckRequirements.AsOfficeATPCheckRequirements() (*OfficeATPCheckRequirements, bool)`
- New function `IncidentsClient.ListOfBookmarks(context.Context, string, string, string, string) (IncidentBookmarkList, error)`
- New function `DataConnectorsCheckRequirements.AsOfficeATPCheckRequirements() (*OfficeATPCheckRequirements, bool)`
- New function `FileHashEntity.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `EyesOn.AsUeba() (*Ueba, bool)`
- New function `PossibleThreatIntelligenceSortingCriteriaValues() []ThreatIntelligenceSortingCriteria`
- New function `EntityAnalytics.AsBasicSettings() (BasicSettings, bool)`
- New function `IPEntity.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `AATPCheckRequirements.AsOfficeATPCheckRequirements() (*OfficeATPCheckRequirements, bool)`
- New function `PossibleSourceValues() []Source`
- New function `OfficeATPDataConnector.MarshalJSON() ([]byte, error)`
- New function `OfficeATPDataConnector.AsAATPDataConnector() (*AATPDataConnector, bool)`
- New function `FileEntity.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `HuntingBookmark.AsMalwareEntity() (*MalwareEntity, bool)`
- New function `AwsCloudTrailCheckRequirements.AsOfficeATPCheckRequirements() (*OfficeATPCheckRequirements, bool)`
- New function `ThreatIntelligenceIndicatorClient.AppendTagsResponder(*http.Response) (autorest.Response, error)`
- New function `TIDataConnector.AsOfficeATPDataConnector() (*OfficeATPDataConnector, bool)`
- New function `ThreatIntelligenceInformationListPage.Response() ThreatIntelligenceInformationList`
- New function `NewWatchlistsClientWithBaseURI(string, string) WatchlistsClient`
- New function `*HuntingBookmark.UnmarshalJSON([]byte) error`
- New function `ThreatIntelligenceIndicatorClient.QueryIndicatorsSender(*http.Request) (*http.Response, error)`
- New function `OfficeATPDataConnector.AsTIDataConnector() (*TIDataConnector, bool)`
- New function `NewWatchlistListIterator(WatchlistListPage) WatchlistListIterator`
- New function `ThreatIntelligenceInformation.AsThreatIntelligenceInformation() (*ThreatIntelligenceInformation, bool)`
- New function `CloudApplicationEntity.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `ThreatIntelligenceIndicatorMetricsClient.List(context.Context, string, string, string) (ThreatIntelligenceMetricsList, error)`
- New function `WatchlistListPage.NotDone() bool`
- New function `WatchlistsClient.ListComplete(context.Context, string, string, string) (WatchlistListIterator, error)`
- New function `ThreatIntelligenceInformation.AsThreatIntelligenceIndicatorModel() (*ThreatIntelligenceIndicatorModel, bool)`
- New function `TiTaxiiDataConnector.AsOfficeATPDataConnector() (*OfficeATPDataConnector, bool)`
- New function `ThreatIntelligenceIndicatorClient.Delete(context.Context, string, string, string, string) (autorest.Response, error)`
- New function `ThreatIntelligenceIndicatorProperties.MarshalJSON() ([]byte, error)`
- New function `NewEntitiesGetTimelineClient(string) EntitiesGetTimelineClient`
- New function `ThreatIntelligenceIndicatorClient.QueryIndicatorsComplete(context.Context, string, string, string, ThreatIntelligenceFilteringCriteria) (ThreatIntelligenceInformationListIterator, error)`
- New function `OfficeATPDataConnector.AsBasicDataConnector() (BasicDataConnector, bool)`
- New function `ThreatIntelligenceInformation.AsBasicThreatIntelligenceInformation() (BasicThreatIntelligenceInformation, bool)`
- New function `IncidentsClient.ListOfEntitiesResponder(*http.Response) (IncidentEntitiesResponse, error)`
- New function `IncidentsClient.ListOfEntities(context.Context, string, string, string, string) (IncidentEntitiesResponse, error)`
- New function `EntityTimelineItem.AsEntityTimelineItem() (*EntityTimelineItem, bool)`
- New function `OfficeATPCheckRequirements.AsDataConnectorsCheckRequirements() (*DataConnectorsCheckRequirements, bool)`
- New function `EntitiesGetTimelineClient.List(context.Context, string, string, string, string, EntityTimelineParameters) (EntityTimelineResponse, error)`
- New function `EntityTimelineItem.AsSecurityAlertTimelineItem() (*SecurityAlertTimelineItem, bool)`
- New function `ThreatIntelligenceInformationListPage.Values() []BasicThreatIntelligenceInformation`
- New function `BookmarkTimelineItem.AsEntityTimelineItem() (*EntityTimelineItem, bool)`
- New function `HuntingBookmark.AsRegistryValueEntity() (*RegistryValueEntity, bool)`
- New function `IncidentCommentsClient.DeleteCommentPreparer(context.Context, string, string, string, string, string) (*http.Request, error)`
- New function `WatchlistsClient.GetSender(*http.Request) (*http.Response, error)`
- New function `*OfficeATPCheckRequirements.UnmarshalJSON([]byte) error`
- New function `RegistryKeyEntity.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `OfficeATPCheckRequirements.AsOfficeATPCheckRequirements() (*OfficeATPCheckRequirements, bool)`
- New function `NewWatchlistListPage(WatchlistList, func(context.Context, WatchlistList) (WatchlistList, error)) WatchlistListPage`
- New function `WatchlistsClient.CreateSender(*http.Request) (*http.Response, error)`
- New function `IncidentsClient.ListOfBookmarksResponder(*http.Response) (IncidentBookmarkList, error)`
- New function `OfficeATPDataConnector.AsASCDataConnector() (*ASCDataConnector, bool)`
- New function `Ueba.AsEntityAnalytics() (*EntityAnalytics, bool)`
- New function `ThreatIntelligenceIndicatorClient.DeleteSender(*http.Request) (*http.Response, error)`
- New function `ActivityTimelineItem.AsBasicEntityTimelineItem() (BasicEntityTimelineItem, bool)`
- New function `NewThreatIntelligenceIndicatorsClientWithBaseURI(string, string) ThreatIntelligenceIndicatorsClient`
- New function `Settings.AsEntityAnalytics() (*EntityAnalytics, bool)`
- New function `ASCCheckRequirements.AsOfficeATPCheckRequirements() (*OfficeATPCheckRequirements, bool)`
- New function `EntitiesGetTimelineClient.ListResponder(*http.Response) (EntityTimelineResponse, error)`
- New function `BookmarkTimelineItem.AsSecurityAlertTimelineItem() (*SecurityAlertTimelineItem, bool)`
- New function `ThreatIntelligenceIndicatorClient.QueryIndicatorsResponder(*http.Response) (ThreatIntelligenceInformationList, error)`
- New function `*Watchlist.UnmarshalJSON([]byte) error`
- New function `ActivityTimelineItem.AsEntityTimelineItem() (*EntityTimelineItem, bool)`
- New function `MCASCheckRequirements.AsOfficeATPCheckRequirements() (*OfficeATPCheckRequirements, bool)`
- New function `*WatchlistListPage.Next() error`
- New function `DNSEntity.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `EntityTimelineItem.AsBookmarkTimelineItem() (*BookmarkTimelineItem, bool)`
- New function `SecurityAlertTimelineItem.AsActivityTimelineItem() (*ActivityTimelineItem, bool)`
- New function `PossibleThreatIntelligenceResourceKindValues() []ThreatIntelligenceResourceKind`
- New function `IncidentsClient.ListOfAlerts(context.Context, string, string, string, string) (IncidentAlertList, error)`
- New function `NewThreatIntelligenceIndicatorMetricsClientWithBaseURI(string, string) ThreatIntelligenceIndicatorMetricsClient`
- New function `SecurityAlertTimelineItem.AsEntityTimelineItem() (*EntityTimelineItem, bool)`
- New function `OfficeATPDataConnector.AsMCASDataConnector() (*MCASDataConnector, bool)`
- New function `WatchlistsClient.DeleteResponder(*http.Response) (autorest.Response, error)`
- New function `ThreatIntelligenceInformation.MarshalJSON() ([]byte, error)`
- New function `ThreatIntelligenceIndicatorClient.AppendTagsPreparer(context.Context, string, string, string, string, ThreatIntelligenceAppendTags) (*http.Request, error)`
- New function `ThreatIntelligenceIndicatorsClient.ListSender(*http.Request) (*http.Response, error)`
- New function `ThreatIntelligenceIndicatorsClient.ListResponder(*http.Response) (ThreatIntelligenceInformationList, error)`
- New function `PossibleSettingKindValues() []SettingKind`
- New function `Watchlist.MarshalJSON() ([]byte, error)`
- New function `EntitiesGetTimelineClient.ListSender(*http.Request) (*http.Response, error)`
- New function `*IncidentEntitiesResponse.UnmarshalJSON([]byte) error`
- New function `OfficeATPDataConnector.AsDataConnector() (*DataConnector, bool)`
- New function `HuntingBookmark.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `ThreatIntelligenceIndicatorClient.CreateIndicatorSender(*http.Request) (*http.Response, error)`
- New function `ThreatIntelligenceIndicatorClient.CreatePreparer(context.Context, string, string, string, string, ThreatIntelligenceIndicatorModelForRequestBody) (*http.Request, error)`
- New function `OfficeATPCheckRequirements.AsBasicDataConnectorsCheckRequirements() (BasicDataConnectorsCheckRequirements, bool)`
- New function `PossibleEntityTimelineKindValues() []EntityTimelineKind`
- New function `*ThreatIntelligenceIndicatorModel.UnmarshalJSON([]byte) error`
- New function `ThreatIntelligenceIndicatorClient.ReplaceTagsResponder(*http.Response) (ThreatIntelligenceInformationModel, error)`
- New function `EntityAnalytics.AsEyesOn() (*EyesOn, bool)`
- New function `Entity.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `*ThreatIntelligenceInformationListIterator.NextWithContext(context.Context) error`
- New function `ThreatIntelligenceIndicatorClient.CreateIndicatorPreparer(context.Context, string, string, string, ThreatIntelligenceIndicatorModelForRequestBody) (*http.Request, error)`
- New function `ThreatIntelligenceIndicatorClient.CreateIndicator(context.Context, string, string, string, ThreatIntelligenceIndicatorModelForRequestBody) (ThreatIntelligenceInformationModel, error)`
- New function `EntityTimelineItem.MarshalJSON() ([]byte, error)`
- New function `*ThreatIntelligenceInformationListPage.NextWithContext(context.Context) error`
- New function `OfficeATPCheckRequirements.AsAADCheckRequirements() (*AADCheckRequirements, bool)`
- New function `IncidentsClient.ListOfAlertsResponder(*http.Response) (IncidentAlertList, error)`
- New function `ThreatIntelligenceIndicatorModel.AsThreatIntelligenceIndicatorModel() (*ThreatIntelligenceIndicatorModel, bool)`
- New function `WatchlistListIterator.Response() WatchlistList`
- New function `HuntingBookmark.AsAccountEntity() (*AccountEntity, bool)`
- New function `WatchlistListIterator.Value() Watchlist`
- New function `Ueba.AsSettings() (*Settings, bool)`
- New function `SecurityAlertTimelineItem.AsBasicEntityTimelineItem() (BasicEntityTimelineItem, bool)`
- New function `OfficeATPCheckRequirements.AsMDATPCheckRequirements() (*MDATPCheckRequirements, bool)`
- New function `AADDataConnector.AsOfficeATPDataConnector() (*OfficeATPDataConnector, bool)`
- New function `ThreatIntelligenceIndicatorClient.DeleteResponder(*http.Response) (autorest.Response, error)`
- New function `*ThreatIntelligenceInformationList.UnmarshalJSON([]byte) error`
- New function `NewThreatIntelligenceInformationListIterator(ThreatIntelligenceInformationListPage) ThreatIntelligenceInformationListIterator`
- New function `Ueba.MarshalJSON() ([]byte, error)`
- New function `ThreatIntelligenceIndicatorClient.GetSender(*http.Request) (*http.Response, error)`
- New function `ThreatIntelligenceIndicatorClient.ReplaceTags(context.Context, string, string, string, string, ThreatIntelligenceIndicatorModelForRequestBody) (ThreatIntelligenceInformationModel, error)`
- New function `EntityAnalytics.AsSettings() (*Settings, bool)`
- New function `HuntingBookmark.AsIoTDeviceEntity() (*IoTDeviceEntity, bool)`
- New function `OfficeATPDataConnector.AsOfficeDataConnector() (*OfficeDataConnector, bool)`
- New function `AzureResourceEntity.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `HuntingBookmark.AsSecurityAlert() (*SecurityAlert, bool)`
- New function `ThreatIntelligenceIndicatorsClient.ListComplete(context.Context, string, string, string, string, *int32, string, string) (ThreatIntelligenceInformationListIterator, error)`
- New function `ThreatIntelligenceInformationListPage.NotDone() bool`
- New function `*OfficeATPDataConnector.UnmarshalJSON([]byte) error`
- New function `MalwareEntity.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `TICheckRequirements.AsOfficeATPCheckRequirements() (*OfficeATPCheckRequirements, bool)`
- New function `SecurityAlertTimelineItem.MarshalJSON() ([]byte, error)`
- New function `OfficeATPDataConnector.AsAADDataConnector() (*AADDataConnector, bool)`
- New function `BookmarkTimelineItem.MarshalJSON() ([]byte, error)`
- New function `OfficeATPCheckRequirements.AsAwsCloudTrailCheckRequirements() (*AwsCloudTrailCheckRequirements, bool)`
- New function `OfficeATPCheckRequirements.AsTiTaxiiCheckRequirements() (*TiTaxiiCheckRequirements, bool)`
- New function `EntityAnalytics.MarshalJSON() ([]byte, error)`
- New function `HuntingBookmark.AsEntity() (*Entity, bool)`
- New function `*EntityTimelineResponse.UnmarshalJSON([]byte) error`
- New function `IncidentsClient.ListOfEntitiesPreparer(context.Context, string, string, string, string) (*http.Request, error)`
- New function `AATPDataConnector.AsOfficeATPDataConnector() (*OfficeATPDataConnector, bool)`
- New function `ActivityTimelineItem.AsBookmarkTimelineItem() (*BookmarkTimelineItem, bool)`
- New function `AwsCloudTrailDataConnector.AsOfficeATPDataConnector() (*OfficeATPDataConnector, bool)`
- New function `NewThreatIntelligenceIndicatorMetricsClient(string) ThreatIntelligenceIndicatorMetricsClient`
- New function `SecurityAlert.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `*ThreatIntelligenceInformationModel.UnmarshalJSON([]byte) error`
- New function `SecurityAlertTimelineItem.AsSecurityAlertTimelineItem() (*SecurityAlertTimelineItem, bool)`
- New function `OfficeATPDataConnector.AsOfficeATPDataConnector() (*OfficeATPDataConnector, bool)`
- New function `IncidentCommentsClient.DeleteCommentSender(*http.Request) (*http.Response, error)`
- New function `ThreatIntelligenceIndicatorsClient.ListPreparer(context.Context, string, string, string, string, *int32, string, string) (*http.Request, error)`
- New function `ThreatIntelligenceIndicatorMetricsClient.ListSender(*http.Request) (*http.Response, error)`
- New function `HuntingBookmark.AsSecurityGroupEntity() (*SecurityGroupEntity, bool)`
- New function `Ueba.AsUeba() (*Ueba, bool)`
- New function `HuntingBookmark.AsDNSEntity() (*DNSEntity, bool)`
- New function `IncidentsClient.ListOfAlertsPreparer(context.Context, string, string, string, string) (*http.Request, error)`
- New function `WatchlistsClient.Create(context.Context, string, string, string, string, Watchlist) (Watchlist, error)`
- New function `AccountEntity.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `OfficeATPCheckRequirements.AsASCCheckRequirements() (*ASCCheckRequirements, bool)`
- New function `NewWatchlistsClient(string) WatchlistsClient`
- New function `ThreatIntelligenceIndicatorClient.AppendTags(context.Context, string, string, string, string, ThreatIntelligenceAppendTags) (autorest.Response, error)`
- New function `OfficeATPDataConnector.AsMDATPDataConnector() (*MDATPDataConnector, bool)`
- New function `ThreatIntelligenceInformationList.MarshalJSON() ([]byte, error)`
- New function `AADCheckRequirements.AsOfficeATPCheckRequirements() (*OfficeATPCheckRequirements, bool)`
- New function `ThreatIntelligenceIndicatorClient.AppendTagsSender(*http.Request) (*http.Response, error)`
- New function `OfficeDataConnector.AsOfficeATPDataConnector() (*OfficeATPDataConnector, bool)`
- New function `WatchlistListPage.Values() []Watchlist`
- New function `ThreatIntelligenceIndicatorMetricsClient.ListPreparer(context.Context, string, string, string) (*http.Request, error)`
- New function `IncidentsClient.ListOfBookmarksPreparer(context.Context, string, string, string, string) (*http.Request, error)`
- New function `OfficeATPCheckRequirements.AsAATPCheckRequirements() (*AATPCheckRequirements, bool)`
- New function `WatchlistList.MarshalJSON() ([]byte, error)`
- New function `WatchlistsClient.CreatePreparer(context.Context, string, string, string, string, Watchlist) (*http.Request, error)`
- New function `WatchlistsClient.List(context.Context, string, string, string) (WatchlistListPage, error)`
- New function `WatchlistsClient.ListSender(*http.Request) (*http.Response, error)`
- New function `HuntingBookmark.AsHostEntity() (*HostEntity, bool)`
- New function `EntityTimelineItem.AsActivityTimelineItem() (*ActivityTimelineItem, bool)`
- New function `NewEntitiesGetTimelineClientWithBaseURI(string, string) EntitiesGetTimelineClient`
- New function `ActivityTimelineItem.AsActivityTimelineItem() (*ActivityTimelineItem, bool)`
- New function `NewThreatIntelligenceInformationListPage(ThreatIntelligenceInformationList, func(context.Context, ThreatIntelligenceInformationList) (ThreatIntelligenceInformationList, error)) ThreatIntelligenceInformationListPage`
- New function `EntityTimelineItem.AsBasicEntityTimelineItem() (BasicEntityTimelineItem, bool)`
- New function `Settings.AsUeba() (*Ueba, bool)`
- New function `MDATPDataConnector.AsOfficeATPDataConnector() (*OfficeATPDataConnector, bool)`
- New function `ThreatIntelligenceIndicatorClient.GetPreparer(context.Context, string, string, string, string) (*http.Request, error)`
- New function `NewThreatIntelligenceIndicatorsClient(string) ThreatIntelligenceIndicatorsClient`
- New function `ThreatIntelligenceIndicatorClient.CreateIndicatorResponder(*http.Response) (ThreatIntelligenceInformationModel, error)`
- New function `ThreatIntelligenceIndicatorClient.Get(context.Context, string, string, string, string) (ThreatIntelligenceInformationModel, error)`
- New function `NewThreatIntelligenceIndicatorClient(string) ThreatIntelligenceIndicatorClient`
- New function `*WatchlistListIterator.NextWithContext(context.Context) error`
- New function `HuntingBookmark.AsCloudApplicationEntity() (*CloudApplicationEntity, bool)`
- New function `OfficeATPCheckRequirements.MarshalJSON() ([]byte, error)`
- New function `WatchlistsClient.ListResponder(*http.Response) (WatchlistList, error)`
- New function `HostEntity.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `ThreatIntelligenceIndicatorClient.QueryIndicators(context.Context, string, string, string, ThreatIntelligenceFilteringCriteria) (ThreatIntelligenceInformationListPage, error)`
- New function `WatchlistsClient.GetResponder(*http.Response) (Watchlist, error)`
- New function `PossibleEventGroupingAggregationKindValues() []EventGroupingAggregationKind`
- New function `*WatchlistListIterator.Next() error`
- New function `OfficeATPDataConnector.AsTiTaxiiDataConnector() (*TiTaxiiDataConnector, bool)`
- New function `WatchlistsClient.GetPreparer(context.Context, string, string, string, string) (*http.Request, error)`
- New function `IncidentsClient.ListOfEntitiesSender(*http.Request) (*http.Response, error)`
- New function `ASCDataConnector.AsOfficeATPDataConnector() (*OfficeATPDataConnector, bool)`
- New function `ThreatIntelligenceIndicatorClient.CreateResponder(*http.Response) (ThreatIntelligenceInformationModel, error)`
- New function `HuntingBookmark.AsBasicEntity() (BasicEntity, bool)`
- New function `IoTDeviceEntity.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `WatchlistListIterator.NotDone() bool`
- New function `TiTaxiiCheckRequirements.AsOfficeATPCheckRequirements() (*OfficeATPCheckRequirements, bool)`
- New function `ThreatIntelligenceIndicatorClient.Create(context.Context, string, string, string, string, ThreatIntelligenceIndicatorModelForRequestBody) (ThreatIntelligenceInformationModel, error)`
- New function `DataConnector.AsOfficeATPDataConnector() (*OfficeATPDataConnector, bool)`
- New function `OfficeATPDataConnector.AsAwsCloudTrailDataConnector() (*AwsCloudTrailDataConnector, bool)`
- New function `WatchlistsClient.Get(context.Context, string, string, string, string) (Watchlist, error)`
- New function `URLEntity.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `PossibleKindBasicEntityTimelineItemValues() []KindBasicEntityTimelineItem`
- New function `ThreatIntelligenceIndicatorMetricsClient.ListResponder(*http.Response) (ThreatIntelligenceMetricsList, error)`
- New function `WatchlistsClient.CreateResponder(*http.Response) (Watchlist, error)`
- New function `SecurityAlertTimelineItem.AsBookmarkTimelineItem() (*BookmarkTimelineItem, bool)`
- New function `BookmarkTimelineItem.AsBasicEntityTimelineItem() (BasicEntityTimelineItem, bool)`
- New function `ThreatIntelligenceInformationListIterator.NotDone() bool`
- New function `SecurityGroupEntity.AsHuntingBookmark() (*HuntingBookmark, bool)`
- New function `BookmarkTimelineItem.AsActivityTimelineItem() (*ActivityTimelineItem, bool)`
- New function `ThreatIntelligenceInformationListIterator.Value() BasicThreatIntelligenceInformation`
- New function `ThreatIntelligenceIndicatorModel.MarshalJSON() ([]byte, error)`
- New function `Ueba.AsBasicSettings() (BasicSettings, bool)`
- New function `HuntingBookmark.AsRegistryKeyEntity() (*RegistryKeyEntity, bool)`
- New function `ThreatIntelligenceIndicatorModel.AsBasicThreatIntelligenceInformation() (BasicThreatIntelligenceInformation, bool)`
- New struct `ActivityTimelineItem`
- New struct `BookmarkTimelineItem`
- New struct `EntitiesGetTimelineClient`
- New struct `EntityAnalytics`
- New struct `EntityAnalyticsProperties`
- New struct `EntityTimelineItem`
- New struct `EntityTimelineParameters`
- New struct `EntityTimelineResponse`
- New struct `EventGroupingSettings`
- New struct `HuntingBookmark`
- New struct `HuntingBookmarkProperties`
- New struct `IncidentAlertList`
- New struct `IncidentBookmarkList`
- New struct `IncidentEntitiesResponse`
- New struct `IncidentEntitiesResultsMetadata`
- New struct `OfficeATPCheckRequirements`
- New struct `OfficeATPCheckRequirementsProperties`
- New struct `OfficeATPDataConnector`
- New struct `OfficeATPDataConnectorProperties`
- New struct `OfficeDataConnectorDataTypesTeams`
- New struct `SecurityAlertTimelineItem`
- New struct `ThreatIntelligenceAppendTags`
- New struct `ThreatIntelligenceFilteringCriteria`
- New struct `ThreatIntelligenceGranularMarkingModel`
- New struct `ThreatIntelligenceIndicatorClient`
- New struct `ThreatIntelligenceIndicatorMetricsClient`
- New struct `ThreatIntelligenceIndicatorModel`
- New struct `ThreatIntelligenceIndicatorModelForRequestBody`
- New struct `ThreatIntelligenceIndicatorProperties`
- New struct `ThreatIntelligenceIndicatorsClient`
- New struct `ThreatIntelligenceInformation`
- New struct `ThreatIntelligenceInformationList`
- New struct `ThreatIntelligenceInformationListIterator`
- New struct `ThreatIntelligenceInformationListPage`
- New struct `ThreatIntelligenceInformationModel`
- New struct `ThreatIntelligenceKillChainPhase`
- New struct `ThreatIntelligenceMetric`
- New struct `ThreatIntelligenceMetricEntity`
- New struct `ThreatIntelligenceMetrics`
- New struct `ThreatIntelligenceMetricsList`
- New struct `ThreatIntelligenceResourceKind1`
- New struct `ThreatIntelligenceSortingCriteria1`
- New struct `TimelineAggregation`
- New struct `TimelineError`
- New struct `TimelineResultsMetadata`
- New struct `Ueba`
- New struct `UebaProperties`
- New struct `Watchlist`
- New struct `WatchlistList`
- New struct `WatchlistListIterator`
- New struct `WatchlistListPage`
- New struct `WatchlistProperties`
- New struct `WatchlistsClient`
- New field `Teams` in struct `OfficeDataConnectorDataTypes`
- New field `EventGroupingSettings` in struct `ScheduledAlertRuleTemplateProperties`
- New field `EventGroupingSettings` in struct `ScheduledAlertRuleProperties`
- New field `EventGroupingSettings` in struct `ScheduledAlertRuleCommonProperties`
- New field `LastModifiedTimeUtc` in struct `IncidentCommentProperties`
- New field `Etag` in struct `IncidentComment`