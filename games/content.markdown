# {{page.title}}

Our arcade will host a variety of games from around the world. Below are {{site.data.games.size}} of the confirmed games you will be able to play when you attend the expo.

<ul class="list-unstyled">
  {% assign sorted_games = site.data.games | sort:"title" %}
  {% for game in sorted_games %}
  <li class="list-data col-container">
    <div class="col-3">
      <a href="{{game.link}}" target="_blank">
        <img src="/assets/images/games/2017/{{game.image}}" class="list-data-photo">
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

# Vendor tables

Although we are no longer accepting games to showcase, we do have tables available for companies that are interested hiring game developers of color and/or sharing their products with our unique demographic. Contact us at gdocexpo@gmail.com to learn more about pricing.

Want to do more? [Sponsor the event.](/sponsor)

<ul class="list-unstyled">
  {% assign sorted_booths = site.data.booths | sort:"name" %}
  {% for booth in sorted_booths %}
  <li class="list-data col-container">
    <div class="col-3">
      <a href="{{booth.link}}" target="_blank">
        <img src="/assets/images/sponsors/2017/{{booth.image}}" class="list-data-photo">
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

----

More information is coming soon. Subscribe to hear when we add new games, speakers, and more! We send emails less than once per week.

{% include mailchimp-form.html %}