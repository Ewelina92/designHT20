---
Title: Analysis 11
Description: My analysis of my own project.
Template: analysis
---

Analysis 11 - Speed and loading
==========================

The goal of this report is to look at my own project's performance and speed, as done previously in kmom05 regarding operating web sites. For reflective purposes, these results will be compared to the results from kmom05.

Selection
-----------------------
I chose to analyze the part of the page that corresponds to the default user experience, which in my opinion consists of the default theme made for the client. The alternative mode (the dark mode), and the documentation page are therefore excluded. 

The project can be reached [here](http://www.student.bth.se/~eaja20/dbwebb-kurser/design/me/kmom10/portfolio/).

![Screenshot of project](%base_url%/image/project.png?w=1200)

Method
-----------------------
I looked at all three pages within the project separately. To get information about the speed and performance I used PageSpeedInsight, and the devtool browser named Network that provided information regarding loading time, the amount of resources and the total page size. Each measurement was conducted three times, and an average value calculated. The data is noted down in a Google Spreadsheet, and available through the links presented below under "Result". The measurements were conducted on the page accessed from the student server, and not by analyzing it locally. 

Result
-----------------------
All data is available [here](https://docs.google.com/spreadsheets/d/19FHOF-ZUIPKkgH3-4ppM00rfUBS_Zz04gk_Ze--0PhU/edit?usp=sharing).
The comparison data is available [here](https://docs.google.com/spreadsheets/d/1ZbIIcGJDxvr4C_A29_3kibigt4cGHYdD5-cc_ZAH36M/edit?pli=1#gid=0), or through the previous analysis.

From the generated reports, multiple possible improvements were suggested, for example the four written below (all three pages got the following suggestions in the same order):
* eliminate render-blocking resources
* serve images in next-gen formats
* preload key requests
* remove unused CSS


Analysis
-----------------------

From the results, it's clear that the general performance (the general grade from PageSpeedInsight) is worse when on a mobile device compared to the desktop version. The mobile version for all the parts of the page were 19,6% worse compared to the desktop version. This result is in line when comparing with the car rentals that were the objects for analyzing in kmom05, where their performance also decreased when used on mobile devices. By comparing these results with the results of the car rentals, it's easier to see a bigger context during analyzing, but since my project page is significantly smaller in size (and not a big site intended for usage by the world every day), the comparison can only serve as an interest point in learning, and no significant conclusions can be made.

My project got four suggestions for how to improve the performance. The biggest one according to PageSpeedInsight concerned taking action against elimination of render-blocking resources. Furthermore, serving images in next-gen formats like e.g. WebP, could increase the speed. Preloading key request like the fontawesome fonts and removing unused CSS were the two minor suggestions. 

The suggested ways of improving my projects performance seems to be points all websites should be aware of and working on. The car rental sites got e.g. suggestions regarding their usage of images, where JPEG was suggested instead of PNG to optimize their size, (which  Beaird et al. [1] also mentions) and in my project where JPEG is widely used, I instead got the suggestion about trying a newer format. Overall, it seems that the handling of images is a major point when working towards a page that works well on all devices. 

The suggestion regarding unused CSS isn't only occurring at my site, since all the other car rental sites got the same comment. It seems, that effective CSS files (and minimized ones are preferred) with thought through code does have an impact on the page. What I find tricky here, is since the major css files are included for all the pages, it seems like a hard task to eliminate all unused css, since it's quite possible, that not every sub-page will be using all of the file that's accessible to the page in whole. In the same spirit, it seems tricky to balance which key requests should be pre-loaded. As noted in the previous analysis, these suggestions are in line with what MOZ [2] highlights as performance affecting measurements. 

Overall, the loading time and speed is, according to me, definitely acceptable in my project, if we operate under the assumption that the time we have to get someones attention is three seconds. Three seconds are also, as I stated in the previous analyses the time I'm comparing to when deciding if a page is slow or fast, where I consider it fast if I as a user get at least two seconds to actually browse the page, and anything below one second would be considered slow. All the three pages were very close in loading time, but the best one (in the desktop version) is the landing page (525ms), followed by the highlights page(527ms) and the about page(554). Since the times are so close though, I can't really comment on why this may be.

There are areas that could need more work, especially the images would be a reasonable part to look into after taking into consideration the authors (mine) knowledge, and some areas are currently outside of my knowledge-box, like the parts concerning the server. 

References
-----------------------

[1] J. Beaird et al., *The principles of beautiful web design*. 4th ed., Australia:  SitePoint Pty. Ltd., 2020.

[2] MOZ, "Page Speed," 2020. [Online]. Available: https://moz.com/learn/seo/page-speed, Accessed on: Dec 04, 2020.

Other
-----------------------

I worked alone, not in a group.