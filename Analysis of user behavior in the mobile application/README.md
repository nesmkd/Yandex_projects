# Description of project - Research of user behavior in the mobile app
## Research Goals
1. Analyze the relationship between the target event (viewing contacts) and other user actions.
2. Evaluate which actions are more frequently performed by users who view contacts.
3. Analyze the time difference between events map -> contacts_show and search -> contacts_show within sessions.

## Additional Materials
- link to a presentation with brief project results and recommendations
  https://drive.google.com/file/d/1luGkl0EZRoSVMMsG2zNVmOOEQUh8SrwD/view?usp=sharing 
- Link to dashboard with graphs and data filtering for dynamic analysis will also be created
  https://public.tableau.com/views/Dashboard_AppThings/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link

## Data Sources
Two datasets in CSV format are provided.

mobile_sources.csv:
- userId — user identifier
- source — source from which the user installed the application

mobile_dataset.csv:
- event.time — time of the event
- user.id — user identifier
- event.name — user action

Types of events in the data:
- advert_open — opened ad cards,
- photos_show — viewed photos in an ad,
- tips_show — saw recommended ads,
- tips_click — clicked on a recommended ad,
- contacts_show and show_contacts — viewed phone number,
- contacts_call — called the number from the ad,
- map — opened the map of ads,
- search_1 — search_7 — various actions related to site search,
- favorites_add — added an ad to favorites.

## Libraries:
Pandas, Numpy, Math, Scipy, Plotly, tqdm.notebook, itertools 

## Research Plan:
1. Data Overview and Exploration
   - Explore data
   - Explore data type
   - Handling duplicated values
   - Handling missing values
   - Handling anomal values
2. Exploratory Data Analysis
   - Exploration the time of activity and session durations of users
   - Define "scenarios" of user behavior (identify those leading to viewing contacts)
   - Calculate conversion and build a funnel for selected scenarios in terms of unique users
   - Analysis of the time difference between events map -> contacts_show and search -> contacts_show within sessions
   - Exploration of the relationship between the source and conversion to the target event
   - Analysis of events performed after the target event
3. Hypothesis testing
   - **Hypothesis #1.** Dependence of conversion to the target event on interaction with recommendations.\
     Some users perform actions tips_show and tips_click, others only tips_show.\
     However, the conversion to contacts view for these two groups of users is equal.\
     H0 = conversion to contacts view for these two groups of users is equal.\
     H1 = conversion to contacts view for these two groups of users is not equal.
   - **Hypothesis #2.** Influence of the "favorites" mark on conversion to the target event.\
     Some users perform the "add to favorites" action, others do not.\
     However, the conversion to contacts view for these two groups is equal.\
     H0 = conversion to contacts view for these two groups of users is equal.\
     H1 = conversion to contacts view for these two groups of users is not equal.
