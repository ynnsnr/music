---
layout: home
---

<div id="banner">
  <h1>Yoann Saunier</h1>
  <h2>Musicien Ingénieur du Son</h2>
  <p>
    Musiques actuelles - Musiques à l'image
  </p>
</div>

<div id="bio" class="centered">
  <h2>Bio</h2>
  <p>
    Musicien, ingénieur du son et compositeur français né le 28 Janvier 1990 à Mont-Saint-Aignan (Normandie),
    Yoann Saunier entre au Conservatoire à rayonnement régional de Rouen à l’âge de 7 ans pour y étudier la guitare classique.
  </p>
  <p>
    Durant l’adolescence il découvre la musique rock, monte un groupe et fait ses premiers pas dans l’enregistrement sonore et la
    production musicale. A sa majorité il part étudier le son à l’image en classe préparatoire Ciné-Sup au Lycée Guist’hau de Nantes où
    il se tourne vers les musiques électroniques et la composition de musiques de films.
  </p>
  <p>
    En 2010, il entre au <strong>Conservatoire National Supérieur
    de Musique et de Danse de Paris</strong>, se spécialise dans la Musique Assistée par Ordinateur et décroche cinq ans plus tard le diplôme de
    Formation Supérieure au Métiers du Son.
  </p>
  <p>
    Aujourd’hui, il collabore avec divers compositeurs de musiques à l’image ou pour le
    théâtre (Eric Demarsan, Marie-Jeanne Serero…), se produit régulièrement sur scène au sein de différents groupes de musiques
    actuelles (<a href="http://www.kabaretmusic.fr/">KAB</a>, <a href="https://www.facebook.com/iammalca/">Malca</a>,
    Mélie Fraisse…) et réalise parallèlement de nombreux remixes avec son duo de DJ, Strass.
  </p>
</div>

<div id="projects" class="centered">
  <h2>Projets</h2>
  {% for project in site.data.projects %}
    <div class="project">
      <div class="picture">
        <img src="/assets/projects/{{ project.picture}}" alt="{{ project.name }}">
      </div>
      <div class="infos">
        <h3>{{ project.name }} <small>de {{ project.author }}</small></h3>
        <h4>{{ project.role }}</h4>

        <p>{{ project.description | markdownify }}</p>
      </div>
    </div>
  {% endfor %}
</div>
