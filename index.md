---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title:
permalink: /
---


<img src="assets/logo.png" alt="Pierce College Logo" style="display: block;margin-left: auto;margin-right: auto;width: 50%;">

**What we are...**

**PierceHacker** provides tutorials and other resources in order to help the **Pierce College** community develop new technical skills and better understand the ways in which technology shapes the work we do both in and out of the classroom. 

*Our motto: Towards a robust and critical information competency!*

# Most Recent Blog Posts

<div id="posts">
  <ul>
    {% for post in site.posts %}
	{% if post.category == "meta" %}
      <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> by <span class="italic">{{ post.author }}</span></li>
	{% endif %}    
{% endfor %}
  </ul>
</div>
