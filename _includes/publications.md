<h2 id="publications" style="margin: 2px 0px -15px;">Publications</h2>
<script type='text/javascript' src='https://d1bxh8uas1mnw7.cloudfront.net/assets/embed.js'></script>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.main %}

<li>
  <div class="col-sm-9" style="position: relative;padding-right: 50px;padding-left: 0px;">
      <div class="title"><a href="{{ link.doi }}">{{ link.title }}</a></div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.journal }}</em>
      </div>
    <div class="links">
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.data %} 
      <a href="{{ link.data }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Data</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.altmetric %}
      <div data-badge-popover="right" data-badge-type="2" data-doi="{{ link.altmetric }}" data-hide-no-mentions="true" class="altmetric-embed"></div>
      {% endif %}
      {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
</div>
</li>

{% endfor %}

</ol>
</div>

