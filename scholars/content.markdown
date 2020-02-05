# {{page.title}}

{% if site.data.scholars.size > 0 %}

<p>
Game Devs of Color Expo is partnering with the Game Developers Conference for the second year! 
</p>
<p>
We're running a scholarship program to bring some amazing creators of color to GDC. GDC can be a career-defining conference, but tickets, travel, and lodging prices can place it out of reach for many developers. 
</p>
<p>
For these amazing scholars we've provided Conference and Summits passes, as well as travel and lodging assistance through our Scholar Program's sponsors!
</p>

<br/>

  <ul class="list-unstyled">
    {% assign sorted_scholars = site.data.scholars | sort:"title" %}
    {% for game in sorted_scholars %}
    <li class="list-data col-container">
      <div class="col-3">
        <a href="{{game.link}}" target="_blank">
          <img src="/assets/images/scholars/2020/{{game.image}}" class="list-data-photo">
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

### We'll be announcing our 2020 GDC Scholars soon. Stay tuned!

{% endif %}

----

## Thanks to our Game Devs of Color Expo GDC Sponsors

<ul class="col-container sponsors-container">


<li class="col-3">
<p>
<br/>
<br/>
<a href="http://www.redhookgames.com/" target="_blank">
<img src="/assets/images/scholars/2020/redhook_logo.png">
<br/>
<br/>
</a>
</p>
</li>

<li class="col-3-2">
<p>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<a href="https://subsetgames.com/" target="_blank">
<img src="/assets/images/scholars/2019/SubsetGames_logo.png">
<br/>
<br/>
</a>
</p>
</li>

</ul>

<ul class="col-container sponsors-container">

<li class="col-3">
<p>
<br/>
<a href="https://maximumcrash.com/" target="_blank">
<img src="/assets/images/scholars/2020/mxmcrash_logo.png">
</a>
</p>
</li>

<li class="col-3">
<p>
<br/>
<a href="https://fullbrig.ht/" target="_blank">
<img src="/assets/images/scholars/2020/fullbright_logo.png">
</a>
</p>
</li>

<li class="col-3">
<p>
<br/>
<a href="http://www.capybaragames.com" target="_blank">
<img src="/assets/images/scholars/2019/CapybaraGames_logo.png">
</a>
</p>
</li>

<li class="col-3">
<p>
<br/>
<br/>
<br/>
<br/>
<br/>
<a href="https://www.supergiantgames.com/" target="_blank">
<img src="/assets/images/scholars/2020/supergiant_logo.png">
</a>
</p>
</li>

<li class="col-3">
<p>
<br/>
<a href="https://www.vlambeer.com/" target="_blank">
<img src="/assets/images/scholars/2020/vlamber_logo.png">
</a>
</p>
</li>

<li class="col-3">
<p>
<a href="http://dreamfeel.org/" target="_blank">
<img src="/assets/images/scholars/2019/dreamfeel_logo.png">
</a>
</p>
</li>
</ul>


----

## Scholarship Committee

<ul class="col-container sponsors-container">
<li class="col-3">
<p>
<img src="/assets/images/scholars/2019/ChrisAlgoo.jpg">
Chris Algoo<br/>
<a href="https://twitter.com/chrisalgoo?lang=en" target="_blank">@ChrisAlgoo</a>
</p>
</li>

<li class="col-3">
<p>
<img src="/assets/images/scholars/2019/ShawnAllen.jpg">
Shawn Allen<br/>
<a href="https://twitter.com/aNuChallenger" target="_blank">@aNuChallenger</a>
</p>
</li>

<li class="col-3">
<p>
<img src="/assets/images/scholars/2019/RachelBazelais.JPG">
Rachél Bazelais<br/>
<a href="https://twitter.com/Popular_Pixels" target="_blank">@Popular_Pixels</a>
</p>
</li>
</ul>

<ul class="col-container sponsors-container">
<li class="col-3">
<p>
<img src="/assets/images/scholars/2019/BrianSChung.jpg">
Brian S. Chung<br/>
<a href="https://twitter.com/BrianSChung" target="_blank">@BrianSChung</a>
</p>
</li>

<li class="col-3">
<p>
<img src="/assets/images/scholars/2019/GJLee.jpg">
GJ Lee<br/>
<a href="https://twitter.com/whereisgj" target="_blank">@whereisgj</a>
</p>
</li>

<li class="col-3">
<p>
<img src="/assets/images/scholars/2019/Emperatriz_Ung.png">
GJ Lee<br/>
<a href="https://twitter.com/mprtrzng" target="_blank">@mprtrzng</a>
</p>
</li>

<li class="col-3">
<p>
<img src="/assets/images/scholars/2019/ReynaldoVargas.JPG">
Reynaldo Vargas<br/>
<a href="https://twitter.com/reymakes" target="_blank">@reymakes</a>
</p>
</li>
</ul>

----

Interesting in applying to our GDC Scholar Program next year? Sign up for our mailing list for news and announcements!

{% include mailchimp-form.html %}