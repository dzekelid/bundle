---
name: Twine
x-slug: twine
description: 'Twine Health is a cloud-based collaborative care platform for chronic
  disease management. It consists of a patient engagement portal, a peer support network,
  a care management solution, and an outcome analytics tool. The platform enables
  users to co-create personalized care plans that serve as common ground for collaboration
  with their care team: their own providers such as physicians and nurse practitioners;
  their family and friends; and coaches such as nurses, pharmacists, health coaches,
  and more.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Bundle
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/bundle/master/_listings/twine/apis.md
specificationVersion: "0.14"
apis:
- name: Twine - Create bundle
  x-api-slug: bundle-post
  description: Create a bundle in a patient's plan
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bundle/master/_listings/twine/bundle-post-openapi.md
- name: Twine - Get a bundle
  x-api-slug: bundleid-get
  description: Get a bundle from a patient's plan.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bundle/master/_listings/twine/bundleid-get-openapi.md
- name: Twine - Update a bundle
  x-api-slug: bundleid-patch
  description: Updte a bundle from a patient's plan.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bundle/master/_listings/twine/bundleid-patch-openapi.md
x-common:
- type: x-api-gallery
  url: http://twilio.api.gallery.streamdata.io
- type: x-api-stack
  url: http://twine.stack.network
- type: x-authentication
  url: http://developer.twinehealth.com/#section/Authentication
- type: x-developer
  url: http://developer.twinehealth.com/
- type: x-website
  url: http://twinehealth.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---