# Liedtexte

Liedtexte zum mitsingen in der Kinderkirche und auf öffentlichen Veranstaltungen in Breitenberg.

# Kategorien

{% assign sorted_site_categories = site.categories | sort %}
{% for category in sorted_site_categories %}
{% capture category_name %}{{ category | first }}{% endcapture %}
## {{ category_name }}
<ul>
{% for post in site.categories[category_name] %}
<li><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></li>
{% endfor %}
</ul>
{% endfor %}

[https://liedtexte.breitenberger-kinderkirche.de/](https://liedtexte.breitenberger-kinderkirche.de/)
