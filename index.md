---
layout: homepage
---

<section id="hero" class="hero-section">
  <div class="hero-avatar">
    <img src="{{ site.avatar }}" alt="{{ site.title }}" />
  </div>
  <div class="hero-info">
    <h1 class="hero-name">
      {{ site.title }}<span class="hero-name-zh">{{ site.chinese_name }}</span>
    </h1>
    <div class="hero-bio">
      <p>
        I am currently an undergraduate student in the YSL Class at Hefei University of Technology (HFUT) (Sep. 2023 – Jul. 2027),
        where I work as a Research Assistant advised by
        <a href="https://faculty.hfut.edu.cn/~Azauye/zh_CN/index.htm" target="_blank" rel="noopener">Prof. Qiang Zhang</a>
        and Prof. Yanjiu Zhong, and collaborate remotely with
        <a href="https://wangxuhongcn.github.io/" target="_blank" rel="noopener">Dr. Xuhong Wang</a>
        at the Shanghai Artificial Intelligence Laboratory.
      </p>
      <p>
        Starting from July 2026, I have also been a Research Assistant at the PEAK Lab, The Hong Kong University of Science and Technology (Guangzhou),
        supervised by <a href="https://changhao-chen.github.io/" target="_blank" rel="noopener">Dr. Changhao Chen</a>.
      </p>
    </div>
    <div class="hero-links">
      {% if site.google_scholar %}
      <a class="social-pill" href="{{ site.google_scholar }}" target="_blank" rel="noopener">
        <i class="ai ai-google-scholar"></i> Google Scholar
      </a>
      {% endif %}
      {% if site.orcid %}
      <a class="social-pill" href="{{ site.orcid }}" target="_blank" rel="noopener">
        <i class="fa-brands fa-orcid"></i> ORCID
      </a>
      {% endif %}
      {% if site.github_link %}
      <a class="social-pill" href="{{ site.github_link }}" target="_blank" rel="noopener">
        <i class="fa-brands fa-github"></i> GitHub
      </a>
      {% endif %}
      {% if site.email %}
      <a class="social-pill" href="mailto:{{ site.email }}">
        <i class="fa-regular fa-envelope"></i> Email
      </a>
      {% endif %}
      {% if site.cv_link %}
      <a class="social-pill" href="{{ site.cv_link }}" target="_blank" rel="noopener">
        <i class="ai ai-cv"></i> CV (PDF)
      </a>
      {% endif %}
    </div>
  </div>
</section>

<section id="about" class="section">
  <h2 class="section-title"><i class="fa-regular fa-user section-icon"></i> About Me</h2>
  <p class="about-core-question">
    My research focuses on <strong>world models</strong> for <strong>generalist, self-improving agents</strong>. Broadly, I am interested in how an agent can <span class="highlight-phrase">learn what matters from what comes after</span>: whether acting in the physical world or updating itself, what an action means becomes clear only through what follows it.
  </p>
  <p class="about-intro">
    More recently, I have been focusing on two threads:
  </p>
  <ul class="about-threads">
    <li>
      <strong>Action Representation &amp; Generation:</strong> Developing robust visual representations and lightweight manipulation policies for reliable, cross-embodiment robotic control.
    </li>
    <li>
      <strong>Recursive Self-Improvement (RSI):</strong> Making better use of accumulated experience across learning rounds, and building standardized testbeds, toolkits, and datasets to enable foresight-driven self-modification.
    </li>
  </ul>
  <div class="callout-list">
    <div class="callout-item">
      <span class="callout-emoji">🤝</span>
      <span>Feel free to reach out via <a href="mailto:{{ site.email }}">Email</a> if you are interested in collaborating on my research!</span>
    </div>
    <div class="callout-item">
      <span class="callout-emoji">🔎</span>
      <span>I am actively looking for <strong>MPhil / Ph.D.</strong> or <strong>Research Assistant (RA)</strong> opportunities.</span>
    </div>
  </div>
</section>

<section id="news" class="section">
  <h2 class="section-title"><i class="fa-regular fa-newspaper section-icon"></i> News</h2>
  <div class="news-list">
    <div class="news-item">
      <span class="news-date">Oct. 2026</span>
      <span class="news-text">Our Chinese invention patent (first inventor) was <strong>granted</strong>!</span>
    </div>
    <div class="news-item">
      <span class="news-date">Jul. 2026</span>
      <span class="news-text">Joined the <strong>PEAK Lab</strong> at HKUST(GZ) as a Research Assistant.</span>
    </div>
    <div class="news-item">
      <span class="news-date">Jun. 2026</span>
      <span class="news-text">Our paper <strong>DRIFT</strong> was published in <em>Expert Systems with Applications</em>.</span>
    </div>
    <div class="news-item">
      <span class="news-date">Nov. 2025</span>
      <span class="news-text">Received <strong>First Prize</strong> in the 19th “Challenge Cup” National College Students’ Extracurricular Academic Science and Technology Works Competition.</span>
    </div>
    <div class="news-item">
      <span class="news-date">Jun. 2025</span>
      <span class="news-text">Selected for the <strong>2025 Excellence Program</strong> of the National College Student Innovation and Entrepreneurship Training Program.</span>
    </div>
  </div>
</section>

{% include publications.md %}

