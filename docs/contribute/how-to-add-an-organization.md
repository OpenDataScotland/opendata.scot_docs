---
title: "How to: add an organization"
---

# How to: add an organization

Files for organisations are in the format
```yaml
---
schema: default
title: Aberdeen City Council
description: Local authority for the Aberdeen City Council area
logo: 'https://upload.wikimedia.org/wikipedia/en/6/69/Aberdeen_City_Council_logo.svg'
type:
  - Local authority
portal_url: ''
org_url: 'http://www.aberdeencity.gov.uk/'
twitter_handle: AberdeenCC
gss_code: S12000033
wikidata_org_qid: ''
wikidata_portal_qid: ''
wdtk_id: aberdeen_city_council
---
```


1. In the JKAN repo, navigate to `jkan/_organizations`, create a new organisation .md file by making a copy of an existing one.

2. Replace values with your new organisation's values

3. Save file, commit and push to `gh-pages` branch 

4. To add an image or logo for the organisation see [How to: add an organization image](../how-to-add-an-organization-image.md)


