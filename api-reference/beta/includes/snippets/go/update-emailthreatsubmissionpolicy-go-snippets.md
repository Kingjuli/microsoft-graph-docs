---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodelssecurity "github.com/microsoftgraph/msgraph-beta-sdk-go/models/security"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodelssecurity.NewEmailThreatSubmissionPolicy()
isReportToMicrosoftEnabled := false
requestBody.SetIsReportToMicrosoftEnabled(&isReportToMicrosoftEnabled) 

result, err := graphClient.Security().ThreatSubmission().EmailThreatSubmissionPolicies().ByEmailThreatSubmissionPolicieId("emailThreatSubmissionPolicy-id").Patch(context.Background(), requestBody, nil)


```