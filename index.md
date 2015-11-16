---
title       : Artemis War 2015
subtitle    : Visualising War Points
author      : 
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

### Pardus, War and War Points
* Pardus: a graphical Massive Multiplayer Online Browser Game
* Set in a futuristic universe where all players pilot a space ship
* Players of three factions strive to gain wealth and fame
* Various professions: traders, fighters, pirates, smugglers, other...

#### 2015: War in the Artemis Universe
* September 2015: War breaks out between the Federation and the Union
* October 2015: The Empire declares war on the Federation in response

#### Faction members earn war points for their heroic actions

* Q. How to track the three factions' progress during the two concurrent wars?

---
#### Data Gathering
* Data screen-scraped from the game's web pages


```
##    SkirmishID CaptureDate    Faction Points Kills Structures Missions Sectors
## 71         FE  2015-11-10 Federation 191612 71517      39995    80100       0
## 72         FE  2015-11-10     Empire 234582 92409      57573    49600   35000
## 73         FE  2015-11-11 Federation 199452 72857      39995    86600       0
## 74         FE  2015-11-11     Empire 240464 96009      57855    51600   35000
```

![plot of chunk FedEmpWarPoints](assets/fig/FedEmpWarPoints-1.png) 
* Started off with one-off graph plots, then evolved into...

---
#### Shiny Application

![Image of Shiny Application](assets/img/shinyapp.png)

---
#### Rounding Off

* Simple plots evolved into more complex plots
* War points often required breakdown by category (kills, missions, sectors captured)
* Gathered data used to derive trend lines
* Daily differences visualised to establish which faction has the momentum
* Shiny enlisted to turn these requirements into a web application
* Interactive plots
 * Clearer progress analysis
 * Aid to strategic planning
 * Hours of fun
* Try the application out at [Shinyapps.io](https://jdirrhind.shinyapps.io/ArtemisWar2015)
* View the source code on [GitHub](https://github.com/jdirrhind/ArtemisWar2015)
* This presentation built using [Slidify](http://slidify.org). Thanks for reviewing!
