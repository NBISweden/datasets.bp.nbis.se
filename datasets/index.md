---
title: "Bigpicture Datasets"
description: "Information on datasets shared on the Bigpicture"
---

Suspendisse potenti. Curabitur quis finibus quam. Morbi sagittis purus leo, vitae rhoncus risus interdum a. Maecenas quis erat nec dolor condimentum facilisis eu sit amet felis. Proin convallis semper pulvinar. In hac habitasse platea dictumst. Sed quis sollicitudin massa. Nam sollicitudin arcu ac leo tincidunt interdum. 

## Datasets on Bigpicture

<div class="dataset-table">
  <table>
    {% for d in site.datasets %}
      {% if d.hidden %}{% continue  %}{% endif %}
      <tr>
        <td><a href="{{site.baseurl}}{{ d.url }}"><img src="{{site.baseurl}}{{ d.other.image | default: d.other.exampleImage[0].thumbnail-url | default: d.other.exampleImage[0].url }}"></a></td>
        <td>
          <a href="{{site.baseurl}}{{ d.url }}">{{ d.datacite.name }}</a><br/>
          <span class="keywords">Keywords: {{ d.datacite.keywords }}.</span><br/>
          <a href="{{ d.datacite["@id"] }}" class="doi">doi:{{ d.datacite["@id"] | remove: "https://doi.org/" }}</a>
        </td>
        <td>{{ d.datacite.datePublished | date: "%Y" }}</td>
      </tr>
    {% endfor %}
  </table>
</div>
