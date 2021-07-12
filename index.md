---
stories:
- Story 1: before_ashlar
---

# Minerva Stories

{% for story_hash in page.stories %}
    {% for story in story_hash %}
- [{{ story[0] }}]({{ site.baseurl }}/{{ story[1] }})
    {% endfor %}
{% endfor %}
