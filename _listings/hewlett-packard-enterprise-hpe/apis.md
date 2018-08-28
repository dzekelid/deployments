---
name: Hewlett Packard Enterprise (HPE)
x-slug: hewlett-packard-enterprise-hpe
description: We help customers use technology to slash the time it takes to turn ideas
  into value. In turn, they transform industries, markets and lives. Some of our customers
  run traditional IT environments. Most are transitioning to a secure, cloud-enabled,
  mobile-friendly infrastructure. Many rely on a combination of both. Wherever they
  are in that journey, we provide the technology and solutions to help them succeed.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Deployments
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/hewlett-packard-enterprise-hpe/apis.md
specificationVersion: "0.14"
apis:
- name: HPE OneSphere API - Get Deployments
  x-api-slug: deployments-get
  description: Returns deployments. It requires any project role or non-'consumer'
    global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/hewlett-packard-enterprise-hpe/deployments-get-openapi.md
- name: HPE OneSphere API - Post Deployments
  x-api-slug: deployments-post
  description: Creates a new deployment. It requires any project role, or the **administrator**
    or **project creator** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/hewlett-packard-enterprise-hpe/deployments-post-openapi.md
- name: HPE OneSphere API - Delete Deployments
  x-api-slug: deploymentsid-delete
  description: Delete a deployment and associated resources. It requires any project
    role, or the **administrator** or **project creator** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/hewlett-packard-enterprise-hpe/deploymentsid-delete-openapi.md
- name: HPE OneSphere API - Get Deployments
  x-api-slug: deploymentsid-get
  description: Returns a deployment based on its id. It requires any project role
    or non-'consumer' global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/hewlett-packard-enterprise-hpe/deploymentsid-get-openapi.md
- name: HPE OneSphere API - Patch Deployments
  x-api-slug: deploymentsid-patch
  description: Updates a deployment. **Requires any project role, or 'administrator'
    or 'project creator' global role**. Allowed fields for PATCH of deployments are
    name(add,replace), volumes(add), k8snumWorkers(add), userData(add), serviceInput(add),
    version(add).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/hewlett-packard-enterprise-hpe/deploymentsid-patch-openapi.md
- name: HPE OneSphere API - Post Deployments Actions
  x-api-slug: deploymentsidactions-post
  description: Peforms an action to change the state of a deployment. It requires
    any project role, or the **administrator** or **project creator** global role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/hewlett-packard-enterprise-hpe/deploymentsidactions-post-openapi.md
- name: HPE OneSphere API - Post Deployments Console
  x-api-slug: deploymentsidconsole-post
  description: Returns a deployment console URL for deployment
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/hewlett-packard-enterprise-hpe/deploymentsidconsole-post-openapi.md
- name: HPE OneSphere API - Get Deployments Kubeconfig
  x-api-slug: deploymentsidkubeconfig-get
  description: Returns the kubeconfig. Applicable only to deployments of Kubernetes
    cluster. **Requires 'consumer' role on workspace**
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/hewlett-packard-enterprise-hpe/deploymentsidkubeconfig-get-openapi.md
x-common:
- type: x-developer
  url: https://developer.hpe.com/
- type: x-github
  url: https://github.com/hewlettpackard
- type: x-openapi
  url: https://raw.githubusercontent.com/HewlettPackard/hpe-onesphere-http/master/swagger.yml
- type: x-twitter
  url: https://twitter.com/HPE
- type: x-website
  url: http://HPE.com
- type: x-api-gallery
  url: http://heroku.api.gallery.streamdata.io
- type: x-api-stack
  url: http://hewlett.packard.enterprise.hpe.stack.network
- type: x-blog
  url: https://developer.hpe.com/blog
- type: x-curated-source
  url: http://community.hpe.com/t5/LoadRunner-and-Performance/LoadRunner-and-VuGen-12-53-load-testing-software-What-s-new-in/ba-p/6885101
- type: x-website
  url: https://www.hpe.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---