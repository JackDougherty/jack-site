---
title: 'Sample Post'
date: 2019-01-01
permalink: /2019/01/01/sample-post/
categories:
  - teaching
  - advising
  - scholarship
  - presentation
  - history
  - policy
  - Educational Studies
  - Trinity College
  - Hartford
  - community engagement
  - technology
  - tutorial
  - GitHub
  - data visualization
  - web writing
---
### Link types
- Visible link uses angle brackets <http://google.com>
- [Embedded link: place text in brackets, URL in parentheses](http://google.com)
- But an embedded link to an internal page or post on this site requires the full URL

### Footnote
Write the main text and insert a bracketed footnote symbol with a unique number or keyword.[^keyword] Then somewhere else in the main text, write the same bracketed footnote symbol and number/keyword, followed by a colon, and the footnote text.

[^keyword]: Here's the footnote text.

### Markdown image with pre-slash pathname (no baseurl because custom domain), actual size, but no caption
![Jack Dougherty](/images/2019/dougherty-jack-150x150.jpg)

### [Liquid templating](https://jekyllrb.com/docs/liquid/) image in root no-slash images  
{% include figure image_path="images/sample-300x200.jpg" alt="sample image" caption="here's the sample image" %}

### Liquid image in root no-slash aligned with caption
{% include figure image_path="images/sample-300x200.jpg" alt="sample image" caption="sample caption" %}{: .align-right}
This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images.

### HTML iframe, with quote marks around with and height, whether percentages or pixels
<iframe src="https://jackdougherty.youcanbook.me/" width="100%" height="600px"></iframe>

### Sample YouTube
{% include video id="3sK7-g0otGM" provider="youtube" %}
