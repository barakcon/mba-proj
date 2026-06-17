This doc will describe the prototype of AdoptAI.
AdoptAI is a product we create that helps companies manage AI adoption, usage and ROI.

The demo should have a "left bar", a "main content" and a "top bar".
In the top bar show the logo in the top left and in the top right show a few options for time ranges (ie "last 30 days" "last 90 days", etc).
In the left bar show the different departments as checkboxes the user can choose which to show, by default shows just the first.
The departments: "R&D", "Sales", "Marketing".
When a department is checked the main content will show relevant data.
At the bottom of the "left bar" show a "settings" button with settings icon.
In the "main content" I want several tabs.

The selected time range and checked departments act as global filters: every tab reflects only the selected departments' data sources, over the selected time range. When multiple departments are checked, data is aggregated across them.

## Main content
Tabs
* AI usage
  * In this tab the main currency is people.
  * Top left should show a graph for each AI data source the number of seats VS the number of weekly users.
  * Top right should show a graph with Token analysis for all the data sources that have them.
  * Under the top row show a timeline graph with the daily AI usage for each data source by number of users.
* AI spend
  * In this tab the main currency is dollars.
  * Top left should show a graph for each AI data source the number of dollars we pay.
  * Top right should show a graph with Token spend analysis for all the data sources that have them.
  * Under the top row show a timeline graph with the daily AI spend for each data source by dollars.
* AI Quality
  * In this section show Quality insights that will highlight potential cost savings.
  * In the top left show the total number of potential savings.
  * In the top right show the cost savings per department.
  * Under it show 4 cards with the main 4 savings opportunities (and highlight it's top 4 out of total ___) some examples:
    * X R&D "AI rules" that can be converted to "AI Skills" that take less context window, it will translate to saving of ____ $ across ____ AI sessions per day.
    * X Scheduled glean agents that run periodically during night and weekends. potential savings ______
    * X Unused Cursor seats where the 100$/user is utilized with less than 10$ worth of tokens.
    * X Marketing campaigns in Google Analytics that are mispriced according to our AI analysis.
    * Poor token efficiency in the Gong sales usage where Salesforce data is mislabeled causing agents to consume 5 times the number of tokens.
* AI ROI ✨
  * Main panel a graph that shows how each department is doing in terms of the KPIs thanks to AI usage. Each KPI is shown as a grouped/stacked bar comparing the value without AI attribution against the value with AI attribution, so the AI-driven lift is visible at a glance.
  * Below it, one small chart per impact metric showing how that metric's AI lift translates into "equivalent headcount" — the number of additional employees it would take to contribute the same gain. Keep each chart compact and consistent so the row reads as a clean set of unit-economics cards.

## UX
* The UX should be clean, simple and light, feeling modern with a strong sense of polish.
* Use generous whitespace, a restrained color palette, and clear typography.
* Add micro animations (hover states, smooth tab and filter transitions, animated chart loads) so the product feels responsive and alive.
* Interactions should feel fast and fluid, never cluttered or heavy.

## Data notes
* You should generate data. Assume a 1200 employees organization.
* The organization is a high tech company.
* Data should be internally consistent across tabs (the same seats, users, and spend reconcile between AI usage, AI spend and AI Quality).

## Data sources and Metrics
R&D row:
- Data Sources: Claude, Cursor, Git, Jira
- Performance Metrics: SDLC efficiency, DORA average
- Tokens usage in: Claude, Cursor

Sales row:
- Data Sources: Salesforce, Gong, Outreach, ZoomInfo
- Performance Metrics: New Logos, New ARR, New Expansions
- Tokens usage in: Gong

Marketing row:
- Data Sources: HubSpot, Google Analytics, Meta Ads, Glean
- Performance Metrics: Referrals, Leads, Exposure
- Tokens usage in: Glean
