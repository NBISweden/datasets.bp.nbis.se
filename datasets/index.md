---
title: "Bigpicture Datasets"
description: "Information on datasets shared on the Bigpicture"
---


Suspendisse ullamcorper dolor ultrices purus lobortis dignissim. Ut in purus vestibulum, egestas tortor eu, ullamcorper nulla. Nunc nunc mi, faucibus ut faucibus et, tincidunt et velit. Ut porta enim ut erat tincidunt vestibulum. Nunc in erat a nulla placerat dignissim. Suspendisse scelerisque sapien at lacinia feugiat. Quisque id maximus ipsum. Nam commodo nisl nunc, eu fermentum arcu varius et. Suspendisse in tempor nibh.

Pellentesque fringilla vehicula justo, ut tincidunt turpis ultricies id. Aliquam quis ex egestas, egestas diam ac, malesuada dui. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Vivamus nunc metus, placerat eu pellentesque ut, rhoncus vitae eros. Etiam dignissim metus urna, a vehicula odio gravida venenatis. Aenean non ante et justo consequat vehicula. Nulla porta faucibus turpis, sed viverra purus molestie vel. Proin at egestas felis, quis bibendum ante. Nulla ut lacinia leo. Etiam sit amet quam nec lorem porta lacinia. Nunc efficitur turpis purus, ac iaculis mauris vulputate eget. Maecenas arcu lectus, tristique vitae porta a, euismod at felis.


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
