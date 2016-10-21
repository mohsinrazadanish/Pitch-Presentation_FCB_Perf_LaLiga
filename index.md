---
title       : "Course Project: Shiny Application and Reproducible Pitch"
subtitle    : "FC Barcelona in La Liga during 2005-2015"
author      : "Muhammad Mohsin Raza Danish"
job         : Data Science Trainee
framework   : io2012   # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [bootstrap]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides

---

<style>

.title-slide {

  background-image:url(assets/img/barca_shirt.png);
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
  /* background-color: #4DBD33; FC Barca blue: #00529F, FC Barca claret: #722F37, grass: #4DBD33, spring green:#00EE76 */
  /* font-color: #00529F; */
  
}

.title-slide hgroup > h1{
  font-family: 'Oswald', sans-serif;
  color: #000000
}

.title-slide hgroup > h2{
  font-family: 'Oswald', 'Calibri', sans-serif;
  color: #000000;
}

.title-slide hgroup > p{
  font-family: 'Oswald', 'Calibri', sans-serif;
  color: #CCCCCC;
}



slide:not(.segue) h2{
  font-family: 'Calibri', Arial, sans-serif;
  font-size: 52px;
  font-style: normal;
  font-weight: bold;
  text-transform: normal;
  letter-spacing: -2px;
  line-height: 1.2em;
  color: #000000;
}


/* Fonts and Spacing */
article p, article li, article li.build, section p, section li{
  font-family: 'Open Sans','Helvetica', 'Crimson Text', 'Garamond',  'Palatino', sans-serif;
  text-align: justify;
  font-size:22px;
  line-height: 1.5em;
  color: #000000;
}

</style>


## FC Barcelona's performance in La Liga during 2005-2015


- FC Barcelona is a top tier football team in Spanish football league, **La Liga**.
- The club is based in **Barcelona**, **Catalonia**, **Spain**.
- The *full name* of the club is **Futbol Club Barcelona** and *short name* is **FCB**.
- The *nicknames* are **Barca** or **Blaugrana**.
- **Red** and **blue** have featured on the Barca shirt for *more than one hundred years* and the Club is widely known as the *Blaugrana* in reference to the names of these colours in the Catalan language.
- Their performance has been at the *top* in the last *10-11* years.
- The app shows a comparison between *FCB* and its *top competitors* in La Liga
- **Top Competitors:**
 *Athletic Bilbao, Atletico Madrid, Real Madrid, Sevilla FC, Valencia CF*


--- #custbg2

<style>
#custbg2 {
  background-color: #4DBD33; /* FC Barca blue: #00529F, FC Barca claret: #722F37, grass: #4DBD33, spring green:#00EE76 */
  <!-- font-color: #00529F; -->
}

#custbg2 h2{
  color: #000000;

}

</style>

## User Instructions

- There is a **widget** on the left that is used to input the *season*.
- On the right in the **main panel**, you see two tabs, one is for comparison with the top competitors and the other is for ranking table.
- In the **Comparison tab**, you see a plot that shows the goals difference of FC Barcelona with its top competitors during the given season.
- The goals difference for home games is shown with label <font color = "magenta">**H**</font> in *magenta* color. 
- The goals difference for away games is shown with label <font color = "blue">**A**</font> in *blue* color.
- The **horizontal line** is at goals difference of zero. This line indicates the *drawn* games. 
- The labels **above** the horizontal line at *y = 0* show the games that Barca **won** by the number of goals on the y-axis. 
- The labels **below** the horizontal line at *y = 0* show the games that Barca **lost** by the number of goals shown on the y-axis.
- The **Rankings tab** shows the rankings of the La Liga for top 20 teams of the season.

--- #custbg3 

<style>

#custbg3 {
  background-color: #7F1734; /* FC Barca blue: #00529F, FC Barca claret: #7F1734 or #722F37, grass: #4DBD33, spring green:#00EE76 */
}

#custbg3 h2{
  color: #000000;
}
</style>

## Rankings (2005-2012)



|  Rank  |     2005     |     2006      |       2007       |      2008       |
|:------:|:------------:|:-------------:|:----------------:|:---------------:|
|   1    | FC Barcelona | FC Barcelona  |   Real Madrid    |  FC Barcelona   |
|   2    | Real Madrid  |  Real Madrid  |  Villarreal CF   |   Real Madrid   |
|   3    | Valencia CF  |  Sevilla FC   |   FC Barcelona   |   Sevilla FC    |
|   4    |  Sevilla FC  |  Valencia CF  |    Sevilla FC    | Atletico Madrid |
|   5    |  CA Osasuna  | Villarreal CF | Atletico Madrid  |  Villarreal CF  |
|   6    |  Celta Vigo  | Real Zaragoza | Racing Santander |   Valencia CF   |



|  Rank  |     2009     |      2010       |      2011       |      2012       |
|:------:|:------------:|:---------------:|:---------------:|:---------------:|
|   1    | FC Barcelona |  FC Barcelona   |   Real Madrid   |  FC Barcelona   |
|   2    | Real Madrid  |   Real Madrid   |  FC Barcelona   |   Real Madrid   |
|   3    | Valencia CF  |   Valencia CF   |   Valencia CF   | Atletico Madrid |
|   4    |  Sevilla FC  |  Villarreal CF  |    Malaga CF    |  Real Sociedad  |
|   5    | RCD Mallorca | Atletico Madrid | Atletico Madrid |   Valencia CF   |
|   6    |  Getafe CF   | Athletic Bilbao |   Levante UD    |    Malaga CF    |


--- #custbg4

<style>
#custbg4 {
  background-color: #FFFFFF; /* FC Barca blue: #00529F, FC Barca claret: #722F37, grass: #4DBD33, spring green:#00EE76, tropical blue: #62B1F6, picasso blue: #0276FD */
  /* font-color: #00529F; */
}

</style>


## Rankings (2013-2015)


|  Rank  |      2013       |      2014       |      2015       |
|:------:|:---------------:|:---------------:|:---------------:|
|   1    | Atletico Madrid |  FC Barcelona   |  FC Barcelona   |
|   2    |  FC Barcelona   |   Real Madrid   |   Real Madrid   |
|   3    |   Real Madrid   | Atletico Madrid | Atletico Madrid |
|   4    | Athletic Bilbao |   Valencia CF   |  Villarreal CF  |
|   5    |   Sevilla FC    |   Sevilla FC    | Athletic Bilbao |
|   6    |  Villarreal CF  |  Villarreal CF  |   Celta Vigo    |

<font size = 3> <br>To use the **Shiny App**, follow the link: <a href ="https://mohsinraza.shinyapps.io/FCB_Performance_LaLiga/"> **Shiny App: FC Barca Performance in La Liga** </a> <br> </font>
<font size = 3> For **Source Code and Documentation of the Shiny App**, follow the link: <a href ="https://github.com/mohsinrazadanish/FCB_Performance_LaLiga"> **Source code: FC Barca Performance in La Liga** </a> <br> </font>
<font size = 3>For **Source Code of the Pitch Presentation**, follow the link: <a href = "https://github.com/mohsinrazadanish/Pitch-Presentation_FCB_Perf_LaLiga"> **Source code: Pitch Presentation for Shiny App 'FC Barca Performance in La Liga'** </a> <br> </font>

<font size=3>**Note:** The background of the title slide is *FC Barca jersey*; that of user instruction is <font color=#4DBD33>**grass**</font> color, and for the rankings I chose <font color=#7F1734>**claret**</font> for the background for Blaugrana. <br> </font>
<font size=3> **Contact:** *For any comments or questions, please write to me at* **mohsinrazadanish@gmail.com** </font>
