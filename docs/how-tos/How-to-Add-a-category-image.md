---
title: "How to: add a new category image"
---

# How to: add a new category image

1. Go to [The Noun Project](https://thenounproject.com)
2. Search for the term for which you want to add a category (e.g. Tourism).
3. Choose an image to fit with the others on ODS.
4. Select to download. You will need to create an account if you don't already have one. 
5. Save the image to your hard drive. Also, copy the text regarding attribution - you will need it again.
6. Open the image in an editor which can deal with SVG files. eg [Inkscape](https://inkscape.org/)
7. Remove any attribution text which has been added to the image and save it to jkan/img/categories (noting the name)
8. In a text editor, open jkan/_data/schemas/categories.yml
9. Edit in the new entry (eg for Tourism)into the correct positions follows

```
- name: Tourism
  logo: /img/categories/tourism.svg
  logo_credit: WEBTECHOPS LLP from the Noun Project
  featured: true
```
10. Save the file.
11. Commit both changes in Git and push the changes to Github. 
12. The navigation will be rebuilt within a couple of minutes. 
13. Check the site: [https://opendata.scot](https://opendata.scot)

Finished! 