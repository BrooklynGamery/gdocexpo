# {{page.title}}

{% if site.data.games.size > 0 %}

Our arcade will host a variety of games from around the world. Below are {{site.data.games.size}} of the confirmed games you will be able to play when you attend the expo. More games are still being announced!


  <ul class="list-unstyled">
    {% assign sorted_games = site.data.games | sort:"title" %}
    {% for game in sorted_games %}
    <li class="list-data col-container">
      <div class="col-3">
        <a href="{{game.link}}" target="_blank">
          <img src="/assets/images/games/2018/{{game.image}}" class="list-data-photo">
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

### Stay tuned for updates soon!

{% endif %}
<!--
# Vendor tables

We will have tables available for companies that are interested hiring game developers of color and/or sharing their products with our unique demographic. Contact us at gdocexpo@gmail.com to learn more about pricing.

Want to do more? [Sponsor the event.](/sponsor)

{% if site.data.booths.size > 0 %}
  <ul class="list-unstyled">
    {% assign sorted_booths = site.data.booths | sort:"name" %}
    {% for booth in sorted_booths %}
    <li class="list-data col-container">
      <div class="col-3">
        <a href="{{booth.link}}" target="_blank">
          <img src="/assets/images/sponsors/2018/{{booth.image}}" class="list-data-photo">
        </a>
      </div>
      <div class="col-3-2">
        <a href="{{booth.link}}" target="_blank">
          <h2 class="list-data-title">{{booth.name}}</h2>
        </a>
        {% if booth.description %}
        <p class="list-data-description text-smaller">{{ booth.description }}</p>
        {% endif %}
      </div>
    </li>
    {% endfor %}
  </ul>
 
{% endif %}
-->
----

More information is coming soon. Subscribe to hear when we add new games, speakers, and more! We send emails less than once per week.

{% include mailchimp-form.html %}