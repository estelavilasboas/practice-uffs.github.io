---
layout: hero
title: "Pessoas"
permalink: /pessoas/
---

<div class="row align-items-center pt-2 pt-lg-5">
    <div class="col-md-7">
        <h2>Pessoas</h2>
        <p class="lead">
          O Programa de Inovação Practice é formado por 2 Coordenadores Gerais, 2 Coordenadores Tecnicos Pedagógicos,
          3 Produtores de Software e 9 Produtores de Conteúdo.
        </p>
    </div>

    <div class="col-md-1"></div>

    <div class="col-md-4">
        <p><img alt="image" class="img-fluid" src="https://cdn.jsdelivr.net/gh/froala/design-blocks@2.0.1/dist/imgs/draws/tabs.svg"></p>
    </div>
</div>

<section class="fdb-block team-8">
  <div class="container">
    <div class="row-50"></div>
    <div class="row"><div class="col-12"><h2>Coordenação Geral</h2><hr /></div></div>

    <div class="row text-left">
      {% assign coordenacao_geral = site.data.people | where:"position","coordenação geral" | sort:"name" %}
      {% for person in coordenacao_geral %}
        {% include person-grid.html %}
      {% endfor %}
    </div>

    <div class="row-70"></div>
    <div class="row"><div class="col-12"><h2>Coordenação Técnico Pedagógica</h2><hr /></div></div>

    <div class="row">
      {% assign cordenacao_pedagogica = site.data.people | where:"position","coordenação técnico pedagógica" | sort:"name" %}
      {% for person in cordenacao_pedagogica %}
        {% include person-grid.html %}
      {% endfor %}
    </div>

    <div class="row-70"></div>
    <div class="row"><div class="col-12"><h2>Produção de Software</h2><hr /></div></div>

    <div class="row">
      {% assign producao_software = site.data.people | where:"position","produção de software" | sort:"name" %}
      {% for person in producao_software %}
        {% include person-grid.html %}
      {% endfor %}
    </div>

    <div class="row-70"></div>
    <div class="row"><div class="col-12"><h2>Produção de Conteúdo</h2><hr /></div></div>

    <div class="row">
      {% assign producao_conteudo = site.data.people | where:"position","produção de conteúdo" | sort:"name" %}
      {% for person in producao_conteudo  %}
        {% include person-grid.html %}
      {% endfor %}
    </div>
  </div>
  </section>