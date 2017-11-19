---
title: "Preprocessors and SSGs"
date: 2017-11-19 -0100
---
<br>
## What do you think of pre-compiling your CSS?  
<br>
Well, I think it is a lot easier compared to regular CSS. It all becomes so much easier to manage through the 
addition of programming basics like *variables*, *functions(mixins)* and *loops*. One reason it's much more efficient is because the use of variables allows you to make changes in your stylesheet without changing alot of classes/divs and other containers separately. For example, instead of having to change the font-size in all your styles you can just change the value of the variable and then use that variable in all cases where you want the same output.  
<br>
Another reason is because it allows more a more understandable parent/child relationship of elements through the use of *nesting*. Nesting makes it alot more easier to read and understand which elements belong to eachother, and it's also a faster way to let child elements share attributes of their parent element. The use of mixins and conditionals is also relevant, since they radically improves the rate at which you can produce certain results in your styles. A good example of mixin efficiency is when you have to add vendor prefixes. Instead of rewriting those same prefixes all over your project you can just create a mixin which does all that for you and then store it in a mixin variable. The ability of mixins to take arguments also improves this usability bonus by letting you easily switch values that the mixin applies. I also find the *@import* option in Sass to drastically improve readbility of your stylesheets by easily allowing you to have a main stylesheet that imports separate stylesheets that all take responsibility over different parts of the layout (typography, container placement, color etc). This allows for easy overview of the project and a good tree of folders that you can traverse when changing stuff in your styles.  
<br>

I mainly used variables, @import and nesting. Due to time constraints on my part I went for a very simple webpage that features close to no advanced functionality. The planned use for this webpage also didn't call for that much styling and functionality, so I tried to keep it simple. Due to the project being pretty small, I didn't find any particular use for loops, mixins and extensions to improve the DRYness of my code. This means that I've basically just skimmed the surface of Sass, but it was enough for this project. I used variables to store information like font-sizes and familys for easy resuablitiy throughout the stylesheets. I also stored some basic content placement information in variables to use in my layout-stylesheet. Nesting was used in all parts where I had to reach child elements, for example the a element in the header class. Finally I used @import to import the substyles fonts and layout to the main scss styles, which in turned is used as the main stylesheet for the website.  
<br>

I can not think of any real cons of using Sass. In bigger projects you could argue that the compilation part of the preprocessor adds lag to the development time, which can add up in the long run. It also makes the outputted CSS quite messy, and the inability to quickly change something through the CSS alone can sometimes be a drag. It also adds a tool to the toolbelt, another part that can eventually fail on you in the most critical times. Other than this the negatives of preprocessors usually go hand in hand with inexperience with the tool. When you've gotten used to working with the tool it is hard to go back (in my opinion.) I've already mentioned the pros in detail but I would summarize them like this: Preprocessors like Sass removes alot of the repetiion that have always dragged CSS usability down. The result is a much easier system to work with and maintain. The Scss-code is shorter, more logical and especially smarter than regular CSS.  
<br>

## What do you think of static site generators?  
<br>

I think they are a great tool to use when you want to produce simple websites, ideally blogs, and other mainly text focused sites where you don't have to (or want to) rely on databases to store information, resulting in very fast and responsive sites. The static nature makes them very easy to manage since they have no outer dependancies on other frameworks, libraries or modules. This also makes them very secure, since they basically just serve very plain HTML.  
<br>
## What is robots.txt and how have you configured it for your site?  
<br>

Robots.txt is a simple tool for making sure that search engine bots only index the parts of your website that you allow them to. This means you can restrict access to specific folders that you may not want indexed, and you can also allow or disallow the bots access to the entire site. This is by no means a security feature, and malicious bots may (and will) ignore this file. I have configured my file to only allow Google full access to crawl my site. I have no particular data I want to keep from Google, and allowing it to index my site will help to make it appear on google searches.  
<br>
## What is humans.txt and how have you configured it for your site?  
<br>

Humans.txt is a tool developed as kind of an answer to the robots.txt idea. The idea is simple: Provide some way to give readers of your site the possibility to get information on the *humans* behind the site without the creator needing to openly provide this information in the website design (for example in the footer). By accessing humans.txt, people can access the information you have put there, which usually consists of the name of the creator of the site, his or her contact information, etc. It is entirely up to the site creator to decide which information goes there.
For my humans.txt, I kept it simple. It only consists of some basic information regarding me and how to contact me, a thank you-section and some site details.
