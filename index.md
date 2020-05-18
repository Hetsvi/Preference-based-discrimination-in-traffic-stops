# Does Police Officer Race Influence Stop Outcomes?

## Project Intro

> *We want this section to introduce the motivation behind the project to the reader. This section will set the stage and emphasize the importance of our analysis.*

 In recent years, in San Diego and in many other cities, tensions between the cities' police forces and its residents have risen. Claims of racial discrimination by police officers have led to numerous investigations and litigation. Studies of U.S. policing data, such as a recent investigation by researchers at San Diego State University, have uncovered instances of police officers treating people in similar situations differently.  It appears that race may play a part in those differing police actions. 

To expand on the studies conducted in this area, our research group is looking to investigate how a police officer’s race affects his or her decision-making process during traffic stops. Police are faced with many choices when monitoring motorists, such as whether to pull a driver over, whether to search the driver and whether to cite and/or arrest the driver.  If race is not an important factor in influencing a police officer's actions, then these outcomes should be independent of the races of both the driver and the officer. To test such an assumption, we will examine traffic stops made under similar circumstances and analyze the outcomes of those stops to determine if the races of the police officer and the driver are a factor in the outcomes. If they are, this might indicate that race does play an important role in the behavior of police officers when conducting traffic stops.

To ensure that our conclusions are more general, and not simply particular to a single police force, we will include data from multiple cities in our study. Florida, South Carolina, and Pittsburgh, Pennsylvania are three places that differ in geographic location as well as racial makeup.  Including these cities in our analysis will allow us to make a more general conclusion as to whether race is a factor in policing and whether such discrimination is localized or more widespread.

<div style="text-align:center"><img src="imgs/us.png" /></div>

Our research is important because it can indicate how the race of police officers assigned to certain service areas affects the racial disparities seen in traffic stops data. The results of this analysis may provide some guidance as to whether discrimination in traffic stops could be lessened by taking the racial composition of the service area into account when assigning police officers of various races to those given areas.

## The Problem

> *We want this section to introduce the problem being assessed to the reader. It will set the stage for our analysis and the propensity score matching technique.*

In our project , we are examining the findings from Antonovics and Knight in *A New Look at Racial Profiling* wherein the two authors further investigated whether preference-based discrimination or statistical discrimination was responsible for the racial disparities seen in traffic stop data. In making this determination, the researchers investigated whether the race of the officer making the stop had an effect on the officer’s decision to search a driver that he had pulled over. The belief is that the experience of police officers over time will cause them to use the observable characteristic, race, as a surrogate for the unobservable characteristics that may cause differences in driving habits. In this report, the authors found that officers are more likely to pull over drivers whose race differs from their own and thus concluded that preference-based discrimination was a key factor in officers’ decisions to conduct searches after traffic stops. To expand on such analysis, our project hopes to investigate how the race of the driver and race of the police officer influence an officer's decision to initiate traffic stops and to search, cite or arrest a driver. Stop pairs by location are as follows:

<div style="text-align:center"><img src="imgs/combined.png" /></div>

## Data Description

> We will describe the data being used in our analysis here. This section will parallel the work that we completed in our exploratory data analysis for Checkpoint #2.

Add information about data ingestion here and include exploratory data analysis...

<div style="text-align:center"><img src="imgs/eda.png" /></div>

*... put interactive plot here to allow audience to do exploratory data analysis for themselves...*

<div style="text-align:center"><img src="imgs/interactive.jpg" /></div>

*... potential to add real-world example of racial bias in traffic stops here...*

## Analysis

> This section will include the bulk of our analysis.

To ensure that we isolate the effect that preference-based discrimination has on an officer’s decision to search, cite or arrest a driver, we must remove, or limit, the effect that other variables (e.g., location, time, stop cause) have on an officer's stop decisions. In our analysis, we will do this by employing propensity score matching in our analysis. Using this statistical matching technique will involve:
1. Developing propensity score functions, which estimate the likelihood of a stop resulting in the driver being searched, cited and arrested. 
2. Computing a propensity score for each stop. 
3. Dividing the traffic stops into multiple groups based on the races of the driver and the officer involved in the stop. 
4. Matching stops from the above groups to form strata. 
5. Compare the means of the stop outcome variable (e.g., 1 for searched/cited/arrested and 0 for not searched/not cited/ not arrested) to estimate the average causal effect of the race variables on the stop outcome. 

*... add more of completed analysis later...*

<div style="text-align:center"><img src="imgs/propensity_placeholder.png" /></div>

## Conclusion / Next Steps

> Wrap up our findings here and propose a solution to the aforementioned problem.

Shown here is what we expect our conclusion plot to look like wherein we identify any statistical significance that we found in our analysis.

<div style="text-align:center"><img src="imgs/conclusion.jpg" /></div>

*... add proposed fixes to police departments to combat racial discrimination ...*