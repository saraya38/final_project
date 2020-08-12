# An Investigation into "Love Island" Contestants

![Picture](https://upload.wikimedia.org/wikipedia/en/9/99/Love_Island_%282015%29_title-card.jpg)

### Final Project for Saraya Danielsen

The reality dating show "Love Island" began in the U.K. in 2015, and has been popular since. This dataset includes all 96 contestants from seasons 2-4 of the British dating reality show, spanning from 2016 to 2019. I found the dataset on the "Data Is Plural" repository and accessed the file on GitHub; it was compiled by Microsoft employee Amy Kate Boyd to be used for educational and teaching purposes.

![tweet](https://media.journalism.berkeley.edu/upload/2020/08/159727289425b1279.png)

You can access the data [here](https://github.com/amynic/love-island-workshop/blob/master/data%20vizualisation/love-island-historical-dataset.csv).

### Age & Gender

The first thing I wanted to investigate was basic characteristics of the contestants, so I looked at age breakdowns and whether it was similar between women and men. I made a pivot table where I grouped by gender, and then grouped by age within each gender. This graph includes all contestants:

<iframe title="Age of All Contestants (2016-2019)" aria-label="Interactive line chart" id="datawrapper-chart-sj2xH" src="https://datawrapper.dwcdn.net/sj2xH/2/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="400"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"])for(var e in a.data["datawrapper-height"]){var t=document.getElementById("datawrapper-chart-"+e)||document.querySelector("iframe[src*='"+e+"']");t&&(t.style.height=a.data["datawrapper-height"][e]+"px")}}))}();
</script>

And these graphs are split by gender:

<iframe title="Age of Female Contestants (2016-2019)" aria-label="Interactive line chart" id="datawrapper-chart-gSj54" src="https://datawrapper.dwcdn.net/gSj54/4/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="400"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"])for(var e in a.data["datawrapper-height"]){var t=document.getElementById("datawrapper-chart-"+e)||document.querySelector("iframe[src*='"+e+"']");t&&(t.style.height=a.data["datawrapper-height"][e]+"px")}}))}();
</script>

<iframe title="Age of Male Contestants (2016-2019)" aria-label="Interactive line chart" id="datawrapper-chart-A7X00" src="https://datawrapper.dwcdn.net/A7X00/5/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="400"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"])for(var e in a.data["datawrapper-height"]){var t=document.getElementById("datawrapper-chart-"+e)||document.querySelector("iframe[src*='"+e+"']");t&&(t.style.height=a.data["datawrapper-height"][e]+"px")}}))}();
</script>

These graphs show that the female demographic is a little younger than the male demographic, but the show as a whole is just very young:

![age](https://media.journalism.berkeley.edu/upload/2020/08/1597274220a6fe4ec.png)

There is only information on strictly male and female categories; it must be noted that "Love Island" as a show is structured around a binary with specifically gender-split activities.

### Professions

I grouped contestants together by profession, and I had to do some cleaning because a few professions were the same, but not grouped together because of different titles. For instance, there were different types of models that I then grouped into 1 category. Then I divided the count column by the total to find the highest percentage professions:

<iframe title="Most Common Professions Among Contestants" aria-label="chart" id="datawrapper-chart-9wCW0" src="https://datawrapper.dwcdn.net/9wCW0/2/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="560"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"])for(var e in a.data["datawrapper-height"]){var t=document.getElementById("datawrapper-chart-"+e)||document.querySelector("iframe[src*='"+e+"']");t&&(t.style.height=a.data["datawrapper-height"][e]+"px")}}))}();
</script>

### Where Are they From?

I used Region and Contestant Outcome (what they placed) to find:
1. What regions the most contestants came from (London)
2. What region produced the most winners/runner-up contestants (Essex)

<iframe title="Where Contestants Are From" aria-label="map" id="datawrapper-chart-1tiQV" src="https://datawrapper.dwcdn.net/1tiQV/3/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="721"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"])for(var e in a.data["datawrapper-height"]){var t=document.getElementById("datawrapper-chart-"+e)||document.querySelector("iframe[src*='"+e+"']");t&&(t.style.height=a.data["datawrapper-height"][e]+"px")}}))}();
</script>

<iframe title="Where the The Show's Winners Come From" aria-label="map" id="datawrapper-chart-swx5b" src="https://datawrapper.dwcdn.net/swx5b/3/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="765"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"])for(var e in a.data["datawrapper-height"]){var t=document.getElementById("datawrapper-chart-"+e)||document.querySelector("iframe[src*='"+e+"']");t&&(t.style.height=a.data["datawrapper-height"][e]+"px")}}))}();
</script>

### Conclusion

I initially wanted to find fun correlations with this data set, but I played with it for a while and I couldn't find anything extremely interesting. For instance, this scrapped graph that I generated looks at how many days contestants spent on the island and how correlated that was with winning (because some contestants are added in as the show goes along, but could still win despite having less time and this could even prove to be an advantage because they make it farther with less work). And while a linear regression line shows that being on the show longer did seem to improve your chances at winning slightly, this idea is a bit intuitive already, and the graph itself is really rigid because people are in strict categories of 1st place, runner-up, 3rd place, and every other contestant in a "Last" category:

<iframe title="Days Spent on Show vs. Winning" aria-label="chart" id="datawrapper-chart-1Bv1u" src="https://datawrapper.dwcdn.net/1Bv1u/2/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="400"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"])for(var e in a.data["datawrapper-height"]){var t=document.getElementById("datawrapper-chart-"+e)||document.querySelector("iframe[src*='"+e+"']");t&&(t.style.height=a.data["datawrapper-height"][e]+"px")}}))}();
</script>

I think that if this dataset was a bit bigger with more column topics, I could have found better and more fun correlations.

In the end, I may have wanted to choose a dataset with more columns or just a little bigger in general; not that it was tiny, but I think I could have done more with a larger dataset. I still had fun though!
