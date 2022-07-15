---
layout: blank
title: "Entrepreneurship In Web3"
permalink: /f22_speakers
---

<table style="table-layout: fixed; font-size: 88%">
  <thead>
      <th style="width: 30%;"> Speaker </th>
      <th style="width: 70%;"> Brief Bio </th>
  </thead>
  <tbody>
    {% for row in site.data.f22_speakers %}
      <tr>
        {% if row.picture %}
          <td style="text-align:center"><img style="object-fit:cover" width=200 height=200 src="{{site.baseurl}}/assets/speakers/{{ row.picture }}" alt={{ row.name }}> 
          <br>
          <b>{{ row.name }}</b> </td>
        {% else %} 
          <td> <b>{{ row.name }}</b> </td>      
        {% endif %}
        <td> {{ row.bio }} </td>
      </tr>
    {% endfor %}
  </tbody>
</table>
