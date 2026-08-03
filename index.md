## About Me

Hi I'm Iptcyq. I code, make games and engineer random stuff on my laptop. 

I just made this site because it's the middle of exam season and I'm bored (and distracted).
Which is also why it's incomplete... I'll get back to updating this eventually?

---
## Project Log

From newest to oldest. Pages in `pages/` with `home_post: true` are listed here automatically.

{% assign posts = site.pages | where: "home_post", true | sort: "date" | reverse %}
{% for post in posts %}
### {{ post.title }}

[<kbd> <br> Read post <br> </kbd>]({{ post.url | relative_url }})
{% if post.badge %}[<kbd> <br> [{{ post.badge }}] <br> </kbd>]({{ post.external_url }}){% endif %}

{{ post.summary }}

{% if post.thumbnail %}<img src="{{ post.thumbnail }}"/>{% endif %}

---
{% endfor %}

## Work In Progress

{% assign wip_posts = site.data.home_posts.wip | sort: "date" | reverse %}
{% for post in wip_posts %}
### {{ post.title }}

{% if post.page_url %}[<kbd> <br> Read post <br> </kbd>]({{ post.page_url | relative_url }}){% endif %}
{% if post.badge and post.external_url %}[<kbd> <br> [{{ post.badge }}] <br> </kbd>]({{ post.external_url }}){% endif %}
{% if post.external_url and post.badge == nil %}[<kbd> <br> {{ post.external_label | default: "External link" }} <br> </kbd>]({{ post.external_url }}){% endif %}

{{ post.summary }}

{% if post.thumbnail %}<img src="{{ post.thumbnail }}"/>{% endif %}
{% if post.thumbnail_2 %}<img src="{{ post.thumbnail_2 }}"/>{% endif %}
{% if post.video %}<video width="320" height="240" controls><source src="{{ post.video }}" type="video/mp4">Your browser does not support the video tag.</video>{% endif %}

---
{% endfor %}

---

## Archive (Maybe Continue Later)

{% assign archive_posts = site.data.home_posts.archive | sort: "date" | reverse %}
{% for post in archive_posts %}
### {{ post.title }}

{% if post.page_url %}[<kbd> <br> Read post <br> </kbd>]({{ post.page_url | relative_url }}){% endif %}
{% if post.badge and post.external_url %}[<kbd> <br> [{{ post.badge }}] <br> </kbd>]({{ post.external_url }}){% endif %}
{% if post.external_url and post.badge == nil %}[<kbd> <br> {{ post.external_label | default: "External link" }} <br> </kbd>]({{ post.external_url }}){% endif %}

{{ post.summary }}

{% if post.thumbnail %}<img src="{{ post.thumbnail }}"/>{% endif %}
{% if post.thumbnail_2 %}<img src="{{ post.thumbnail_2 }}"/>{% endif %}
{% if post.video %}<video width="320" height="240" controls><source src="{{ post.video }}" type="video/mp4">Your browser does not support the video tag.</video>{% endif %}

---
{% endfor %}


---
<p style="font-size:11px"> Last updated in Early March 2026 </p>

<!-- Credits: -->
<!-- <p style="font-size:11px">Page template forked from <a href="https://github.com/evanca/quick-portfolio">evanca</a></p> -->
