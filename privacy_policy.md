<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Privacy Policy — Dermly</title>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400;0,500;1,400&family=Nunito+Sans:wght@300;400;600&display=swap" rel="stylesheet" />
  <style>
    :root {
      --green: #1a9e72;
      --green-light: #e6f7f1;
      --green-dark: #0d6b4d;
      --text: #1c1c1e;
      --text-muted: #6b7280;
      --text-faint: #9ca3af;
      --bg: #fafaf8;
      --bg-card: #ffffff;
      --border: #e8e8e3;
      --accent-bar: #1a9e72;
    }

    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: 'Nunito Sans', sans-serif;
      background: var(--bg);
      color: var(--text);
      font-size: 16px;
      line-height: 1.75;
      font-weight: 400;
    }

    /* ── TOP STRIPE ── */
    .top-bar {
      height: 4px;
      background: linear-gradient(90deg, var(--green) 0%, #57c9a0 100%);
    }

    /* ── HEADER ── */
    header {
      max-width: 720px;
      margin: 0 auto;
      padding: 3.5rem 2rem 2.5rem;
      border-bottom: 1px solid var(--border);
    }

    .wordmark {
      display: inline-flex;
      align-items: center;
      gap: 10px;
      margin-bottom: 1.5rem;
    }

    .wordmark-icon {
      width: 36px;
      height: 36px;
      background: var(--green);
      border-radius: 10px;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .wordmark-icon svg {
      width: 20px;
      height: 20px;
      fill: #fff;
    }

    .wordmark-text {
      font-family: 'Lora', serif;
      font-size: 22px;
      font-weight: 500;
      color: var(--text);
      letter-spacing: -0.3px;
    }

    header h1 {
      font-family: 'Lora', serif;
      font-size: 36px;
      font-weight: 400;
      line-height: 1.2;
      letter-spacing: -0.5px;
      color: var(--text);
      margin-bottom: 0.75rem;
    }

    .header-meta {
      font-size: 13px;
      color: var(--text-muted);
      display: flex;
      gap: 1.5rem;
      flex-wrap: wrap;
    }

    .header-meta span::before {
      content: '· ';
      color: var(--text-faint);
    }

    .header-meta span:first-child::before { content: ''; }

    /* ── SUMMARY STRIP ── */
    .summary-strip {
      max-width: 720px;
      margin: 0 auto;
      padding: 0 2rem;
    }

    .summary-box {
      background: var(--green-light);
      border-left: 3px solid var(--green);
      border-radius: 0 8px 8px 0;
      padding: 1.25rem 1.5rem;
      margin: 2rem 0 2.5rem;
    }

    .summary-box p {
      font-size: 13px;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      color: var(--green-dark);
      margin-bottom: 0.75rem;
    }

    .summary-items {
      list-style: none;
      display: flex;
      flex-direction: column;
      gap: 0.45rem;
    }

    .summary-items li {
      font-size: 14px;
      color: var(--green-dark);
      display: flex;
      align-items: flex-start;
      gap: 8px;
    }

    .summary-items li::before {
      content: '';
      width: 6px;
      height: 6px;
      border-radius: 50%;
      background: var(--green);
      margin-top: 7px;
      flex-shrink: 0;
    }

    /* ── MAIN CONTENT ── */
    main {
      max-width: 720px;
      margin: 0 auto;
      padding: 0 2rem 5rem;
    }

    /* ── SECTIONS ── */
    .section {
      margin-bottom: 3rem;
      padding-bottom: 3rem;
      border-bottom: 1px solid var(--border);
    }

    .section:last-of-type {
      border-bottom: none;
    }

    .section-label {
      font-size: 11px;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      color: var(--green);
      margin-bottom: 0.5rem;
    }

    .section h2 {
      font-family: 'Lora', serif;
      font-size: 24px;
      font-weight: 400;
      color: var(--text);
      margin-bottom: 1.25rem;
      line-height: 1.3;
    }

    .section p {
      font-size: 15px;
      color: #3a3a3c;
      line-height: 1.8;
      margin-bottom: 1rem;
    }

    .section p:last-child { margin-bottom: 0; }

    /* ── INFO CARDS ── */
    .info-cards {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 12px;
      margin: 1.5rem 0;
    }

    @media (max-width: 540px) {
      .info-cards { grid-template-columns: 1fr; }
    }

    .info-card {
      background: var(--bg-card);
      border: 1px solid var(--border);
      border-radius: 10px;
      padding: 1.1rem 1.25rem;
    }

    .info-card-label {
      font-size: 11px;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      color: var(--text-faint);
      margin-bottom: 0.35rem;
    }

    .info-card-value {
      font-size: 14px;
      color: var(--text);
      font-weight: 400;
      line-height: 1.5;
    }

    /* ── TABLE ── */
    .data-table {
      width: 100%;
      border-collapse: collapse;
      font-size: 14px;
      margin: 1.5rem 0;
      border: 1px solid var(--border);
      border-radius: 10px;
      overflow: hidden;
    }

    .data-table th {
      background: #f4f4f0;
      text-align: left;
      padding: 10px 14px;
      font-size: 11px;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      color: var(--text-muted);
      border-bottom: 1px solid var(--border);
    }

    .data-table td {
      padding: 11px 14px;
      border-bottom: 1px solid var(--border);
      color: #3a3a3c;
      vertical-align: top;
      line-height: 1.55;
    }

    .data-table tr:last-child td {
      border-bottom: none;
    }

    .badge {
      display: inline-block;
      font-size: 11px;
      font-weight: 600;
      padding: 2px 8px;
      border-radius: 20px;
    }

    .badge-no   { background: #fde8e8; color: #b91c1c; }
    .badge-yes  { background: var(--green-light); color: var(--green-dark); }
    .badge-note { background: #fef3c7; color: #92400e; }

    /* ── CONTACT BLOCK ── */
    .contact-block {
      background: var(--bg-card);
      border: 1px solid var(--border);
      border-radius: 12px;
      padding: 1.5rem 1.75rem;
      margin-top: 1.25rem;
      display: flex;
      align-items: center;
      gap: 1.25rem;
    }

    .contact-icon {
      width: 44px;
      height: 44px;
      background: var(--green-light);
      border-radius: 50%;
      flex-shrink: 0;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .contact-icon svg {
      width: 20px;
      height: 20px;
      fill: var(--green-dark);
    }

    .contact-block p {
      margin: 0;
      font-size: 14px;
      color: var(--text-muted);
    }

    .contact-block a {
      display: block;
      font-size: 15px;
      font-weight: 600;
      color: var(--green-dark);
      text-decoration: none;
      margin-bottom: 2px;
    }

    .contact-block a:hover { text-decoration: underline; }

    /* ── FOOTER ── */
    footer {
      max-width: 720px;
      margin: 0 auto;
      padding: 2rem 2rem 3rem;
      border-top: 1px solid var(--border);
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      gap: 0.75rem;
    }

    footer p {
      font-size: 12px;
      color: var(--text-faint);
    }

    footer a {
      font-size: 12px;
      color: var(--text-muted);
      text-decoration: none;
    }

    footer a:hover { color: var(--green); }
  </style>
</head>
<body>

<div class="top-bar"></div>

<!-- HEADER -->
<header>
  <div class="wordmark">
    <div class="wordmark-icon">
      <!-- leaf icon -->
      <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
        <path d="M17 8C8 10 5.9 16.17 3.82 21C4.84 21 7.3 20 8 17C8.5 20 11 22 15 22C17 22 21 20 21 14C21 9 17 8 17 8Z"/>
      </svg>
    </div>
    <span class="wordmark-text">Dermly</span>
  </div>

  <h1>Privacy Policy</h1>

  <div class="header-meta">
    <span>Effective date: May 2, 2026</span>
    <span>Last updated: May 2, 2026</span>
    <span>Applies to: Dermly mobile app</span>
  </div>
</header>

<!-- SUMMARY STRIP -->
<div class="summary-strip">
  <div class="summary-box">
    <p>The short version</p>
    <ul class="summary-items">
      <li>Dermly collects zero personal data from you.</li>
      <li>All your data lives on your device and is deleted when you uninstall the app.</li>
      <li>Barcodes and search terms are sent to OpenBeautyFacts to look up products — no personal info attached.</li>
      <li>Google Fonts CDN receives your IP address on first launch for font delivery.</li>
      <li>We never sell, share, or monetise anything related to you.</li>
    </ul>
  </div>
</div>

<!-- MAIN -->
<main>

  <!-- 1. Introduction -->
  <div class="section">
    <p class="section-label">01</p>
    <h2>Introduction</h2>
    <p>
      Dermly ("we," "our," or "us") is a skincare ingredient analysis app developed by Devbrid. This Privacy Policy explains how we handle information when you use the Dermly mobile application.
    </p>
    <p>
      We built Dermly with a privacy-first approach. We do not create accounts, track behaviour, or store anything on our own servers. The policy below is our commitment to transparency about the very limited external interactions the app does make.
    </p>
  </div>

  <!-- 2. Information We Collect -->
  <div class="section">
    <p class="section-label">02</p>
    <h2>Information we collect — and don't collect</h2>
    <p>
      Dermly does not collect, transmit, or store any personally identifiable information (PII). There are no accounts, no sign-ups, and no analytics.
    </p>

    <table class="data-table">
      <thead>
        <tr>
          <th>Data type</th>
          <th>Collected by us?</th>
          <th>Notes</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Name, email, phone</td>
          <td><span class="badge badge-no">Never</span></td>
          <td>No accounts, no sign-up.</td>
        </tr>
        <tr>
          <td>Location</td>
          <td><span class="badge badge-no">Never</span></td>
          <td>App does not request location permission.</td>
        </tr>
        <tr>
          <td>Camera / photos</td>
          <td><span class="badge badge-no">Never</span></td>
          <td>Used locally on-device only; images are not uploaded.</td>
        </tr>
        <tr>
          <td>Usage & analytics</td>
          <td><span class="badge badge-no">Never</span></td>
          <td>No analytics SDKs integrated.</td>
        </tr>
        <tr>
          <td>Barcodes & search terms</td>
          <td><span class="badge badge-note">Third-party</span></td>
          <td>Sent to OpenBeautyFacts API to look up products. No PII attached.</td>
        </tr>
        <tr>
          <td>IP address (fonts)</td>
          <td><span class="badge badge-note">Third-party</span></td>
          <td>Google Fonts CDN receives your IP on first launch for font delivery.</td>
        </tr>
        <tr>
          <td>App preferences & history</td>
          <td><span class="badge badge-yes">On-device</span></td>
          <td>Stored locally only. Deleted on uninstall.</td>
        </tr>
      </tbody>
    </table>
  </div>

  <!-- 3. Data Stored on Your Device -->
  <div class="section">
    <p class="section-label">03</p>
    <h2>Data stored on your device</h2>
    <p>
      Any preferences, scan history, or ingredient data you interact with in Dermly is stored exclusively in your device's local storage using standard mobile OS mechanisms. This data:
    </p>
    <div class="info-cards">
      <div class="info-card">
        <div class="info-card-label">Access</div>
        <div class="info-card-value">Only you, on your device. We have no access.</div>
      </div>
      <div class="info-card">
        <div class="info-card-label">Deletion</div>
        <div class="info-card-value">Automatically deleted when you uninstall Dermly.</div>
      </div>
      <div class="info-card">
        <div class="info-card-label">Backup</div>
        <div class="info-card-value">May be included in your OS-level device backup (e.g. iCloud / Google Backup), subject to your own settings.</div>
      </div>
      <div class="info-card">
        <div class="info-card-label">Server sync</div>
        <div class="info-card-value">Never synced to any Dermly or Devbrid server.</div>
      </div>
    </div>
  </div>

  <!-- 4. Third-Party Services -->
  <div class="section">
    <p class="section-label">04</p>
    <h2>Third-party services</h2>

    <p>Dermly communicates with two external services:</p>

    <table class="data-table">
      <thead>
        <tr>
          <th>Service</th>
          <th>Purpose</th>
          <th>Data sent</th>
          <th>Their policy</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td><strong>OpenBeautyFacts</strong></td>
          <td>Product ingredient lookup via barcode scan or search</td>
          <td>Barcode number or product search term. No user identifiers.</td>
          <td><a href="https://world.openbeautyfacts.org/privacy" target="_blank" rel="noopener">openbeautyfacts.org/privacy</a></td>
        </tr>
        <tr>
          <td><strong>Google Fonts CDN</strong></td>
          <td>Loading display fonts on first app launch</td>
          <td>Your IP address (standard HTTP request). Google may log this per their CDN policy.</td>
          <td><a href="https://policies.google.com/privacy" target="_blank" rel="noopener">policies.google.com/privacy</a></td>
        </tr>
      </tbody>
    </table>

    <p>
      We do not use advertising networks, social media SDKs, crash-reporting services (e.g. Firebase Crashlytics), or any other third-party SDK that collects data.
    </p>
    <p>
      <strong>Note on Google Fonts:</strong> If you would like to avoid your IP being shared with Google, you may block network access to <code>fonts.googleapis.com</code> at the OS or network firewall level. The app will fall back to a system font gracefully.
    </p>
  </div>

  <!-- 5. Children's Privacy -->
  <div class="section">
    <p class="section-label">05</p>
    <h2>Children's privacy</h2>
    <p>
      Dermly does not knowingly collect any information from children under the age of 13 (or 16 in the EU/EEA under GDPR). Because we collect no personal data at all, Dermly is safe for users of all ages. If you believe your child's data has somehow been collected, please contact us at <a href="mailto:help@devbrid.in">help@devbrid.in</a> and we will investigate promptly.
    </p>
  </div>

  <!-- 6. Your Rights (GDPR / Privacy Laws) -->
  <div class="section">
    <p class="section-label">06</p>
    <h2>Your rights under GDPR and applicable privacy laws</h2>
    <p>
      Because Dermly does not collect or store personal data on our servers, most GDPR data subject rights (access, rectification, portability, erasure) are exercised simply by managing or deleting the app on your own device.
    </p>
    <p>
      If you have any questions about your rights, want confirmation that we hold no data about you, or wish to make a formal deletion request, you can contact us at any time:
    </p>

    <div class="contact-block">
      <div class="contact-icon">
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path d="M20 4H4C2.9 4 2 4.9 2 6V18C2 19.1 2.9 20 4 20H20C21.1 20 22 19.1 22 18V6C22 4.9 21.1 4 20 4ZM20 8L12 13 4 8V6L12 11 20 6V8Z"/>
        </svg>
      </div>
      <div>
        <a href="mailto:help@devbrid.in">help@devbrid.in</a>
        <p>Privacy requests are acknowledged within 72 hours and resolved within 30 days.</p>
      </div>
    </div>

    <p style="margin-top:1.25rem">
      If you are in the EU/EEA and believe we have not addressed your concern adequately, you have the right to lodge a complaint with your local data protection authority.
    </p>
  </div>

  <!-- 7. Data Security -->
  <div class="section">
    <p class="section-label">07</p>
    <h2>Data security</h2>
    <p>
      Since we hold no personal data on our servers, there is no centralised database to breach. The only data that exists lives locally on your device and is protected by your device's own security model (e.g. iOS Secure Enclave, Android Keystore). We recommend keeping your device OS updated and using screen lock to protect your local app data.
    </p>
  </div>

  <!-- 8. Changes to This Policy -->
  <div class="section">
    <p class="section-label">08</p>
    <h2>Changes to this policy</h2>
    <p>
      We may update this Privacy Policy from time to time. Any changes will be posted at <a href="https://originlhibrid.github.io/privacy_policy" target="_blank" rel="noopener">originlhibrid.github.io/privacy_policy</a> with an updated effective date. For material changes, we will include an in-app notification. Continued use of Dermly after changes constitutes acceptance of the updated policy.
    </p>
  </div>

  <!-- 9. Contact -->
  <div class="section">
    <p class="section-label">09</p>
    <h2>Contact us</h2>
    <p>
      If you have any questions, concerns, or requests relating to this Privacy Policy or how Dermly handles data, please reach out:
    </p>

    <div class="contact-block">
      <div class="contact-icon">
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path d="M20 4H4C2.9 4 2 4.9 2 6V18C2 19.1 2.9 20 4 20H20C21.1 20 22 19.1 22 18V6C22 4.9 21.1 4 20 4ZM20 8L12 13 4 8V6L12 11 20 6V8Z"/>
        </svg>
      </div>
      <div>
        <a href="mailto:help@devbrid.in">help@devbrid.in</a>
        <p>Devbrid — Developer of Dermly</p>
      </div>
    </div>
  </div>

</main>

<!-- FOOTER -->
<footer>
  <p>© 2026 Devbrid. All rights reserved.</p>
  <a href="https://originlhibrid.github.io/privacy_policy" target="_blank" rel="noopener">originlhibrid.github.io/privacy_policy</a>
</footer>

</body>
</html>
