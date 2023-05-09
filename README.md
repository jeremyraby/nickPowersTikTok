# About

Nick Powers ([@thatnickpowersguy](https://www.tiktok.com/@thatnickpowersguy)) has compiled and maintained a spreadsheet of various data detailing social issues in the US including information such as economic factors (how much a Big Mac costs in each state) and political factors (the percentage of the state's voters who voted for Joe Biden or Donald Trump in the 2020 presidential election). "The Spreadsheet" has 250 fields for comparing each state against each other and is available for free as a CSV (how I got it) on Nick's [website]( https://www.thatnickpowersguy.com/).

## Firearm info

I initially was interested in analyzing data relating to deaths caused by firearms. I was raised in a military family and often went hunting as a kid. News media are full of stories about gun violence and various proposals for stemming the loss of life, including both extremes of outright gun bans and "Constitutional carry" and I wanted to have a look at what may **actually** work instead of reading propaganda or opinion pieces. In addition to being bombarded by news of yet another tragedy, I have some skin in this game as my family has had losses due to gun violence and I still have friends working in schools. This (basically) uniquely American problem has long been out of hand and it's past time we look into solutions that will be effective.

The Spreadsheet includes several fields which I thought might be correlated with gun violence, whether negatively or positively:

| Fields Used for Analysis |     |
| ------------------------ | --- |
| Rates of firearm ownership | Does the state require reporting stolen weapons? |
| Rates of violent crime per 100k | How much money was donated from the NRA |
| Rates of firearm deaths per 100k | % of the state voted for Joe Biden |
| % of population who experience domestic violence | % of the state voted for Donald Trump |
| Rate of drug overdoses | Number of police in the state per 100k |
| % of the populaiton below the poverty line | Is there a state assault weapons registration law? |
| Rates of suicide per 100k |

## Digging In

**Before beginning my analysis, I hypothesized that the more conservatively a state leans (based on 2020 presidential votes) the more likely that state will be to have higher rates of gun deaths due to lax regulation.**

### Sources

As detailed in the table above, I analyzed several issues I believed may be correlated with higher rates of gun deaths. All of the visualizations for these analyses can be found on GitHub as a [PowerPoint presentation](https://github.com/jeremyraby/nickPowersTikTok/blob/main/firearmDeaths.pptx) or a [pdf](https://github.com/jeremyraby/nickPowersTikTok/blob/main/firearmDeaths.pdf). I found several surprising relationships in the data and some that, sadly, weren't so surprising. I began my analysis by reading up on all the data sources used for The Spreadsheet. I was happy to learn that most of the data sources were pretty reputable - many come from the CDC, FBI, and the US Census Bureau. Some of the cited data sources, however, are trade organizations such as Zillow or are being cited by a third party like The Brady Campaign.

### Findings

To learn how best to combat gun violence, it's useful to know where we stand on the issue. It turns out the US experienced [45,222](https://wonder.cdc.gov/controller/datarequest/D158;jsessionid=B76F9B53AF4C1C03C33CDF78FFEB) deaths due to gun violence in 2020 with an average 13.7 per 100k and a high of 28.6 gun deaths per 100k people in Mississippi. This led me to some perfunctory questions: does gun ownership reduce violent crime? does gun ownership reduce gun deaths? Comparing rates of violent crime and gun ownership per state, I found only a weak positive correlation (*r* = 0.32). Comparing gun ownership and gun deaths, however, revealed a much stronger relationship (*r* = 0.79).

In addition to rates of gun ownership and deaths, I also looked at other factors I believed may tell a more complete story. I was surprised to learn that gun ownership has a very low relationship with rates of domestic violence against women (r = 0.25) and political leaning also is less correlated to gun deaths than simply owning a gun -  of the top 10 states for both gun deaths and votes for Donald Trump in 2020, there are only four states in common and the correlation is only *r* = 0.68 vs *r* = 0.79. Poverty has a similar relationship to gun deaths as does political leanings (*r* = 0.65). Sadly, the strongest relationship I found was between gun ownership and suicides (*r* = 0.82).

While I found a few factors that were positively correlated with higher rates of gun deaths - suicides, gun ownership, leaning conservative - I also wanted to see if anything was associated with fewer gun deaths. Interestingly, at least to teenage-me, states that either don't require registering assault weapons or outright prohibit their registration account for more than 90% of gun deaths in the US compared to states that require registering assault weapons. There is also a 20% and 43% decrease in gun violence and gun deaths, respectively, when state laws require lost or stolen guns be reported to the authorities. Speaking of the authorities, there is no correlation between the number of police in a state per 100k people and gun deaths (*r* = 0.01).

## Conclusion

This is an obviously contentious issue that deserves to be discussed with grace and humility. Deaths caused by firearms have increased by 23% between 2018 & 2021 (the limits of the [CDC Wonder database](https://wonder.cdc.gov/)) and 2023 is keeping pace. Setting politics aside, it *should* be obvious that this is not only a problem, but one which only seems to get worse. As a data professional, and gun owner, I feel the need to find a way to contribute to a solution.

While this was a quick project, and not particularly wide-ranging, I do think it's reasonable to draw a few conclusions and make a strong recommendation. Suicides may be more strongly associated with firearm deaths, but having access to guns makes the attempt far more likely to be successful; access to firearms, then, (measured by ownership) is the key factor in the high number of firearm deaths we have in America. There have been a number of proposed solutions to the problem of access over the years, but the fact remains "access" is a protected right under the law and the Supreme Court *Heller* (2008) decision has ensured a broad interpretation of the second amendment. How, then, can we regulate access short of a constitutional amendment?

There are two options I was able to study with these data: state laws requiring assault weapon registration and reporting stolen or lost firearms. Even though registering assault weapons is associated with a much larger decrease in firearm deaths (a whopping 92%!), the proposal has major political complications as seemingly-benign as defining "asssault weapon" all the way to including fears of [Hitler-esque monstrosity](https://scholarship.law.columbia.edu/cgi/viewcontent.cgi?article=1671&context=faculty_scholarship). So, in spite of a less dramatic impact I believe it would be a better first step to simply enact legislation requiring gun owners report to the police if they've lost one of their guns (or had it stolen). I found an average **42% decrease** in firearm deaths in states which have these laws compared to states that don't. It's reported that stolen guns are often transferred to people who can't legally buy one themselves - increasing their barriers to possessing firearms is not only prudent, it's effective.

## Get Active

So what can you do as a citizen? For starters, educate yourself! Check my work (and let me know if you find any discrepancies!), read a variety of reputable sources and maybe run some of your own analyses. Next, you can check out [VoteSmart](https://justfacts.votesmart.org/), a non-partisan organization where you can look up your elected officials as well as their voting history on a number of issues including gun control as well as finding their contact information to write or call their offices.

### Sources

Below are a few sources I haven't already hyperlinked:

Photo by <a href="https://unsplash.com/@jay_rembert?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Jay Rembert</a> on <a href="https://unsplash.com/photos/wTUm3le1WqI?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>

[Nick Powers' original data sources](https://www.thatnickpowersguy.com/services-1)

[Everytown For Gun Safety](https://everytownresearch.org/rankings/law/lost-and-stolen-reporting/#:~:text=Gun%20thefts%20occur%20at%20staggering,to%20identify%20gun%20trafficking%20rings.)