## page incomplete

In the_od_bods repo
1. Run the following scripts to refresh API calls
```
arcgis.py
dcat.py
Import_DCAT.ipynb
```
2. RUN merge_data(). Either in analytics.ipynb. Or as a script by itself, which updates data/merged_output.csv and creates a copy for data/archive/ 
```
python3 analytics/merge_data.py
```
3. RUN export2jkan.py which replaces ..jkan/_datasets/ in the jkan repo
```
python3.9 export2jkan.py
```
4. Push the_od_bods if there are any processing changes to save, but push jkan repo to update the opendata.scot frontend.
5. Check that github push is successful and wait patiently for things to rebuild, can take a couple minutes.
