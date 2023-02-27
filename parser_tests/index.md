---
title: "Bigpicture Datasets using YAML parser"
description: "YAML parser datasets"
---

Suspendisse potenti. Curabitur quis finibus quam. Morbi sagittis purus leo, vitae rhoncus risus interdum a. Maecenas quis erat nec dolor condimentum facilisis eu sit amet felis. Proin convallis semper pulvinar. In hac habitasse platea dictumst. Sed quis sollicitudin massa. Nam sollicitudin arcu ac leo tincidunt interdum. 

## Datasets on Bigpicture using YAML parser

<div class="dataset-table">
  <table>
    {% for d in site.parserdatasets %}
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
