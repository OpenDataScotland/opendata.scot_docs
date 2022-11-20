---
title: "How to: add a new page"
---

# How to: add a new page

In the jkan repo:
1. Adding the html file:
- Add a .html at root jkan/.
- include this schema at the top of the .html file

```yaml
---
title: About
layout: default
permalink: /about/
---
{% include breadcrumbs.html %}
```

- Update the <title> and <permalink>. Add content and save

2. Adding link to navigation bar
- go to jkan/_config.yml in root
- find the section `#Nav bar`
- add to structure and update <title> and <url/permalink>

```yaml
 - title: About
    url: /about/
```
- Save

3. Commit-Push to repo and wait for page to rebuild
4. Refresh opendata.scot and check.
5. Done!



