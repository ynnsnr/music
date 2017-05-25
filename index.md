---
layout: home
---

<div id="banner">
  <h1>Yoann Saunier</h1>
  <h2>Musicien Ingénieur du Son</h2>
  <p>
    Musiques actuelles - Musiques à l'image <br>Identités sonores
  </p>
</div>

<div id="bio" class="centered">
  <h2>Bio</h2>
  <p>
    Musicien, ingénieur du son et compositeur d'origine normande, Yoann Saunier entre au <a href="http://www.conservatoirederouen.fr">Conservatoire à rayonnement régional</a> de Rouen à l’âge de 7 ans pour y pratiquer la guitare classique. Il étudie le son à l’image en classe préparatoire <a href="http://guisthau.paysdelaloire.e-lyco.fr/le-superieur/cine-sup-/">Ciné-Sup</a> au Lycée Guist’hau de Nantes où
    il se forme aux musiques électroniques et à la composition de musiques de films
  </p>
  <p>
    En 2010, il entre au <a href="http://www.conservatoiredeparis.fr">Conservatoire National Supérieur de Musique et de Danse de Paris</a>, se spécialise dans la Musique Assistée par Ordinateur et décroche le diplôme de la <a href="http://www.fsms.fr">Formation Supérieure au Métiers du Son</a>
  </p>
  <p>
    Dorénavant, il collabore avec divers compositeurs de musiques à l’image ou pour le théâtre (<a href="http://edemarsan.free.fr/index_f.htm">Eric Demarsan</a>, <a href="https://www.mariejeanneserero.fr">Marie-Jeanne Serero…</a>), se produit régulièrement sur scène au sein de différents groupes de musiques actuelles (<a href="http://www.kabaretmusic.fr">KAB</a>, <a href="https://www.facebook.com/iammalca">Malca</a>,
    <a href="http://www.meliefraisse.com">Mélie Fraisse…</a>) et réalise parallèlement de nombreux remixes avec son duo <a href="https://soundcloud.com/strassreleases">Strass</a>
  </p>
</div>

<div id="projects" class="centered">
  <h2>Projets</h2>
  {% for project in site.data.projects %}
    <div class="project">
      <div class="picture">
        {% if project.url %}
          <a href="{{ project.url }}">
            <img src="/assets/projects/{{ project.picture }}" alt="{{ project.name }}">
          </a>
        {% else %}
          <img src="/assets/projects/{{ project.picture }}" alt="{{ project.name }}">
        {% endif %}
      </div>
      <div class="infos">
        <h3>
          {{ project.name }}
          {% if project.author %}
            <small>de {{ project.author }}</small>
          {% endif %}
        </h3>
        <h4>{{ project.role }}</h4>

        <p>{{ project.description | markdownify }}</p>
      </div>
    </div>
  {% endfor %}
</div>

<div id="awards" class="centered">
  <h2>Distinctions</h2>

  {% for award in site.data.awards %}
    <div class="project">
      <div class="picture">
        {% if award.url %}
          <a href="{{ award.url }}">
            <img src="/assets/awards/{{ award.picture }}" alt="{{ award.name }}">
          </a>
        {% else %}
          <img src="/assets/awards/{{ award.picture }}" alt="{{ award.name }}">
        {% endif %}
      </div>
      <div class="infos">
        <h3>
          {{ award.name | markdownify }}
        </h3>
        <p>{{ award.description | markdownify }}</p>
      </div>
    </div>
  {% endfor %}
</div>

<div id="contact" class="centered">
  <h2>Contact</h2>

  <p>
    Vous souhaitez travailler avec moi ? Je réponds rapidement par mail 👉 <a href="mailto:yoann@saunier.me">yoann@saunier.me</a>
  </p>
</div>
