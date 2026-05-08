# manrrique-studio.github.io

<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Rian Manrrique | Consultor Zoho CRM</title>
<link rel="preconnect" href="https://fonts.googleapis.com"/>
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin/>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet"/>
<style>
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{font-family:'Inter',sans-serif;background:#f8f9fb;color:#0b0b0f;overflow-x:hidden}

/* ── NAV ── */
nav{position:fixed;top:0;left:0;right:0;z-index:100;padding:20px 7%;display:flex;align-items:center;justify-content:space-between;background:rgba(248,249,251,0.85);backdrop-filter:blur(16px);border-bottom:1px solid rgba(0,0,0,0.05)}
.nav-logo{font-size:18px;font-weight:700;color:#0b0b0f;text-decoration:none;letter-spacing:-0.5px}
.nav-logo span{background:linear-gradient(90deg,#8b5cf6,#4ade80);-webkit-background-clip:text;-webkit-text-fill-color:transparent}
.nav-links{display:flex;align-items:center;gap:36px}
.nav-links a{font-size:14px;color:#5d6470;text-decoration:none;font-weight:500;transition:.2s}
.nav-links a:hover{color:#0b0b0f}
.nav-cta{background:linear-gradient(90deg,#8b5cf6,#4ade80);color:white;padding:10px 24px;border-radius:10px;font-size:14px;font-weight:600;text-decoration:none;transition:.2s}
.nav-cta:hover{opacity:.9}
.nav-mobile-btn{display:none;background:none;border:none;font-size:22px;cursor:pointer;color:#0b0b0f}

/* ── HERO ── */
.hero{min-height:100vh;padding:140px 7% 100px;display:flex;align-items:center;background:#f8f9fb;position:relative;overflow:hidden}
.hero::before{content:'';position:absolute;top:-200px;right:-200px;width:700px;height:700px;border-radius:50%;background:radial-gradient(circle,rgba(139,92,246,0.08) 0%,transparent 70%);pointer-events:none}
.hero::after{content:'';position:absolute;bottom:-150px;left:-100px;width:500px;height:500px;border-radius:50%;background:radial-gradient(circle,rgba(74,222,128,0.06) 0%,transparent 70%);pointer-events:none}
.hero-inner{max-width:1400px;margin:0 auto;width:100%;display:flex;align-items:center;gap:80px}
.hero-text{flex:1.1;position:relative;z-index:1}
.hero-tag{display:inline-flex;align-items:center;gap:8px;font-size:13px;letter-spacing:4px;color:#7c5cff;font-weight:600;margin-bottom:32px}
.hero-tag::before{content:'';width:8px;height:8px;border-radius:50%;background:#7c5cff;animation:pulse 2s infinite}
@keyframes pulse{0%,100%{opacity:1;transform:scale(1)}50%{opacity:.5;transform:scale(1.3)}}
.hero h1{font-size:76px;line-height:1.03;font-weight:800;color:#0b0b0f;margin-bottom:16px;letter-spacing:-2px}
.hero h1 em{font-style:normal;background:linear-gradient(90deg,#8b5cf6,#4ade80);-webkit-background-clip:text;-webkit-text-fill-color:transparent}
.hero-sub{font-size:22px;line-height:1.65;color:#5d6470;max-width:560px;margin-bottom:48px}
.hero-btns{display:flex;gap:16px;flex-wrap:wrap}
.btn-primary{background:linear-gradient(90deg,#8b5cf6,#4ade80);color:white;padding:16px 36px;border-radius:14px;font-size:16px;font-weight:700;text-decoration:none;transition:.2s}
.btn-primary:hover{opacity:.9;transform:translateY(-2px)}
.btn-secondary{background:white;color:#0b0b0f;padding:16px 36px;border-radius:14px;font-size:16px;font-weight:600;text-decoration:none;border:1px solid rgba(0,0,0,0.08);transition:.2s}
.btn-secondary:hover{border-color:rgba(139,92,246,.3);transform:translateY(-2px)}
.hero-stats{display:flex;gap:48px;margin-top:64px;padding-top:48px;border-top:1px solid rgba(0,0,0,0.06)}
.stat-item{}
.stat-number{font-size:38px;font-weight:800;color:#0b0b0f;line-height:1;margin-bottom:6px}
.stat-number span{background:linear-gradient(90deg,#8b5cf6,#4ade80);-webkit-background-clip:text;-webkit-text-fill-color:transparent}
.stat-label{font-size:14px;color:#9ca3af;font-weight:500}
.hero-visual{flex:1;display:flex;justify-content:center;align-items:center;position:relative;z-index:1}
.hero-card-stack{position:relative;width:100%;max-width:500px}
.hcard{background:white;border:1px solid rgba(0,0,0,0.06);border-radius:24px;padding:28px 32px;box-shadow:0 20px 60px rgba(0,0,0,0.06);animation:float 6s ease-in-out infinite}
.hcard-2{position:absolute;top:-40px;right:-30px;width:82%;background:rgba(248,249,251,.95);border:1px solid rgba(139,92,246,.15);border-radius:20px;padding:20px 24px;animation-delay:-2s}
.hcard-3{position:absolute;bottom:-30px;left:-20px;width:70%;background:rgba(248,249,251,.95);border:1px solid rgba(74,222,128,.2);border-radius:20px;padding:18px 22px;animation-delay:-4s}
@keyframes float{0%,100%{transform:translateY(0)}50%{transform:translateY(-12px)}}
.hcard-label{font-size:11px;letter-spacing:3px;color:#9ca3af;font-weight:600;margin-bottom:10px}
.hcard-val{font-size:28px;font-weight:800;color:#0b0b0f;margin-bottom:4px}
.hcard-val span{font-size:16px;color:#22c55e;font-weight:600}
.hcard-bar{height:6px;background:#f3f4f6;border-radius:10px;margin-top:12px;overflow:hidden}
.hcard-bar-fill{height:100%;border-radius:10px;background:linear-gradient(90deg,#8b5cf6,#4ade80)}
.hcard-row{display:flex;align-items:center;gap:10px}
.hcard-dot{width:10px;height:10px;border-radius:50%}
.hcard-text{font-size:13px;color:#374151;font-weight:500}

/* ── CONTAINER GERAL ── */
.container{max-width:1400px;margin:0 auto}
.section-tag{font-size:13px;letter-spacing:4px;color:#7c5cff;font-weight:600}

/* ── DORES ── */
.operation-section{width:100%;padding:120px 7%;background:#f8f9fb}
.top-content{display:flex;align-items:center;justify-content:space-between;gap:80px;margin-bottom:80px}
.text-content{flex:1}
.tag{font-size:13px;letter-spacing:4px;color:#7c5cff;font-weight:600}
.text-content h2{font-size:72px;line-height:1.05;margin:24px 0 12px;color:#0b0b0f;font-weight:700}
.text-content h3{font-size:58px;line-height:1.1;font-weight:400;color:#1e1e24;margin-bottom:32px}
.text-content h3 span{background:linear-gradient(90deg,#8b5cf6,#4ade80);-webkit-background-clip:text;-webkit-text-fill-color:transparent}
.text-content p{font-size:20px;line-height:1.8;color:#5d6470;margin-bottom:22px;max-width:650px}
.visual-content{flex:1;display:flex;justify-content:center}
.visual-content img{width:100%;max-width:700px;object-fit:contain;filter:drop-shadow(0 20px 40px rgba(0,0,0,0.08));animation:float 6s ease-in-out infinite}
.cards{display:grid;grid-template-columns:repeat(3,1fr);gap:24px;margin-top:40px}
.card{background:rgba(255,255,255,0.7);border:1px solid rgba(0,0,0,0.05);backdrop-filter:blur(10px);border-radius:32px;padding:42px;transition:.3s ease}
.card:hover{transform:translateY(-6px)}
.icon{width:62px;height:62px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:24px;margin-bottom:24px}
.green{background:#ecfdf3;color:#22c55e}
.purple{background:#f4efff;color:#8b5cf6}
.blue{background:#eef4ff;color:#3b82f6}
.card h4{font-size:30px;margin-bottom:24px;color:#111827}
.card ul{list-style:none;padding:0;margin:0}
.card li{font-size:18px;color:#5d6470;margin-bottom:18px;position:relative;padding-left:22px}
.card li::before{content:'•';position:absolute;left:0;color:#8b5cf6}
.bottom-highlight{margin-top:60px;width:100%;background:white;border:1px solid rgba(0,0,0,0.05);border-radius:24px;padding:28px 34px;display:flex;align-items:center;justify-content:center;gap:14px;font-size:28px;color:#151515;box-shadow:0 10px 30px rgba(0,0,0,0.03)}
.bottom-highlight span{width:42px;height:42px;border-radius:50%;background:#f3f4f6;display:flex;align-items:center;justify-content:center;font-weight:700}
.bottom-highlight strong{color:#7c5cff}

/* ── SERVIÇOS ── */
.sv-section{padding:120px 7%;background:white}
.sv-h2{font-size:64px;line-height:1.05;margin:24px 0 12px;color:#0b0b0f;font-weight:700}
.sv-h3{font-size:48px;line-height:1.1;font-weight:400;color:#1e1e24;margin-bottom:32px}
.sv-h3 span{background:linear-gradient(90deg,#8b5cf6,#4ade80);-webkit-background-clip:text;-webkit-text-fill-color:transparent}
.sv-lead{font-size:20px;line-height:1.8;color:#5d6470;max-width:700px;margin-bottom:60px}
.sv-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:24px;margin-bottom:32px}
.sv-card{background:rgba(255,255,255,0.7);border:1px solid rgba(0,0,0,0.05);backdrop-filter:blur(10px);border-radius:32px;padding:42px;transition:.3s ease;position:relative;overflow:hidden}
.sv-card:hover{transform:translateY(-6px)}
.sv-card::before{content:'';position:absolute;top:0;left:0;right:0;height:3px}
.sv-card.c1::before{background:linear-gradient(90deg,#8b5cf6,#a78bfa)}
.sv-card.c2::before{background:linear-gradient(90deg,#4ade80,#22c55e)}
.sv-card.c3::before{background:linear-gradient(90deg,#3b82f6,#60a5fa)}
.sv-card.c4::before{background:linear-gradient(90deg,#f59e0b,#fbbf24)}
.sv-card.c5::before{background:linear-gradient(90deg,#ec4899,#f472b6)}
.sv-card.c6::before{background:linear-gradient(90deg,#8b5cf6,#4ade80)}
.sv-icon{width:62px;height:62px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:26px;margin-bottom:24px}
.ic-purple{background:#f4efff;color:#8b5cf6}
.ic-green{background:#ecfdf3;color:#22c55e}
.ic-blue{background:#eef4ff;color:#3b82f6}
.ic-amber{background:#fffbeb;color:#f59e0b}
.ic-pink{background:#fdf2f8;color:#ec4899}
.ic-mix{background:linear-gradient(135deg,#f4efff,#ecfdf3);color:#8b5cf6}
.sv-card h4{font-size:24px;margin-bottom:12px;color:#111827;font-weight:600}
.sv-card p{font-size:16px;color:#5d6470;line-height:1.7;margin-bottom:16px}
.sv-tags{display:flex;flex-wrap:wrap;gap:8px;margin-top:4px}
.sv-pill{font-size:12px;font-weight:500;padding:4px 12px;border-radius:20px;background:#f3f4f6;color:#6b7280}
.sv-cta{margin-top:48px;background:#f8f9fb;border:1px solid rgba(0,0,0,0.05);border-radius:24px;padding:32px 40px;display:flex;align-items:center;justify-content:space-between;gap:24px}
.sv-cta p{font-size:22px;color:#151515;font-weight:500}
.sv-cta a{background:linear-gradient(90deg,#8b5cf6,#4ade80);color:white;text-decoration:none;padding:14px 32px;border-radius:14px;font-size:16px;font-weight:600;white-space:nowrap;transition:.2s}
.sv-cta a:hover{opacity:.9}

/* ── PROJETOS ── */
.pj-section{padding:120px 7%;background:#f8f9fb}
.pj-h2{font-size:64px;line-height:1.05;margin:24px 0 48px;color:#0b0b0f;font-weight:700}
.pj-h2 span{background:linear-gradient(90deg,#8b5cf6,#4ade80);-webkit-background-clip:text;-webkit-text-fill-color:transparent}
.pj-card{background:white;border:1px solid rgba(0,0,0,0.05);border-radius:40px;overflow:hidden;display:grid;grid-template-columns:1fr 1fr;min-height:540px;margin-bottom:32px}
.pj-left{padding:64px;display:flex;flex-direction:column;justify-content:space-between}
.pj-right{padding:64px;display:flex;flex-direction:column;justify-content:space-between;position:relative;overflow:hidden}
.pj-right-dark{background:linear-gradient(135deg,#0b0b0f 0%,#1a1030 100%)}
.pj-right-teal{background:linear-gradient(135deg,#042c53 0%,#0c3d2e 100%)}
.pj-right-amber{background:linear-gradient(135deg,#1a0a00 0%,#2d1500 60%,#1a0a00 100%)}
.pj-right::before{content:'';position:absolute;top:-80px;right:-80px;width:320px;height:320px;border-radius:50%}
.pj-right-dark::before{background:radial-gradient(circle,rgba(139,92,246,0.25) 0%,transparent 70%)}
.pj-right-teal::before{background:radial-gradient(circle,rgba(59,130,246,0.25) 0%,transparent 70%)}
.pj-right-amber::before{background:radial-gradient(circle,rgba(251,191,36,0.2) 0%,transparent 70%)}
.pj-right::after{content:'';position:absolute;bottom:-60px;left:-40px;width:200px;height:200px;border-radius:50%}
.pj-right-dark::after{background:radial-gradient(circle,rgba(74,222,128,0.15) 0%,transparent 70%)}
.pj-right-teal::after{background:radial-gradient(circle,rgba(74,222,128,0.2) 0%,transparent 70%)}
.pj-right-amber::after{background:radial-gradient(circle,rgba(234,88,12,0.15) 0%,transparent 70%)}
.pj-client-row{display:flex;align-items:center;gap:16px;margin-bottom:28px}
.pj-badge-purple{background:#f4efff;color:#7c5cff;font-size:12px;font-weight:600;letter-spacing:3px;padding:6px 14px;border-radius:8px}
.pj-badge-blue{background:#eef4ff;color:#3b82f6;font-size:12px;font-weight:600;letter-spacing:3px;padding:6px 14px;border-radius:8px}
.pj-badge-amber{background:#fffbeb;color:#b45309;font-size:12px;font-weight:600;letter-spacing:3px;padding:6px 14px;border-radius:8px}
.pj-industry{font-size:14px;color:#9ca3af;font-weight:500}
.pj-client-name{font-size:46px;font-weight:700;color:#0b0b0f;line-height:1.05;margin-bottom:14px}
.pj-role-badge{display:inline-flex;align-items:center;gap:8px;border-radius:10px;padding:8px 16px;margin-bottom:20px}
.pj-role-purple{background:#f4efff;border:1px solid rgba(139,92,246,0.2)}
.pj-role-blue{background:#eef4ff;border:1px solid rgba(59,130,246,0.2)}
.pj-role-amber{background:#fffbeb;border:1px solid rgba(245,158,11,0.25)}
.pj-role-badge span{font-size:13px;font-weight:600}
.pj-role-purple span{color:#7c5cff}
.pj-role-blue span{color:#2563eb}
.pj-role-amber span{color:#b45309}
.pj-desc{font-size:16px;color:#5d6470;line-height:1.75;margin-bottom:24px}
.pj-switch{display:flex;align-items:center;gap:12px;background:#f8f9fb;border:1px solid rgba(0,0,0,0.06);border-radius:16px;padding:16px 20px}
.pj-switch-from{font-size:14px;color:#9ca3af;text-decoration:line-through}
.pj-switch-arrow{font-size:18px;color:#8b5cf6}
.pj-switch-to{font-size:14px;font-weight:600;color:#111827}
.pj-del-title-purple{font-size:13px;letter-spacing:3px;color:#8b5cf6;font-weight:600;margin-bottom:24px;position:relative;z-index:1}
.pj-del-title-blue{font-size:13px;letter-spacing:3px;color:#60a5fa;font-weight:600;margin-bottom:22px;position:relative;z-index:1}
.pj-del-title-amber{font-size:13px;letter-spacing:3px;color:#fbbf24;font-weight:600;margin-bottom:20px;position:relative;z-index:1}
.pj-del-list{list-style:none;display:flex;flex-direction:column;gap:13px;position:relative;z-index:1}
.pj-del-list li{display:flex;align-items:flex-start;gap:12px;font-size:14px;color:rgba(255,255,255,0.85);line-height:1.5}
.dot-purple{width:20px;height:20px;border-radius:50%;background:rgba(139,92,246,0.3);display:flex;align-items:center;justify-content:center;font-size:9px;color:#c4b5fd;flex-shrink:0;margin-top:2px}
.dot-blue{width:20px;height:20px;border-radius:50%;background:rgba(59,130,246,0.3);display:flex;align-items:center;justify-content:center;font-size:9px;color:#93c5fd;flex-shrink:0;margin-top:2px}
.dot-amber{width:20px;height:20px;border-radius:50%;background:rgba(251,191,36,0.25);display:flex;align-items:center;justify-content:center;font-size:9px;color:#fcd34d;flex-shrink:0;margin-top:2px}
.result-block{position:relative;z-index:1;border-radius:20px;padding:24px 28px;margin-top:20px}
.rb-green{background:rgba(255,255,255,0.07);border:1px solid rgba(255,255,255,0.12)}
.rb-amber{background:rgba(255,255,255,0.06);border:1px solid rgba(251,191,36,0.2)}
.result-label-green{font-size:11px;letter-spacing:3px;color:#86efac;font-weight:600;margin-bottom:8px}
.result-label-amber{font-size:11px;letter-spacing:3px;color:#fcd34d;font-weight:600;margin-bottom:8px}
.result-number{font-size:44px;font-weight:800;color:white;line-height:1;margin-bottom:5px}
.result-number em{font-style:normal}
.result-em-green{font-size:22px;color:#86efac}
.result-em-small{font-size:16px;color:rgba(255,255,255,0.4)}
.result-sub{font-size:13px;color:rgba(255,255,255,0.5);line-height:1.5;margin-top:4px}
.result-before{display:flex;align-items:center;gap:10px;margin-top:12px}
.result-before s{font-size:13px;color:rgba(255,255,255,0.35)}
.result-before em{font-style:normal;font-size:13px;color:#86efac;font-weight:600}
.result-row{display:flex;align-items:center;gap:12px;margin-bottom:6px}
.result-from{font-size:22px;font-weight:700;color:rgba(255,255,255,0.3);text-decoration:line-through}
.result-arrow{font-size:18px;color:#fbbf24}
.result-to{font-size:40px;font-weight:800;color:white;line-height:1}
.result-growth{display:inline-flex;align-items:center;gap:6px;background:rgba(74,222,128,0.15);border:1px solid rgba(74,222,128,0.25);border-radius:8px;padding:5px 12px;margin-top:10px}
.result-growth span{font-size:13px;font-weight:700;color:#86efac}
.tools-row{display:flex;flex-wrap:wrap;gap:8px;padding-top:24px}
.tool-chip{font-size:12px;font-weight:600;padding:5px 12px;border-radius:8px}
.tc-purple{background:#f4efff;color:#7c5cff}
.tc-blue{background:#eef4ff;color:#2563eb}
.tc-green{background:#ecfdf3;color:#16a34a}
.tc-amber{background:#fffbeb;color:#b45309}
.tc-orange{background:#fff7ed;color:#ea580c}
.tc-gray{background:#f3f4f6;color:#374151}

/* VS block */
.pj-vs{margin-top:0;background:white;border:1px solid rgba(0,0,0,0.05);border-radius:32px;padding:48px;margin-bottom:0}
.pj-vs-title{font-size:13px;letter-spacing:4px;color:#7c5cff;font-weight:600;margin-bottom:12px}
.pj-vs-h3{font-size:34px;font-weight:700;color:#0b0b0f;margin-bottom:40px;line-height:1.2}
.pj-vs-h3 span{background:linear-gradient(90deg,#8b5cf6,#4ade80);-webkit-background-clip:text;-webkit-text-fill-color:transparent}
.vs-grid{display:grid;grid-template-columns:1fr 1fr;gap:16px}
.vs-item{background:#f8f9fb;border:1px solid rgba(0,0,0,0.05);border-radius:18px;padding:24px;display:flex;gap:14px;align-items:flex-start}
.vs-icon-wrap{width:42px;height:42px;border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:18px;flex-shrink:0}
.vs-icon-wrap.g{background:#ecfdf3;color:#22c55e}
.vs-icon-wrap.p{background:#f4efff;color:#8b5cf6}
.vs-icon-wrap.b{background:#eef4ff;color:#3b82f6}
.vs-icon-wrap.a{background:#fffbeb;color:#f59e0b}
.vs-item h5{font-size:15px;font-weight:600;color:#111827;margin-bottom:5px}
.vs-item p{font-size:14px;color:#6b7280;line-height:1.6}
.vs-note{margin-top:24px;background:linear-gradient(90deg,rgba(139,92,246,0.06),rgba(74,222,128,0.06));border:1px solid rgba(139,92,246,0.12);border-radius:14px;padding:18px 22px;font-size:15px;color:#374151;text-align:center}
.vs-note strong{color:#7c5cff}

/* ── SOBRE ── */
.sobre-section{padding:120px 7%;background:white}
.sobre-inner{max-width:1400px;margin:0 auto;display:grid;grid-template-columns:1fr 1fr;gap:80px;align-items:center}
.sobre-text .section-tag{margin-bottom:24px;display:block}
.sobre-text h2{font-size:56px;font-weight:700;line-height:1.1;color:#0b0b0f;margin-bottom:28px}
.sobre-text h2 span{background:linear-gradient(90deg,#8b5cf6,#4ade80);-webkit-background-clip:text;-webkit-text-fill-color:transparent}
.sobre-text p{font-size:18px;line-height:1.8;color:#5d6470;margin-bottom:20px}
.sobre-chips{display:flex;flex-wrap:wrap;gap:10px;margin-top:32px}
.sobre-chip{font-size:13px;font-weight:600;padding:8px 18px;border-radius:20px;background:#f4efff;color:#7c5cff;border:1px solid rgba(139,92,246,0.15)}
.sobre-visual{display:flex;flex-direction:column;gap:20px}
.sobre-card{background:#f8f9fb;border:1px solid rgba(0,0,0,0.05);border-radius:24px;padding:32px}
.sobre-card-icon{font-size:28px;margin-bottom:16px}
.sobre-card h4{font-size:20px;font-weight:600;color:#111827;margin-bottom:8px}
.sobre-card p{font-size:15px;color:#6b7280;line-height:1.65}

/* ── CONTATO ── */
.contato-section{padding:120px 7%;background:#f8f9fb}
.contato-inner{max-width:900px;margin:0 auto;text-align:center}
.contato-inner .section-tag{display:inline-block;margin-bottom:24px}
.contato-inner h2{font-size:60px;font-weight:700;line-height:1.1;color:#0b0b0f;margin-bottom:20px}
.contato-inner h2 span{background:linear-gradient(90deg,#8b5cf6,#4ade80);-webkit-background-clip:text;-webkit-text-fill-color:transparent}
.contato-inner p{font-size:20px;color:#5d6470;line-height:1.7;margin-bottom:48px;max-width:600px;margin-left:auto;margin-right:auto}
.contato-cards{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;margin-bottom:48px}
.cc{background:white;border:1px solid rgba(0,0,0,0.05);border-radius:24px;padding:32px 24px;text-align:center;text-decoration:none;transition:.3s;display:block}
.cc:hover{transform:translateY(-6px);border-color:rgba(139,92,246,.2)}
.cc-icon{font-size:28px;margin-bottom:14px}
.cc h4{font-size:16px;font-weight:600;color:#111827;margin-bottom:6px}
.cc p{font-size:14px;color:#6b7280}
.contato-cta{background:linear-gradient(135deg,#0b0b0f,#1a1030);border-radius:28px;padding:52px;color:white}
.contato-cta h3{font-size:36px;font-weight:700;margin-bottom:12px}
.contato-cta p{font-size:18px;color:rgba(255,255,255,0.65);margin-bottom:32px;max-width:500px;margin-left:auto;margin-right:auto}
.contato-cta a{background:linear-gradient(90deg,#8b5cf6,#4ade80);color:white;text-decoration:none;padding:16px 40px;border-radius:14px;font-size:16px;font-weight:700;display:inline-block;transition:.2s}
.contato-cta a:hover{opacity:.9}

/* ── FOOTER ── */
footer{background:#0b0b0f;padding:48px 7%;display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:24px}
.footer-logo{font-size:18px;font-weight:700;color:white;letter-spacing:-0.5px}
.footer-logo span{background:linear-gradient(90deg,#8b5cf6,#4ade80);-webkit-background-clip:text;-webkit-text-fill-color:transparent}
.footer-links{display:flex;gap:32px}
.footer-links a{font-size:14px;color:rgba(255,255,255,0.5);text-decoration:none;transition:.2s}
.footer-links a:hover{color:white}
.footer-copy{font-size:13px;color:rgba(255,255,255,0.3)}

/* ── RESPONSIVE ── */
@media(max-width:1100px){
  .hero h1{font-size:54px}
  .hero-stats{gap:32px}
  .hero-visual{display:none}
  .top-content{flex-direction:column}
  .text-content h2{font-size:54px}
  .text-content h3{font-size:42px}
  .cards{grid-template-columns:1fr}
  .sv-grid{grid-template-columns:repeat(2,1fr)}
  .sv-h2{font-size:48px}
  .pj-h2{font-size:48px}
  .pj-card{grid-template-columns:1fr}
  .pj-client-name{font-size:36px}
  .vs-grid{grid-template-columns:1fr}
  .sobre-inner{grid-template-columns:1fr}
  .contato-cards{grid-template-columns:1fr}
}
@media(max-width:768px){
  nav{padding:16px 5%}
  .nav-links{display:none}
  .nav-mobile-btn{display:block}
  .hero{padding:120px 5% 80px}
  .hero h1{font-size:40px;letter-spacing:-1px}
  .hero-sub{font-size:18px}
  .hero-stats{gap:24px;flex-wrap:wrap}
  .stat-number{font-size:28px}
  .operation-section,.sv-section,.pj-section,.sobre-section,.contato-section{padding:80px 5%}
  .text-content h2{font-size:40px}
  .text-content h3{font-size:30px}
  .text-content p{font-size:18px}
  .bottom-highlight{font-size:20px;text-align:center;flex-direction:column}
  .sv-grid{grid-template-columns:1fr}
  .sv-h2,.pj-h2{font-size:36px}
  .sv-cta{flex-direction:column;text-align:center}
  .pj-left,.pj-right{padding:36px}
  .pj-client-name{font-size:28px}
  .pj-vs{padding:28px 20px}
  .pj-vs-h3{font-size:26px}
  .sobre-text h2{font-size:38px}
  .contato-inner h2{font-size:38px}
  .contato-cta{padding:36px 24px}
  .contato-cta h3{font-size:26px}
  footer{flex-direction:column;text-align:center}
  .footer-links{flex-wrap:wrap;justify-content:center;gap:20px}
}
</style>
</head>
<body>

<!-- ══ NAV ══ -->
<nav id="top">
  <a href="#top" class="nav-logo">Rian <span>Manrrique</span></a>
  <div class="nav-links">
    <a href="#servicos">Serviços</a>
    <a href="#projetos">Projetos</a>
    <a href="#sobre">Sobre</a>
    <a href="#contato" class="nav-cta">Fale comigo</a>
  </div>
  <button class="nav-mobile-btn" onclick="this.nextElementSibling.classList.toggle('open')">☰</button>
</nav>

<!-- ══ HERO ══ -->
<section class="hero">
  <div class="hero-inner">
    <div class="hero-text">
      <div class="hero-tag">CONSULTOR ZOHO CRM</div>
      <h1>Operação comercial<br/>que <em>escala</em><br/>de verdade.</h1>
      <p class="hero-sub">Implanto o ecossistema Zoho do zero — CRM, automações, dashboards e integrações — para que seu processo comercial rode sem caos, sem retrabalho e com dados para decidir.</p>
      <div class="hero-btns">
        <a href="#projetos" class="btn-primary">Ver projetos →</a>
        <a href="#contato" class="btn-secondary">Fale comigo</a>
      </div>
      <div class="hero-stats">
        <div class="stat-item">
          <div class="stat-number"><span>3+</span></div>
          <div class="stat-label">Anos de experiência</div>
        </div>
        <div class="stat-item">
          <div class="stat-number"><span>300%</span></div>
          <div class="stat-label">Crescimento em clientes</div>
        </div>
        <div class="stat-item">
          <div class="stat-number"><span>R$100k</span></div>
          <div class="stat-label">Maior resultado em 1 dia</div>
        </div>
      </div>
    </div>
    <div class="hero-visual">
      <div class="hero-card-stack">
        <div class="hcard hcard-2">
          <div class="hcard-label">PIPELINE ATIVO</div>
          <div class="hcard-val">R$ 240k <span>↑ 18%</span></div>
          <div class="hcard-bar"><div class="hcard-bar-fill" style="width:72%"></div></div>
        </div>
        <div class="hcard">
          <div class="hcard-label">DASHBOARD ZOHO CRM</div>
          <div class="hcard-val">47 leads <span>↑ hoje</span></div>
          <div style="display:flex;flex-direction:column;gap:10px;margin-top:16px">
            <div class="hcard-row"><div class="hcard-dot" style="background:#8b5cf6"></div><div class="hcard-text">Qualificação automática ativa</div></div>
            <div class="hcard-row"><div class="hcard-dot" style="background:#22c55e"></div><div class="hcard-text">Workflow rodando</div></div>
            <div class="hcard-row"><div class="hcard-dot" style="background:#3b82f6"></div><div class="hcard-text">Notificações internas on</div></div>
          </div>
        </div>
        <div class="hcard hcard-3">
          <div class="hcard-label">CONVERSÃO</div>
          <div class="hcard-val">34% <span>↑ meta</span></div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ══ DORES ══ -->
<section class="operation-section">
  <div class="container" style="padding:0 0">
    <div class="top-content">
      <div class="text-content">
        <span class="tag">MUITO ALÉM DO MARKETING</span>
        <h2>O problema não está <br/>na entrada de clientes.</h2>
        <h3>Está no que acontece <span>depois</span></h3>
        <p>Mensagens que se perdem, atendimentos sem padrão, processos manuais e falta de controle.</p>
        <p>Quando a operação não acompanha o crescimento, o resultado é retrabalho, atraso e oportunidades desperdiçadas.</p>
      </div>
      <div class="visual-content">
        <img src="dashboard.png" alt="CRM Dashboard" onerror="this.style.display='none'"/>
      </div>
    </div>
    <div class="cards">
      <div class="card">
        <div class="icon green">⌁</div>
        <h4>1. Atendimento</h4>
        <ul>
          <li>Conversas espalhadas</li>
          <li>Respostas lentas</li>
          <li>Falta de histórico</li>
        </ul>
      </div>
      <div class="card">
        <div class="icon purple">⌘</div>
        <h4>2. Processo</h4>
        <ul>
          <li>Tudo manual</li>
          <li>Sem padrão</li>
          <li>Difícil de escalar</li>
        </ul>
      </div>
      <div class="card">
        <div class="icon blue">◔</div>
        <h4>3. Gestão</h4>
        <ul>
          <li>Falta de controle</li>
          <li>Dados perdidos</li>
          <li>Decisões no escuro</li>
        </ul>
      </div>
    </div>
    <div class="bottom-highlight">
      <span>!</span>
      Sem estrutura, crescer só aumenta o <strong>caos.</strong>
    </div>
  </div>
</section>

<!-- ══ SERVIÇOS ══ -->
<section class="sv-section" id="servicos">
  <div class="container">
    <span class="section-tag">O QUE EU FAÇO</span>
    <h2 class="sv-h2">Consultoria Zoho CRM<br/>do diagnóstico à<br/><em style="font-style:normal;background:linear-gradient(90deg,#8b5cf6,#4ade80);-webkit-background-clip:text;-webkit-text-fill-color:transparent">operação rodando.</em></h2>
    <p class="sv-lead">Não entrego só uma ferramenta configurada. Entrego um processo comercial estruturado, automatizado e pronto para escalar — dentro do ecossistema Zoho.</p>
    <div class="sv-grid">
      <div class="sv-card c1">
        <div class="sv-icon ic-purple">⚙</div>
        <h4>Implantação de CRM</h4>
        <p>Configuração completa do Zoho CRM: módulos, campos, pipelines, permissões e funil de vendas adaptado ao seu processo comercial.</p>
        <div class="sv-tags"><span class="sv-pill">Zoho CRM</span><span class="sv-pill">Módulos</span><span class="sv-pill">Pipelines</span></div>
      </div>
      <div class="sv-card c2">
        <div class="sv-icon ic-green">⌁</div>
        <h4>Automações & Workflows</h4>
        <p>Regras de workflow, gatilhos automáticos e notificações internas para que nenhuma oportunidade caia no esquecimento.</p>
        <div class="sv-tags"><span class="sv-pill">Workflows</span><span class="sv-pill">Notificações</span><span class="sv-pill">Gatilhos</span></div>
      </div>
      <div class="sv-card c3">
        <div class="sv-icon ic-blue">◔</div>
        <h4>Dashboards & Métricas</h4>
        <p>Dashboards personalizados para visualizar o funil em tempo real, identificar gargalos e tomar decisões com dados.</p>
        <div class="sv-tags"><span class="sv-pill">Relatórios</span><span class="sv-pill">KPIs</span><span class="sv-pill">Funil</span></div>
      </div>
      <div class="sv-card c4">
        <div class="sv-icon ic-amber">⌘</div>
        <h4>Funções em Deluge</h4>
        <p>Scripts personalizados em Deluge para automatizar cálculos, mail merge, envio de propostas e integrações entre apps Zoho.</p>
        <div class="sv-tags"><span class="sv-pill">Deluge</span><span class="sv-pill">Mail Merge</span><span class="sv-pill">Propostas</span></div>
      </div>
      <div class="sv-card c5">
        <div class="sv-icon ic-pink">◈</div>
        <h4>Zoho Desk & Suporte</h4>
        <p>Implementação do Zoho Desk para centralizar o atendimento pós-venda, tickets e SLA — integrado ao CRM.</p>
        <div class="sv-tags"><span class="sv-pill">Zoho Desk</span><span class="sv-pill">Tickets</span><span class="sv-pill">SLA</span></div>
      </div>
      <div class="sv-card c6">
        <div class="sv-icon ic-mix">◉</div>
        <h4>Ecossistema Zoho One</h4>
        <p>Integração entre as apps do Zoho One para que CRM, suporte, e-mail e relatórios falem entre si — sem depender de terceiros.</p>
        <div class="sv-tags"><span class="sv-pill">Zoho One</span><span class="sv-pill">Integração</span><span class="sv-pill">Ecossistema</span></div>
      </div>
    </div>
    <div class="sv-cta">
      <p>Pronto para estruturar sua operação comercial?</p>
      <a href="#contato">Fale comigo →</a>
    </div>
  </div>
</section>

<!-- ══ PROJETOS ══ -->
<section class="pj-section" id="projetos">
  <div class="container">
    <span class="section-tag">PROJETOS</span>
    <h2 class="pj-h2">Resultados que <span>falam por si.</span></h2>

    <!-- ALS GLOBAL -->
    <div class="pj-card">
      <div class="pj-left">
        <div>
          <div class="pj-client-row">
            <span class="pj-badge-purple">ZOHO CRM</span>
            <span class="pj-industry">Serviços de Testes &amp; Inspeção Global</span>
          </div>
          <h3 class="pj-client-name">ALS Global</h3>
          <div class="pj-role-badge pj-role-purple"><span>◈ Consultor Zoho CRM</span></div>
          <p class="pj-desc">Uma das maiores empresas de testes analíticos do mundo — presente em mais de 65 países, atendendo mineração, ciências da vida e indústria. Com processo comercial distribuído e ferramentas fragmentadas, precisavam de um CRM que unificasse tudo dentro de um único ecossistema.</p>
        </div>
        <div class="pj-switch">
          <span class="pj-switch-from">Microsoft Dynamics 365</span>
          <span class="pj-switch-arrow">→</span>
          <span class="pj-switch-to">Zoho One (CRM + Desk)</span>
        </div>
      </div>
      <div class="pj-right pj-right-dark">
        <div>
          <p class="pj-del-title-purple">O QUE FOI ENTREGUE</p>
          <ul class="pj-del-list">
            <li><span class="dot-purple">1</span>Módulos completos: Negociações, Oportunidades, Empresas, Contatos, Orçamentos e Propostas</li>
            <li><span class="dot-purple">2</span>Workflows para manter o processo comercial rodando sem intervenção manual</li>
            <li><span class="dot-purple">3</span>Regras de layout para garantir preenchimento correto e seguimento do funil</li>
            <li><span class="dot-purple">4</span>Dashboards com métricas de pipeline e sistema de notificação interna de movimentações</li>
            <li><span class="dot-purple">5</span>Funções em Deluge para automações avançadas nas negociações</li>
            <li><span class="dot-purple">6</span>Mail Merge para envio de propostas comerciais diretamente pelo Zoho</li>
            <li><span class="dot-purple">7</span>Zoho Desk implantado e integrado ao CRM para suporte pós-venda</li>
          </ul>
        </div>
      </div>
    </div>

    <!-- VS MICROSOFT -->
    <div class="pj-vs" style="margin-bottom:32px">
      <p class="pj-vs-title">POR QUE ZOHO CRM</p>
      <h3 class="pj-vs-h3">Mais resultado.<br/><span>Menos complexidade.</span></h3>
      <div class="vs-grid">
        <div class="vs-item"><div class="vs-icon-wrap g">✦</div><div><h5>Ecossistema nativo integrado</h5><p>CRM, suporte, e-mail, relatórios e automações dentro de um único ecossistema. No Dynamics, cada módulo adicional custa mais e exige configuração separada.</p></div></div>
        <div class="vs-item"><div class="vs-icon-wrap p">⚡</div><div><h5>Implantação mais rápida</h5><p>Interface intuitiva e configuração sem grandes equipes de TI. O Dynamics exige consultoria especializada cara e ciclos longos de implementação.</p></div></div>
        <div class="vs-item"><div class="vs-icon-wrap b">◎</div><div><h5>Customização sem custo extra</h5><p>Deluge permite criar funções e automações avançadas nativamente. No Dynamics isso requer Power Automate ou Power Apps — licenças adicionais.</p></div></div>
        <div class="vs-item"><div class="vs-icon-wrap a">◈</div><div><h5>Custo-benefício superior</h5><p>Zoho One entrega mais de 45 aplicações integradas por uma fração do custo do pacote equivalente da Microsoft com Dynamics + Power Platform.</p></div></div>
      </div>
      <div class="vs-note">A ALS saiu de uma plataforma cara e fragmentada para um <strong>ecossistema unificado</strong> — com o processo comercial 100% dentro do Zoho.</div>
    </div>

    <!-- TUDO DE FILTRO -->
    <div class="pj-card">
      <div class="pj-left">
        <div>
          <div class="pj-client-row">
            <span class="pj-badge-blue">MARKETING AUTOMATION</span>
            <span class="pj-industry">Tratamento de Água &amp; Purificadores</span>
          </div>
          <h3 class="pj-client-name">Tudo de Filtro</h3>
          <div class="pj-role-badge pj-role-blue"><span>◈ Analista de Marketing</span></div>
          <p class="pj-desc">Empresa especializada em filtros de entrada, purificadores e bebedouros. Operava sem estrutura de marketing digital — sem automação, sem rastreamento do tráfego e sem integração entre canais. O ecossistema Zoho mudou esse cenário completamente.</p>
        </div>
        <div class="tools-row">
          <span class="tool-chip tc-blue">Zoho Marketing Automation</span>
          <span class="tool-chip tc-blue">Zoho Campaigns</span>
          <span class="tool-chip tc-blue">Zoho SalesIQ</span>
          <span class="tool-chip tc-purple">Zoho PageSense</span>
          <span class="tool-chip tc-green">Make</span>
          <span class="tool-chip tc-orange">WATI (WhatsApp)</span>
        </div>
      </div>
      <div class="pj-right pj-right-teal">
        <div>
          <p class="pj-del-title-blue">O QUE FOI IMPLEMENTADO</p>
          <ul class="pj-del-list">
            <li><span class="dot-blue">1</span>Marketing Automation e Zoho Campaigns para nutrição de leads e disparos de e-mail marketing segmentados</li>
            <li><span class="dot-blue">2</span>Zoho SalesIQ integrado ao site para captura e qualificação de visitantes em tempo real</li>
            <li><span class="dot-blue">3</span>Integração do tráfego pago via Make para enviar dados de leads direto ao CRM</li>
            <li><span class="dot-blue">4</span>Zoho PageSense no site para heatmap e análise de comportamento em tempo real</li>
            <li><span class="dot-blue">5</span>Listas de transmissão no WhatsApp via WATI para alcance direto e personalizado</li>
          </ul>
        </div>
        <div class="result-block rb-green">
          <p class="result-label-green">RESULTADO</p>
          <p class="result-number"><em class="result-em-green">R$</em> 100k <em class="result-em-small">em um único dia</em></p>
          <p class="result-sub">Maior faturamento diário da história da empresa — resultado direto da estrutura de marketing implementada.</p>
          <div class="result-before"><s>Teto anterior: R$ 200k/mês</s><em>→ superado em 24h</em></div>
        </div>
      </div>
    </div>

    <!-- GREGO METAL -->
    <div class="pj-card">
      <div class="pj-left">
        <div>
          <div class="pj-client-row">
            <span class="pj-badge-amber">E-COMMERCE</span>
            <span class="pj-industry">Acessórios Premium em Aço Inox</span>
          </div>
          <h3 class="pj-client-name">Grego Metal</h3>
          <div class="pj-role-badge pj-role-amber"><span>◈ Analista de E-commerce &amp; Performance Digital</span></div>
          <p class="pj-desc">Marca voltada ao segmento premium de acessórios e acabamentos em aço inox para ambientes sofisticados. Ao assumir a operação digital, o faturamento diário estava limitado a R$ 10k — sem estrutura de ADS, sem integração de sistemas e sem estratégia de marketplace.</p>
        </div>
        <div class="tools-row">
          <span class="tool-chip tc-amber">Mercado Livre</span>
          <span class="tool-chip tc-amber">Shopee</span>
          <span class="tool-chip tc-amber">Amazon</span>
          <span class="tool-chip tc-gray">Bling ERP</span>
          <span class="tool-chip tc-green">Olist</span>
          <span class="tool-chip tc-blue">Google Ads</span>
          <span class="tool-chip tc-blue">Meta Ads</span>
          <span class="tool-chip tc-gray">Loja Integrada</span>
        </div>
      </div>
      <div class="pj-right pj-right-amber">
        <div>
          <p class="pj-del-title-amber">O QUE FOI IMPLEMENTADO</p>
          <ul class="pj-del-list">
            <li><span class="dot-amber">1</span>Gestão estratégica dos principais marketplaces com otimização de catálogo e posicionamento</li>
            <li><span class="dot-amber">2</span>Campanhas patrocinadas (ADS) nos marketplaces e plataformas digitais com foco em ROAS</li>
            <li><span class="dot-amber">3</span>Estratégias de precificação competitiva e gestão de buybox</li>
            <li><span class="dot-amber">4</span>Integração operacional com Bling e Olist para sincronização de estoque e pedidos</li>
            <li><span class="dot-amber">5</span>Manutenção e otimização do e-commerce na Loja Integrada</li>
            <li><span class="dot-amber">6</span>E-mail marketing e comunicação digital para base de clientes</li>
            <li><span class="dot-amber">7</span>Análise de indicadores de performance e relatórios de crescimento</li>
          </ul>
        </div>
        <div class="result-block rb-amber">
          <p class="result-label-amber">RESULTADO</p>
          <div class="result-row">
            <span class="result-from">R$ 10k</span>
            <span class="result-arrow">→</span>
            <span class="result-to">R$ 40k<em style="font-size:16px;color:rgba(255,255,255,0.4)">/dia</em></span>
          </div>
          <p class="result-sub">Crescimento de 4x no faturamento diário com implementação de ADS e estruturação da operação digital.</p>
          <div class="result-growth"><span>↑ 300% de crescimento no faturamento diário</span></div>
        </div>
      </div>
    </div>

  </div>
</section>

<!-- ══ SOBRE ══ -->
<section class="sobre-section" id="sobre">
  <div class="container">
    <div class="sobre-inner">
      <div class="sobre-text">
        <span class="section-tag">SOBRE</span>
        <h2>Design com propósito.<br/><span>Dados com intenção.</span></h2>
        <p>Sou Rianderson Manrrique, 22 anos, de São José dos Campos. Consultor Zoho CRM e designer com visão estratégica — une criatividade e análise para entregar resultados reais.</p>
        <p>Minha trajetória passa por e-commerce, marketplaces, marketing digital e automações — experiências que me tornaram um profissional que entende o negócio inteiro, não só a ferramenta.</p>
        <p style="font-size:16px;font-style:italic;color:#9ca3af;border-left:3px solid #8b5cf6;padding-left:20px;margin-top:8px">"O Manrrique Creative Design Studio é um espaço onde o design vai além da estética: é uma ferramenta para criar experiências autênticas."</p>
        <div class="sobre-chips">
          <span class="sobre-chip">Zoho CRM</span>
          <span class="sobre-chip">Deluge</span>
          <span class="sobre-chip">Marketing Automation</span>
          <span class="sobre-chip">E-commerce</span>
          <span class="sobre-chip">ADS</span>
          <span class="sobre-chip">Design</span>
        </div>
      </div>
      <div class="sobre-visual">
        <div class="sobre-card">
          <div class="sobre-card-icon">⚙</div>
          <h4>Consultoria Zoho CRM</h4>
          <p>Implantação completa do ecossistema Zoho — do CRM ao Desk, com automações, dashboards e funções em Deluge.</p>
        </div>
        <div class="sobre-card">
          <div class="sobre-card-icon">◔</div>
          <h4>Performance Digital</h4>
          <p>ADS, marketplaces, e-mail marketing e integrações que conectam tráfego ao CRM e transformam leads em faturamento.</p>
        </div>
        <div class="sobre-card">
          <div class="sobre-card-icon">✦</div>
          <h4>Design Criativo</h4>
          <p>Identidade visual, artes para redes sociais e sites — comunicação visual que atrai, converte e representa a marca.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ══ CONTATO ══ -->
<section class="contato-section" id="contato">
  <div class="container">
    <div class="contato-inner">
      <span class="section-tag">CONTATO</span>
      <h2>Vamos estruturar sua<br/><span>operação juntos?</span></h2>
      <p>Se você quer organizar seu processo comercial, implantar o Zoho ou escalar suas vendas digitais — me chama. Respondo rápido.</p>
      <div class="contato-cards">
        <a class="cc" href="mailto:Rianderson.manrrique0@gmail.com">
          <div class="cc-icon">✉</div>
          <h4>E-mail</h4>
          <p>Rianderson.manrrique0@gmail.com</p>
        </a>
        <a class="cc" href="tel:+5511996437620">
          <div class="cc-icon">☎</div>
          <h4>Telefone</h4>
          <p>11 9 9643-7620</p>
        </a>
        <a class="cc" href="https://www.instagram.com/manrrique_rian/" target="_blank">
          <div class="cc-icon">◈</div>
          <h4>Instagram</h4>
          <p>@manrrique_rian</p>
        </a>
      </div>
      <div class="contato-cta">
        <h3>São José dos Campos, SP</h3>
        <p>Atendo presencialmente na região e remotamente para todo o Brasil.</p>
        <a href="mailto:Rianderson.manrrique0@gmail.com">Enviar mensagem →</a>
      </div>
    </div>
  </div>
</section>

<!-- ══ FOOTER ══ -->
<footer>
  <div class="footer-logo">Rian <span>Manrrique</span></div>
  <div class="footer-links">
    <a href="#servicos">Serviços</a>
    <a href="#projetos">Projetos</a>
    <a href="#sobre">Sobre</a>
    <a href="https://www.instagram.com/manrrique_rian/" target="_blank">Instagram</a>
    <a href="https://rianmanrrik27.wixstudio.com/portifolio" target="_blank">Portfólio Design</a>
  </div>
  <div class="footer-copy">© 2025 Rian Manrrique · Consultor Zoho CRM</div>
</footer>

</body>
</html>
