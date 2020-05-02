# Design and Process

When building a site it is important to consider a few factors. 

First, **who is the site for**? Who is your target audience considering location, community, average income, devices the community has, how often they use the web, etc. It is good practice to ask the client their target audience. But it is hard to please *everyone*. 

**Hypotheticals** - make hypthetical characters based on your typical target audience. Making sure audequate qualities and data to make a statistical analysis. 

Second, **why people visit the site**? To determine why people are coming to your site, ask:

1. Attempt to discover the motivations for why visitors come to the site. 
1. Examine the goals of the visitor. 

Third, **what visitors are trying to achieve**. Consider key tasks and motivations as to why someone would visit your site. 

Create a list of reasons why people would visit the site. Then assin the list to your hypthetical characters. 

Fourth, **what information your visitors need**. For those that are on your site, consider what information they need to achieve their goals quickly. 

You can prioritize certain information based on your target audience. Be sure to stand out for those that you want, and even those that aren't meant to be there. What kind of background info can you provide or what differntiates you from the rest. 

Fifth, **how often people visit**. Think about how often you have to update the page. Some services do not require constant updates if their service is not that demanding. The same goes with information and how often it must be updated. 

# Site Maps

After knowing what needs to on the site, organize the information into sections. Create a diagram of pages that will be used to structure the site aka **site map**. 

**Card sorting** is a technique used to help determine what information should go on what page. This is done by grouping related information pertaining to the visitor. They then can be grouped together to create different sections of the site. 

# Wireframe
A wireframe is a simple sketch of the key  that will go on each page. It is like the barebones of the site, no color no style just formatting. 

# Using design for your message

+ A designer needs to priortize the information communicated on their site. 
+ Where do you want the login link, the contact us link, the about me, etc. Use some styling to make certain information pop out. A **visual hierarchy** is useful to help users focus on the key messages to draw people's attention. 
+ Group together related content.

# Visual Hierarchy

>**Visual hierarchy** refers to the order in which your eyes perceive what they see.

## A few ways to group
1. **Proximity**: items closer together = more importance
1. **Closure**: shaping items together creating an irregular shape that can fit in an imaginary box
1. **Continuance**: items placed in line or curve = more related
1. **White Space**: related items closer parted from unrelated items
1. **Color**: correct background color behind important information
1. **Borders**: borders making important information stand out 

Similarity in designs, repetition of qualities, consistency, headings = more related. 

# Site Navigation
The site navigation should be **concise**, **clear**, and **selective**, **contextual**, **interactive**, and **consistent**. 

# HTML5
```<article></article>``` acts as a container for any section of a page that could stand on its own. If a page has multiple articles then they will live in their own tags. They can also be nested within each other. 

```<aside></aside>``` it has two purposes
1. it should contain information related to the article (when inside a ```<article>``` tag) 
1. it should contain information related to the **whole** page

```<section></section>``` groups related content together, and each section should have its own heading! They may have multiple articles within them. 

```<hgroup></hgroup>``` it groups a set of one or more heading (1-6) tags. 

```<figure></figure>``` it contains any content that is referenced from the main flow of an article. It should only be used when the content simply referes to the element. Can go with the ```<img src=```>, and should always containg a **figcaption**.

```<figcaption></figcaption>``` provides a text or description of the figure it is within. 

```<div></div>``` an important way to group related elements. 

+ using an id or class attribute on ```<div>``` allows you to create CSS style rules for how much space the element should occupon and change the appearance of those elements.

```<a></a>``` is used to reference links but in HTML5 you can group a whole block as a link ex: 

```<a href="FILE.html"><article><h1></h1><p></p></article></a>```

### For older browsers!
Since older browers may not understand some of html5 elements it will display it as inline code. In that case, use the code below in CSS so they can become block elements:

```header. section. footer. aside. nav. article. figure```

```{display: block;}```

# Extra Markup

```<!DOCTYPE html>``` tells the browser which version of html to use. It also helps the browser render a page correctly. **It should be the first thing on each page!**

```<!-- TEXT -->``` is used to comment out the TEXT written. On a mac shortcut is 

```cmd + /```

```id=""``` is used in html to uniquely identify the one element from other elements on the page. The first character in the text should start with a letter or an underscore! With JS, id attributes can be used to allow the script to work with this element. 

```class=""``` rather than uniquely identifying one element on a page, you can identify more than one. Its value should describe the class it belongs to. 

**Block level elements** are elements that always appear to start on a new line in browser. Like h, p, and ul tags. 

**Inline elements** are elements that appear to continue on the same line with other elements. Like the a and img tags.

```<span></span>``` is the inline equivalent to ```<div>```. It is used to control the appearance of the content of those elements in CSS. 

```<iframe></iframe>``` short for inline frame, is a window cut into your page where you can see another page. **This is very useful when linking a Google Map onto a page and an html page!**
+ Both ```height="###"``` and ```width="###"```, followed by
+ along with it is the ```src="LINK"``` attribute that specifies the link.

```<meta>``` lives in the ```<head>``` element and contains information about the page. It is not shown to users but helps search sites. It does not have a closing tag!

The name attribute of a ```<meta name=""``` tag indicates an intention to specify a description of the page when followed by a ```content=""/>```

> ```<meta http-equiv="pragma"```
>      ```content="no-cache"/>```
    
    * This code prevents the browser from storing the page locally to save time downloading it another visit 

Using ```expires``` instead of ```pragma``` as well as a specific day, date, and time time-zone for the cache to expire. 

Shorcut for copyright is ```&copy``` or ```&#169```, for ```&``` it is ```&amp``` or ```&#38```