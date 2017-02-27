# {{page.title}}

<ul class="list-unstyled">
  {% for talk in site.data.talks %}
  <li>
    <h2>{{talk.time}} - {{talk.title}}</h2>
  {% if talk.speakers || talk.description%}
    <p>
    {% if talk.speakers %}
      <strong> Speakers: {{ talk.speakers | array_to_sentence_string }}</strong>
    {% endif %}
      <br>
    {% if talk.description %}
      {{ talk.description }}
    {% endif %}
    </p>
    {% endif %}
  </li>
{% endfor %}
</ul>

----

More information is coming soon. Subscribe to hear when we add new games, speakers, and more! We send emails less than once per week.

{% include mailchimp-form.html %}