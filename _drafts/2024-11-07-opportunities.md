---
title: 'Sample Post'
date: 2019-01-01
last_modified_at: 2024-01-01
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
## Markdown formatting with Minimal Mistakes Jekyll theme
Text after header appears in new line.  
At the end of the line above, add two blank spaces to make next sentence appear on a new line.


'm interested in talking with students who might be a good match for any of these opportunities. Some are definite, while others are pending funding:

1) Research Assistant to help and Trinity Library staff to prepare existing digital history resources (oral interview recordings and transcripts; video recordings; scanned maps and documents) collected for my OnTheLine.trincoll.edu book to be uploaded to the [OnTheLine section of the CT Digital Archive](https://collections.ctdigitalarchive.org/node/307586)
Must be detail-oriented student, preferably with interest in 20th-century history of education, housing, and Hartford's city-suburb region.
J-term 2025: part-time remote work around 10 hours/week for around $16/hour, with possibility to continue in person during Spring 2025

2) Teaching Assistant for Educ 206: Data Visualization for All to facilitate student learning during class and also regular office hours outside of class
Must have successfully completed course, preferably a student who had to work at learning the material, to better coach other students for whom the content does not come naturally.
Fall 2025 (tentatively MW 11:30-12:45am) and/or Spring 2026 (tentatively same class time)
Either earn 1 co-curricular credit or earn around $16/hour for 3-4 hours/week

Lists:  
- Visible link uses angle brackets <https://www.fabriziomusacchio.com/blog/2021-08-11-Minimal_Mistakes_Cheat_Sheet/#via-markdown>
- [Embedded link text in brackets, URL in parentheses](http://google.com)
- Note that embedded links to internal pages or posts on this site require the full URL <https://jackdougherty.org/...>

- Single tic marks for short one-line `code` snippets
- Use 3 tics and add 4 spaces after each line for multi-line code snippets, like this reminder about code manually added to `assets > css > main.scss`:
```
.feature__wrapper {    
    margin-bottom: 0;    
    border-bottom: 0;    
}    
```

## Images
Maximum 1000px original image width, or resize with css styling. Use JPG or PNG at any resolution.

### No caption: Markdown formatted (slash prefix pathname) at full size
![sample](/images/sample-300x200.jpg)

### No caption with text wrap: Markdown image with kramdown alignment and 25% sizing
![sample](/images/sample-300x200.jpg){: .align-right style="width: 25%;"} Insert one space then text wrap with Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

### With centered caption: Liquid formatted (no slash prefix pathname) with kramdown at full size
{% include figure image_path="images/sample-1000x600.jpg" alt="sample image" caption="here's the caption with markdown-flavored [link](https://handsondataviz.org)" %}{: .align-center}

### With centered caption: Liquid formatted with kramdown and css styling at 50% size
{% include figure image_path="images/sample-1000x600.jpg" alt="sample image" caption="here's the caption with markdown-flavored [link](https://handsondataviz.org)" %}{: .align-center style="width:50%;"}

See more details <https://www.fabriziomusacchio.com/blog/2021-08-11-Minimal_Mistakes_Cheat_Sheet>


### HTML iframe, with quote marks for width and height, whether percentages or pixels
<iframe src="https://jackdougherty.youcanbook.me/" width="100%" height="600px"></iframe>

### YouTube with Liquid formatting
{% include video id="3sK7-g0otGM" provider="youtube" %}

### Kaltura video special embed code for iframe
<iframe src="https://cdnapisec.kaltura.com/p/2366381/sp/236638100/embedIframeJs/uiconf_id/42684261/partner_id/2366381?iframeembed=true&playerId=kplayer&entry_id=1_aq660eab&flashvars[streamerType]=auto"  allowfullscreen webkitallowfullscreen mozAllowFullScreen allow="autoplay *; fullscreen *; encrypted-media *" frameborder="0"></iframe>

Note: Removed `width="560" height="395"` from the iframe tag, which defaults to smaller frame that displays nicely on small screens and can be expanded on large screens.
