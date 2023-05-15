---
title: "Bigpicture Datasets using YAML parser"
description: "YAML parser datasets"
---

The following datasets are the pilot clinical datasets uploaded to the Big picture archive.

## Clinical datasets uploaded to Big picture archive

<div class="dataset-table">
  <table>
    {% for d in site.clinicaldatasets %}
      {% if d.hidden %}{% continue  %}{% endif %}
      <tr>
        <td><a href="{{site.baseurl}}{{ d.url }}"><img src="{{site.baseurl}}{{ d.image | default: d.exampleImage[0].thumbnail-url | default: dexampleImage[0].url }}"></a></td>
        <td>
          <a href="{{site.baseurl}}{{ d.url }}">{{ d.name }}</a><br/>
          </td>
        <td>{{ d.datacite.datePublished | date: "%Y" }}</td>
      </tr>
    {% endfor %}
  </table>
</div>
