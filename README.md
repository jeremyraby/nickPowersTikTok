# About

Nick Powers (@thatnickpowersguy) has compiled and maintained a spreadsheet of various data detailing social issues in the US including economic factors (how much a Big Mac costs in each state) and the percentage of the state's voters who voted for Joe Biden or Donald Trump in the 2020 presidential election. "The spreadsheet" has 250 fields for comparing each state against each other and is available for free as a CSV (how I got it) on Nick's [website]( https://www.thatnickpowersguy.com/).

## Firearm info

I initially was interested in analyzing data relating to deaths caused by firearms. I was raised in a military family and often went hunting as a kid. News media are full of stories about gun violence and various proposals for stemming the loss of life, including both extremes of outright gun bans and "Constitutional carry" and I wanted to have a look at what may **actually** work instead of reading propaganda or opinion pieces. In addition to being bombarded by news of yet another tragedy, I have some skin in this game as my family has had losses due to gun violence and I was personally in a school lockdown as a teacher when a student brought a gun to school (thankfully the student posted threats on facebook and police intercepted them before anyone was hurt). This (basically) uniquely American problem has long been out of hand and it's past time we look into solutions that will be effective.

The Spreadsheet includes several fields which I thought be correlated with gun violence, whether negatively or positively:

| Fields Used for Analysis |     |
| ------------------------ | --- |
| Rates of firearm ownership | Does the state require reporting stolen weapons? |
| Rates violent crime per 100k | How much money was donated from the NRA |
| Rates offirearm deaths per 100k | % of the state voted for Joe Biden |
| % of population who experience domestic violence | % of the state voted for Donald Trump |
| Rate of drug overdoses | Number of police in the state per 100k |
| % of the populaiton below the poverty line | Is there a state assault weapons registration law? |
| Rates of suicide per 100k |

## Digging In

**Before beginning my analysis, I hypothesized that the more conservatively a state leans (based on 2020 presidential votes) the more likely that state will be to have higher rates of gun deaths due to lax regulation.**

### Sources

As detailed in the table above, I analyzed several issues I believed may be correlated with higher rates of gun deaths. All of the visualizations for these analyses can be found on GitHub as a [PowerPoint presentation](https://github.com/jeremyraby/nickPowersTikTok/blob/main/firearmDeaths.pptx) or a [pdf](https://github.com/jeremyraby/nickPowersTikTok/blob/main/firearmDeaths.pdf). I found several surprising relationships in the data and some that, sadly, weren't so surprising. I began my analysis by reading up on all the data sources used for The Spreadsheet. I was happy to learn that most of the data sources were pretty reputable - many come from the CDC, FBI, and the US Census Bureau. Some of the cited data sources, however, are trade organizations such as Zillow or are being cited by a third party like The Brady Campaign.

### Findings

To learn how best to combat gun violence, it's useful to know where we stand on the issue. It turns out the US experienced [45,222](https://wonder.cdc.gov/controller/datarequest/D158;jsessionid=B76F9B53AF4C1C03C33CDF78FFEB) deaths due to gun violence in 2020 with an average 13.7 per 100k and a high of 28.6 gun deaths per 100k people in Mississippi. This led me to some perfunctory questions: does gun ownership reduce violent crime? does gun ownership reduce gun deaths? Comparing rates of violent crime and gun ownership per state, I found only a weak positive corelation (*r* = 0.32). Comparing gun ownership and gun deaths, however, revealed a much stronger relationship (*r* = 0.79).

In addition to rates of gun ownership and deaths, I also looked at other factors I believed may tell a more complete story. I was surprised to learn that gun ownership has a very low relationship with rates of domestic violence against women (r = 0.25) and political leaning also is less correlated to gun deaths than simply owning a gun -  of the top 10 states for both gun deaths and votes for Donald Trump in 2020, there are only four states in common and the correlation is only *r* = 0.68 vs *r* = 0.79. Poverty has a similar relationship to gun deaths as does political leanings. Sadly, the strongest relationship I found was between gun ownership and suicides (*r* = 0.82).

## Conclusion



While I found a few factors that were positively correlated with higher rates of gun deaths - suicides, gun ownership, leaning conservative - I also wanted to see if anything was associated with fewer gun deaths. Interestingly, at least to teenage-me, states that either don't require registering assault weapons or outright prohibit their registration account for more than 90% of gun deaths in the US compared to states that require registering assault weapons. There is also a 43% and 46% decrease in gun violence and gun deaths, respectively, when state laws require lost or stolen guns be reported to the authorities. Speaking of the authorities, there is no correlation between the number of police in a state per 100k people and gun deaths (*r* = 0.01). 

- Do states with higher rates of firearm ownership have higher rates of suicide mortality?
  - Data come from CDC for 2021, per 100k residents
  - I've heard that states with higher gun ownership have more suicides, but I couldn't believe an Pearson correlation of 0.82!
    - It makes some sense in that more guns the attempt is more likely to be successful, but also that someone may be more likely to attempt if a probably successful method is easily available

- Do states with more money donated by the gun lobby have less violent crime?
  - Money donated by gun lobby data comes from Brady Council and is reported as how much money has been donated to the state's currently-serving federal senators over the course of their careers.
  - Mitt Romney has had way more money donated than anyone else
  - There's basically no relationship between money donated by gun lobby and violent crime or gun deaths

- Do states that require reporting lost or stolen guns have less violent crime/gun deaths?
  - Not sure where these data come from, but I did find from [Everytown](https://everytownresearch.org/rankings/law/lost-and-stolen-reporting/) that 15 states require reporting of stolen/lost guns
  - States requiring reporing max violent crime = 478 / 100K
  - States without reporting max violent crime = 837.8 / 100k
  - States requiring reporing max gun deaths = 15.4 / 100k
  - States without reporting max gun deaths = 28.6 / 100k
  - 43% difference in violent crime
  - 46% difference in gun deaths

- Do states with higher violent crime rates have more drug overdoses?
  - Surpised to find no correlation (r = 0.02)
  - Data from CDC and records drug od mortalities

- Are states which lean red (measured by having a higher percentage of votes cast for Trump than Biden in 2020) less likely to have gun deaths?
  - Red states are highly correlated with a high amount of gun deaths (r = 0.68).
    - This is a slightly weaker relationship than gun ownership vs gun deaths, but that makes sense because gun owners aren't only in red states

- Do states with more poverty have more crime?
  - There's a moderate positive relationship between violent crime and poverty rates (r = 0.48), but a stronger correlation between gun deaths and poverty (r = 0.65)
  - poverty data third party from the US Census Bureau


Hey y'all, I'm working on a project analyzing/visualizing some various shit about the country. I'm currently working on something about guns, but I have a data set that is really extensive and I figured some of y'all may be interested in some of it. I have the different fields broadly categorized in a google sheets and I'd appreciate it if you wouldn't mind taking a look-see and letting me know if there are any topics you'd like me to explore. Here's the link to the data categories: https://docs.google.com/spreadsheets/d/1a94XNgpIOefc12vtiKNoB1SC-u1CULwO5YxudBq6TR0/edit?usp=sharing

And here's a read-only version of the dataset if you want to get an idea of how it's organized: https://www.thatnickpowersguy.com/blank-page