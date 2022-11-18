Images are not held locally, but are pointed to. 

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

There are two ways to add an image: by cloning the repo, editing files locally, and pushing changes back to Github or editing the orgaisation's file directly on Github. 

We recommend the second direct approach which is explained below. 


To add an image, 

1. Ensure you have edit rights on the repo. You can ask to be added to the team on our [Slack group](https://join.slack.com/t/opendatascotland/shared_invite/zt-yfcc64tg-xIF1cOxkWbKZqI8ZBPzkGg). 

2. Navigate to https://github.com/OpenDataScotland/jkan/tree/gh-pages/_organizations. 

3. Open the MD file for the target organization e.g. Aberdeenshire council. Click on the Edit This File (pencil symbol) to the right of the page on the light-grey bar.
4. Find a logo  - either from Wikipedia (which is good for councils etc) or from the organisation's own website. If you are using wikipedia:

	a. Go to Wikipedia (e.g. https://en.wikipedia.org/wiki/Category:Scottish_council_logos) and find the organization. 

	b. Click on the link, then on the logo itself. Copy the file address.

	If you are looking on the company website, you can load the website, then look at the site code. Look for "logo" and see if there is a direct link. Sometimes you need to stitch a relative path to the site root. Test that your link works in another tab. 

5. In the MD file edit the line 
```yaml
logo: ''
```
and add the link between the single quotes.
```yaml
logo: 'https://upload.wikimedia.org/wikipedia/en/1/12/Aberdeenshire_Council.svg'
```

- Scroll down and save

6. Add a mesasge = "add logo"  and wait for page to rebuild
7. Refresh opendata.scot and check.
8. Done!


