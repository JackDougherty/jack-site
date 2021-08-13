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
### Markdown formatting
Text after header appears in new line.  
At the end of the line above, add two blank spaces to make next sentence appear on a new line.

### Link types
- Visible link uses angle brackets <http://google.com>
- [Embedded link: place text in brackets, URL in parentheses](http://google.com)
- But an embedded link to an internal page or post on this site requires the full URL

### Footnote
Write the main text and insert a bracketed footnote symbol with a unique number or keyword.[^keyword] Then somewhere else in the main text, write the same bracketed footnote symbol and number/keyword, followed by a colon, and the footnote text.

[^keyword]: Here's the footnote text.

### Markdown image: actual-size, no-caption, pre-slash pathname (no baseurl because custom domain)
![Jack Dougherty](/images/2019/dougherty-jack-150x150.jpg)

### Liquid image: actual size, caption, no slash  
{% include figure image_path="images/sample-300x200.jpg" alt="sample image" caption="here's the sample image" %}

### Liquid image aligned with caption, actual size, no slash
{% include figure image_path="images/sample-300x200.jpg" alt="sample image" caption="sample caption" %}{: .align-right}
This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images. This sample text demonstrates the wrap-around feature with aligned images.

Read more about [Liquid templating](https://jekyllrb.com/docs/liquid/)

### HTML iframe, with quote marks around with and height, whether percentages or pixels
<iframe src="https://jackdougherty.youcanbook.me/" width="100%" height="600px"></iframe>

### Sample YouTube
{% include video id="3sK7-g0otGM" provider="youtube" %}

### Kaltura video special embed code for iframe
<iframe src="https://cdnapisec.kaltura.com/p/2366381/sp/236638100/embedIframeJs/uiconf_id/42684261/partner_id/2366381?iframeembed=true&playerId=kplayer&entry_id=1_aq660eab&flashvars[streamerType]=auto"  allowfullscreen webkitallowfullscreen mozAllowFullScreen allow="autoplay *; fullscreen *; encrypted-media *" frameborder="0"></iframe>

Note: Removed `width="560" height="395"` from the iframe tag, which defaults to smaller frame that displays nicely on small screens and can be expanded on large screens.
