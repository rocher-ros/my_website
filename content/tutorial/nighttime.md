+++
title = "Estimating k with the nigh-time regression method in streams"

date = 2018-09-09T00:00:00
# lastmod = 2018-09-09T00:00:00

draft = false  # Is this a draft? true/false
toc = true  # Show table of contents? true/false
type = "docs"  # Do not modify.

# Add menu entry to sidebar.
linktitle = "Night-time regression"
[menu.tutorial]
  parent = ""
  weight = 3
+++


The night time regression is a method used to calculate the gas transfer coefficient in streams. The theory is that once photosynthesis ceases during the day, the oxygen concentration rises with a rate that is proportional to the reareation coefficient. Then, performing a linear regression between the oxygen deficit and the rate of change of oxygen as independent variable, the slope of the regression is equal to the reareation coefficient. If you have good diel curves of oxygen and need some kind of estimates of k, have a look!! See the article "Primary production in Flowing waters" by Howard T. Odum for further details and a full theory. The code is available [here](https://github.com/rocher-ros/nighttime_regression_multiple/wiki).

{{< figure library="1" src="NTR_example.png" title="" >}}