/* ============ RESET & GLOBAL ============ */
* { margin: 0; padding: 0; box-sizing: border-box; }

:root {
  /* 🎨 COR DA MARCA — SUBSTITUI PELA COR DO LOGOTIPO */
  --accent: #3d8bfd;
  --accent-hover: #2d7aed;
  --accent-glow: rgba(61, 139, 253, 0.18);
  --accent-soft: rgba(61, 139, 253, 0.08);

  --bg: #0a0c0f;
  --bg-alt: #0e1116;
  --surface: #161b22;
  --border: #232a33;
  --text: #e6edf3;
  --text-dim: #9ba7b4;

  --radius: 16px;
  --radius-sm: 10px;
  --transition: 0.25s cubic-bezier(0.2, 0.9, 0.4, 1);

  --font-sans: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
  --max-width: 1200px;
}

html { scroll-behavior: smooth; -webkit-text-size-adjust: 100%; }

body {
  font-family: var(--font-sans);
  background: var(--bg);
  color: var(--text);
  line-height: 1.6;
  letter-spacing: 0.01em;
  -webkit-font-smoothing: antialiased;
  overflow-x: hidden;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

a { color: inherit; text-decoration: none; transition: color var(--transition); }
img { max-width: 100%; display: block; height: auto; }
ul { list-style: none; }

h1, h2, h3, h4 { font-weight: 650; line-height: 1.2; letter-spacing: -0.02em; }
h1 { font-size: clamp(2rem, 6.5vw, 3.6rem); font-weight: 700; letter-spacing: -0.03em; }
h2 { font-size: clamp(1.5rem, 4.5vw, 2.4rem); }
h3 { font-size: clamp(1.15rem, 3.5vw, 1.45rem); }
h4 { font-size: 1rem; }

p { color: var(--text-dim); font-size: clamp(0.95rem, 2.4vw, 1.05rem); }
.narrow { max-width: 720px; margin-left: auto; margin-right: auto; }
.center { margin-left: auto; margin-right: auto; text-align: center; }
.text-center { text-align: center; }

/* ============ LAYOUT ============ */
.container { width: 100%; max-width: var(--max-width); margin: 0 auto; padding: 0 1.25rem; }
.section { padding: 3.5rem 0; }
.section-alt { background: var(--bg-alt); border-top: 1px solid var(--border); border-bottom: 1px solid var(--border); }

@media (min-width: 768px) {
  .section { padding: 5rem 0; }
  .container { padding: 0 2rem; }
}

/* ============ HEADER ============ */
.site-header {
  position: sticky; top: 0; z-index: 100;
  background: rgba(10, 12, 15, 0.88);
  backdrop-filter: blur(14px);
  -webkit-backdrop-filter: blur(14px);
  border-bottom: 1px solid var(--border);
}
.nav-wrapper { display: flex; align-items: center; justify-content: space-between; padding: 0.8rem 0; gap: 1rem; }

.logo { display: flex; align-items: center; gap: 0.6rem; font-weight: 700; letter-spacing: -0.02em; }
.logo-img { width: 32px; height: 32px; object-fit: contain; border-radius: 8px; }
.logo-text { font-size: 1.25rem; color: var(--text); }
.logo-text strong { color: var(--accent); font-weight: 700; }

.nav-desktop { display: none; align-items: center; gap: 1.8rem; font-size: 0.92rem; font-weight: 500; color: var(--text-dim); }
.nav-desktop a { position: relative; padding: 0.25rem 0; }
.nav-desktop a:hover, .nav-desktop a.active { color: var(--text); }
.nav-desktop a::after {
  content: ''; position: absolute; left: 0; bottom: -2px;
  width: 0; height: 2px; background: var(--accent); border-radius: 2px;
  transition: width var(--transition);
}
.nav-desktop a:hover::after, .nav-desktop a.active::after { width: 100%; }
.nav-desktop .btn::after { display: none; }

/* ============ BUTTONS ============ */
.btn {
  display: inline-flex; align-items: center; justify-content: center;
  gap: 0.4rem; padding: 0.7rem 1.5rem; border-radius: 100px;
  font-weight: 550; font-size: 0.9rem; cursor: pointer;
  border: 1px solid transparent; background: transparent;
  color: var(--text); font-family: inherit; line-height: 1.4;
  transition: all var(--transition); white-space: nowrap;
}
.btn-primary {
  background: var(--accent); color: #fff; border-color: var(--accent);
  box-shadow: 0 0 20px var(--accent-glow);
}
.btn-primary:hover {
  background: var(--accent-hover); border-color: var(--accent-hover);
  transform: translateY(-1px);
  box-shadow: 0 8px 24px var(--accent-glow);
}
.btn-outline { border-color: var(--border); color: var(--text-dim); }
.btn-outline:hover { border-color: var(--accent); color: var(--text); background: var(--accent-soft); }
.btn-sm { padding: 0.5rem 1.1rem; font-size: 0.82rem; }

/* ============ HAMBURGER ============ */
.hamburger {
  display: flex; flex-direction: column; justify-content: center; align-items: center;
  width: 42px; height: 42px; border-radius: 12px;
  border: 1px solid var(--border); background: transparent;
  cursor: pointer; gap: 5px; transition: border-color var(--transition);
}
.hamburger:hover { border-color: var(--accent); }
.hamburger span {
  display: block; width: 20px; height: 2px;
  background: var(--text); border-radius: 2px;
  transition: all var(--transition); transform-origin: center;
}
.hamburger.active span:nth-child(1) { transform: translateY(7px) rotate(45deg); }
.hamburger.active span:nth-child(2) { opacity: 0; }
.hamburger.active span:nth-child(3) { transform: translateY(-7px) rotate(-45deg); }

/* ============ MOBILE MENU ============ */
.mobile-menu {
  position: fixed; top: 0; right: -100%;
  width: min(82vw, 320px); height: 100dvh;
  background: #0e1116;
  border-left: 1px solid var(--border);
  padding: 5rem 1.5rem 2rem;
  display: flex; flex-direction: column; gap: 0.4rem;
  transition: right 0.35s cubic-bezier(0.2, 0.9, 0.4, 1);
  z-index: 99; overflow-y: auto;
}
.mobile-menu.open { right: 0; }
.mobile-menu a {
  padding: 0.9rem 1rem; border-radius: var(--radius-sm);
  color: var(--text-dim); font-weight: 500; font-size: 1rem;
  border: 1px solid transparent;
}
.mobile-menu a:hover, .mobile-menu a.active {
  color: var(--text); background: var(--surface); border-color: var(--border);
}
.mobile-menu .btn { margin-top: 1rem; width: 100%; }

.menu-overlay {
  position: fixed; inset: 0; background: rgba(0,0,0,0.55);
  backdrop-filter: blur(4px); z-index: 98;
  opacity: 0; pointer-events: none; transition: opacity 0.3s ease;
}
.menu-overlay.active { opacity: 1; pointer-events: all; }

@media (min-width: 900px) {
  .nav-desktop { display: flex; }
  .hamburger { display: none; }
  .mobile-menu, .menu-overlay { display: none; }
}

/* ============ HERO ============ */
.hero { position: relative; padding: 3rem 0 4rem; overflow: hidden; }
.hero::before {
  content: ''; position: absolute; top: -30%; right: -10%;
  width: 500px; height: 500px;
  background: radial-gradient(circle, var(--accent-soft) 0%, transparent 70%);
  border-radius: 50%; pointer-events: none;
}
.hero::after {
  content: ''; position: absolute; bottom: -20%; left: -10%;
  width: 400px; height: 400px;
  background: radial-gradient(circle, var(--accent-soft) 0%, transparent 70%);
  border-radius: 50%; pointer-events: none;
}
.hero-grid { display: grid; gap: 2.5rem; align-items: center; position: relative; z-index: 1; }
@media (min-width: 900px) {
  .hero-grid { grid-template-columns: 1.1fr 0.9fr; gap: 3rem; }
  .hero { padding: 5rem 0 6rem; }
}

.eyebrow {
  display: inline-block;
  font-size: 0.78rem; font-weight: 600; letter-spacing: 0.18em;
  text-transform: uppercase; color: var(--accent);
  margin-bottom: 1rem;
}
.hero h1 { margin-bottom: 1.2rem; }
.hero p { margin-bottom: 2rem; font-size: clamp(1rem, 2.6vw, 1.15rem); }
.hero-actions { display: flex; flex-wrap: wrap; gap: 0.9rem; }
.center-actions { justify-content: center; }

/* ============ TECH VISUAL ============ */
.tech-visual { display: flex; justify-content: center; align-items: center; min-height: 280px; }
.tech-orbit { position: relative; width: min(100%, 380px); aspect-ratio: 1; display: flex; justify-content: center; align-items: center; }
.tech-ring {
  position: absolute; border-radius: 50%;
  border: 1px solid var(--accent-soft);
  animation: spin 20s linear infinite;
}
.tech-ring:nth-child(1) { width: 100%; height: 100%; animation-duration: 25s; }
.tech-ring:nth-child(2) {
  width: 75%; height: 75%; animation-duration: 18s; animation-direction: reverse;
  border-color: rgba(61,139,253,0.25);
}
.tech-ring:nth-child(3) {
  width: 50%; height: 50%; animation-duration: 12s;
  border-color: rgba(61,139,253,0.35);
}
.tech-core {
  width: 30%; height: 30%;
  background: radial-gradient(circle at 30% 30%, var(--accent), #1a4a9e);
  border-radius: 50%;
  box-shadow: 0 0 60px var(--accent-glow), 0 0 120px var(--accent-soft);
  position: relative; z-index: 2;
  animation: pulse 3s ease-in-out infinite;
}
.tech-dot {
  position: absolute; width: 8px; height: 8px;
  background: var(--accent); border-radius: 50%;
  box-shadow: 0 0 12px var(--accent);
}
.tech-dot:nth-child(4) { top: 0; left: 50%; transform: translateX(-50%); }
.tech-dot:nth-child(5) { bottom: 0; left: 50%; transform: translateX(-50%); }
.tech-dot:nth-child(6) { left: 0; top: 50%; transform: translateY(-50%); }
.tech-dot:nth-child(7) { right: 0; top: 50%; transform: translateY(-50%); }

@keyframes spin { to { transform: rotate(360deg); } }
@keyframes pulse {
  0%, 100% { transform: scale(1); opacity: 1; }
  50% { transform: scale(1.08); opacity: 0.9; }
}

/* ============ CARDS ============ */
.card {
  background: var(--surface); border: 1px solid var(--border);
  border-radius: var(--radius); padding: 1.8rem 1.5rem;
  display: flex; flex-direction: column; gap: 0.8rem;
  transition: all var(--transition); height: 100%;
}
.card:hover {
  border-color: var(--accent);
  transform: translateY(-4px);
  box-shadow: 0 12px 40px rgba(0,0,0,0.35);
}
.card h3 { color: var(--text); }
.card p { font-size: 0.95rem; flex: 1; }
.card .btn { align-self: flex-start; margin-top: 0.5rem; }
.card.text-center .btn, .card.text-center .tag { align-self: center; }

.card-icon {
  font-size: 1.6rem; width: 48px; height: 48px;
  display: flex; align-items: center; justify-content: center;
  background: var(--accent-soft); border-radius: 12px;
  border: 1px solid var(--accent-soft); margin-bottom: 0.4rem;
}

.badge {
  display: inline-block; padding: 0.28rem 0.85rem;
  border-radius: 100px; background: var(--accent-soft);
  color: var(--accent); font-size: 0.72rem; font-weight: 600;
  letter-spacing: 0.08em; text-transform: uppercase; width: fit-content;
}

.product-card { min-height: 240px; }
.feature-project { max-width: 720px; margin: 0 auto; }

/* ============ GRIDS ============ */
.grid-2, .grid-3, .grid-4 { display: grid; gap: 1.2rem; grid-template-columns: 1fr; }
@media (min-width: 600px) {
  .grid-2 { grid-template-columns: repeat(2, 1fr); }
  .grid-3 { grid-template-columns: repeat(2, 1fr); }
  .grid-4 { grid-template-columns: repeat(2, 1fr); }
}
@media (min-width: 900px) {
  .grid-3 { grid-template-columns: repeat(3, 1fr); }
  .grid-4 { grid-template-columns: repeat(4, 1fr); }
}

/* ============ FEATURES ============ */
.feature {
  padding: 1.4rem 1.2rem; background: var(--surface);
  border: 1px solid var(--border); border-radius: var(--radius);
  transition: all var(--transition);
}
.feature:hover { border-color: var(--accent); transform: translateY(-3px); }
.feature h4 { color: var(--text); margin-bottom: 0.5rem; font-size: 1.05rem; }
.feature p { font-size: 0.92rem; }

/* ============ TAGS ============ */
.tags { display: flex; flex-wrap: wrap; gap: 0.6rem; margin-top: 1.5rem; }
.tag {
  display: inline-flex; align-items: center; padding: 0.45rem 1rem;
  border-radius: 100px; background: var(--surface);
  border: 1px solid var(--border); font-size: 0.82rem;
  font-weight: 500; color: var(--text-dim);
  transition: all var(--transition); width: fit-content;
}
.tag:hover { border-color: var(--accent); color: var(--text); background: var(--accent-soft); }

/* ============ ECOSYSTEM ============ */
.ecosystem { display: flex; flex-direction: column; align-items: center; gap: 1.2rem; padding: 2rem 0; }
.ecosystem-node {
  background: var(--surface); border: 1px solid var(--border);
  border-radius: var(--radius); padding: 1rem 2rem;
  font-weight: 600; font-size: 1.05rem; text-align: center;
  width: 100%; max-width: 320px; transition: all var(--transition);
}
.ecosystem-node.root {
  border-color: var(--accent); box-shadow: 0 0 30px var(--accent-glow);
  font-size: 1.3rem; color: var(--accent);
}
.ecosystem-arrow { font-size: 1.5rem; color: var(--accent); opacity: 0.6; }
.ecosystem-branches { display: grid; grid-template-columns: 1fr; gap: 0.8rem; width: 100%; max-width: 500px; }
@media (min-width: 600px) { .ecosystem-branches { grid-template-columns: repeat(2, 1fr); } }
.ecosystem-branches .ecosystem-node { max-width: none; font-size: 0.92rem; padding: 0.85rem 1rem; }

/* ============ IA STUDIO ============ */
.ia-studio {
  background: linear-gradient(135deg, var(--accent-soft) 0%, rgba(61,139,253,0.02) 100%);
  border: 1px solid rgba(61,139,253,0.25);
  border-radius: var(--radius); padding: 2rem 1.5rem;
}
@media (min-width: 768px) { .ia-studio { padding: 3rem 2.5rem; } }
.ia-studio h2 { color: var(--accent); font-size: clamp(1.5rem, 4vw, 2.2rem); margin-bottom: 0.4rem; }
.ia-studio p { margin-bottom: 1rem; }

.ia-features {
  display: grid; grid-template-columns: repeat(2, 1fr);
  gap: 0.7rem; margin: 1.5rem 0;
}
@media (min-width: 600px) { .ia-features { grid-template-columns: repeat(3, 1fr); } }
@media (min-width: 900px) { .ia-features { grid-template-columns: repeat(4, 1fr); } }
.ia-features li {
  background: var(--bg); border: 1px solid var(--border);
  border-radius: var(--radius-sm); padding: 0.7rem 1rem;
  font-size: 0.85rem; color: var(--text-dim); text-align: center;
  transition: all var(--transition);
}
.ia-features li:hover { border-color: var(--accent); color: var(--text); }

/* ============ PRINCIPLES LIST ============ */
.principles { margin-top: 1rem; display: flex; flex-direction: column; gap: 0.8rem; }
.principles li {
  padding: 0.9rem 1.1rem; background: var(--surface);
  border: 1px solid var(--border); border-left: 3px solid var(--accent);
  border-radius: var(--radius-sm); color: var(--text-dim);
  font-size: 0.95rem; transition: all var(--transition);
}
.principles li:hover { color: var(--text); transform: translateX(4px); }

/* ============ PAGE HEADER ============ */
.page-header { padding: 3rem 0 2rem; text-align: center; }
.page-header h1 { margin-bottom: 0.8rem; }

/* ============ CONTACT ============ */
.contact-card {
  background: var(--surface); border: 1px solid var(--border);
  border-radius: var(--radius); padding: 2rem 1.5rem;
  text-align: center; max-width: 600px; margin: 0 auto;
  transition: all var(--transition);
}
.contact-card:hover { border-color: var(--accent); }
.contact-card .email {
  font-size: clamp(1rem, 3vw, 1.25rem); font-weight: 600;
  color: var(--accent); margin: 1rem 0 1.5rem; word-break: break-all;
}

/* ============ FOOTER ============ */
.site-footer {
  background: var(--bg-alt); border-top: 1px solid var(--border);
  padding: 3rem 0 2rem; margin-top: auto;
}
.footer-grid { display: grid; gap: 2rem; grid-template-columns: 1fr; }
@media (min-width: 600px) { .footer-grid { grid-template-columns: 2fr 1fr 1fr; } }
.footer-brand .logo { margin-bottom: 0.8rem; }
.footer-brand p { font-size: 0.9rem; }
.footer-links h4 {
  font-size: 0.8rem; text-transform: uppercase; letter-spacing: 0.1em;
  color: var(--text-dim); margin-bottom: 1rem;
}
.footer-links ul { display: flex; flex-direction: column; gap: 0.6rem; }
.footer-links a { font-size: 0.9rem; color: var(--text-dim); }
.footer-links a:hover { color: var(--accent); }
.footer-bottom {
  margin-top: 2.5rem; padding-top: 1.5rem;
  border-top: 1px solid var(--border);
  display: flex; flex-direction: column; gap: 1rem;
  align-items: center; text-align: center;
  font-size: 0.85rem; color: var(--text-dim);
}
.footer-bottom-links { display: flex; gap: 1.5rem; flex-wrap: wrap; justify-content: center; }
.footer-bottom-links a { color: var(--text-dim); font-size: 0.85rem; }
.footer-bottom-links a:hover { color: var(--accent); }

/* ============ UTILITIES ============ */
.mt-2 { margin-top: 1rem; }
.mt-3 { margin-top: 1.5rem; }
.mb-2 { margin-bottom: 1rem; }
.mb-3 { margin-bottom: 1.5rem; }
.mb-4 { margin-bottom: 2rem; }

/* ============ FADE-IN ============ */
.fade-in { opacity: 0; transform: translateY(20px); transition: opacity 0.6s ease, transform 0.6s ease; }
.fade-in.visible { opacity: 1; transform: translateY(0); }

/* ============ FOCUS ============ */
a:focus-visible, button:focus-visible {
  outline: 2px solid var(--accent); outline-offset: 3px; border-radius: 4px;
}

/* ============ SCROLLBAR ============ */
::-webkit-scrollbar { width: 6px; }
::-webkit-scrollbar-track { background: var(--bg); }
::-webkit-scrollbar-thumb { background: var(--border); border-radius: 3px; }
::-webkit-scrollbar-thumb:hover { background: var(--accent); }