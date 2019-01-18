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
        <a href="{{scholar.link}}" target="_blank">
          <h2 class="list-data-title">{{scholar.title}}</h2>
        </a>
        <h3 class="list-data-title">{{scholar.team}}</h3>
        {% if scholar.description %}
        <p class="list-data-description text-smaller">{{ scholar.description }}</p>
        {% endif %}
      </div>
    </li>
    {% endfor %}
  </ul>
  <br>

{% else %}

### We'll be announcing our 2019 GDC Scholar soon. Stay tuned!

{% endif %}

----

Interesting in applying for our GDC Scholar Program next year? Sign up for our mailing list for news and announcements!

{% include mailchimp-form.html %}