<section id="projects" class="section">
  <h2 class="section-title"><i class="fa-solid fa-gears section-icon"></i> Selected Projects</h2>
  <div class="card-grid">
    <article class="info-card">
      <div class="info-card-header">
        <h3 class="info-card-title">Continual Growth Mechanisms for Space Embodied-Intelligence Robots</h3>
        <span class="info-card-meta">Sep. 2025 – Sep. 2026</span>
      </div>
      <div class="info-card-subtitle">Core Member · CASC Fifth Academy Project</div>
      <p>
        Contributed to continually adaptive lunar-construction robots by developing an Isaac Sim–MuJoCo simulation platform, multimodal task and failure data pipelines, and algorithms for coordinated updates to robot structure, control policies, and task knowledge.
      </p>
    </article>

    <article class="info-card">
      <div class="info-card-header">
        <h3 class="info-card-title">Heterogeneous Multi-Robot Decision System</h3>
        <span class="info-card-meta">May 2025 – May 2026</span>
      </div>
      <div class="info-card-subtitle">Team Lead · Invention Patent Granted (1st Inventor) &amp; Software Copyright Filed</div>
      <p>
        Led a heterogeneous multi-robot decision pipeline in which an LLM interpreted multimodal observations and assigned tasks by robot capability, followed by path planning, execution, and closed-loop feedback.
      </p>
    </article>
  </div>
</section>

<section id="honors" class="section">
  <h2 class="section-title"><i class="fa-solid fa-award section-icon"></i> Honors &amp; Awards</h2>
  <ul class="honors-list">
    <li><strong>First Prize</strong>, 19th “Challenge Cup” National College Students’ Extracurricular Academic Science and Technology Works Competition, 2025.</li>
    <li><strong>2025 Excellence Program</strong>, National College Student Innovation and Entrepreneurship Training Program.</li>
  </ul>
</section>

<section id="skills" class="section">
  <h2 class="section-title"><i class="fa-solid fa-wrench section-icon"></i> Technical Skills</h2>
  <div class="skills-grid">
    <div class="skill-row">
      <span class="skill-label">Research Areas</span>
      <div class="skill-pills">
        <span class="skill-pill">Diffusion Policies</span>
        <span class="skill-pill">Vision-Language-Action Models</span>
        <span class="skill-pill">World-Action Models</span>
        <span class="skill-pill">Recursive Self-Improvement</span>
        <span class="skill-pill">Representation Learning</span>
      </div>
    </div>
    <div class="skill-row">
      <span class="skill-label">Programming &amp; ML</span>
      <div class="skill-pills">
        <span class="skill-pill">Python</span>
        <span class="skill-pill">C/C++</span>
        <span class="skill-pill">Bash</span>
        <span class="skill-pill">PyTorch</span>
      </div>
    </div>
    <div class="skill-row">
      <span class="skill-label">Robotics &amp; Tools</span>
      <div class="skill-pills">
        <span class="skill-pill">ROS 2</span>
        <span class="skill-pill">MuJoCo</span>
        <span class="skill-pill">Isaac Sim</span>
        <span class="skill-pill">Gazebo</span>
        <span class="skill-pill">Unitree SDK</span>
        <span class="skill-pill">Linux</span>
        <span class="skill-pill">Git</span>
        <span class="skill-pill">LaTeX</span>
      </div>
    </div>
  </div>
</section>

<section id="life" class="section">
  <h2 class="section-title"><i class="fa-solid fa-camera-retro section-icon"></i> Life</h2>
  <div class="life-grid">
    <div class="life-text">
      <p>
        Outside of research, I enjoy taking life slow—noticing good architecture, roadside flowers, and passing scenery. I am also learning photography, listening to J-POP, and enjoying a good beer.
      </p>
      <p class="life-hint">
        <i class="fa-regular fa-hand-pointer"></i> Hover the photo stack to fan out · Click to view full photo
      </p>
    </div>
    <div class="photo-stack-wrap">
      <div class="photo-stack" aria-label="Photography stack">
        <button type="button" class="stack-card" data-src="./assets/img/photos/photo-1.png" aria-label="View photo 1">
          <img src="./assets/img/photos/photo-1.png" alt="Photography 1" loading="lazy" />
        </button>
        <button type="button" class="stack-card" data-src="./assets/img/photos/photo-2.png" aria-label="View photo 2">
          <img src="./assets/img/photos/photo-2.png" alt="Photography 2" loading="lazy" />
        </button>
        <button type="button" class="stack-card" data-src="./assets/img/photos/photo-3.png" aria-label="View photo 3">
          <img src="./assets/img/photos/photo-3.png" alt="Photography 3" loading="lazy" />
        </button>
        <button type="button" class="stack-card" data-src="./assets/img/photos/photo-4.png" aria-label="View photo 4">
          <img src="./assets/img/photos/photo-4.png" alt="Photography 4" loading="lazy" />
        </button>
        <button type="button" class="stack-card" data-src="./assets/img/photos/photo-5.png" aria-label="View photo 5">
          <img src="./assets/img/photos/photo-5.png" alt="Photography 5" loading="lazy" />
        </button>
        <button type="button" class="stack-card" data-src="./assets/img/photos/photo-6.png" aria-label="View photo 6">
          <img src="./assets/img/photos/photo-6.png" alt="Photography 6" loading="lazy" />
        </button>
      </div>
    </div>
  </div>
</section>
