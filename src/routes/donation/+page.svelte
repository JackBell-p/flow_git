<div class="donate-wrapper">
  <main class="minimal-content">
    <header class="page-header">
      <h1 class="page-title">Sponsor</h1>
      <div class="full-divider"></div>
    </header>

    <section class="donate-section">
      <div class="text-content">
        <p class="main-desc">
          如果这个项目为你节省了时间，或者带来了些许灵感，欢迎请我喝杯咖啡。
        </p>
        <p class="sub-desc">
          你的支持是我持续维护和开源的动力。
        </p>
      </div>

      <div class="qr-container">
        <div class="qr-card">
          <div class="qr-header wechat">
            <svg viewBox="0 0 24 24" width="16" height="16" fill="currentColor">
              <path d="M8.5 13.5c-3.59 0-6.5-2.46-6.5-5.5s2.91-5.5 6.5-5.5 6.5 2.46 6.5 5.5c0 1.4-.63 2.68-1.66 3.68l.48 1.54-1.74-.88c-.98.43-2.06.66-3.08.66zm8.5 2c-3.04 0-5.5-2.02-5.5-4.5s2.46-4.5 5.5-4.5 5.5 2.02 5.5 4.5c0 1.14-.52 2.19-1.39 3l.4 1.25-1.45-.73c-.8.35-1.68.53-2.56.53z"/>
            </svg>
            <span>微信支付</span>
          </div>
          <div class="qr-image-box">
            <img src="/mm_facetoface_collect_qrcode_1772980656303.png" alt="微信收款码" class="qr-image" />
          </div>
        </div>

        <div class="qr-card">
          <div class="qr-header alipay">
            <svg viewBox="0 0 24 24" width="16" height="16" fill="currentColor">
              <path d="M21 4H3a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h18a1 1 0 0 0 1-1V5a1 1 0 0 0-1-1zm-1 14H4V6h16v12zm-3-7h-2v-2h2v2zm-4 0h-2v-2h2v2zm-4 0H7v-2h2v2z" />
            </svg>
            <span>支付宝</span>
          </div>
          <div class="qr-image-box">
            <img src="/1772980683655.jpg" alt="支付宝收款码" class="qr-image" />
          </div>
        </div>
      </div>
      
      <div class="thank-you-note">
        — 感谢你的慷慨与支持 —
      </div>
    </section>
  </main>
</div>

<style>
  :root {
    --text-title: #0f172a;
    --text-body: #475569;
    --text-light: #94a3b8;
    --border-color: #e2e8f0;
    --bg-light: #f8fafc;
    --wechat-color: #07c160;
    --alipay-color: #1677ff;
  }

  .donate-wrapper {
    max-width: 650px;
    margin: 4rem auto;
    padding: 0 1.5rem;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
    color: var(--text-body);
    line-height: 1.6;
    -webkit-font-smoothing: antialiased;
  }

  .page-header {
    margin-bottom: 0;
  }

  .page-title {
    font-size: 4.5rem;
    font-weight: 900;
    line-height: 1;
    margin: 0;
    letter-spacing: -0.04em;
    color: var(--text-title);
  }

  .full-divider {
    height: 1px;
    background: var(--border-color);
    width: 100%;
    margin: 2.5rem 0;
  }

  .donate-section {
    padding-top: 0;
  }

  .text-content {
    margin-bottom: 3rem;
  }

  .main-desc {
    font-size: 1.05rem;
    font-weight: 500;
    color: var(--text-title);
    margin: 0 0 0.5rem 0;
    line-height: 1.6;
  }

  .sub-desc {
    font-size: 0.95rem;
    color: var(--text-body);
    margin: 0;
    opacity: 0.85;
  }

  .qr-container {
    display: flex;
    gap: 2rem;
    margin-bottom: 3rem;
  }

  .qr-card {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 1.5rem;
    border: 1px solid var(--border-color);
    border-radius: 12px;
    background: #ffffff;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }

  .qr-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 12px 24px rgba(15, 23, 42, 0.04);
  }

  .qr-header {
    display: flex;
    align-items: center;
    gap: 8px;
    font-size: 0.85rem;
    font-weight: 600;
    margin-bottom: 1.2rem;
    letter-spacing: 0.05em;
  }

  .qr-header.wechat {
    color: var(--wechat-color);
  }

  .qr-header.alipay {
    color: var(--alipay-color);
  }

  .qr-image-box {
    width: 100%;
    aspect-ratio: 3 / 5;
    background-color: var(--bg-light);
    border: 1px dashed var(--border-color);
    border-radius: 8px;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
    position: relative;
  }

  .qr-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
    color: transparent; 
  }

  .qr-image-box::before {
    content: "二维码图片";
    position: absolute;
    color: var(--text-light);
    font-size: 0.8rem;
    font-weight: 500;
    z-index: 0;
  }

  .qr-image {
    position: relative;
    z-index: 1;
  }

  .thank-you-note {
    text-align: center;
    font-size: 0.8rem;
    font-weight: 500;
    color: var(--text-light);
    letter-spacing: 0.1em;
  }

  @media (max-width: 600px) {
    .page-title { font-size: 3.5rem; }
    .donate-wrapper { margin-top: 4rem; }
    .qr-container {
      flex-direction: column;
      gap: 1.5rem;
    }
    .qr-card {
      padding: 2rem;
    }
  }
</style>
