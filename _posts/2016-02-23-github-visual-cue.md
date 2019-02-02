---
id: 2451
title: GitHub browser is great, but needs a directional visual cue
date: 2016-02-23T13:11:03+00:00
author: jdoughe2
layout: post
guid: http://commons.trincoll.edu/jackdougherty/?p=2451
permalink: /2016/02/23/github-visual-cue/
categories:
  - Blog posts
---
I continue to be impressed with GitHub&#8217;s browser interface, which makes sharing, editing, and web hosting code or text so easy for novices. Next week I&#8217;ll start teaching GitHub to my undergraduate data visualization seminar, which includes many students who have never touched a piece of code in their lives. We primarily stick with the browser interface to avoid overwhelming newbies, since it does nearly everything we need.  But there&#8217;s one small user interface revision that would make it easier for students to learn how to make pull requests inside the browser.

The problem: The current GitHub browser interface provides no visual cue about the DIRECTION of the pull request, as shown below:<figure id="attachment_2452" style="width: 467px" class="wp-caption aligncenter">

<a href="http://localhost/wordpress/wp-content/uploads/2016/02/Github-browser-pull-request.png" rel="attachment wp-att-2452"><img class="size-full wp-image-2452" src="http://localhost/wordpress/wp-content/uploads/2016/02/Github-browser-pull-request.png" alt="No directional visual cue in the current browser" width="467" height="220" srcset="http://localhost/wordpress/wp-content/uploads/2016/02/Github-browser-pull-request.png 467w, http://localhost/wordpress/wp-content/uploads/2016/02/Github-browser-pull-request-300x141.png 300w" sizes="(max-width: 467px) 100vw, 467px" /></a><figcaption class="wp-caption-text">No directional visual cue in the current browser</figcaption></figure> 

In my teaching tutorials, I have to create a &#8220;TO &#8212; FROM&#8221; screenshot to help my students understand the direction of the pull request, as shown here:<figure id="attachment_2453" style="width: 325px" class="wp-caption aligncenter">

<a href="http://localhost/wordpress/wp-content/uploads/2016/02/GitHub-ToFrom.png" rel="attachment wp-att-2453"><img class="size-full wp-image-2453" src="http://localhost/wordpress/wp-content/uploads/2016/02/GitHub-ToFrom.png" alt="My modified &quot;To -- From&quot; tutorial screenshot" width="325" height="204" srcset="http://localhost/wordpress/wp-content/uploads/2016/02/GitHub-ToFrom.png 325w, http://localhost/wordpress/wp-content/uploads/2016/02/GitHub-ToFrom-300x188.png 300w" sizes="(max-width: 325px) 100vw, 325px" /></a><figcaption class="wp-caption-text">My modified &#8220;To &#8212; From&#8221; tutorial screenshot</figcaption></figure> 

Clearly, GitHub would be even better if this step were more intuitive. Here&#8217;s two possible solutions for the developers to consider:

1) GitHub Desktop for Mac already includes a directional visual cue, where the sending branch box is shaped like an arrow, pointing into the receiving branch, as shown below. You could replicate this in the GitHub browser interface.<figure id="attachment_2454" style="width: 281px" class="wp-caption aligncenter">

<a href="http://localhost/wordpress/wp-content/uploads/2016/02/GitHub-desktop-visual-cue.png" rel="attachment wp-att-2454"><img class="size-full wp-image-2454" src="http://localhost/wordpress/wp-content/uploads/2016/02/GitHub-desktop-visual-cue.png" alt="GitHub Desktop for Mac has a directional visual cue" width="281" height="201" /></a><figcaption class="wp-caption-text">GitHub Desktop for Mac has a directional visual cue</figcaption></figure> 

2) Or if that&#8217;s too complicated, a simple fix for the browser interface might be to change the current ambiguous symbols (&#8230;) into a visual direction cue with different punctuation (<&#8212;), as shown here:<figure id="attachment_2455" style="width: 409px" class="wp-caption aligncenter">

<a href="http://localhost/wordpress/wp-content/uploads/2016/02/Github-browser-pull-request-modified.png" rel="attachment wp-att-2455"><img class="size-full wp-image-2455" src="http://localhost/wordpress/wp-content/uploads/2016/02/Github-browser-pull-request-modified.png" alt="A simple fix: change (...) to (<--)" width="409" height="223" srcset="http://localhost/wordpress/wp-content/uploads/2016/02/Github-browser-pull-request-modified.png 409w, http://localhost/wordpress/wp-content/uploads/2016/02/Github-browser-pull-request-modified-300x164.png 300w" sizes="(max-width: 409px) 100vw, 409px" /></a><figcaption class="wp-caption-text">A simple fix: change (&#8230;) to (<&#8211;)</figcaption></figure> 

Once again, just trying to suggest a simple way to make the GitHub browser interface even easier for novices to use.