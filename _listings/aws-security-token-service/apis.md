---
name: AWS Security Token Service
x-slug: aws-security-token-service
description: The AWS Security Token Service (STS) is a web service that enables you
  to request temporary, limited-privilege credentials for AWS Identity and Access
  Management (IAM) users or for users that you authenticate (federated users).
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM_AWSSTS.png
x-kinRank: "10"
x-alexaRank: "0"
tags: OpenID
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/openid/master/_listings/aws-security-token-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Security Token Service API - Assume Role With Web Identity
  x-api-slug: actionassumerolewithwebidentity-get
  description: |-
    Returns a set of temporary security credentials for users who have been authenticated
          in a mobile or web application with a web identity provider, such as Amazon Cognito, Login with Amazon,
          Facebook, Google, or any OpenID Connect-compatible identity provider.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM_AWSSTS.png
  humanURL: http://docs.aws.amazon.com/STS/latest/APIReference/Welcome.html
  baseURL: :///
  tags: Amazon Web Services, Authentication, Security, Stack Network, API Service
    Provider, API Service Provider, API Provider, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/openid/master/_listings/aws-security-token-service/actionassumerolewithwebidentity-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.s3.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.security.token.service.stack.network
- type: x-documentation
  url: http://docs.aws.amazon.com/STS/latest/APIReference/
- type: x-errors
  url: http://docs.aws.amazon.com/STS/latest/APIReference/CommonErrors.html
- type: x-website
  url: http://docs.aws.amazon.com/STS/latest/APIReference/Welcome.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---