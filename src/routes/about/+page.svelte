<script lang="ts">

</script>

<div class="about-wrapper">
  <main class="minimal-content">
    <header class="version-display">
      <div class="version-row">
        <h1 class="version-title">
          <span class="v-label">V0</span><span class="v-sub">.1.0</span>
        </h1>
      </div>
      
      <div class="full-divider"></div>
    </header>

    <section class="developer-section">
      <div class="dev-container">
        <div class="label-group">
          <span class="label">Developer</span>
        </div>
        
        <div class="bio-content">
          <p class="main-bio">
            你好，我是本项目的设计者JACK BELL。热衷于构建能够解决访问GITHUB问题且具有良好速度的工具。
          </p>
          <p class="sub-bio">
            如果你在使用过程中发现了 Bug 或有任何改进建议，欢迎通过GITHUB提交ISSUE。
          </p>
        </div>

        <div class="contact-links">
          <a href="https://github.com/JackBell-p/flow_git" target="_blank" class="text-link">
            <svg viewBox="0 0 24 24" width="14" height="14" fill="currentColor"><path d="M12 2A10 10 0 0 0 2 12c0 4.42 2.87 8.17 6.84 9.5.5.08.66-.23.66-.5v-1.69c-2.77.6-3.36-1.34-3.36-1.34-.46-1.16-1.11-1.47-1.11-1.47-.91-.62.07-.6.07-.6 1 .07 1.53 1.03 1.53 1.03.87 1.52 2.34 1.07 2.91.83.09-.65.35-1.09.63-1.34-2.22-.25-4.55-1.11-4.55-4.92 0-1.11.38-2 1.03-2.71-.1-.25-.45-1.29.1-2.64 0 0 .84-.27 2.75 1.02.79-.22 1.65-.33 2.5-.33.85 0 1.71.11 2.5.33 1.91-1.29 2.75-1.02 2.75-1.02.55 1.35.2 2.39.1 2.64.65.71 1.03 1.6 1.03 2.71 0 3.82-2.34 4.66-4.57 4.91.36.31.69.92.69 1.85V21c0 .27.16.59.67.5C19.14 20.16 22 16.42 22 12A10 10 0 0 0 12 2z"></path></svg>
            GitHub
          </a>
        </div>
      </div>
    </section>
  </main>
</div>

<style>
  :root {
    --primary: #2563eb;
    --text-title: #0f172a;
    --text-body: #475569;
    --text-light: #94a3b8;
    --border-color: #e2e8f0;
  }

  .about-wrapper {
    max-width: 650px;
    margin: 4rem auto;
    padding: 0 1.5rem;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
    color: var(--text-body);
    line-height: 1.6;
    -webkit-font-smoothing: antialiased;
  }

  .version-display {
    margin-bottom: 0;
  }

  .version-row {
    display: flex;
    align-items: center;
    margin-bottom: 0;
  }

  .version-title {
    font-size: 6rem;
    font-weight: 900;
    line-height: 0.8;
    margin: 0;
    letter-spacing: -0.05em;
    color: var(--text-title);
  }

  .v-sub {
    font-weight: 200;
    color: var(--text-light);
    letter-spacing: -0.02em;
  }

  .full-divider {
    height: 1px;
    background: var(--border-color);
    width: 100%;
    margin: 2.5rem 0;
  }

  .developer-section {
    padding-top: 0;
  }

  .label-group {
    display: flex;
    align-items: center;
    margin-bottom: 1.5rem;
  }

  .label {
    font-size: 0.75rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.15em;
    color: var(--text-light);
  }

  .bio-content {
    margin-bottom: 2rem;
  }

  .bio-content p {
    margin: 0 0 1rem 0;
    font-size: 1rem;
    line-height: 1.7;
  }

  .main-bio {
    color: var(--text-title);
    font-weight: 500;
  }

  .sub-bio {
    color: var(--text-body);
    font-size: 0.95rem;
    opacity: 0.85;
  }

  .contact-links {
    display: flex;
    align-items: center;
    gap: 12px;
  }

  .text-link {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    color: var(--text-body);
    text-decoration: none;
    font-size: 0.85rem;
    font-weight: 600;
    padding: 8px 16px;
    border: 1px solid var(--border-color);
    border-radius: 20px;
    transition: all 0.2s ease;
  }

  .text-link:hover {
    color: var(--text-title);
    border-color: var(--text-title);
    background: rgba(15, 23, 42, 0.04);
  }

  @media (max-width: 600px) {
    .version-title { font-size: 4rem; }
    .about-wrapper { margin-top: 6rem; }
  }
</style>
