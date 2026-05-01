
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>Tyson Hub | Official Telegram Channels</title>
  <!-- Google Fonts & Font Awesome -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', sans-serif;
      background: radial-gradient(circle at 10% 20%, #0b0719, #03010f);
      color: #f0f0f0;
      line-height: 1.4;
      scroll-behavior: smooth;
    }

    /* custom scrollbar */
    ::-webkit-scrollbar {
      width: 6px;
    }
    ::-webkit-scrollbar-track {
      background: #1a1729;
    }
    ::-webkit-scrollbar-thumb {
      background: #6a3ef0;
      border-radius: 12px;
    }

    .container {
      max-width: 1300px;
      margin: 0 auto;
      padding: 2rem 1.5rem 3rem;
    }

    /* Header section */
    .logo-area {
      text-align: center;
      margin-bottom: 1.2rem;
    }
    .brand-badge {
      display: inline-flex;
      align-items: center;
      gap: 12px;
      background: rgba(106, 62, 240, 0.18);
      backdrop-filter: blur(8px);
      padding: 0.5rem 1.5rem;
      border-radius: 100px;
      border: 1px solid rgba(106, 62, 240, 0.4);
      margin-bottom: 1rem;
    }
    .brand-badge i {
      font-size: 1.6rem;
      color: #b47cff;
    }
    .brand-badge span {
      font-weight: 700;
      font-size: 1.3rem;
      letter-spacing: -0.3px;
      background: linear-gradient(135deg, #FFFFFF, #c084fc);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
    }
    h1 {
      font-size: 2.7rem;
      font-weight: 800;
      background: linear-gradient(145deg, #fff, #c084fc, #a855f7);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      letter-spacing: -0.5px;
      margin-bottom: 0.5rem;
    }
    .tagline {
      font-size: 1.05rem;
      color: #bcaeff;
      margin-bottom: 2rem;
      font-weight: 500;
      opacity: 0.9;
    }

    /* owner card premium */
    .owner-card {
      background: linear-gradient(115deg, rgba(25, 20, 45, 0.85), rgba(15, 10, 30, 0.9));
      backdrop-filter: blur(12px);
      border-radius: 2rem;
      border: 1px solid rgba(168, 85, 247, 0.5);
      padding: 1rem 2rem;
      margin-bottom: 3rem;
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: 1rem;
      box-shadow: 0 12px 30px rgba(0, 0, 0, 0.4), 0 0 12px rgba(168, 85, 247, 0.2);
      transition: all 0.2s;
    }
    .owner-info {
      display: flex;
      align-items: center;
      gap: 1rem;
      flex-wrap: wrap;
    }
    .owner-icon {
      background: #6a3ef0;
      width: 52px;
      height: 52px;
      border-radius: 60px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.7rem;
      box-shadow: 0 0 10px #a855f7;
    }
    .owner-text h3 {
      font-size: 1rem;
      font-weight: 500;
      letter-spacing: 1px;
      color: #c7b9ff;
      margin-bottom: 4px;
    }
    .owner-id {
      font-size: 1.65rem;
      font-weight: 800;
      background: linear-gradient(135deg, #ffffff, #e0aaff);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      letter-spacing: -0.2px;
      cursor: pointer;
      transition: 0.2s;
    }
    .owner-id:hover {
      filter: brightness(1.1);
      text-shadow: 0 0 5px #c084fc;
    }
    .owner-actions {
      display: flex;
      gap: 12px;
      align-items: center;
    }
    .btn-outline-light {
      background: transparent;
      border: 1px solid #a855f7;
      padding: 0.6rem 1.3rem;
      border-radius: 40px;
      font-weight: 600;
      color: #e2d9ff;
      transition: 0.2s;
      cursor: pointer;
      font-size: 0.85rem;
      display: inline-flex;
      align-items: center;
      gap: 8px;
    }
    .btn-outline-light:hover {
      background: #a855f7;
      color: white;
      border-color: #c084fc;
      transform: scale(0.98);
    }
    .btn-filled {
      background: linear-gradient(95deg, #6a3ef0, #a855f7);
      border: none;
      padding: 0.6rem 1.4rem;
      border-radius: 40px;
      font-weight: 600;
      color: white;
      transition: 0.2s;
      text-decoration: none;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      font-size: 0.85rem;
      box-shadow: 0 4px 12px rgba(106, 62, 240, 0.4);
    }
    .btn-filled:hover {
      background: linear-gradient(95deg, #825cf5, #bf77ff);
      transform: translateY(-2px);
    }
    .copy-toast {
      position: fixed;
      bottom: 30px;
      left: 50%;
      transform: translateX(-50%);
      background: #1e1a35e6;
      backdrop-filter: blur(12px);
      padding: 10px 20px;
      border-radius: 60px;
      font-size: 0.85rem;
      font-weight: 500;
      color: white;
      border-left: 4px solid #a855f7;
      z-index: 1000;
      pointer-events: none;
      transition: opacity 0.2s;
      font-family: monospace;
      box-shadow: 0 4px 18px black;
    }

    /* Grid cards */
    .channels-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(330px, 1fr));
      gap: 1.8rem;
      margin: 2rem 0 2.5rem;
    }
    .channel-card {
      background: rgba(18, 14, 32, 0.7);
      backdrop-filter: blur(8px);
      border-radius: 1.8rem;
      border: 1px solid rgba(168, 85, 247, 0.25);
      padding: 1.5rem 1.4rem;
      transition: all 0.25s ease;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
      display: flex;
      flex-direction: column;
      position: relative;
      overflow: hidden;
    }
    .channel-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 4px;
      height: 100%;
      background: linear-gradient(to bottom, #a855f7, #6a3ef0);
      border-radius: 4px 0 0 4px;
    }
    .channel-card:hover {
      transform: translateY(-6px);
      border-color: rgba(168, 85, 247, 0.7);
      box-shadow: 0 18px 32px -8px black;
      background: rgba(26, 20, 48, 0.8);
    }
    .card-icon {
      font-size: 2.3rem;
      margin-bottom: 1rem;
      color: #c084fc;
      width: fit-content;
      background: rgba(128, 90, 240, 0.15);
      padding: 0.5rem;
      border-radius: 1.2rem;
      display: inline-flex;
      align-items: center;
      justify-content: center;
    }
    .channel-title {
      font-size: 1.4rem;
      font-weight: 700;
      line-height: 1.3;
      margin-bottom: 0.7rem;
      letter-spacing: -0.2px;
      word-break: break-word;
    }
    .channel-desc {
      color: #cdc6f0;
      font-size: 0.88rem;
      margin-bottom: 1.4rem;
      line-height: 1.45;
      opacity: 0.85;
    }
    .card-footer {
      margin-top: auto;
    }
    .join-btn {
      width: 100%;
      background: rgba(106, 62, 240, 0.2);
      border: 1px solid #a077f0;
      border-radius: 60px;
      padding: 0.7rem 0;
      font-weight: 600;
      color: #f0eaff;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 12px;
      transition: 0.2s;
      text-decoration: none;
      font-size: 0.9rem;
      backdrop-filter: blur(2px);
    }
    .join-btn i {
      font-size: 1rem;
    }
    .join-btn:hover {
      background: #a855f7;
      border-color: #c289ff;
      color: white;
      gap: 16px;
    }

    .footer-note {
      text-align: center;
      margin-top: 3rem;
      padding-top: 1.8rem;
      border-top: 1px dashed rgba(168, 85, 247, 0.4);
      font-size: 0.8rem;
      color: #9a8ec9;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1.5rem;
    }
    .footer-note a {
      color: #d1b3ff;
      text-decoration: none;
      transition: 0.2s;
    }
    .footer-note a:hover {
      color: white;
      text-decoration: underline;
    }
    @media (max-width: 700px) {
      .container {
        padding: 1.5rem 1rem;
      }
      h1 {
        font-size: 2rem;
      }
      .owner-card {
        flex-direction: column;
        align-items: stretch;
        text-align: center;
      }
      .owner-actions {
        justify-content: center;
      }
      .owner-info {
        justify-content: center;
      }
      .channel-title {
        font-size: 1.25rem;
      }
    }
    .glow-text {
      font-weight: 500;
    }
  </style>
</head>
<body>
<div class="container">
  <!-- header branding -->
  <div class="logo-area">
    <div class="brand-badge">
      <i class="fab fa-telegram-plane"></i>
      <span>TYSON ECOSYSTEM</span>
      <i class="fas fa-bolt"></i>
    </div>
    <h1>TYSON <span style="background: linear-gradient(145deg,#fff,#b77eff);-webkit-background-clip:text;background-clip:text;color:transparent;">OFFICIAL HUB</span></h1>
    <div class="tagline">
      <i class="fas fa-gem" style="font-size: 0.8rem;"></i> Premium Telegram channels • Hacks • Giveaways • VIP Predictions
    </div>
  </div>

  <!-- Owner ID card with direct contact -->
  <div class="owner-card">
    <div class="owner-info">
      <div class="owner-icon">
        <i class="fas fa-crown"></i>
      </div>
      <div class="owner-text">
        <h3><i class="fas fa-user-shield"></i> CHANNEL OWNER</h3>
        <div class="owner-id" id="ownerIdCopy">@TYSON_OWNER</div>
      </div>
    </div>
    <div class="owner-actions">
      <a href="https://t.me/TYSON_OWNER" target="_blank" class="btn-filled" rel="noopener noreferrer">
        <i class="fab fa-telegram"></i> Message Owner
      </a>
      <button class="btn-outline-light" id="copyOwnerBtn">
        <i class="far fa-copy"></i> Copy ID
      </button>
    </div>
  </div>

  <!-- Channels Grid : using exact details and links from request -->
  <div class="channels-grid">
    <!-- 1. FREE HACK CHANNEL -->
    <div class="channel-card">
      <div class="card-icon"><i class="fas fa-user-secret"></i></div>
      <div class="channel-title">𝗙𝗥𝗘𝗘 𝗛𝗔𝗖𝗞 𝗖𝗛𝗔𝗡𝗡𝗘𝗟</div>
      <div class="channel-desc">Access exclusive hacking resources, tools & tutorials. Daily updates and premium methods.</div>
      <div class="card-footer">
        <a href="https://t.me/+kFhnhnlONOszMmNl" target="_blank" rel="noopener noreferrer" class="join-btn">
          <i class="fab fa-telegram"></i> Join Channel <i class="fas fa-arrow-right"></i>
        </a>
      </div>
    </div>
    <!-- 2. FREE CASE GIVEAWAY -->
    <div class="channel-card">
      <div class="card-icon"><i class="fas fa-gift"></i></div>
      <div class="channel-title">𝗙𝗥𝗘𝗘 𝗖𝗔𝗦𝗘 𝗚𝗜𝗩𝗘𝗪𝗔𝗬</div>
      <div class="channel-desc">Win daily cases, skins, rewards & mystery boxes. Limited giveaways for active members.</div>
      <div class="card-footer">
        <a href="https://t.me/+-VZNCztN6YhhY2U1" target="_blank" rel="noopener noreferrer" class="join-btn">
          <i class="fab fa-telegram"></i> Claim Rewards <i class="fas fa-arrow-right"></i>
        </a>
      </div>
    </div>
    <!-- 3. ALL PREDICTION TYSON -->
    <div class="channel-card">
      <div class="card-icon"><i class="fas fa-chart-line"></i></div>
      <div class="channel-title">𝗔𝗟𝗟 𝗣𝗥𝗘𝗗𝗜𝗖𝗧𝗜𝗢𝗡 𝗧𝗬𝗦𝗢𝗡</div>
      <div class="channel-desc">Accurate match predictions, betting tips, and win probability analysis. Don't miss out.</div>
      <div class="card-footer">
        <a href="https://t.me/+F6YlLUwilLFjMTVl" target="_blank" rel="noopener noreferrer" class="join-btn">
          <i class="fab fa-telegram"></i> Get Predictions <i class="fas fa-arrow-right"></i>
        </a>
      </div>
    </div>
    <!-- 4. TYSON VIP HACK SEVER (spelling preserved) -->
    <div class="channel-card">
      <div class="card-icon"><i class="fas fa-shield-haltered"></i></div>
      <div class="channel-title">𝗧𝗬𝗦𝗢𝗡 𝗩𝗜𝗣 𝗛𝗔𝗖𝗞 𝗦𝗘𝗩𝗘𝗥</div>
      <div class="channel-desc">Private VIP hacking server, premium tools, bypasses and 24/7 support.</div>
      <div class="card-footer">
        <a href="https://t.me/TYSON_OK_WIN_HACK" target="_blank" rel="noopener noreferrer" class="join-btn">
          <i class="fab fa-telegram"></i> Enter VIP <i class="fas fa-arrow-right"></i>
        </a>
      </div>
    </div>
    <!-- 5. TYSON TRADING HUB -->
    <div class="channel-card">
      <div class="card-icon"><i class="fas fa-chart-simple"></i></div>
      <div class="channel-title">𝗧𝗬𝗦𝗢𝗡 𝗧𝗥𝗔𝗗𝗜𝗡𝗚 𝗛𝗨𝗕</div>
      <div class="channel-desc">Forex, crypto & stock signals. Expert trade calls & market analysis daily.</div>
      <div class="card-footer">
        <a href="https://t.me/+kFhnhnlONOszMmNl" target="_blank" rel="noopener noreferrer" class="join-btn">
          <i class="fab fa-telegram"></i> Join Trading Hub <i class="fas fa-arrow-right"></i>
        </a>
      </div>
    </div>
    <!-- 6. FREE GIVEAWAY 🎁✨ BY TYSON -->
    <div class="channel-card">
      <div class="card-icon"><i class="fas fa-trophy"></i></div>
      <div class="channel-title">𝗙𝗥𝗘𝗘 𝗚𝗜𝗩𝗘𝗔𝗪𝗔𝗬🎁✨ 𝗕𝗬 𝗧𝗬𝗦𝗢𝗡</div>
      <div class="channel-desc">Exclusive gift boxes, promo codes, and surprise airdrops - active members only.</div>
      <div class="card-footer">
        <a href="https://t.me/+lWy3kfNbfWg0OGQ1" target="_blank" rel="noopener noreferrer" class="join-btn">
          <i class="fab fa-telegram"></i> Get Gift <i class="fas fa-arrow-right"></i>
        </a>
      </div>
    </div>
  </div>

  <!-- extra info / highlights -->
  <div class="footer-note">
    <span><i class="fab fa-telegram"></i> 100% Official Channels</span>
    <span><i class="fas fa-shield-alt"></i> Trusted by 10k+ members</span>
    <span><i class="fas fa-bolt"></i> Daily active updates</span>
    <span><i class="fas fa-user-tie"></i> Owner: <strong>@TYSON_OWNER</strong></span>
  </div>
  <div style="text-align: center; font-size: 0.7rem; margin-top: 1.5rem; opacity: 0.6;">
    ⚡ Join the fastest growing Telegram community | All links are verified
  </div>
</div>

<script>
  // Smooth copy functionality for owner ID
  const ownerSpan = document.getElementById('ownerIdCopy');
  const copyBtn = document.getElementById('copyOwnerBtn');
  let toastTimeout = null;

  function showCopyToast(message) {
    // remove existing toast if any
    const existingToast = document.querySelector('.copy-toast');
    if(existingToast) existingToast.remove();
    const toast = document.createElement('div');
    toast.className = 'copy-toast';
    toast.innerHTML = `<i class="fas fa-check-circle" style="color:#c084fc;"></i> ${message}`;
    document.body.appendChild(toast);
    setTimeout(() => {
      if(toast) toast.style.opacity = '0';
      setTimeout(() => toast.remove(), 300);
    }, 2000);
  }

  function copyOwnerId() {
    const textToCopy = '@TYSON_OWNER';
    navigator.clipboard.writeText(textToCopy).then(() => {
      showCopyToast('Copied: @TYSON_OWNER');
    }).catch(() => {
      // fallback
      const textArea = document.createElement('textarea');
      textArea.value = textToCopy;
      document.body.appendChild(textArea);
      textArea.select();
      document.execCommand('copy');
      document.body.removeChild(textArea);
      showCopyToast('Copied: @TYSON_OWNER');
    });
  }

  if(copyBtn) {
    copyBtn.addEventListener('click', copyOwnerId);
  }
  if(ownerSpan) {
    ownerSpan.addEventListener('click', copyOwnerId);
    ownerSpan.style.cursor = 'pointer';
  }

  // Optional: additional hover tooltip for owner id
  const tooltipStyle = document.createElement('style');
  tooltipStyle.textContent = `
    .owner-id:hover::after {
      content: "Click to copy";
      position: absolute;
      background: #1e1a2f;
      font-size: 0.7rem;
      padding: 4px 8px;
      border-radius: 20px;
      margin-left: 8px;
      white-space: nowrap;
      color: #c9b6ff;
      border: 1px solid #a855f7;
      pointer-events: none;
    }
    .owner-id {
      position: relative;
      display: inline-block;
    }
  `;
  document.head.appendChild(tooltipStyle);
</script>
</body>
</html>
