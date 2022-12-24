---
title: "How to: modify category keywords "
---

# How to: modify category keywords

All dataset categories have keywords which are used to assign categories to datasets. If these keywords are present in the Title or Description of a dataset, the dataset is assigned that category. A dataset can have multiple categories.

1. Locate in `the_od_bods/ODSCategories.json`
2. Modify the json file to add, edit, remove keywords or key phrases
    - These keywords/phrases should be unambigous and near-distinct to the category. There may be some overlap between categories but we discourage it
3. Save the .json file
4. In terminal, in `/the_od_bods`, run
```
python merge_data.py
```
5. Check results in `the_od_bods/data/merged_output.csv`

If there are issues executing locally, check [How to: run backend locally](/How-to-run-backend-locally.md)
