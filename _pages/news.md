---
 title: "News Overview | DOGE University"
 layout: textlay
 excerpt: "Browse the latest news and updates at DOGE University."
 sitemap: false
 permalink: /news/
---

# Latest News

{% assign sorted_news = site.news | sort: "date" | reverse %}
<ul>
{% for news_item in sorted_news %}
  <li>
    <a href="{{ news_item.url }}">{{ news_item.title }}</a>
    <small>({{ news_item.date | date: "%B %d, %Y" }})</small>
  </li>
{% endfor %}
</ul> 