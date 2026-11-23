<section id="publications" class="section">
  <h2 class="section-title"><i class="fa-regular fa-file-lines section-icon"></i> Publications &amp; Preprints</h2>
  <div class="pub-list">
    {% for link in site.data.publications.main %}
    <article class="pub-card">
      <div class="pub-thumb">
        {% if link.image %}
        <img src="{{ link.image }}" alt="{{ link.title }}" loading="lazy" />
        {% else %}
        <div class="pub-thumb-placeholder">
          <span>{{ link.conference_short }}</span>
        </div>
        {% endif %}
        {% if link.conference_short %}
        <span class="pub-badge {% if link.status_type == 'published' %}badge-published{% else %}badge-review{% endif %}">
          {{ link.conference_short }}
        </span>
        {% endif %}
      </div>
      <div class="pub-body">
        <h3 class="pub-title">
          {% if link.doi %}
          <a href="{{ link.doi }}" target="_blank" rel="noopener">{{ link.title }}</a>
          {% elsif link.pdf %}
          <a href="{{ link.pdf }}" target="_blank" rel="noopener">{{ link.title }}</a>
          {% else %}
          {{ link.title }}
          {% endif %}
        </h3>
        <div class="pub-authors">{{ link.authors }}</div>
        <div class="pub-venue">{{ link.conference }}</div>
        {% if link.summary %}
        <p class="pub-summary">{{ link.summary }}</p>
        {% endif %}
        <div class="pub-links">
          {% if link.doi %}
          <a class="btn-chip" href="{{ link.doi }}" target="_blank" rel="noopener"><i class="fa-solid fa-link"></i> DOI</a>
          {% endif %}
          {% if link.pdf %}
          <a class="btn-chip" href="{{ link.pdf }}" target="_blank" rel="noopener"><i class="fa-regular fa-file-pdf"></i> PDF</a>
          {% endif %}
          {% if link.code %}
          <a class="btn-chip" href="{{ link.code }}" target="_blank" rel="noopener"><i class="fa-brands fa-github"></i> Code</a>
          {% endif %}
          {% if link.bibtex %}
          <button type="button" class="btn-chip btn-bib" data-target="bib-{{ forloop.index }}">
            <i class="fa-solid fa-quote-right"></i> BibTeX
          </button>
          {% endif %}
        </div>
        {% if link.bibtex %}
        <div id="bib-{{ forloop.index }}" class="bibtex-box" hidden>
          <div class="bibtex-header">
            <span>BibTeX</span>
            <button type="button" class="btn-copy-bib" data-copy-target="bib-code-{{ forloop.index }}">Copy</button>
          </div>
          <pre><code id="bib-code-{{ forloop.index }}">{{ link.bibtex | escape }}</code></pre>
        </div>
        {% endif %}
      </div>
    </article>
    {% endfor %}
  </div>
</section>
