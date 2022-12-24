---
title: "How to: run backend locally"
---

# How to: run backend locally

This is if you'd like to replicate the pipeline action/ `the_od_bods` repo on a local machine.

It will gather fresh data from API calls and web scrapers, process them, then write prepared listings to the local JKAN repo. 

1. Have `the_od_bods` and `jkan` repos on local in the same directory
    - `git clone` if it's the first time, or `git pull` to update repos
    - you must have the `jkan` repo in local, even if you don't intend to use it, or the pipeline action will fail.

2. Set up or update python environment
    - `the_od_bods` repo runs exclusively in python
    - python packages needed are specified in `the_od_bods/requirements.txt`
    - you may use any environment manager of your choice: conda, venv, poetry or other.

3. Run `main.sh`
    - in terminal, in `the_od_bods`, execute the shell script `sh main.sh`
    - wait for confirmation message "main.sh complete"
    - whole action can take ~15 minutes to complete

4. To see changes in frontend see [How to: Run frontend locally](about/how-to-run-frontend-locally.md)