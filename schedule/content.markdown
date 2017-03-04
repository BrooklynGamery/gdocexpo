# {{page.title}}

The event will be held on June 24, 2017 at the historic Schomburg Center in New York City. All panels, talks, educational sessions, and an arcade will feature game players and developers of color.

<ul class="list-unstyled">
  {% for talk in site.data.talks %}
  <li class="list-data">
    <div class="list-data-header">
      <span class="list-data-time">{{talk.time}}</span>
      <h2 class="list-data-title">{{talk.title}}</h2>
    </div>
    {% if talk.speakers || talk.description %}
      <div class="list-data-content">
      {% if talk.speakers %}
        <p class="list-data-attribution">{{ talk.speakers | array_to_sentence_string }}</p>
      {% endif %}
      {% if talk.description %}
        <p class="list-data-description">{{ talk.description }}</p>
      {% endif %}
      </div>
    {% endif %}
  </li>
{% endfor %}
</ul>

----

More information is coming soon. Subscribe to hear when we add new games, speakers, and more! We send emails less than once per week.

{% include mailchimp-form.html %}