---
Title: Kmom02
Description: My report for Kmom02.
Template: kmom
---

Kmom02
=========
In this part of the course the focus was on learning how to use Markdown, SASS and further exploring the possibilities in Pico. It was also necessary to learn how to use Node and npm to be able to install and run e.g. SASS with its various available commands.

I have never used Node, npm or npm scrips before so it was very new to me and is therefore my biggest TIL this week. I notice similarities with the composer that installed Pico, and even though it’s a bit confusing with a lot of new techniques, it’s easier this week to see the benefit of using a program that handles the packages for me. I didn’t experience much trouble while using the npm calls, like “npm run style” or “npm run lint” per se, except that the lint-call gave me some issues. Even though it’s configured to support nesting up to five elements, it decided to complain in one file only about more than one element when nested. I couldn’t figure this problem out, so I solved it by nesting that one css-rule the old fashioned way. Furthermore it complained about id-selectors in the html-code in index.twig, so I had to add class-names, and I also had to search in the javascript file to find the function that erased the class-names to fix this. And lastly, it didn’t like the “-webkit-transition”, which I had no clue how to fix, since it was supplied in the direct from school code, and since today is a Saturday I commented it out, checked that nothing broke, and I am planning on addressing this issue with the teachers next upcoming working-day.

So far I really like SASS (there are two ways to write it, I’m using the method for .scss files), since it offers a lot more flexible and easy ways to write css. I especially like the fact that you can nest elements, the overview is, according to me, better. I haven’t used variables in a wide range there yet, but also here I like how I can set a variable and name it, which not only makes it easy to reuse, but the name instantly tells me what this specific variable was intended for. I chose to put watch flags on both style.css and style.min.css with the “-- watch” notation, which was supposed to handle the compiling into .css every time I save the .scss file, but that didn’t work all the time, so I still had to combine it with “npm run style”. So I’m slightly disappointed with that feature, since I first couldn’t understand why my css didn’t always update - but after figuring it out the development of the site still went smoothly. I chose to do all the extra assignments to learn as much as possible, and the trickiest part was figuring out how to access the google fonts files needed as .woff and .woff2 files, but a bit of googling solved that.

In my theme I’m going for a quite neutral page to give it a laid-back professional vibe that lets you directly focus on the content, but I combine it will colourful accents to highlight that professional doesn’t have to lack energy - and to mimic the importance of colourful bright moments in life that brings a smile to your face. I didn’t start off with a plan on how my design should look, it got build after I chose the images that were supposed to, in some way, reflect me. It was easy to choose Montserrat and Raleway as my fonts, since they offered a serious but soft impression to my page, while they didn’t emanate the amount of classical sophistication that a serif would and which I feel would look less good in combination with he spurts of colour in my theme. I chose to set the font-sizes and the spacing of letters after seeing the video with Emil Folino, and after reading The Principles of Beautiful Web Design. 

I chose to divide up my code in the .scss files depending on what they addressed, e.g. I:
* have one variables.scss file that handles all my variables,
* put the basic layout like positioning, sizes etc. into the layout.scss that’s imported in base.scss, while I kept theme-based style like e.g. colouring and fonts in style.scss (which imports all other necessary files),
* put the navbar into one .scss file to have it nicely grouped,
have the responsiveness in one file for the time being.

This organization may be something I will change later depending on how my code develops further into the course.