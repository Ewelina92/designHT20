---
Title: Kmom06
Description: My report for Kmom06.
Template: kmom
---

Kmom06
=========

This week’s focus was on design principles and accessibility (and performance) of web sites. By learning about design elements it made it a bit easier to look at pages and see what I like or dislike about them. It feels a bit harder to, by myself, combine the elements into something that looks smashing, but looking at different portfolios as I did in my analysis task makes it easier, although I don’t feel like I had the time to explore all the CSS and possibilities that I find good-looking. Especially the movement aspect is a part I would like to learn more about, and something I noticed in the assignment that other people make use of. I found it interesting also, that two chose to use Wordpress when creating their portfolios, so I’m more impressed by the one who designed and coded the page without using website builders.

I did try to implement a bit of movement in my page, by making the images in the gallery stick out/pop out as a hovering effect, together with a subtle box shadow, with the aim of providing movement and depth. I also tried improving the balance on the landing page, by making the image a bit larger.

The final touch is, for me, the small changes to make the website feel complete. In the context of web design, it may be as easy as adding a color, or modifying the balance of the page.

What I also did this week, is that I improved the accessibility of the pages so they reached 100, and I worked a bit on the performance. My goal was to reach at least 90 in performance on all the pages, something I think I managed to do. For example I got the performance of the gallery from 51 to 92 on mobile (mobile was worse on every page). Although if I ctrl + shift + R sometimes the performance is 70, and sometimes over 90 in the gallery, so it’s a bit inconsistent. Some of the measures I used to reach my goals were:

* I chose a different size for the images in the gallery, e.g. when three columns are used on a desktop I load in the image with the width 400px by adding “&w=400”. 
* I added the language attribute to my html-tags.
* I set the tab index to 0 instead of 1 on the toggle menu. 
* I worked on making sure my text isn’t invisible during web font load, by adding font-display: swap in the @font-face.
* I tried preloading some suggested fonts that Lighthouse provided.

My TIL this week is that relative small measures, can have a huge impact on my page’s performance and make it more accessible. For example by having a smaller page size, it’s easier to load if the network connection isn’t the best, and by having alt attributes on the images, I make them accessible to be read out.