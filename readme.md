# HM Taxonomy Filter
## A Wordpress Plugin to filter posts by multiple taxonomies and terms

With HM Taxonomy Filter you can filter any of Wordpress' archive page in by terms of multiple [custom taxonomies](http://codex.wordpress.org/Taxonomies/). 

### Usage

Filter posts by appending a filter slug to the archive's permalink:

`http://example.com/{archive}/filter/{taxonomy-a}:{term-a1}+{term-a2},{taxonomy-b}:{term-b3}+{term-b4}`

filters *archive* by terms **A1** and **A2** from taxonomy **A** and terms **B3** and **B4** from taxonomy **B**.

### Template tags

`<?php hm_taxonomyfilter_navigation(); ?>` shows an hierarchical list of all custom taxonomies and their terms. 
Clicking on a term adds it to the current filter, clicking on terms already used removes them from the current filter.

`<?php hm_taxonomyfilter_status(); ?>` shows only the currently used taxonomies and terms.

**The plugin renders only plain markup, it's up to you to style it up!**