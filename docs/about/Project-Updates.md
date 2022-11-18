# June 2022
- presented to the Aberdeen Python User Group meetup on 8 Jun. [Slides here](https://docs.google.com/presentation/d/1LEngLvSD7kPS95VVZzdJ8BGFI32jykuvweiykjxPw3E/edit#slide=id.p) and [challenges set here](https://github.com/PythonAberdeen/user_group/blob/master/2022-06/README.md)


# May 2022
- A very successful hack weekend at CTC26!
    - 8 contributors and an estimated 120 person hours!
    - set up monitoring alerts to auto open/close a ticket on our github project board when a publisher’s url goes offline so we know to investigate. 
    - refactored API call scripts so they use a single source for publisher URLs for easier long-term maintenance
    - successfully automated the entire pipeline using github actions 
    - exposed our web analytics by exporting to a new [analytics repo](https://github.com/OpenDataScotland/opendata.scot_analytics)
    - created 3 web scrapers converting our manual sources into automated calls
    - improved categorisation including a new dedicated tourism category
    - changed the way we create URLs, from arbitary ID to org+dataset name combination. This preserves URL permanency.



# April 2022
- added plausible analytics to opendata.scot. Now we can quantify how many people are accessing the service! 
- reduced the number of categories in the datasets from 744 to 14! The category filter is now usable again
- automated a tiny bit more of the data listing process
- we've been having some really exciting conversations about how to make dataset categorisation clever-er.

# March 2022
- we raised more issues but no commits in march.

# February 2022
- Hack weekend at CTC25!
- added more sources including Public Health Scotland (PHS), Edinburgh City Council and Glasgow City Council which takes us up to 900+ datasets
- Refreshed data from already known sources
- started to look at comparing dataset movement between Jun 2021 and Feb 2022 (8 months)
- started archive of dataset snapshots
- Fixed several display errors
- Fixed issue where datasets of the same name but different casing would overwrite.
- tidied licensing categories
- converted some of the static graphs in /Analytics to be real-time charts
- tidied up data cleaning pipelines and improved documentation around it

# January 2022
- A well-deserved break to recover from Christmas/Covid.
- Milestone 22Q1: Improve Data Started

# December 2021
- Added some datasets and organisations from wikidata
- improved usability of interface
- Attempted upgrade from Bootstrap 3 to Bootstrap 5. That didn't work out.

# November 2021
- We had a very productive hack weekend at CTC24!
    - closed 10 issues, opened 6 new ones
    - 5 authors, over 200 commits, and 600 files.
    - with thanks to other participants on another project whose work fed into OD_BODS also
- We have a brand new shiny working website [opendata.scot](www.opendata.scot) (complete with footer and licensing information)
- Added all 427 of our known datasets to the listing (no new data refresh)
- The listing has filtering and search functionality (thanks to JKAN.io)
- Added a (nearly complete) list of 152 scottish organisations (and with logos)
- Made several new pages to help the Learn element of the project (Analytics, What is OD?, About)
- Added a form for users to suggest open datasets they want to see, and for others to see what has been suggested.
- Added 2 new "how to" guides to the wiki (adding a new page, adding an organisation image)

# October 2021
- We now have a project plan for the next 12 months! 
- Created a dedicated slack channel and github repo.
- Transferred the original CTC23 repo to its new home in the ODS organisation
- Centralised all our to-do lists and notes in the repo.
- This repo is now the brain of the project.
- We bought a new custom domain www.opendata.scot!
- We started trialing the open source JKAN.io to use as our front-end
- Preparation now underway for mini-projects to run at CTC24 - exciting!

