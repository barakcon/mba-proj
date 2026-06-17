This doc will describe the prototype of AdoptAI.
AdoptAI is a a product we create that helps companies manage the AI adoption, usage and ROI.

The demo should have a "left bar", a "main content" and a "top bar".
In the top bar simply show the logo in the top left and in the top right show a few options for time ranges (ie "last 30 days" "last 90 days", etc).
In the left bar show the different departments as checkboxes the user can choose which to show, by default shows just the first.
The departments: "R&D", "Sales", "Marketing".
When a department is checked the main content will show relevant data.
At the bottom of the "left bar" show a "settings" button with settings icon.
In the "main content" I want several tabs.

## Main content
Tabs
* AI usage
  * In this tab the main curreny is people.
  * Top left should show a graph for each AI data source the number of seats VS the number of weekly users.
  * Top right should show a graph with Token analysis for all the data sources that have them.
  * Under the top row show a timeline graph with the daily AI usage for each data source by number of users.
* AI spend
  * In this tab the main curreny is dollars.
  * Top left should show a graph for each AI data source the number dollars we pay.
  * Top right should show a graph with Token spend analysis for all the data sources that have them.
  * Under the top row show a timeline graph with the daily AI usage for each data source by dollars.
* AI Quality
  * In this section show Quality insights that will highlight potential cose savings.
  * In the top left show the total number of potential savings.
  * In the top right show the cost savings per department
  * Under it show 4 cards with the main 4 savings opportunities (and highlight it's top 4 out of total ___) some examples:
    * X R&D "AI rules" that can be converted to "AI Skills" that take less context window, it will translate to saving of ____ $ across ____ AI sessions per day.
    * X Scheduled glean agents that run periodically during night and weekends. potential savings ______
    * X Unused Cursor seats where the 100$/user is utilized with less that 10$ worth of tokens.
    * X Marketing campaigns in Google Analytics that are mispriced according to our AI analysis.
    * Poor token efficiency in the Gong sales usage where Salesforce data is mislabled causing agents to consume 5 times the number of tokens. 
* AI ROI ✨
  * Main panel a graph that shows How each department is doing in terms of the KPIs thanks to AI usage.
  * Second panel shows token unit economics where systems that are token based show the estimated impact on each mein metric.


## UX
* The UX should be clean, simple and light, feeling modern with a strong sense of polish.
* Use generous whitespace, a restrained color palette, and clear typography.
* Add micro animations (hover states, smooth tab and filter transitions, animated chart loads) so the product feels responsive and alive.
* Interactions should feel fast and fluid, never cluttered or heavy.

## Data notes
* You should generate data. Assume a 1200 employees organization.
* The organization is a high tech company.
* Data sources and KPIs


## Data sources and Metrics
R&D row:
- Data Sources: Claude, Cursor, Git, Jira
- Performance Metrics: SDLC, DORA
- Tokens usage in: Claude, Cursor

Sales row:
- Data Sources: Salesforce, Gong, Outreach, ZoomInfo
- Performance Metrics: New Logos, New ARR, New Expansions
- Tokens usage in: Gong

Marketing row:
- Data Sources: HubSpot, Google Analytics, Meta Ads, Glean
- Performance Metrics: Referrals, Leads, Exposure
- Tokens usage in: Glean