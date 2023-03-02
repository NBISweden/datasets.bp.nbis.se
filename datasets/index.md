---
title: "Bigpicture Datasets"
description: "Information on datasets shared on the Bigpicture"
---

This is a prototype website for Dataset description pages / DOI landing pages for Bigpicture.

This website is openly accessible to Everyone on the Internet, because the purpose of Dataset description pages / DOI landing pages is to be accessible to anyone on the Internet.

The reason for Dataset description pages / DOI landing pages to be openly accessible to anyone on the Internet, is so that a potential user can learn 
1) that a dataset exists, 2) how it can be used, 3) why they should bother applying for access, and 3) how to apply for access.

This website was set up on instruction from wp3 (data contributor) leadership, with a starting point in the AIDA Data Hub Dataset register format, in order to iterate toward a suitable format for Dataset description pages / DOI landing pages in Bigpicture, in dialogue with the reference group consisting of data contributor representatives, which is authorized by the managing board to make decisions for this prototype. This will happen in two-week feedback iterations. When the reference group is happy with the format, it will be submitted to the managing board for approval for integration into the Bigpicture metadata standard. 

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
