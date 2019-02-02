---
title: 'Migrating from Wordpress to Jekyll'
date: 2019-01-13
permalink: /2019/01/13/wordpress-to-jekyll/
categories:
  - technology
  - web writing
---
This month I took the plunge, and migrated my personal website from the Trinity College WordPress platform <http://commons.trincoll.edu/jackdougherty> to my own domain with a Jekyll static-site generator <http://jackdougherty.org>. Since 2011, I've created over 125 posts and pages on my personal WordPress site (and countless more on related WordPress scholarly sites, which are still intact for now.)

Why make this big shift? As usual, it's driven by a combination of factors:

## WordPress Worries
- How stable is my campus WordPress platform? Trinity's Ed Technology center has hosted a large multi-user WordPress platform <http://commons.trincoll.edu> since around 2011, and I was one of the early adopters. But it's become increasingly unclear to me whether this large platform is regularly backed up, and basic maintenance seems uncertain. (Trinity is currently running WordPress 4.8.1, which was released in August 2017, nearly a year and a half ago at this writing. The latest version is 5.0x, which is a major WP redesign with a new block-editing system.) Over the years I've learned that WordPress sites are complex beasts (especially individual sites on multiuser platforms), backups require keeping track of different pieces (the WP software, plugins, themes, uploads, and the separate database), and migrating all of these items to another WordPress platform can be very tricky. If my campus WordPress platform were to suddenly stop running (which has happened for a few hours here and there), all of my web writing hosted on that platform would go *poof*, which makes me a bit nervous. And even if Trinity's platform has a good backup, migrating from one WP platform to WP platform can be challenging.

## Static-Site Benefits
- In some people's minds, a static-site generator may sound like taking a step backwards from 2010-era WordPress to 2000-era DreamWeaver HMTL coding, because there's no drop-and-drag visual editor. And at first glance, "Jekyll" sounds like a monster, and the code even looks like one, too. But static-site generators have many advantages, at least for me. The workflow described below (writing in Markdown format, using a Jekyll remote theme, and publishing via GitHub Pages) is very similar to how I now write my others books (such as [On The Line](http://ontheline.trincoll.edu) and [Data Visualization for All](http://datavizforall.org)), and how I work with open-source code on GitHub. The static-site generator is *speedy* and the content loads *very quickly* in visitors' web browsers. Nearly all of the navigation features that attracted me to WordPress years ago are relatively easy to re-create with this two-column Jekyll theme. My content is leaner and more portable, in case I need to move it to another platform in future years (or decades). Finally, now it's entirely on my domain <http://jackdougherty.org>. While this means I'm no longer dependent on my campus's servers, that also means I'm responsible for maintaining it myself. Good thing that the static-site generator is simpler than WordPress's many moving parts.

## How It Works
All content now resides on a personal domain <http://jackdougherty.org> with a workflow that should be simpler (at least for me) for the future. Here's the basic steps I followed, and see more details in the [Site Info page](site_info):
- Create a free account on [GitHub](http://github.com), and create and publish a personal repository <https://github.com/JackDougherty/jackdougherty.github.io>
- Optional: If you don't like the default GitHub Pages personal repo domain name (mine would have been <http://jackdougherty.github.io>), purchase your own domain name (I recommend buying from <http://ReclaimHosting.com>)
- Compose in the lightweight [Markdown format](https://en.wikipedia.org/wiki/Markdown) with the [Atom editor](https://atom.io/)
- Format posts and pages using a remote Jekyll theme called [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) by Michael Rose
- Use [GitHub Desktop](https://desktop.github.com/) to push edits from my local drive to my personal GitHub repository, using the GitHub Pages feature to automatically publish Jekyll-based content as a static site, which quickly loads on your browser.
- PS: Thanks also to Ben Balter for creating the [WordPress to Jekyll Exporter plugin](https://ben.balter.com/wordpress-to-jekyll-exporter/), which quickly converted over 100MB of WordPress posts, pages, and images into Jekyll-formatted content.

## What could possibly go wrong?
Hey, it's the web, and lots of things could disappear or break down in future years. But I'm betting that Markdown and Jekyll will prevail as a quasi-generic format in the future. So if the Minimal Mistakes developer stops making improvements for his theme down the road, I *should* be able to easily migrate all posts and pages to another Markdown/Jekyll theme. Or if GitHub goes belly-up under its Microsoft ownership, I *should* be able to easily migrate the workflow to another host.

Now maybe I'll actually post more often. . . since it appears that I neglected to add new content to my personal Wordpress site for all of 2018. . . but hey, I was busy working on other sites!
