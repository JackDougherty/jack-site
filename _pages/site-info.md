---
title: "Site Info"
permalink: /site-info/
date: 2019-02-02
---
Read more about my WordPress-to-Jekyll transition at <http://jackdougherty.org/2019/02/17/wordpress-to-jekyll-github>

## How It Works: Static-Site Generator with Markdown, Jekyll remote theme, and GitHub Pages
Take a brief tour of my public GitHub repo for my personal site at <https://github.com/jackdougherty/jack-site>.

{% include figure image_path="images/2019/jack-site-atom-screenshot.png" alt="site screenshot in Atom Editor" caption="Screenshot of my new personal site files, as seen with Atom Editor" %}

- My primary site content resides in two key folders -- pages and posts -- named from familiar WordPress concepts.
- For example, my "teaching.md" page is written in easy-to-read [Markdown format](https://en.wikipedia.org/wiki/Markdown), with header info at the top, followed by text and links.
- My photos are uploaded to the images folder, and PDFs to the documents folder. The data folder contains the website navigation menu.
- The `_config.yml` file contains my site settings, written in [Jekyll](https://jekyllrb.com/) code, based on the [Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/) located elsewhere on GitHub.
- After making edits to the web content on my local computer, I push updates to my [free online GitHub account](http://github.com) with the user-friendly [GitHub Desktop](https://desktop.github.com/) tool (which I prefer over the command-line version). Publishing my content through [GitHub Pages](https://pages.github.com/) automatically converts Markdown and Jekyll code into static HTML pages, which appear in your web browser under my [custom domain name](https://help.github.com/articles/using-a-custom-domain-with-github-pages/).

### One-minute video: Website with Jekyll remote-theme and GitHub Pages
{% include video id="1eYPa6XVIXM" provider="youtube" %}

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
migrate old WP pages on advising, pathways to this site and/or Educ WP
- clean up old WP posts to match Markdown format; remove old images
- redirect old WP site to this site
- improve Site search configuation to include Pages, not just Posts <https://mmistakes.github.io/minimal-mistakes/docs/configuration/>
  - Try Google Custom Search Engine <https://mmistakes.github.io/minimal-mistakes/docs/configuration/#google-custom-search-engine>
  - Try Jekyll Algolia - see deployment guide for GitHub Pages: <https://community.algolia.com/jekyll-algolia/github-pages.html>
- change CSS for images from 100 width to auto?
  - https://github.com/mmistakes/minimal-mistakes/issues/1963
  - https://github.com/mmistakes/minimal-mistakes/issues/1583
- modify footer to add Creative Commons licensing. See `_includes` > footer > custom.html snippets, or footer.html

## Formatting Guide

### Link types
- Visible link uses angle brackets <http://google.com>
- [Embedded link: place text in brackets, URL in parentheses](http://google.com)
- But an embedded link to an internal page or post on this site requires the full URL

### Footnote
Write the main text and insert a bracketed footnote symbol with a unique number or keyword.[^keyword] Then somewhere else in the main text, write the same bracketed footnote symbol and number/keyword, followed by a colon, and the footnote text.

[^keyword]: Here's the footnote text.

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

### Redirect
I modified config.yml to accept jekyll-redirect-from plugin for GitHub Pages, but have only succeeded with the redirect_to option. See <https://github.com/jekyll/jekyll-redirect-from#redirect-to>
