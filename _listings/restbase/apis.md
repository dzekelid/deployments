---
name: RESTBase
x-slug: restbase
description: RESTBase is a caching / storing API proxy. Its configuration is based
  on Swagger specs, and its primary storage backend is using Cassandra. It powers
  rest.wikimedia.org, the Wikimedia REST content API currently in beta production.
  As a proxy, RESTBase does not perform any significant content processing itself.
  Instead, it requests content transformations from backend services when needed,
  and typically (depending on configuration) stores it back for later retrieval.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/RESTBase-Logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Deployments
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/restbase/apis.md
specificationVersion: "0.14"
apis: []
x-common:
- type: x-github
  url: https://github.com/wikimedia/restbase
- type: x-website
  url: http://www.mediawiki.org/wiki/RESTBase
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---