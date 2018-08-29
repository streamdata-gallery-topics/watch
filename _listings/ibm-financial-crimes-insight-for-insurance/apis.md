---
name: IBM Financial Crimes Insight for Insurance
x-slug: ibm-financial-crimes-insight-for-insurance
description: IBM&reg; Financial Crimes Insight&reg; for Insurance V3.0, formerly known
  as IBM Counter Fraud Management for Insurance, is now being offered as a cloud service
  offering. It helps organizations analyze data to determine the fraud risk of claims,
  medical providers, and other business entities, manage the full investigation lifecycle,
  and report on outcomes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
x-kinRank: "7"
x-alexaRank: ""
tags: Watch
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/apis.md
specificationVersion: "0.14"
apis:
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve a list
    of the registered watchlists
  x-api-slug: ibmfciplatformfactwatchlist-get
  description: This method is used to retrieve the list of registered watchlists from
    the database
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlist-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Persist the provided
    watchlist into the local database
  x-api-slug: ibmfciplatformfactwatchlist-post
  description: 'This method is used to persist the contents of a watchlist into the
    database.  Note: This method uses some data import functionality to create business
    object entries, then calls putWatchlist to create/update a watchlist for the provided
    identifier, and finally calls putWatchlistItem for every object created. This
    one also has the caveat of needing a disposition defined, but in this case all
    you need to pass in is the stereotype value.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlist-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlist-post-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve the contents
    of a watchlist, based on its id
  x-api-slug: ibmfciplatformfactwatchlistid-get
  description: This method is used to retrieve the contents of a watchlist from the
    database
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlistid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlistid-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve a list
    of the registered watchlists
  x-api-slug: ibmfciplatformfactwatchlist-get
  description: This method is used to retrieve the list of registered watchlists from
    the database
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlist-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Persist the provided
    watchlist into the local database
  x-api-slug: ibmfciplatformfactwatchlist-post
  description: 'This method is used to persist the contents of a watchlist into the
    database.  Note: This method uses some data import functionality to create business
    object entries, then calls putWatchlist to create/update a watchlist for the provided
    identifier, and finally calls putWatchlistItem for every object created. This
    one also has the caveat of needing a disposition defined, but in this case all
    you need to pass in is the stereotype value.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlist-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlist-post-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve the contents
    of a watchlist, based on its id
  x-api-slug: ibmfciplatformfactwatchlistid-get
  description: This method is used to retrieve the contents of a watchlist from the
    database
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlistid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlistid-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve a list
    of the registered watchlists
  x-api-slug: ibmfciplatformfactwatchlist-get
  description: This method is used to retrieve the list of registered watchlists from
    the database
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlist-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve the contents
    of a watchlist, based on its id
  x-api-slug: ibmfciplatformfactwatchlistid-get
  description: This method is used to retrieve the contents of a watchlist from the
    database
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlistid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlistid-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Persist the provided
    watchlist into the local database
  x-api-slug: ibmfciplatformfactwatchlist-post
  description: 'This method is used to persist the contents of a watchlist into the
    database.  Note: This method uses some data import functionality to create business
    object entries, then calls putWatchlist to create/update a watchlist for the provided
    identifier, and finally calls putWatchlistItem for every object created. This
    one also has the caveat of needing a disposition defined, but in this case all
    you need to pass in is the stereotype value.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlist-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/watch/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlist-post-openapi.md
x-common:
- type: x-openapi
  url: https://www.ibm.com/support/knowledgecenter/SSC2HF_3.0.0/api/fcii-insurance-v3.0.0.yaml?origin=swagger-ui
- type: x-pricing
  url: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN#echargex
- type: x-website
  url: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
- type: x-api-gallery
  url: http://ibm.cloud.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ibm.financial.crimes.insight.for.insurance.stack.network
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---