# A-problem-by-McKinsey-Predictive-maintenance-of-naval-heavy-cutting-machinery
Widgets created for McKinsey-Shape proposed problem, 7th Workshop on Mathematical Solutions for Industrial Problems - IMPA, 6-10 September, 2021

https://user-images.githubusercontent.com/58062750/136110368-bab54da6-a966-4738-b895-722a0f1a51b1.mp4


McKinsey and Shape proposed a Predictive Maintenance challenge for participants of the 7th Workshop on Mathematical Solutions for Industrial Problems - IMPA, 2021. The goal was to predict failure, allowing for scheduling of maintenance and minimal machine-idle time. Each machine has a number of rotating blades that cut different types of products, to be used in the production of ship parts. A synthetic database was provided, containing a qualitative variable 'Type' (of cut product) which can be L (low), M (medium) or H (high). The quantitative variables available are thermo-mechanical - air temperature, process temperature (temperature of the blade), rotational speed of the blade, torque applied on the blade, moment (dependent on torque), and delta temperature (difference between blade's temperature 5 min before the measurement and current temperature) - and temporal - age of the blade, in minutes, associated to a Boolean indicator of failure (at time t, failure is 0 or 1). Time is reset after each blade replacement. Blades can fail many times before requiring replacement. Blades can have short or long life (circa 200 minutes).

After the initial data exploratory analysis and proposed dimensionality reduction and feature engineering, our group run several ML methods and delivered a compared analysis that can be found at https://centropi.impa.br/7wsmpi/.

This repository contains a few webapps that I have prepared for the data exploration. Taking advantage of the ternary classification of cuts, I explored the lifespan of the blades per "cut composition": can we find a correlation between quality of cut product and frequency of failure or blade lifespan?

![cuttypeill_](https://user-images.githubusercontent.com/58062750/135894319-014448d4-2973-423e-b052-dfbd47473bf8.png)


A naive approach gives a negative answer, as you can find in the available files. You can play with the widgets and see that no particular trend is found for lifespan or number of failures per type of cut.
