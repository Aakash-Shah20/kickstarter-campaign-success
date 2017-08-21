# kickstarter-campaign-success
What insights around Kickstarter campaign success can we discover, and how can we proactively predict campaign outcome?

**This project was done by Rachel Downs and Muhammad Ghuari for and MIS elective at UT Austin.**

## Project Objectives:
Kickstarter is an online crowdfunding platform aimed at helping people get their ideas funded while building a community of fans to support their ideas. While Kickstarter publishes many advice and best-practices articles on their blog, over half of campaigns still fail.

*Why does this matter?* Well unlike their competitor, Indiegogo, Kickstarter campaign projects follow an "all or nothing" funding model. This means that if a Kickstarter campaign fails, both the project creators are disappointed, as well as the people who did contribute because the project will not be completed in any capacity.

This project's objectives are the following:
1. Understand the marketplace of Kickstarter including timing of campaigns posted, types of projects, location of campaigns, description of campaigns and more
2. Provide insight into attributes that set campaigns up for a higher rate of success to inform campaign creation in the future
3. Build a predictive model that allows Kickstarter to identify high-failure-risk campaigns before they fail and provide supplemental advice and material to the creators
4. Identify a business opportunity for Kickstarter by finding campaigns just below the predicted threshold of success and helping them get to their goal, helping both parties earn revenue

## Methodology:
This dataset contains data on 20,632 Kickstarter campaigns on the site as of February 1st 2017. Important attributes are described below:
- Project: a finite work with a clear goal that you’d like to bring to life (aka campaign)
- Funding goal: amount of money that a creator needs to complete their project
- Name: name of project on Kickstarter
- Blurb: the short description displayed under the name of your project and on the browse page
- Pledged and backers: amount of money that a project has raised and people that have supported it at the point of the API pull
- State: successful, failed, cancelled, live or suspended
- Deadline, state changed, created at, launched at: deadline given for successful funding, state changed when campaign went to success or failure, time the project was created at, time the project was launched at
- Other attributes in this dataset: country, currency, category

To attain a deeper understanding of our data and to have more attributes to explore, we also created the following features out of the data for our analysis:
- Name and blurb (description) length including and excluding “stop words” - name_len_clean, blurb_len_clean
- Day of week and hour of the day for creation, launch and deadline date - deadline_weekday, created_at_weekday, lauched_at_weekday, deadline_hour, created_at_hour, launched_at_hour
- Days between creation and launch, and days between launch and deadline - create_to_launch, launch_to_deadline


## [Read our project report.](https://data.world/rdowns26/kickstarter-campaigns/file/Term%20Project%20Report.pdf)

This data was collected from [WebRobots.io](https://webrobots.io/kickstarter-datasets/)
