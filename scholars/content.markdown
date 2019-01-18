# {{page.title}}

{% if site.data.scholars.size > 0 %}

Blurb about scholars.


  <ul class="list-unstyled">
    {% assign sorted_scholars = site.data.scholars | sort:"title" %}
    {% for game in sorted_scholars %}
    <li class="list-data col-container">
      <div class="col-3">
        <a href="{{game.link}}" target="_blank">
          <img src="/assets/images/scholars/2019/{{game.image}}" class="list-data-photo">
        </a>
      </div>
      <div class="col-3-2">
        <a href="{{game.link}}" target="_blank">
          <h2 class="list-data-title">{{game.title}}</h2>
        </a>
        <h3 class="list-data-title">{{game.team}}</h3>
        {% if game.description %}
        <p class="list-data-description text-smaller">{{ game.description }}</p>
        {% endif %}
      </div>
    </li>
    {% endfor %}
  </ul>
  <br>

{% else %}

### We'll be announcing our 2019 GDC Scholars soon. Stay tuned!

{% endif %}

----

### Sponsor info

----

Interesting in applying for our GDC Scholar Program next year? Sign up for our mailing list for news and announcements!

{% include mailchimp-form.html %}

