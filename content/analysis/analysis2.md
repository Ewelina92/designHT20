---
Title: Analysis 2
Description: My analysis regarding performance and speed
Template: analysis
---

Analysis 2 - Performance and speed
==========================

The goal of this report is to look at three freely chosen websites' performance and speed, to learn about how these
aspects can be imporoved.

Selection
-----------------------

I chose to continue with the three car rental websites I used for the previous report. For more information about how they were
chosen, please read the previous report.
The chosen car rentals were Hertz, Sixt and Europcar. Their pages are the following:
* https://www.hertz.se/rentacar/reservation/
* https://www.sixt.se/
* https://www.europcar.se/sv-se

![Hertz above the fold](%base_url%/image/hertz1.png?w=1200)
![Sixt above the fold](%base_url%/image/sixt1.png?w=1200)
![Europcar above the fold](%base_url%/image/europcar1.png?w=1200)

Method
-----------------------

To get information about the speed and performance, I used PageSpeedInsight and the information avaible under Network in the devtools in the browser. Fomr PageSpeedInsight I noted down the total grade, and from the devtools I look at the loading time, the amount of resources and the total size of the page. I did each measurement three times, and calcualted the average value. All information was noted down using Google Spreadsheet. To get suggestions for possible improvements I 
used PageSpeedInsight and Lighthouse from the devtools. 

Result
-----------------------
All data is avaible at https://docs.google.com/spreadsheets/d/1ZbIIcGJDxvr4C_A29_3kibigt4cGHYdD5-cc_ZAH36M/edit?pli=1#gid=0.

From the generated reports, I could see that possible improvementpoints were for example:

For Hertz:
* removing unsused JavaScript and improving it to reduce the execution time
* removing unused CSS
* enabling text compression with e.g. gzip
* optimizing images by e.g. using jpeg intead of png
* trying to avoid using excessive Dom sizes

For Sixt:
* improve the internal server response time
* removing unsused JavaScript and improving it by e.g. minifying it
* removing unused CSS
* optimizing images by e.g. using jpeg intead of png
* trying to avoid using excessive Dom sizes

For Europcar:
* removing unsused JavaScript and improving it to reduce the execution time
* removing unused CSS
* trying to avoid using excessive Dom sizes


Analysis
-----------------------

From the general grades it's clear that the best site in both desktop and mobile is Sixt. Followed by Eurpocar and lastly Hertz.

In general, all the websites were a lot better at their desktop version compared to their mobile version, although Sixt is clearly more 
successful. Hertz mobile version was 67.8% worse than its desktop version, Europcar was 71.2% worse and Sixt only 31.8% worse. In general, it seems like you have
about 3 seconds to get someones attention, so you don't want to spend much time on loading a page, it should go quick. I think this is a reasonable time limit,
while I might have more time to wait while leisurely browsing at home, but when I want information fast, each second counts when I google and go through their options.

So the result of the grade concerning the mobile device felt a bit surprising to me after
visiting all of them on my google pixel 3a smartphone, where Sixt not only felt like it took time to load, there's also a long bit of scrolling if you're curios about
what they write and show. I also felt it wasn't completely made for my phone except for the main content at the top. Europcar on the other hand, seemed to handle
their mobile application well, even though they also had a lot of scrolling, compared to Hertz that nice sums up just the necessities without much scrolling options
on the first page. I would say that anything that gives me 2 seconds of active time on a page is fast, and anything less than 1 second is slow (in this 3 second limit).So when it comes to the desktop, Sixt and Europcar manage better than Hertz which required a full 4.5 seconds. 

By using the reports I can see that they all have similar suggestions to what could improve their performance, e.g. optimizing their javascript and CSS by removing the parts they don't use, and by going through their code to write it more effectively if possible. They all also could potentially improve their DOM to get
smaller sized pages. In summary, the most common improvements seem to refer to their usage of CSS and JavaScript. Both Hertz and Sixt got comments on their choice of images, for example they could overlook their choices of type, since the image format JPEG as Beaird et al. [1] explains often offer smaller file sizes when using 24-bit compared color compared to PNG. Further when working with images, they should make sure they use not only the right format, but also shows what's necessary and needed to show, especially in their mobile version. Since images should be relevant, interesting and appealing [1].

These suggestions are well in line with MOZ [2] that highlights exactly these topics, like compression, minifying JavaScript, CSS and HTML, improving server response time and optimizing images.

References
-----------------------

[1] J. Beaird et al., *The principles of beautiful web design*. 4th ed., Australia:  SitePoint Pty. Ltd., 2020.

[2] MOZ, "Page Speed," 2020. [Online]. Available: https://moz.com/learn/seo/page-speed, Accessed on: Dec 04, 2020.

Other
-----------------------

I worked alone, not in a group.