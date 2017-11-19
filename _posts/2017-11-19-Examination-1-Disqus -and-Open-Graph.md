---
title: "Disqus and Open Graph"
date: 2017-11-19 -0100
---
<br>
## How did you implement comments to blog posts?  
<br>
It was pretty easy to implement comments using Disqus. The only thing you had to do was sign up on their 
website and then follow the instructions. By including the disqus script in my wrapper layout and putting the logic
for it in my post.html I managed to get all pages of the type "post" to include comments. One of the 
shortcomings with a static site is exactly this: the inabiity to add dynamic functionality like comments, without using services like *Disqus*.  
<br>
## What is Open Graph and how do you make use of it?  
<br>
Open Graph is a protocol that enables you to show particular parts of your website when it's being shared
on for example Facebook. It consist of alot of different tags that can help identify your website, but the most common ones are the ones that share your websites title, type, URL and a fitting picture. It can also feature a description tag,which lets you describe what your webpage is about for the people that see it shared. It is used by adding metadata-tags to your head HTML-element.