---
name: Urban Airship
x-slug: urban-airship
description: A market-leading mobile app engagement, mobile analytics, mobile data
  integration and mobile wallet marketing solution.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
x-kinRank: "8"
x-alexaRank: "79571"
tags: Pins
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/pins/master/_listings/urban-airship/apis.md
specificationVersion: "0.14"
apis:
- name: Urban Airship - Put Device Pins Pin
  x-api-slug: device-pinspin-put
  description: Registers a BlackBerry PIN. This is optional, but recommended, for
    BlackBerry push messages. This returns HTTP 201 Created for the first registration
    and 200 OK for any updates. If you wish to include additional information about
    a device pin, for instance an alias or tags, include a JSON payload along with
    this request. Not including one of these keys removes it from the device pin.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pins/master/_listings/urban-airship/device-pinspin-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pins/master/_listings/urban-airship/device-pinspin-put-openapi.md
- name: Urban Airship - Get Device Pins Pin
  x-api-slug: device-pinspin-get
  description: Gets Device PIN information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pins/master/_listings/urban-airship/device-pinspin-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pins/master/_listings/urban-airship/device-pinspin-get-openapi.md
- name: Urban Airship - Delete Device Pins Pin
  x-api-slug: device-pinspin-delete
  description: Marks a PIN as inactive. No notifications will be delivered to it until
    a PUT is executed again.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pins/master/_listings/urban-airship/device-pinspin-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pins/master/_listings/urban-airship/device-pinspin-delete-openapi.md
x-common:
- type: x-website
  url: http://urbanairship.com/
- type: x-android-sdk
  url: http://docs.urbanairship.com/platform/android.html
- type: x-api-gallery
  url: http://ulster.bank.api.gallery.streamdata.io
- type: x-api-stack
  url: http://urban.airship.stack.network
- type: x-blackberry-sdk
  url: http://docs.urbanairship.com/platform/blackberry.html
- type: x-blog
  url: http://urbanairship.com/blog
- type: x-blog-rss
  url: http://urbanairship.com/blog/rss
- type: x-case-studies
  url: http://urbanairship.com/resources/case-studies
- type: x-crunchbase
  url: http://www.crunchbase.com/company/urban-airship
- type: x-crunchbase
  url: https://crunchbase.com/organization/urban-airship
- type: x-developer
  url: http://docs.urbanairship.com/
- type: x-email
  url: legal@urbanairship.com
- type: x-email
  url: privacy@urbanairship.com
- type: x-email
  url: support@urbanairship.com
- type: x-github
  url: https://github.com/urbanairship
- type: x-glossary
  url: http://docs.urbanairship.com/reference/glossary.html
- type: x-ios-sdk
  url: http://docs.urbanairship.com/platform/ios.html
- type: x-linkedin
  url: https://www.linkedin.com/company/urban-airship/
- type: x-phonegap-sdk
  url: http://docs.urbanairship.com/platform/phonegap.html
- type: x-pricing
  url: https://www.urbanairship.com/products/engage/pricing
- type: x-privacy
  url: http://urbanairship.com/legal/privacy-policy
- type: x-security
  url: http://docs.urbanairship.com/reference/app_keys_secrets.html
- type: x-twitter
  url: https://twitter.com/urbanairship
- type: x-website
  url: http://urbanairship.com
- type: x-white-papers
  url: http://urbanairship.com/resources/whitepapers
- type: x-windows-sdk
  url: http://docs.urbanairship.com/platform/windows.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---