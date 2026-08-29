<h2 id="publications">Publications</h2>

<div class="publications">
  <ol class="bibliography">
    {% for publication in site.data.publications.main %}
    <li class="publication-item">
      <span class="venue-badge">{{ publication.conference_short }}</span>
      <div class="publication-title">
        <a href="{{ publication.paper }}">{{ publication.title }}</a>
      </div>
      <div class="publication-authors">{{ publication.authors }}</div>
      <div class="publication-venue"><em>{{ publication.conference }}</em></div>
      <div class="publication-links">
        <a href="{{ publication.paper }}">Paper</a>
        <a href="{{ publication.code }}">Code</a>
      </div>
      <div class="publication-note">{{ publication.note }}</div>
    </li>
    {% endfor %}
  </ol>
</div>
