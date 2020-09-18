<!--# {{page.title}}-->

All listed times are in your local time zone. Check out <a class="page-link" href="https://app.swapcard.com/event/2020-game-devs-of-color-expo/exhibitors/RXZlbnRWaWV3XzU4OTEz?">the full schedule on Swapcard.

<iframe src="https://app.swapcard.com/widget/event/2020-game-devs-of-color-expo/plannings/RXZlbnRWaWV3XzQ3ODA0?showActions=true" style="border: none; margin: 0px; width: 100%; display: block; height: calc(100vh - 100px);">
</iframe>

<!--

<p align="center"><img src="/assets/images/speakers/2019/speakers_header.jpg"/></p>


All times in EDT
<ul class="list-unstyled">
  {% for talk in site.data.talks %}
  <li class="list-data">
    <div class="list-data-header">
      <span class="list-data-time">{{talk.time}}</span>
      <h2 class="list-data-title">{{talk.title}}</h2>
    </div>
    {% if talk.speakers or talk.description %}
    <div class="list-data-content">
      {% if talk.description %}
      <p class="list-data-description">{{ talk.description }}</p>
      {% endif %}
      {% if talk.speakers %}
      <h3>Speakers:</h3>
      <ul class="list-unstyled col-container">
      {% for speaker in talk.speakers %}
        <li class="{% if speaker.featured == false %}col-3{% else %}col-container{% endif %}">
          <div class="{% if speaker.featured == true %}col-3{% endif %}">
            {% if speaker.photo %}<img src="/assets/images/speakers/2019/{{speaker.photo}}" class="list-data-photo">{% endif %}
          </div>
          <div class="{% if speaker.featured == true %} col-3-2{% endif %}">
            <h4>{{ speaker.name }}</h4>
            {% if speaker.company %}
            <h5 class="list-data-title">{{ speaker.company }}</h5>
            {% endif %}
            <p class="text-smaller">{{speaker.bio}}</p>
          </div>
        </li>
        {% endfor %}
      </ul>
      {% endif %}
    </div>
    {% endif %}
  </li>
  {% endfor %}
</ul>

-->

----

More information is coming soon. Subscribe to hear when we add new games, speakers, and more! We send emails less than once per week.

{% include mailchimp-form.html %}