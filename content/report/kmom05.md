---
Title: Kmom05
Description: My report for Kmom05.
Template: kmom
---

Kmom05
=========

This week the focus was on page speed, performance and images. When I was writing my analysis regarding performance and speed, it struck me immediately how much worse the pages were doing on a mobile device compared to when used on a desktop. Not only does it seem like they need to work on their responsiveness, but when I looked at the generated reports it seems like all of them had both unused css and javascript, but also not entirely optimized javascript from a performance perspective. 

I tried to implement the tips and tricks I learned from the analysis, so I e.g. went through my CSS and tried to remove what’s not in use, like the css I saved for an alert note from the beginning of this course that I’m not using. I also went from using regular CSS files to load in minified CSS files instead to compress the size of my files. What I also did this week, is that I changed my hard coded menus for kmoms and analyses into dynamic ones with the help of "pages.foldername" and for-loops.

Usually when working with pictures, I make use of some simple photo handling program on the computer, since I never really alter the pictures more than some cropping. Lately I’ve been using Figma a bit also. Cimage seem like a good tool for usage in web-context, mostly due to all the functionality that still leaves the original image untouched. This makes it possible to load in one single image, instead of three versions of the same one. For this assignment (I took my pictures from unsplash), I used the crop options to have three versions of the image depending on screen size, and got good guidance from how Niklas showed the 1 to 1 ratio, and how he used <picture> and srcset. As a result, instead of loading in the original picture (I’m using sunrise-1.jpeg as example) which is 1.3MB large, I instead get the same picture, but to the size of 12.1kB when cropping it to a width of 375px to fit the smallest screens. Although before I could enjoy the benefits of Cimage, I needed help (which I got in the discord group) to track down what’s been keeping Cimage from loading in pictures with the path “image/gallery”. Turned out, the permissions were a bit wrong and quickly fixed with chmod 777. After uploading my portfolio to the student server I noticed it takes a long time for the server to handle the requests to Cimage (if I open the image in another tab and remove the Cimage requests it works like a charm), which makes the gallery load really slowly and inconsistently, at times it does not manage to show all nine images. Although there have been issues with the server this week, so maybe it's just not completely fixed yet.

After this week, I feel like my understanding of choosing the right sizes of images have increased. Not only does it affect the time it takes to load a website, it also affects the layout and the feeling I get when I visit a site. I like that the images fit nicely no matter the screen size, and that I don’t have to wait ages for them to load. Nowadays I suppose it’s getting more and more common to have unlimited data on portable devices, but for those who don’t, it makes a lot of difference on how much browsing they can do, if the site is optimized for taking up as little data as possible.

<div class="embed-container">
    <iframe src="https://www.youtube.com/embed/L_jWHffIx5E" frameborder="0" allowfullscreen></iframe>
</div>