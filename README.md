# Census Summary Level Codes
I wanted to share a CSV file I made of the different Census Summary Level code names. This is based off of the list compiled by the State of Missouri's [Missouri Census Data Center](http://mcdc.missouri.edu/allabout/sumlevs/).

This CSV makes it easy to join Summary Level codes with their respective Summary Level code names. 

If you're using R, you can do this easily with [dplyr's](https://github.com/hadley/dplyr) left_join function:
```
left_join(census.data.frame, summary.level.codes, by = "SUMLEV")
```
