---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphsecurity "github.com/microsoftgraph/msgraph-sdk-go/security"
	  graphmodelssecurity "github.com/microsoftgraph/msgraph-sdk-go/models/security"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphsecurity.NewApplyTagsPostRequestBody()


ediscoveryReviewTag := graphmodelssecurity.NewEdiscoveryReviewTag()
id := "d3d99dc704a74801b792b3e1e722aa0d"
ediscoveryReviewTag.SetId(&id) 

tagsToAdd := []graphmodelssecurity.ediscoveryReviewTagable {
	ediscoveryReviewTag,
}
requestBody.SetTagsToAdd(tagsToAdd)

graphClient.Security().Cases().EdiscoveryCases().ByEdiscoveryCaseId("ediscoveryCase-id").ReviewSets().ByReviewSetId("ediscoveryReviewSet-id").Queries().ByQuerieId("ediscoveryReviewSetQuery-id").MicrosoftGraphSecurityApplyTags().Post(context.Background(), requestBody, nil)


```