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
      {% if talk.description %}
      <p class="list-data-description">{{ talk.description }}</p>
      {% endif %}
      {% if talk.speakers %}
      <h3>Speakers:</h3>
      <ul class="list-unstyled col-container">
      {% for speaker in talk.speakers %}
        <li class="col-3">
          <img src="/assets/images/speakers/2017/{{speaker.photo}}" class="list-data-photo">
          <h4>{{ speaker.name }}</h4>
          <p class="text-smaller">{{speaker.bio}}</p>
        </li>
        {% endfor %}
      </ul>
      {% endif %}
    </div>
    {% endif %}
  </li>
  {% endfor %}
</ul>

----

More information is coming soon. Subscribe to hear when we add new games, speakers, and more! We send emails less than once per week.

{% include mailchimp-form.html %}