---
name: AppVeyor CI
x-slug: appveyor-ci
description: We provide continuous integration tools for Windows developers. The service
  is offered for free to open-source projects, we offer subscriptions for private
  projects and AppVeyor Enterprise installations on customer premises.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
x-kinRank: "7"
x-alexaRank: "35479"
tags: Deployments
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/appveyor-ci/apis.md
specificationVersion: "0.14"
apis:
- name: App Veyor Post Deployments
  x-api-slug: app-veyor
  description: Post deployments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
  humanURL: http://appveyor.com
  baseURL: https://ci.appveyor.com//api//deployments
  tags: Deployments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/appveyor-ci/deployments-post-openapi.md
- name: App Veyor Delete Deployments Stop
  x-api-slug: app-veyor
  description: Delete deployments stop.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
  humanURL: http://appveyor.com
  baseURL: https://ci.appveyor.com//api//deployments/stop
  tags: Deployments,Stop
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/appveyor-ci/deploymentsstop-delete-openapi.md
- name: App Veyor Get Deployments Deploymentid
  x-api-slug: app-veyor
  description: Get deployments deploymentid.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
  humanURL: http://appveyor.com
  baseURL: https://ci.appveyor.com//api//deployments/{deploymentId}
  tags: Deployments,DeploymentId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/appveyor-ci/deploymentsdeploymentid-get-openapi.md
- name: App Veyor Parameters Deployments Deploymentid
  x-api-slug: app-veyor
  description: Parameters deployments deploymentid.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
  humanURL: http://appveyor.com
  baseURL: https://ci.appveyor.com//api//deployments/{deploymentId}
  tags: Deployments,DeploymentId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/appveyor-ci/deploymentsdeploymentid-parameters-openapi.md
- name: App Veyor Get Environments Deploymentenvironmentid Deployments
  x-api-slug: app-veyor
  description: Get environments deploymentenvironmentid deployments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
  humanURL: http://appveyor.com
  baseURL: https://ci.appveyor.com//api//environments/{deploymentEnvironmentId}/deployments
  tags: Environments,DeploymentEnvironmentId,Deployments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/appveyor-ci/environmentsdeploymentenvironmentiddeployments-get-openapi.md
- name: App Veyor Parameters Environments Deploymentenvironmentid Deployments
  x-api-slug: app-veyor
  description: Parameters environments deploymentenvironmentid deployments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
  humanURL: http://appveyor.com
  baseURL: https://ci.appveyor.com//api//environments/{deploymentEnvironmentId}/deployments
  tags: Environments,DeploymentEnvironmentId,Deployments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/appveyor-ci/environmentsdeploymentenvironmentiddeployments-parameters-openapi.md
- name: App Veyor Get Projects Accountname Projectslug Deployments
  x-api-slug: app-veyor
  description: Get projects accountname projectslug deployments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
  humanURL: http://appveyor.com
  baseURL: https://ci.appveyor.com//api//projects/{accountName}/{projectSlug}/deployments
  tags: Projects,AccountName,ProjectSlug,Deployments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/appveyor-ci/projectsaccountnameprojectslugdeployments-get-openapi.md
- name: App Veyor Parameters Projects Accountname Projectslug Deployments
  x-api-slug: app-veyor
  description: Parameters projects accountname projectslug deployments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
  humanURL: http://appveyor.com
  baseURL: https://ci.appveyor.com//api//projects/{accountName}/{projectSlug}/deployments
  tags: Projects,AccountName,ProjectSlug,Deployments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/appveyor-ci/projectsaccountnameprojectslugdeployments-parameters-openapi.md
- name: App Veyor
  x-api-slug: app-veyor
  description: We provide continuous integration tools for Windows developers. The
    service is offered for free to open-source projects, we offer subscriptions for
    private projects and AppVeyor Enterprise installations on customer premises.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28368-app-veyor.jpg
  humanURL: http://appveyor.com
  baseURL: https://ci.appveyor.com//api
  tags: Deployments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/deployments/master/_listings/appveyor-ci/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/appveyor-systems-inc
- type: x-documentation
  url: https://www.appveyor.com/docs/
- type: x-email
  url: jobs@appveyor.com
- type: x-email
  url: team@appveyor.com
- type: x-email
  url: privacy@appveyor.com
- type: x-twitter
  url: https://twitter.com/appveyor
- type: x-website
  url: http://appveyor.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---