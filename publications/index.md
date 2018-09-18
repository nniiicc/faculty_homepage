---
layout: default
section: publications
title: "Publications"
---

# Publications

You can find open access links to all of my articles at:
- [Google Scholar](https://scholar.google.com/citations?user=XOjXz98AAAAJ&hl=en)
- [DBLP](http://dblp.uni-trier.de/pers/hd/w/Weber:Nicholas_M=)    

%Need a conditional statement here that does not print year if no publications... And figure out a way to space pubcs...

{% for year in (2002..2018) reversed %}
<h2>{{ year }}</h2>
{% bibliography --query @*[year = {{year}}] %}
<br>
{% endfor %}
