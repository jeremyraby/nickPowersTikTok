# About

This is a practice repo using "the speadsheet" from @thatnickpowersguy on TikTok.

## Firearm info

- Compare states
  - firearm ownership
  - violent crime per 100k
  - firearm deaths per 100k
  - % domestic violence
    - men
    - women
  - drug od rate
  - poverty rate
  - suicide rate
  - require reporting stolen weapons
  - $ donated from gun rights activists
  - voted biden
  - voted trump

### Questions & hypotheses

> Some of this I've either read about over the years or have actually seen a TT from Nick about the individual topic.

General thoughts: more "conservative" (based on Trump/Biden votes in 2020) states will have more liberal firearms laws than more "liberal" states but will have worse indicators regarding crime.

- Do states with higher rates of firearm ownership have lower rates of violent crime?
  - Read about data sources for relevant fields:
    - size (sq mi)
      - taken thrid-party from US Census
    - population
      - taken from USDA ERS
    - firearm ownership
      - supposedly ultimately comes from Pew. This is also just going to be hard to trust regardless of source because people won't necessarily be truthful on surveys since registration isn't universally required
    - violent crime per 100k
      - from Wikipedia, reported in 2020
  - Suprised to find a weak correlation between rates of firearm ownership and rates of violent crime (r = 0.32).

- Do states with higher rates of firearm ownership have lower rates of firearm deaths?
  - Firearm deaths per 100k data come from CDC and are as reported in 2021
  - Shocked to find such a high correlation (r = 0.79) between rates of firearm ownership and rates of firearm deaths per 100k

- Do states with higher rates of firearm ownership have lower rates of domestic violence against women?
  - % domestic violence against women
    - reported by the National Coaltion Against Domestic Violence, but many of their sources are reliable (CDC, BLS)
  - Weak correlation with higher rates of gun ownership and higher rates of domestic violence against women ( r = 0.25)

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
    - The percentage difference between two values is calculated by dividing the absolute value of the difference between two numbers by the average of those two numbers. Multiplying the result by 100 will yield the solution in percent, rather than decimal form.
      - Max violent crime % diff =(ABS(478-837.8)/AVERAGE(478,837.8)*100) = 54.7%
      - Max gun deaths % diff =(ABS(15.4-28.6)/AVERAGE(15.4,28.6)*100) = 60%

- Do states with higher violent crime rates have more drug overdoses?
  - Surpised to find no correlation (r = 0.02)
  - Data from CDC and records drug od mortalities

- Are states which lean red (measured by having a higher percentage of votes cast for Trump than Biden in 2020) less likely to have gun deaths?
  - Red states are highly correlated with a high amount of gun deaths (r = 0.68).
    - This is a slightly weaker relationship than gun ownership vs gun deaths, but that makes sense because gun owners aren't only in red states

- Do states with more poverty have more crime?
  - There's a moderate positive relationship between violent crime and poverty rates (r = 0.48), but a stronger correlation between gun deaths and poverty (r = 0.65)
  - poverty data third party from the US Census Bureau