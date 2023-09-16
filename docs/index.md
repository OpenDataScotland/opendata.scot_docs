<style>
.col-md-3 {
    display:none;
}

</style>

# Quick start guide
Welcome to the documentation for [opendata.scot](https://opendata.scot/)!

This page is intended to point you to the information that matters most to you, dependent on whether you're coming to Open Data Scotland as an Analyst, Data Engineer or Web Developer.

## Analyst
- See the opendata.scot dataset listing in [json format](https://opendata.scot/datasets.json)
- Discover stories about visitor behaviour on opendata.scot by looking at our [site analytics data output](https://github.com/OpenDataScotland/opendata.scot_analytics) or in [browser version](https://opendata.scot/about/siteanalytics/)
- Browse inspiring examples of [other projects using open data](https://opendata.scot/resources/) both in Scotland and abroad
- Reference guides for [working with Scottish open data](https://opendata.scot/resources/)
- As an analyst, you might not need to store to any of the repos, but have a look at what stories have made it to the [website](https://opendata.scot/analytics/), and the ideas which [haven't quite made it there yet](https://github.com/OpenDataScotland/the_od_bods/tree/main/analytics). Any shared analytics code can be stored in repo [the_od_bods/analytics](https://github.com/OpenDataScotland/the_od_bods/tree/main/analytics)
- Analysts will be most interested in tickets related to [analytics](https://github.com/orgs/OpenDataScotland/projects/3/views/1?filterQuery=label%3Aanalytics+)

## Data Engineer
- Learn about our [pipeline architecture](architecture/architecture.md) and the [tools and tech we use in the pipeline](architecture/tools-and-tech.md)
- Understand how the [repos are used](architecture/repositories.md)
- For data engineering, the three most important repos used in the pipeline are 
    - [the-od-bods](https://github.com/OpenDataScotland/the_od_bods) for scaping and sourcing
    - [opendata.scot_pipeline](https://github.com/OpenDataScotland/opendata.scot_pipeline) repo where the scheduled pipeline actions are, and 
    - [JKAN](https://github.com/OpenDataScotland/jkan) for output display.
- Data Engineers will be most interested in tickets related to [adding new data sources](https://github.com/orgs/OpenDataScotland/projects/3/views/1?filterQuery=label%3A%22new+source%22) or [data engineering](https://github.com/orgs/OpenDataScotland/projects/3/views/1?filterQuery=label%3A%22data+engineering%22)

## Web Developer
- The most important repo for the web developer is the [JKAN](https://github.com/OpenDataScotland/jkan) repo where all code for the static site is kept.
- Read this guide on how to [deploy the front-end for testing locally](contribute/how-to-run-frontend-locally.md)
- Web developers will be most interested in tickets related to [JKAN](https://github.com/orgs/OpenDataScotland/projects/3/views/4) or [front end](https://github.com/orgs/OpenDataScotland/projects/3/views/1?filterQuery=label%3A%22front+end%22)



## Other
- Read about the project, its history, what it's trying to do, what it's achieved, and where it's headed in the [About](about/about-the-project.md) section

- Browse the [Contribute](contribute/contribution-guide.md) section for step-by-step guides on how to run the project locally and other repeating tasks we keep forgetting.


If you have any questions, feedback or general comments, definitely [contact the team](about/contact.md)