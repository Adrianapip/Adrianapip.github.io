Title: Wagtail for my Tasty Pastry blog
Date: 2019-08-01 
Category: General
Tags: Python, Django, Tasty Pastry
Slug: wagtail-for-my-tasty-pastry-blog
Authors: Adriana
Summary: How I came to choose wagtail as a cms, and some useful references I've collected
Status: published

I started Tasty Pastry by coding the html/css manually (and pretty crappily at that) but as a means to figure out the mechanics of my site. I knew I wanted an interactive cooking app, but I also wanted a blog feature. In the beginning, it was not clear to me if these were going to be two seperate apps in my Tasty Pastry project. In my mind, all things could be considered a 'blog post', but not all blog posts would belong in the interactive cooking app. For instance, consider a write up that compares types of pie pans. Where to put such information?

I decided to put aside the interactive cooking app and start with the all encompasing blog posts.

As I started writing 'blog posts', I figured out some sort of generic layout that I was happy with. I would come up with a recipe in Notion to  maintain my files and references, and then manually move that content into hand written html files. Recipes follow a basic format: a block of text for the introduction, a table for ingredients, and a list for intructions. 

Copying and pasting got real tedious, real fast.

It was time to move onto a content management system (cms) to maintain my files. 

I'm aware of different established cms that exist and are pretty popular: wordpress, etc. But. I'm a complicated creature. I have this tendancy to try to combine everything I know into a single project as to potentially yield the best/most efficient set of results. 

If I were keen on learning how to bake really well, I would just go with wordpress, or squarespace, and focus on my writing and baking. But, I'm also interested in becoming a better programmer. So let's just design this damn thing from the ground up! My thinking behind this is that eventually, I will want to have more control over Tasty Pastry. That is, I'm not planning on it being just a baking blog. There are plenty of great ones out there already, and I feel I can leverage my skills in a different manner. 

I went with wagtail for a couple of reasons. It was [suggested by a Hello Web App author Tracy Osborn](https://hellowebbooks.com/news/moved-hellowebbookscom-static-site-generator-full-django-site/) and that's how I started to implement it in my site. Once I realized how simple it was to get it up and working (I knew a little about Django at that point) I just kept going.

It took me about a day to get it working within my project, and to get the models and templates written.

Working with an app that already has lots of documentation allows me to understand the django framework a little better - how models work with templates, and how data is stored and retrieved in terms of managing content. 

If you're looking for a CMS that has good documentation, from a beginner's perspective, this may be a place to start. 

###Here are some good references that may help you alond your wagtail journey:   

[I found these tutorials sometimes more helpful than the official wagtail documentation.](https://www.accordbox.com/blog/wagtail-tutorials-building-blog-part-2/)

[Coding for Everybody also has some excellent wagtail video tutorials.](https://www.youtube.com/channel/UCwbsAsY_C6EmGI6_JHhECEQ) I really enjoy his laid-back teaching style and he tends to explain things pretty thoroughly. Highly recommend. 

[I use streamfield blocks for my editing interface.](http://docs.wagtail.io/en/latest/topics/streamfield.html#streamfield) It just gives me more flexiblity with the types of content I want to post.

[A github awesome list containing different packages you can add to your wagtail interface and other cool resources that the wagtail community has built.](https://github.com/springload/awesome-wagtail#bloggingnews)

[The github repo containing the source code for the app. Here I was able to find some html files that I needed in order to customize my blog. For instance, I altered the table.html file for my recipe ingredients tables so that they functioned in the way I wanted: checkboxes before every ingredient, etc.](https://github.com/wagtail/wagtail)