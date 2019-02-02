---
title: "Site Info"
permalink: /site-info/
date: 2019-02-02
---

## Migrating from WordPress to Jekyll
- Learn why and how I [migrated from WordPress to Jekyll](2019/01/01/wordpress-to-jekyll) with this Minimal-Mistakes remote theme

## Customizations not fully documented in Minimal Mistakes Theme
- replace Home with static page, not recent posts
  - delete default index.hmtl from root
  - place home.md in `_pages`
  - in config near bottom add `"_pages"`
  - in data > navigation, use `"url: /"`

## Theme modification
- On home.md feature_row, to delete "Learn More" button but keep clickable images with excerpt text
- In `_includes` > feature_row, line 46, delete this portion: `{{ f.btn_label | default: site.data.ui-text[site.locale].more_label | default: "Learn More" }}`

## Steps to create [Scholarship page](/scholarship/):
- in Zotero, install customized CSL citation style [chicago-chrono-abstract-bib.csl](https://github.com/JackDougherty/zotero-custom-styles)
- in Zotero collection > create bib with custom CSL > to clipboard
- paste into Markdown converter: <https://euangoddard.github.io/clipboard2markdown/>


## TO DO
- clean up WP post migration and reduce image clutter
- change CSS for images from 100 width to auto?
  - https://github.com/mmistakes/minimal-mistakes/issues/1963
  - https://github.com/mmistakes/minimal-mistakes/issues/1583
- configure Site search to include Pages, not just Posts <https://mmistakes.github.io/minimal-mistakes/docs/configuration/>
  - Try Google Custom Search Engine <https://mmistakes.github.io/minimal-mistakes/docs/configuration/#google-custom-search-engine>
  - Try Jekyll Algolia - see deployment guide for GitHub Pages: <https://community.algolia.com/jekyll-algolia/github-pages.html>
- configure Google Analytics
- modify footer to add Creative Commons licensing. See `_includes` > footer > custom.html snippets, or footer.html
- modify CSS to reduce height of feature__wrapper in home.md
- can Atom Editor be coded to auto-update dates inserted into Pages (last updated...)?

## Formatting Guide

### Link types
- Visible link uses angle brackets <http://google.com>
- [Embedded link: place text in brackets, URL in parentheses](http://google.com)
- But an embedded link to an internal page or post on this site requires the full URL

### Markdown image with pre-slash pathname (no baseurl because custom domain), actual size, but no caption
![root image caption](/images/sample-300x200.jpg)

### [Liquid templating](https://jekyllrb.com/docs/liquid/) image in root no-slash images  
{% include figure image_path="images/sample-300x200.jpg" alt="sample image" caption="here's the sample image" %}

### Liquid image in root no-slash aligned with caption
{% include figure image_path="images/sample-300x200.jpg" alt="sample image" caption="sample caption" %}{: .align-right}
This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images.

### HTML iframe, with quote marks around with and height, whether percentages or pixels
Code:
```html
<iframe src="https://jackdougherty.youcanbook.me/" width="100%" height="600px"></iframe>
```
Demo:
<iframe src="https://jackdougherty.youcanbook.me/" width="100%" height="600px"></iframe>

### YouTube embed
Code:
{% raw %}
```markdown
{% include video id="3sK7-g0otGM" provider="youtube" %}
```
{% endraw %}

Demo:
{% include video id="3sK7-g0otGM" provider="youtube" %}
