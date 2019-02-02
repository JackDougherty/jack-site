---
title: "Site Info"
permalink: /site-info/
date: 2019-01-20
---

## Migrating from WordPress to Jekyll
- Learn why and how I [migrated from WordPress to Jekyll](2019/01/01/wordpress-to-jekyll) with this Minimal-Mistakes remote theme

## Customizations not fully documented in Minimal Mistakes Theme
- replace Home with static page, not recent posts
  - delete default index.hmtl from root
  - place home.md in _pages
  - in config near bottom add `"_pages"`
  - in data > navigation, use `"url: /"`

## Theme modification

On home.md feature_row, to delete "Learn More" button but keep clickable images with excerpt text

In _includes > feature_row, line 46, delete this portion: `{{ f.btn_label | default: site.data.ui-text[site.locale].more_label | default: "Learn More" }}`

## Steps to create [Scholarship page](/scholarship/):
- in Zotero, install customized CSL citation style [chicago-chrono-abstract-bib.csl](https://github.com/JackDougherty/zotero-custom-styles)
- in Zotero collection > create bib with custom CSL > to clipboard
- paste into Markdown converter: <https://euangoddard.github.io/clipboard2markdown/>


## TO DO
- clean up WP post migration and reduce image clutter
- currently I have two images folder (one for posts, one for pages). figure out why posts allow pathname to /images at root level, but pages do not (yet)
- configure Site search to include Pages, not just Posts <https://mmistakes.github.io/minimal-mistakes/docs/configuration/>
  - Try Google Custom Search Engine <https://mmistakes.github.io/minimal-mistakes/docs/configuration/#google-custom-search-engine>
  - Try Jekyll Algolia - see deployment guide for GitHub Pages: <https://community.algolia.com/jekyll-algolia/github-pages.html>
- configure Google Analytics
- modify footer to add Creative Commons licensing. See _includes > footer > custom.html snippets, or footer.html
- modify CSS to reduce height of feature__wrapper in home.md
- can Atom Editor be coded to auto-update dates inserted into Pages (last updated...)?


## Formatting Guide

### List of sample links
- [Embedded link](http://google.com)
- Visible link <http://google.com>

### HTML iframe, with quote marks around with and height, whether percentages or pixels

Code:
```html
<iframe src="https://jackdougherty.youcanbook.me/" width="100%" height="600px"></iframe>
```
Demo:
<iframe src="https://jackdougherty.youcanbook.me/" width="100%" height="600px"></iframe>

### Image without caption using Markdown

Pathname refers to `assets/images/` folder

Code (to come)

Demo:

![](assets/images/sample-300x200.jpg)

### Image with caption [Liquid templating](https://jekyllrb.com/docs/liquid/)

Use Liquid (caption appears in Minimal-Mistakes theme) instead of Markdown (no caption appears). Pathname refers to `assets/images/` folder

Code:
{% raw %}
```markdown
{% include figure image_path="assets/images/sample-300x200.jpg" alt="sample image" caption="here's the sample image" %}
```
{% endraw %}

Demo:
{% include figure image_path="assets/images/sample-300x200.jpg" alt="sample image" caption="here's the sample image" %}

### Image alignment (right or left) with caption

Code:
{% raw %}
```markdown
{% include figure image_path="/images/sample-300x200.jpg" alt="sample image" caption="sample caption" %}{: .align-right}
This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images.
```
{% endraw %}

Demo:
{% include figure image_path="/images/sample-300x200.jpg" alt="sample image" caption="sample caption" %}{: .align-right}
This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images.

### YouTube embed
Code:
{% raw %}
```markdown
{% include video id="3sK7-g0otGM" provider="youtube" %}
```
{% endraw %}

Demo:
{% include video id="3sK7-g0otGM" provider="youtube" %}
