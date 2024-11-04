---
# This is the front matter for the news layout
layout: default  # You can set this to another layout if you have one
---

# {{ page.title }}  # Display the title of the news article

**Published on:** {{ page.date | date: "%B %d, %Y" }}

{{ content }}  # This renders the main content of the article
