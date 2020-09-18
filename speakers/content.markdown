<!-- # {{page.title}}-->

<iframe src="https://app.swapcard.com/widget/event/2020-game-devs-of-color-expo/speakers?showActions=true" style="border: none; margin: 0px; width: 100%; display: block; height: calc(100vh - 100px);"></iframe>

<!--<img src="/assets/images/speakers/2019/speakers_header.jpg"/>

All times in EST
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

Stay in the loop. Subscribe to hear updates about our annual event! We usually send emails less than once per week. Emails are infrequent.

{% include mailchimp-form.html %}