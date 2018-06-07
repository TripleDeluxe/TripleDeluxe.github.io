---
layout: default
title: L'équipe
permalink: /Lequipe/
---
<link rel="stylesheet" href="/assets/css/Lequipe.css">

<ul>
    <h1>Présentation de la Team Rocket</h1>
    {% for membre in site.data.membres %}
    <hr />
    <li>
        <h2>{{membre.firstname}} {{membre.lastname}}</h2>
        <div><img src="/assets/img/membres/{{membre.img}}" alt="photo d'un des membres de l'équipe" class="img-membre"/></div>
        <p class="descr-membre">{{membre.descr}}</p>
    </li>
    {% endfor %}
</ul>