<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes, viewport-fit=cover">
  <title>Tyson Ecosystem | Official Telegram Hub</title>
  <!-- Font Awesome 6 (free) -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: radial-gradient(circle at 10% 20%, #0c091f, #02010a);
      font-family: system-ui, -apple-system, 'Segoe UI', 'Inter', 'Helvetica Neue', sans-serif;
      color: #ededf5;
      line-height: 1.4;
      padding: 0;
      margin: 0;
    }

    /* main container - tighter on mobile */
    .container {
      max-width: 580px;
      margin: 0 auto;
      padding: 1.2rem 1rem 2.2rem;
    }

    /* header section */
    .telegram-badge {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      background: rgba(106, 62, 240, 0.2);
      backdrop-filter: blur(6px);
      width: fit-content;
      margin: 0 auto 1rem auto;
      padding: 0.4rem 1.2rem;
      border-radius: 100px;
      border: 1px solid rgba(168, 85, 247, 0.5);
    }
    .telegram-badge i {
      font-size: 1.2rem;
      color: #bb9eff;
    }
    .telegram-badge span {
      font-weight: 600;
      font-size: 0.9rem;
      letter-spacing: 0.5px;
    }
    h1 {
      font-size: 2.1rem;
      font-weight: 800;
      text-align: center;
      background: linear-gradient(135deg, #ffffff, #cb9eff, #a855f7);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      margin-bottom: 0.25rem;
      letter-spacing: -0.3px;
    }
    .tagline {
      text-align: center;
      font-size: 0.85rem;
      color: #b9abff;
      margin-bottom: 1.5rem;
      border-bottom: 1px dashed rgba(168, 85, 247, 0.3);
      display: inline-block;
      width: 100%;
      padding-bottom: 0.6rem;
    }
    .tagline i {
      margin: 0 4px;
    }

    /* owner card - mobile optimized */
    .owner-card {
      background: rgba(20, 16, 40, 0.8);
      backdrop-filter: blur(12px);
      border-radius: 1.6rem;
      padding: 1rem 1.2rem;
      margin-bottom: 2rem;
      border: 1px solid rgba(168, 85, 247, 0.5);
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: 0.8rem;
    }
    .owner-left {
      display: flex;
      align-items: center;
      gap: 0.8rem;
      flex-wrap: wrap;
    }
    .owner-icon {
      background: linear-gradient(145deg, #6a3ef0, #9b4dff);
      width: 48px;
      height: 48px;
      border-radius: 60px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.5rem;
      box-shadow: 0 0 8px #b77eff;
    }
    .owner-info h4 {
      font-size: 0.7rem;
      font-weight: 500;
      color: #bbadff;
      letter-spacing: 0.5px;
      margin-bottom: 0.2rem;
    }
    .owner-id {
      font-size: 1.3rem;
      font-weight: 800;
      background: linear-gradient(135deg, #f0eaff, #d9bcff);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      cursor: pointer;
      display: inline-flex;
      align-items: center;
      gap: 5px;
    }
    .owner-id i {
      font-size: 1rem;
      color: #bc9eff;
    }
    .owner-actions {
      display: flex;
      gap: 10px;
      align-items: center;
    }
    .btn-sm {
      background: rgba(168, 85, 247, 0.2);
      border: 1px solid #a36efa;
      padding: 0.5rem 1rem;
      border-radius: 40px;
      font-size: 0.75rem;
      font-weight: 600;
      color: #e6dbff;
      cursor: pointer;
      display: inline-flex;
      align-items: center;
      gap: 6px;
      transition: 0.2s;
    }
    .btn-sm-filled {
      background: linear-gradient(95deg, #6a3ef0, #a855f7);
      border: none;
      padding: 0.5rem 1rem;
      border-radius: 40px;
      font-size: 0.75rem;
      font-weight: 600;
      color: white;
      text-decoration: none;
      display: inline-flex;
      align-items: center;
      gap: 6px;
      box-shadow: 0 2px 8px rgba(106, 62, 240, 0.4);
    }
    .btn-sm-filled:active, .btn-sm:active {
      transform: scale(0.96);
    }

    /* channel cards grid - single column on phones */
    .channels-list {
      display: flex;
      flex-direction: column;
      gap: 1.2rem;
      margin: 1.8rem 0 2rem;
    }
    .channel-card {
      background: rgba(15, 12, 28, 0.7);
      backdrop-filter: blur(8px);
      border-radius: 1.4rem;
      border: 1px solid rgba(168, 85, 247, 0.3);
      padding: 1rem 1.2rem;
      transition: all 0.2s ease;
      box-shadow: 0 6px 14px rgba(0, 0, 0, 0.25);
    }
    .channel-card:active {
      transform: scale(0.99);
    }
    .card-header {
      display: flex;
      align-items: center;
      gap: 12px;
      margin-bottom: 10px;
    }
    .card-icon {
      background: rgba(128, 90, 240, 0.2);
      width: 44px;
      height: 44px;
      border-radius: 1.2rem;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.6rem;
      color: #cdadff;
    }
    .channel-title {
      font-size: 1.2rem;
      font-weight: 700;
      letter-spacing: -0.2px;
      word-break: break-word;
      line-height: 1.25;
    }
    .channel-desc {
      font-size: 0.8rem;
      color: #cbc4f0;
      margin: 0.6rem 0 1rem 0;
      padding-left: 4px;
      line-height: 1.4;
    }
    .join-btn {
      background: transparent;
      width: 100%;
      border: 1px solid #906cf0;
      border-radius: 60px;
      padding: 0.7rem 0;
      font-weight: 600;
      font-size: 0.85rem;
      color: #ede7ff;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      text-decoration: none;
      transition: 0.2s;
    }
    .join-btn i {
      font-size: 0.9rem;
    }
    .join-btn:active {
      background: #a855f7;
      border-color: #c68eff;
      color: white;
      gap: 14px;
    }

    /* footer */
    .footer-stats {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1rem;
      margin: 1.8rem 0 1rem;
      padding-top: 1rem;
      border-top: 1px solid rgba(168, 85, 247, 0.3);
      font-size: 0.7rem;
      color: #9b8bcb;
    }
    .footer-stats span i {
      margin-right: 5px;
    }
    .small-note {
      text-align: center;
      font-size: 0.65rem;
      opacity: 0.7;
      margin-top: 0.8rem;
    }

    /* toast for copy */
    .copy-toast {
      position: fixed;
      bottom: 24px;
      left: 50%;
      transform: translateX(-50%);
      background: #1a1635dd;
      backdrop-filter: blur(20px);
      padding: 8px 18px;
      border-radius: 40px;
      font-size: 0.8rem;
      font-weight: 500;
      z-index: 2000;
      color: white;
      border-left: 3px solid #b77eff;
      box-shadow: 0 4px 12px black;
      pointer-events: none;
      white-space: nowrap;
    }

    /* mobile extra tuning */
    @media (max-width: 480px) {
      .container {
        padding: 1rem 0.9rem 2rem;
      }
      h1 {
        font-size: 1.85rem;
      }
      .owner-id {
        font-size: 1.1rem;
      }
      .owner-card {
        padding: 0.8rem 1rem;
      }
      .owner-left {
        gap: 0.6rem;
      }
      .owner-icon {
        width: 42px;
        height: 42px;
        font-size: 1.3rem;
      }
      .btn-sm, .btn-sm-filled {
        padding: 0.45rem 0.9rem;
        font-size: 0.7rem;
      }
      .channel-title {
        font-size: 1.05rem;
      }
      .card-icon {
        width: 38px;
        height: 38px;
        font-size: 1.35rem;
      }
      .join-btn {
        padding: 0.6rem 0;
      }
    }

    /* hover only for desktop — not needed on mobile, but fine */
    .join-btn:hover, .btn-sm-filled:hover, .btn-sm:hover {
      background: #a855f7;
      border-color: #c98fff;
      color: white;
    }
    .channel-card:hover {
      border-color: rgba(168, 85, 247, 0.7);
      background: rgba(25, 20, 45, 0.85);
    }
  </style>
</head>
<body>

<div class="container">
  <!-- header exactly as per image style -->
  <div class="telegram-badge">
    <i class="fab fa-telegram-plane"></i>
    <span>TYSON ECOSYSTEM</span>
    <i class="fas fa-bolt"></i>
  </div>
  <h1>TYSON OFFICIAL HUB</h1>
  <div class="tagline">
    <i class="fas fa-gem"></i> Premium Telegram channels • Hacks • Giveaways • VIP Predictions
  </div>

  <!-- Owner card with copy + direct message -->
  <div class="owner-card">
    <div class="owner-left">
      <div class="owner-icon">
        <i class="fas fa-crown"></i>
      </div>
      <div class="owner-info">
        <h4><i class="fas fa-user-shield"></i> CHANNEL OWNER</h4>
        <div class="owner-id" id="ownerIdCopy">
          @TYSON_OWNER <i class="far fa-copy" style="font-size: 0.75rem;"></i>
        </div>
      </div>
    </div>
    <div class="owner-actions">
      <a href="https://t.me/TYSON_OWNER" target="_blank" rel="noopener noreferrer" class="btn-sm-filled">
        <i class="fab fa-telegram"></i> Message
      </a>
      <button class="btn-sm" id="copyOwnerBtn">
        <i class="far fa-copy"></i> Copy ID
      </button>
    </div>
  </div>

  <!-- Channels list (exactly from the description, all original links) -->
  <div class="channels-list">
    <!-- 1. FREE HACK CHANNEL -->
    <div class="channel-card">
      <div class="card-header">
        <div class="card-icon"><i class="fas fa-user-secret"></i></div>
        <div class="channel-title">𝗙𝗥𝗘𝗘 𝗛𝗔𝗖𝗞 𝗖𝗛𝗔𝗡𝗡𝗘𝗟</div>
      </div>
      <div class="channel-desc">Access exclusive hacking resources, tools & tutorials. Daily updates and premium methods.</div>
      <a href="https://t.me/+kFhnhnlONOszMmNl" target="_blank" rel="noopener noreferrer" class="join-btn">
        <i class="fab fa-telegram"></i> Join Channel <i class="fas fa-arrow-right"></i>
      </a>
    </div>

    <!-- 2. FREE CASE GIVEAWAY -->
    <div class="channel-card">
      <div class="card-header">
        <div class="card-icon"><i class="fas fa-gift"></i></div>
        <div class="channel-title">𝗙𝗥𝗘𝗘 𝗖𝗔𝗦𝗘 𝗚𝗜𝗩𝗘𝗪𝗔𝗬</div>
      </div>
      <div class="channel-desc">Win daily cases, skins, rewards & mystery boxes. Limited giveaways for active members.</div>
      <a href="https://t.me/+-VZNCztN6YhhY2U1" target="_blank" rel="noopener noreferrer" class="join-btn">
        <i class="fab fa-telegram"></i> Claim Rewards <i class="fas fa-arrow-right"></i>
      </a>
    </div>

    <!-- 3. ALL PREDICTION TYSON -->
    <div class="channel-card">
      <div class="card-header">
        <div class="card-icon"><i class="fas fa-chart-line"></i></div>
        <div class="channel-title">𝗔𝗟𝗟 𝗣𝗥𝗘𝗗𝗜𝗖𝗧𝗜𝗢𝗡 𝗧𝗬𝗦𝗢𝗡</div>
      </div>
      <div class="channel-desc">Accurate match predictions, betting tips, and win probability analysis. Don't miss out.</div>
      <a href="https://t.me/+F6YlLUwilLFjMTVl" target="_blank" rel="noopener noreferrer" class="join-btn">
        <i class="fab fa-telegram"></i> Get Predictions <i class="fas fa-arrow-right"></i>
      </a>
    </div>

    <!-- 4. TYSON VIP HACK SEVER (exact spelling) -->
    <div class="channel-card">
      <div class="card-header">
        <div class="card-icon"><i class="fas fa-shield-haltered"></i></div>
        <div class="channel-title">𝗧𝗬𝗦𝗢𝗡 𝗩𝗜𝗣 𝗛𝗔𝗖𝗞 𝗦𝗘𝗩𝗘𝗥</div>
      </div>
      <div class="channel-desc">Private VIP hacking server, premium tools, bypasses and 24/7 support.</div>
      <a href="https://t.me/TYSON_OK_WIN_HACK" target="_blank" rel="noopener noreferrer" class="join-btn">
        <i class="fab fa-telegram"></i> Enter VIP <i class="fas fa-arrow-right"></i>
      </a>
    </div>

    <!-- 5. TYSON TRADING HUB (link identical to first, but as provided) -->
    <div class="channel-card">
      <div class="card-header">
        <div class="card-icon"><i class="fas fa-chart-simple"></i></div>
        <div class="channel-title">𝗧𝗬𝗦𝗢𝗡 𝗧𝗥𝗔𝗗𝗜𝗡𝗚 𝗛𝗨𝗕</div>
      </div>
      <div class="channel-desc">Forex, crypto & stock signals. Expert trade calls & market analysis daily.</div>
      <a href="https://t.me/+kFhnhnlONOszMmNl" target="_blank" rel="noopener noreferrer" class="join-btn">
        <i class="fab fa-telegram"></i> Join Trading Hub <i class="fas fa-arrow-right"></i>
      </a>
    </div>

    <!-- 6. FREE GIVEAWAY 🎁✨ BY TYSON -->
    <div class="channel-card">
      <div class="card-header">
        <div class="card-icon"><i class="fas fa-trophy"></i></div>
        <div class="channel-title">𝗙𝗥𝗘𝗘 𝗚𝗜𝗩𝗘𝗔𝗪𝗔𝗬🎁✨ 𝗕𝗬 𝗧𝗬𝗦𝗢𝗡</div>
      </div>
      <div class="channel-desc">Exclusive gift boxes, promo codes, and surprise airdrops - active members only.</div>
      <a href="https://t.me/+lWy3kfNbfWg0OGQ1" target="_blank" rel="noopener noreferrer" class="join-btn">
        <i class="fab fa-telegram"></i> Get Gift <i class="fas fa-arrow-right"></i>
      </a>
    </div>
  </div>

  <!-- footer stats exactly as image style -->
  <div class="footer-stats">
    <span><i class="fab fa-telegram"></i> 100% Official Channels</span>
    <span><i class="fas fa-users"></i> Trusted by 10k+ members</span>
    <span><i class="fas fa-bolt"></i> Daily active updates</span>
    <span><i class="fas fa-user-tie"></i> Owner: <strong>@TYSON_OWNER</strong></span>
  </div>
  <div class="small-note">
    🔗 Join the fastest growing Telegram community | All links are verified
  </div>
</div>

<script>
  // Copy Owner ID functionality with smooth toast
  const ownerElement = document.getElementById('ownerIdCopy');
  const copyBtn = document.getElementById('copyOwnerBtn');

  function showToast(msg) {
    const existing = document.querySelector('.copy-toast');
    if(existing) existing.remove();
    const toast = document.createElement('div');
    toast.className = 'copy-toast';
    toast.innerHTML = `<i class="fas fa-check-circle" style="color:#c084fc;"></i> ${msg}`;
    document.body.appendChild(toast);
    setTimeout(() => {
      toast.style.opacity = '0';
      setTimeout(() => toast.remove(), 250);
    }, 2000);
  }

  function copyOwnerText() {
    const text = '@TYSON_OWNER';
    navigator.clipboard.writeText(text).then(() => {
      showToast('Copied: @TYSON_OWNER');
    }).catch(() => {
      // fallback for old browsers
      const textarea = document.createElement('textarea');
      textarea.value = text;
      document.body.appendChild(textarea);
      textarea.select();
      document.execCommand('copy');
      document.body.removeChild(textarea);
      showToast('Copied: @TYSON_OWNER');
    });
  }

  if (copyBtn) copyBtn.addEventListener('click', copyOwnerText);
  if (ownerElement) ownerElement.addEventListener('click', copyOwnerText);

  // add small hover tooltip effect for owner (optional)
  ownerElement.style.cursor = 'pointer';
</script>
</body>
</html>
