# diadieuf
site de vente
[index.html.html](https://github.com/user-attachments/files/28321328/index.html.html)
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Diadieuf — Cartes de Vœux, Fêtes & Cadeaux d'Entreprise 🇸🇳</title>
<link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&family=Instrument+Serif:ital@0;1&display=swap" rel="stylesheet">
<style>
:root{
  --or:#F25A0A;--or2:#FF7A30;--or3:#FF9A60;--or-light:#FFF0E8;--or-dark:#C04500;
  --ink:#0A0806;--white:#FFFFFF;--grey:#F5F2EF;--grey2:#EAE6E1;--grey3:#B0A898;
  --txt:#2A2218;--txt2:#6A5E50;--border:#E8E0D5;--shadow:rgba(242,90,10,0.12);
  --green:#00A651;--blue:#0066CC;--red:#E02020;
  --card-r:20px;
}
*{margin:0;padding:0;box-sizing:border-box;}
html{scroll-behavior:smooth;}
body{font-family:'Plus Jakarta Sans',sans-serif;background:var(--grey);color:var(--txt);min-height:100vh;}

/* ─── TOPBAR ─── */
.topbar{background:var(--or);color:#fff;text-align:center;padding:8px;font-size:.75rem;font-weight:600;letter-spacing:.06em;}

/* ─── NAV ─── */
nav{background:#fff;border-bottom:1px solid var(--border);position:sticky;top:0;z-index:100;box-shadow:0 2px 12px rgba(0,0,0,.06);}
.nav-inner{max-width:1200px;margin:0 auto;padding:0 20px;height:64px;display:flex;align-items:center;justify-content:space-between;gap:1rem;}
.nav-logo{display:flex;align-items:center;gap:10px;cursor:pointer;text-decoration:none;}
.nav-logo-icon{width:40px;height:40px;background:linear-gradient(135deg,var(--or),var(--or2));border-radius:12px;display:flex;align-items:center;justify-content:center;font-size:1.3rem;box-shadow:0 4px 12px var(--shadow);}
.nav-logo-text{font-family:'Instrument Serif',serif;font-size:1.5rem;color:var(--ink);font-style:italic;}
.nav-logo-text span{color:var(--or);}
.nav-right{display:flex;align-items:center;gap:.8rem;}
.nav-cart-btn{background:var(--or);color:#fff;border:none;padding:10px 20px;border-radius:30px;font-family:'Plus Jakarta Sans',sans-serif;font-size:.85rem;font-weight:700;cursor:pointer;display:flex;align-items:center;gap:8px;transition:all .2s;box-shadow:0 4px 12px var(--shadow);}
.nav-cart-btn:hover{background:var(--or-dark);transform:translateY(-1px);}
.cbadge{background:#fff;color:var(--or);border-radius:50%;width:20px;height:20px;font-size:.72rem;display:flex;align-items:center;justify-content:center;font-weight:800;}
.nav-flag{font-size:1.2rem;}

/* ─── HERO ─── */
.hero{background:linear-gradient(135deg,var(--or-dark) 0%,var(--or) 50%,var(--or2) 100%);color:#fff;padding:3rem 20px 4rem;position:relative;overflow:hidden;}
.hero::before{content:'';position:absolute;inset:0;background:url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none'%3E%3Ccircle cx='30' cy='30' r='20' stroke='rgba(255,255,255,0.06)' stroke-width='1'/%3E%3Ccircle cx='0' cy='0' r='20' stroke='rgba(255,255,255,0.04)' stroke-width='1'/%3E%3Ccircle cx='60' cy='60' r='20' stroke='rgba(255,255,255,0.04)' stroke-width='1'/%3E%3C/g%3E%3C/svg%3E");}
.hero-inner{max-width:1200px;margin:0 auto;position:relative;z-index:1;display:grid;grid-template-columns:1fr auto;align-items:center;gap:2rem;}
.hero-tag{display:inline-block;background:rgba(255,255,255,.2);backdrop-filter:blur(8px);border:1px solid rgba(255,255,255,.3);padding:5px 14px;border-radius:20px;font-size:.72rem;font-weight:700;letter-spacing:.1em;text-transform:uppercase;margin-bottom:1rem;}
.hero h1{font-family:'Instrument Serif',serif;font-size:clamp(2rem,4vw,3rem);line-height:1.15;margin-bottom:.8rem;font-weight:400;}
.hero h1 strong{font-weight:400;font-style:italic;}
.hero-sub{font-size:.95rem;opacity:.85;line-height:1.7;max-width:480px;margin-bottom:1.5rem;}
.hero-actions{display:flex;gap:.8rem;flex-wrap:wrap;}
.btn-white{background:#fff;color:var(--or);border:none;padding:12px 24px;border-radius:30px;font-family:'Plus Jakarta Sans',sans-serif;font-size:.88rem;font-weight:700;cursor:pointer;transition:all .2s;box-shadow:0 4px 16px rgba(0,0,0,.15);}
.btn-white:hover{transform:translateY(-2px);box-shadow:0 8px 24px rgba(0,0,0,.2);}
.btn-outline{background:transparent;color:#fff;border:2px solid rgba(255,255,255,.5);padding:12px 24px;border-radius:30px;font-family:'Plus Jakarta Sans',sans-serif;font-size:.88rem;font-weight:600;cursor:pointer;transition:all .2s;}
.btn-outline:hover{border-color:#fff;background:rgba(255,255,255,.1);}
.hero-stats{display:flex;gap:1.5rem;flex-wrap:wrap;}
.hero-stat{text-align:center;}
.hero-stat-num{font-size:1.5rem;font-weight:800;display:block;}
.hero-stat-lbl{font-size:.72rem;opacity:.75;}
.hero-cards-preview{display:flex;gap:-10px;position:relative;}
.preview-card{width:90px;height:120px;border-radius:12px;box-shadow:0 8px 24px rgba(0,0,0,.25);overflow:hidden;border:2px solid rgba(255,255,255,.3);}
.preview-card:nth-child(2){transform:rotate(5deg) translateX(-10px);}
.preview-card:nth-child(3){transform:rotate(-3deg) translateX(-20px);}
.preview-card svg{width:100%;height:100%;}

/* ─── PAY BANNER ─── */
.pay-banner{background:#fff;border-bottom:1px solid var(--border);}
.pay-banner-inner{max-width:1200px;margin:0 auto;padding:14px 20px;display:flex;align-items:center;justify-content:center;gap:2rem;flex-wrap:wrap;}
.pay-item{display:flex;align-items:center;gap:8px;font-size:.82rem;font-weight:600;color:var(--txt2);}
.pay-item .pi{width:32px;height:32px;border-radius:8px;display:flex;align-items:center;justify-content:center;font-size:1rem;}
.pi-or{background:#FF6200;color:#fff;}
.pi-wv{background:#0066CC;color:#fff;}
.pi-cb{background:linear-gradient(135deg,#1A1A2E,#16213E);color:#fff;}
.pi-visa{background:#1A1F71;color:#fff;font-size:.6rem;font-weight:900;}

/* ─── MAIN ─── */
.main{max-width:1200px;margin:0 auto;padding:2rem 20px 4rem;}

/* ─── CATÉGORIE TABS ─── */
.cat-tabs{display:flex;gap:.5rem;overflow-x:auto;padding-bottom:.5rem;margin-bottom:2rem;scrollbar-width:none;}
.cat-tabs::-webkit-scrollbar{display:none;}
.cat-tab{display:flex;align-items:center;gap:6px;padding:10px 18px;border-radius:30px;border:1.5px solid var(--border);background:#fff;font-size:.83rem;font-weight:600;cursor:pointer;transition:all .2s;white-space:nowrap;color:var(--txt2);}
.cat-tab:hover{border-color:var(--or);color:var(--or);}
.cat-tab.on{background:var(--or);color:#fff;border-color:var(--or);box-shadow:0 4px 12px var(--shadow);}

/* ─── SECTION CATÉGORIE ─── */
.cat-section{margin-bottom:3rem;}
.cat-section-header{display:flex;align-items:center;gap:12px;margin-bottom:1.5rem;padding-bottom:1rem;border-bottom:2px solid var(--border);}
.cat-section-icon{width:44px;height:44px;background:var(--or-light);border-radius:12px;display:flex;align-items:center;justify-content:center;font-size:1.4rem;}
.cat-section-title{font-family:'Instrument Serif',serif;font-size:1.5rem;font-style:italic;}
.cat-section-count{background:var(--or-light);color:var(--or);padding:3px 10px;border-radius:20px;font-size:.75rem;font-weight:700;margin-left:auto;}

/* ─── GRILLE CARTES ─── */
.cards-row{display:grid;grid-template-columns:repeat(4,1fr);gap:1.2rem;}
@media(max-width:900px){.cards-row{grid-template-columns:repeat(2,1fr);}}
@media(max-width:500px){.cards-row{grid-template-columns:1fr 1fr;gap:.8rem;}}

/* ─── CARTE PRODUIT ─── */
.pcard{background:#fff;border-radius:var(--card-r);overflow:hidden;cursor:pointer;transition:all .3s cubic-bezier(.4,0,.2,1);border:1.5px solid var(--border);position:relative;}
.pcard:hover{box-shadow:0 16px 40px rgba(0,0,0,.12);transform:translateY(-4px);border-color:var(--or3);}
.pcard-img{height:180px;position:relative;overflow:hidden;}
.pcard-img svg{width:100%;height:100%;display:block;}
.pcard-badge{position:absolute;top:8px;left:8px;padding:3px 9px;border-radius:10px;font-size:.65rem;font-weight:700;letter-spacing:.04em;}
.pb-new{background:var(--or);color:#fff;}
.pb-best{background:#FFD700;color:#0A0806;}
.pb-prem{background:linear-gradient(135deg,#C8922A,#E8C060);color:#fff;}
.pcard-music{position:absolute;bottom:8px;right:8px;background:rgba(0,0,0,.6);backdrop-filter:blur(6px);color:#fff;padding:4px 9px;border-radius:10px;font-size:.62rem;font-weight:600;display:flex;align-items:center;gap:4px;}
.pcard-info{padding:.9rem 1rem 1rem;}
.pcard-name{font-weight:700;font-size:.9rem;margin-bottom:2px;color:var(--ink);}
.pcard-cat{font-size:.72rem;color:var(--txt2);margin-bottom:.7rem;}
.pcard-foot{display:flex;align-items:center;justify-content:space-between;}
.pcard-price{font-weight:800;font-size:.95rem;color:var(--or);}
.pcard-add{background:var(--or);color:#fff;border:none;width:32px;height:32px;border-radius:50%;font-size:1.1rem;cursor:pointer;display:flex;align-items:center;justify-content:center;transition:all .2s;box-shadow:0 3px 8px var(--shadow);}
.pcard-add:hover{background:var(--or-dark);transform:scale(1.1);}

/* ─── DRAWER PANIER ─── */
.cart-overlay{position:fixed;inset:0;background:rgba(0,0,0,.4);z-index:400;opacity:0;pointer-events:none;transition:opacity .3s;backdrop-filter:blur(3px);}
.cart-overlay.open{opacity:1;pointer-events:all;}
.cart-drawer{position:fixed;right:0;top:0;bottom:0;width:420px;max-width:100vw;background:#fff;z-index:401;transform:translateX(100%);transition:transform .35s cubic-bezier(.4,0,.2,1);display:flex;flex-direction:column;box-shadow:-8px 0 40px rgba(0,0,0,.15);}
.cart-drawer.open{transform:translateX(0);}
.cart-header{background:var(--or);color:#fff;padding:1.2rem 1.5rem;display:flex;align-items:center;justify-content:space-between;}
.cart-header h3{font-size:1.1rem;font-weight:700;}
.cart-close{background:rgba(255,255,255,.2);border:none;color:#fff;width:34px;height:34px;border-radius:50%;font-size:1.2rem;cursor:pointer;display:flex;align-items:center;justify-content:center;transition:background .2s;}
.cart-close:hover{background:rgba(255,255,255,.3);}
.cart-items-list{flex:1;overflow-y:auto;padding:1rem 1.5rem;}
.cart-item{display:flex;gap:.9rem;padding:.9rem 0;border-bottom:1px solid var(--border);}
.cart-item:last-child{border-bottom:none;}
.ci-thumb{width:56px;height:75px;border-radius:10px;overflow:hidden;flex-shrink:0;border:1px solid var(--border);}
.ci-thumb svg{width:100%;height:100%;}
.ci-info{flex:1;}
.ci-name{font-weight:700;font-size:.85rem;margin-bottom:2px;}
.ci-meta{font-size:.72rem;color:var(--txt2);line-height:1.5;}
.ci-tags{display:flex;gap:.4rem;flex-wrap:wrap;margin-top:.3rem;}
.ci-tag{padding:2px 7px;border-radius:8px;font-size:.65rem;font-weight:700;}
.ci-tag-or{background:#FFF0E0;color:var(--or);}
.ci-tag-wv{background:#E0EEFF;color:var(--blue);}
.ci-tag-mu{background:#E8FFE8;color:var(--green);}
.ci-right{display:flex;flex-direction:column;align-items:flex-end;gap:.4rem;}
.ci-price{font-weight:800;font-size:.88rem;color:var(--or);}
.ci-del{background:none;border:none;color:var(--grey3);cursor:pointer;font-size:.9rem;padding:4px;transition:color .2s;}
.ci-del:hover{color:var(--red);}
.cart-footer{padding:1rem 1.5rem;border-top:1px solid var(--border);background:var(--grey);}
.cart-summary-rows{margin-bottom:1rem;}
.cs-row{display:flex;justify-content:space-between;padding:5px 0;font-size:.83rem;color:var(--txt2);}
.cs-row.tot{font-weight:800;font-size:1rem;color:var(--ink);padding-top:.5rem;border-top:1px solid var(--border);margin-top:.3rem;}
.cs-row.tot span:last-child{color:var(--or);}
.checkout-btn{background:var(--or);color:#fff;border:none;padding:15px;border-radius:14px;font-family:'Plus Jakarta Sans',sans-serif;font-size:1rem;font-weight:700;cursor:pointer;width:100%;transition:all .25s;box-shadow:0 4px 16px var(--shadow);}
.checkout-btn:hover{background:var(--or-dark);transform:translateY(-1px);}
.cart-empty{text-align:center;padding:3rem 1rem;color:var(--txt2);}
.cart-empty .cei{font-size:3rem;margin-bottom:.8rem;}
.cart-empty p{font-size:.88rem;}

/* ─── MODAL ÉDITEUR ─── */
.modal-ov{display:none;position:fixed;inset:0;z-index:500;background:rgba(0,0,0,.5);backdrop-filter:blur(4px);align-items:center;justify-content:center;padding:1rem;}
.modal-ov.open{display:flex;}
.modal-box{background:#fff;border-radius:24px;width:100%;max-width:760px;max-height:90vh;overflow-y:auto;animation:mIn .3s ease;}
.modal-top{background:linear-gradient(135deg,var(--or-dark),var(--or));color:#fff;padding:1.5rem 2rem;border-radius:24px 24px 0 0;display:flex;align-items:center;justify-content:space-between;}
.modal-top h2{font-family:'Instrument Serif',serif;font-size:1.4rem;font-style:italic;}
.modal-close{background:rgba(255,255,255,.2);border:none;color:#fff;width:34px;height:34px;border-radius:50%;font-size:1.3rem;cursor:pointer;display:flex;align-items:center;justify-content:center;}
.modal-body{padding:1.5rem 2rem;display:grid;grid-template-columns:1fr 1fr;gap:1.5rem;}
@media(max-width:600px){.modal-body{grid-template-columns:1fr;}}

/* FLIP PREVIEW */
.flip-scene{width:100%;aspect-ratio:3/4;perspective:1200px;cursor:pointer;max-width:220px;margin:0 auto;}
.flip-inner{width:100%;height:100%;position:relative;transform-style:preserve-3d;transition:transform .8s cubic-bezier(.4,0,.2,1);}
.flip-inner.flipped{transform:rotateY(180deg);}
.flip-f,.flip-b{position:absolute;inset:0;border-radius:16px;backface-visibility:hidden;overflow:hidden;box-shadow:0 12px 36px rgba(0,0,0,.15);}
.flip-b{transform:rotateY(180deg);}
.flip-f svg,.flip-b svg{width:100%;height:100%;}
.recto-ol{position:absolute;inset:0;background:linear-gradient(to top,rgba(0,0,0,.72),rgba(0,0,0,.1) 55%,transparent);display:flex;flex-direction:column;justify-content:flex-end;padding:1rem;}
.ro-title{font-family:'Instrument Serif',serif;font-size:1.1rem;font-style:italic;color:#fff;margin-bottom:.3rem;}
.ro-msg{font-size:.68rem;color:rgba(255,255,255,.8);line-height:1.5;margin-bottom:.4rem;}
.ro-gift{font-size:.62rem;font-weight:700;padding:3px 8px;border-radius:8px;display:none;margin-bottom:.2rem;}
.ro-gift.show{display:inline-block;}
.ro-gift-or{background:rgba(255,98,0,.3);color:#FFCC99;border:1px solid rgba(255,98,0,.4);}
.ro-gift-wv{background:rgba(0,102,204,.25);color:#99CCFF;border:1px solid rgba(0,102,204,.4);}
.ro-music{font-size:.6rem;color:rgba(255,255,255,.7);display:flex;align-items:center;gap:3px;}
.ro-sig{font-size:.62rem;color:rgba(255,255,255,.5);font-style:italic;align-self:flex-end;}
.flip-actions{display:flex;gap:.5rem;justify-content:center;margin-top:.7rem;}
.fa-btn{padding:6px 14px;border-radius:14px;font-size:.75rem;font-weight:600;cursor:pointer;border:1.5px solid var(--border);background:#fff;transition:all .2s;display:flex;align-items:center;gap:5px;}
.fa-btn:hover{border-color:var(--or);color:var(--or);}
.fa-btn.primary{background:var(--or);color:#fff;border-color:var(--or);}

/* VERSO CHOOSER */
.verso-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:.5rem;margin-bottom:.9rem;}
.vt{border:2px solid var(--border);border-radius:10px;overflow:hidden;cursor:pointer;transition:all .2s;}
.vt:hover{transform:translateY(-2px);}
.vt.on{border-color:var(--or);}
.vt-img{height:44px;}
.vt-img svg{width:100%;height:100%;}
.vt-name{font-size:.62rem;font-weight:700;color:var(--txt2);text-align:center;padding:.25rem 0;}

/* FORMS */
.f-sec{background:var(--grey);border-radius:14px;padding:1.1rem;margin-bottom:.9rem;}
.f-sec-title{font-weight:700;font-size:.83rem;margin-bottom:.8rem;display:flex;align-items:center;gap:.4rem;}
.fg{margin-bottom:.7rem;}
.fg:last-child{margin-bottom:0;}
.fg label{display:block;font-size:.75rem;font-weight:600;color:var(--txt2);margin-bottom:4px;}
.fg input,.fg textarea,.fg select{width:100%;border:1.5px solid var(--border);border-radius:10px;padding:9px 12px;font-family:'Plus Jakarta Sans',sans-serif;font-size:.85rem;color:var(--ink);background:#fff;outline:none;transition:border-color .2s;resize:vertical;}
.fg input:focus,.fg textarea:focus,.fg select:focus{border-color:var(--or);}

/* GIFT TOGGLE */
.gift-toggle-row{display:flex;align-items:center;gap:9px;cursor:pointer;padding:.7rem;background:#fff;border-radius:10px;border:1.5px solid var(--border);margin-bottom:.8rem;transition:border-color .2s;}
.gift-toggle-row:hover{border-color:var(--or3);}
.tgsw{width:42px;height:23px;background:var(--border);border-radius:12px;position:relative;transition:background .25s;flex-shrink:0;}
.tgsw::after{content:'';position:absolute;top:2.5px;left:2.5px;width:18px;height:18px;background:#fff;border-radius:50%;transition:transform .25s;box-shadow:0 1px 3px rgba(0,0,0,.2);}
.tgsw.on{background:var(--or);}
.tgsw.on::after{transform:translateX(19px);}
.gift-lbl{font-size:.85rem;font-weight:600;}
.gift-body{display:none;flex-direction:column;gap:.7rem;}
.gift-body.open{display:flex;}
.ops{display:grid;grid-template-columns:1fr 1fr;gap:.6rem;}
.op-btn{border:2px solid var(--border);border-radius:12px;padding:10px 8px;text-align:center;cursor:pointer;transition:all .2s;background:#fff;}
.op-btn.sel-or{border-color:var(--or);background:#FFF5EE;}
.op-btn.sel-wv{border-color:var(--blue);background:#EEF5FF;}
.op-icon{font-size:1.5rem;margin-bottom:2px;}
.op-name{font-size:.72rem;font-weight:700;}
.amts{display:flex;flex-wrap:wrap;gap:.4rem;}
.achip{padding:5px 11px;border-radius:12px;border:1.5px solid var(--border);font-size:.75rem;font-weight:600;cursor:pointer;background:#fff;transition:all .2s;}
.achip:hover{border-color:var(--or);color:var(--or);}
.achip.on{background:var(--or);color:#fff;border-color:var(--or);}

/* MUSIC IN CARD - pre-set */
.music-info-box{background:linear-gradient(135deg,#0A0820,#1A1040);border-radius:12px;padding:1rem;color:#fff;}
.music-info-box .mib-title{font-weight:700;font-size:.83rem;margin-bottom:.2rem;color:#fff;}
.music-info-box .mib-sub{font-size:.7rem;color:rgba(255,255,255,.5);margin-bottom:.8rem;}
.music-track-display{display:flex;align-items:center;gap:.8rem;padding:.7rem;background:rgba(255,255,255,.08);border-radius:10px;border:1px solid rgba(255,255,255,.12);}
.mtd-icon{width:36px;height:36px;border-radius:8px;background:#1DB954;display:flex;align-items:center;justify-content:center;font-size:1rem;flex-shrink:0;}
.mtd-info{flex:1;}
.mtd-name{font-size:.8rem;font-weight:600;color:#fff;}
.mtd-artist{font-size:.68rem;color:rgba(255,255,255,.6);}
.mtd-play{font-size:1.1rem;cursor:pointer;color:#1DB954;transition:transform .2s;}
.mtd-play:hover{transform:scale(1.1);}
.np-anim{display:flex;gap:2px;align-items:flex-end;height:14px;}
.np-b{width:3px;background:#1DB954;border-radius:2px;animation:eq .7s ease-in-out infinite;}
.np-b:nth-child(2){animation-delay:.2s;}
.np-b:nth-child(3){animation-delay:.4s;}

.add-to-cart-btn{background:var(--or);color:#fff;border:none;padding:14px;border-radius:14px;font-family:'Plus Jakarta Sans',sans-serif;font-size:.95rem;font-weight:700;cursor:pointer;width:100%;margin-top:.5rem;transition:all .25s;box-shadow:0 4px 16px var(--shadow);display:flex;align-items:center;justify-content:center;gap:8px;}
.add-to-cart-btn:hover{background:var(--or-dark);transform:translateY(-1px);}

/* ─── MODAL PAIEMENT ─── */
.pay-modal-ov{display:none;position:fixed;inset:0;z-index:600;background:rgba(0,0,0,.55);backdrop-filter:blur(5px);align-items:center;justify-content:center;padding:1rem;}
.pay-modal-ov.open{display:flex;}
.pay-modal{background:#fff;border-radius:24px;width:100%;max-width:480px;max-height:90vh;overflow-y:auto;animation:mIn .3s ease;}
.pay-modal-header{background:linear-gradient(135deg,var(--or-dark),var(--or));color:#fff;padding:1.5rem 1.8rem;border-radius:24px 24px 0 0;display:flex;align-items:center;justify-content:space-between;}
.pay-modal-header h3{font-family:'Instrument Serif',serif;font-size:1.3rem;font-style:italic;}
.pay-modal-body{padding:1.5rem 1.8rem;}

/* ÉTAPES PAIEMENT */
.pay-steps{display:flex;gap:.4rem;margin-bottom:1.5rem;}
.ps{flex:1;height:4px;border-radius:2px;background:var(--border);transition:background .3s;}
.ps.done{background:var(--or);}
.ps.active{background:var(--or3);}

/* MÉTHODES PAIEMENT */
.pay-methods-grid{display:grid;grid-template-columns:1fr 1fr 1fr;gap:.6rem;margin-bottom:1.2rem;}
.pmb{border:2px solid var(--border);border-radius:14px;padding:12px 8px;text-align:center;cursor:pointer;transition:all .2s;background:#fff;}
.pmb:hover{transform:translateY(-2px);box-shadow:0 4px 12px rgba(0,0,0,.08);}
.pmb.on{border-color:var(--or);background:var(--or-light);}
.pmb-icon{font-size:1.5rem;margin-bottom:4px;}
.pmb-name{font-size:.7rem;font-weight:700;color:var(--txt2);}
.pmb.on .pmb-name{color:var(--or);}

/* CARTE BANCAIRE FORM */
.card-form{background:var(--grey);border-radius:16px;padding:1.2rem;margin-bottom:1rem;}
.card-preview-box{background:linear-gradient(135deg,#1A1A2E 0%,#16213E 50%,#0F3460 100%);border-radius:14px;padding:1.2rem;margin-bottom:1rem;color:#fff;position:relative;overflow:hidden;}
.card-preview-box::before{content:'';position:absolute;top:-30%;right:-10%;width:200px;height:200px;border-radius:50%;background:rgba(255,255,255,.04);}
.cpb-chip{width:32px;height:24px;background:linear-gradient(135deg,#D4A800,#FFD700);border-radius:5px;margin-bottom:.8rem;}
.cpb-num{font-size:1.1rem;font-weight:600;letter-spacing:.18em;margin-bottom:.8rem;font-family:monospace;}
.cpb-row{display:flex;justify-content:space-between;}
.cpb-label{font-size:.6rem;opacity:.6;margin-bottom:2px;}
.cpb-val{font-size:.8rem;font-weight:600;}
.cpb-visa{position:absolute;bottom:1rem;right:1rem;font-size:.7rem;font-weight:900;opacity:.8;}
.card-logos{position:absolute;top:1rem;right:1rem;display:flex;gap:4px;}
.cl-circle{width:20px;height:20px;border-radius:50%;}

.pay-info-box{background:var(--grey);border-radius:12px;padding:.8rem 1rem;font-size:.77rem;color:var(--txt2);display:flex;gap:.6rem;margin-bottom:1rem;line-height:1.5;}
.pay-secure-badges{display:flex;gap:.6rem;justify-content:center;margin-bottom:1rem;flex-wrap:wrap;}
.psb{display:flex;align-items:center;gap:4px;font-size:.68rem;color:var(--txt2);font-weight:600;}
.pay-total-row{display:flex;justify-content:space-between;align-items:center;padding:.8rem 1rem;background:var(--or-light);border-radius:12px;margin-bottom:1rem;border:1px solid var(--or3);}
.ptr-lbl{font-size:.85rem;font-weight:600;}
.ptr-amt{font-size:1.1rem;font-weight:800;color:var(--or);}
.pay-confirm-btn{background:var(--or);color:#fff;border:none;padding:15px;border-radius:14px;font-family:'Plus Jakarta Sans',sans-serif;font-size:1rem;font-weight:700;cursor:pointer;width:100%;transition:all .25s;box-shadow:0 4px 16px var(--shadow);}
.pay-confirm-btn:hover{background:var(--or-dark);}

/* SUCCESS */
.succ-screen{text-align:center;padding:2rem 1rem;}
.succ-icon{width:72px;height:72px;background:linear-gradient(135deg,var(--or),var(--or2));border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:2rem;margin:0 auto 1rem;box-shadow:0 8px 24px var(--shadow);}
.succ-screen h3{font-family:'Instrument Serif',serif;font-size:1.5rem;margin-bottom:.5rem;}
.succ-screen p{font-size:.88rem;color:var(--txt2);line-height:1.7;margin-bottom:1.5rem;}
.succ-ref{background:var(--grey);border-radius:10px;padding:.6rem 1rem;display:inline-block;font-size:.8rem;font-weight:700;color:var(--or);margin-bottom:1.5rem;}

/* ─── FOOTER ─── */
footer{background:var(--ink);color:rgba(255,255,255,.5);padding:2.5rem 20px;margin-top:2rem;}
.footer-inner{max-width:1200px;margin:0 auto;display:grid;grid-template-columns:1fr 1fr 1fr;gap:2rem;}
.footer-brand .fb-logo{font-family:'Instrument Serif',serif;font-size:1.5rem;font-style:italic;color:#fff;margin-bottom:.4rem;}
.footer-brand .fb-logo span{color:var(--or);}
.footer-brand p{font-size:.8rem;line-height:1.6;}
.footer-links h4{font-size:.83rem;font-weight:700;color:#fff;margin-bottom:.8rem;}
.footer-links a{display:block;font-size:.78rem;color:rgba(255,255,255,.5);text-decoration:none;margin-bottom:.4rem;transition:color .2s;cursor:pointer;}
.footer-links a:hover{color:var(--or);}
.footer-bottom{max-width:1200px;margin:.2rem auto 0;border-top:1px solid rgba(255,255,255,.1);padding-top:1.2rem;display:flex;justify-content:space-between;font-size:.75rem;flex-wrap:wrap;gap:.5rem;}

/* ─── TOAST ─── */
.toast{position:fixed;bottom:1.5rem;left:50%;transform:translateX(-50%) translateY(100px);background:var(--ink);color:#fff;padding:12px 20px;border-radius:30px;font-size:.85rem;font-weight:600;display:flex;align-items:center;gap:8px;z-index:700;opacity:0;transition:all .35s cubic-bezier(.34,1.56,.64,1);box-shadow:0 8px 24px rgba(0,0,0,.25);white-space:nowrap;}
.toast.show{transform:translateX(-50%) translateY(0);opacity:1;}
.toast-dot{width:8px;height:8px;border-radius:50%;background:var(--or);flex-shrink:0;}

@keyframes mIn{from{opacity:0;transform:scale(.96) translateY(16px)}to{opacity:1;transform:scale(1) translateY(0)}}
@keyframes eq{0%,100%{height:5px}50%{height:13px}}
@keyframes fadeUp{from{opacity:0;transform:translateY(20px)}to{opacity:1;transform:translateY(0)}}

/* ─── BUYER FORM MODAL ─── */
.buyer-modal-ov{display:none;position:fixed;inset:0;z-index:550;background:rgba(0,0,0,.55);backdrop-filter:blur(5px);align-items:center;justify-content:center;padding:1rem;}
.buyer-modal-ov.open{display:flex;}
.buyer-modal{background:#fff;border-radius:24px;width:100%;max-width:460px;animation:mIn .3s ease;overflow:hidden;}
.buyer-modal-top{background:linear-gradient(135deg,var(--or-dark),var(--or));color:#fff;padding:1.4rem 1.8rem;display:flex;align-items:center;justify-content:space-between;}
.buyer-modal-top h3{font-family:'Instrument Serif',serif;font-size:1.3rem;font-style:italic;}
.buyer-modal-body{padding:1.5rem 1.8rem;}
.buyer-modal-body .fg{margin-bottom:.9rem;}
.buyer-modal-body .fg label{display:block;font-size:.78rem;font-weight:700;color:var(--txt2);margin-bottom:5px;}
.buyer-modal-body .fg input{width:100%;border:1.5px solid var(--border);border-radius:10px;padding:11px 14px;font-family:'Plus Jakarta Sans',sans-serif;font-size:.9rem;color:var(--ink);background:#FDFAF6;outline:none;transition:border-color .2s;}
.buyer-modal-body .fg input:focus{border-color:var(--or);}

/* PHONE INPUT WITH FLAG */
.phone-field{display:flex;gap:.5rem;align-items:center;}
.country-select{flex-shrink:0;border:1.5px solid var(--border);border-radius:10px;padding:10px 8px;background:#FDFAF6;font-family:'Plus Jakarta Sans',sans-serif;font-size:.82rem;color:var(--ink);outline:none;cursor:pointer;transition:border-color .2s;height:46px;width:140px;appearance:auto;}
.country-select:focus{border-color:var(--or);}
.phone-number-input{flex:1;border:1.5px solid var(--border);border-radius:10px;padding:12px 14px;font-family:'Plus Jakarta Sans',sans-serif;font-size:.9rem;color:var(--ink);background:#FDFAF6;outline:none;transition:border-color .2s;height:46px;min-width:0;}
.phone-number-input:focus{border-color:var(--or);}
.phone-preview{font-size:.75rem;color:var(--txt2);margin-top:5px;padding:0 2px;}
.phone-preview span{color:var(--or);font-weight:700;}

.buyer-note{background:var(--or-light);border-radius:10px;padding:.7rem 1rem;font-size:.78rem;color:var(--or-dark);margin-bottom:1rem;line-height:1.5;}
.buyer-confirm-btn{background:var(--or);color:#fff;border:none;padding:14px;border-radius:14px;font-family:'Plus Jakarta Sans',sans-serif;font-size:.95rem;font-weight:700;cursor:pointer;width:100%;transition:all .25s;box-shadow:0 4px 16px var(--shadow);}
.buyer-confirm-btn:hover{background:var(--or-dark);}

/* ─── REMERCIEMENT BADGE ─── */
.remerciement-banner{background:linear-gradient(135deg,#1A0A2E,#2D1B4E);color:#fff;margin:2rem 0 1rem;border-radius:16px;padding:1.2rem 1.5rem;display:flex;align-items:center;gap:1rem;}
.rb-icon{width:48px;height:48px;background:linear-gradient(135deg,var(--or),var(--or2));border-radius:12px;display:flex;align-items:center;justify-content:center;font-size:1.5rem;flex-shrink:0;}
.rb-text h3{font-family:'Instrument Serif',serif;font-size:1.1rem;font-style:italic;margin-bottom:.2rem;}
.rb-text p{font-size:.78rem;opacity:.75;line-height:1.5;}

/* ─── CARD SUBLIME HOVER EFFECTS ─── */
.pcard::after{content:'';position:absolute;inset:0;background:linear-gradient(to top,rgba(242,90,10,.08),transparent);opacity:0;transition:opacity .3s;pointer-events:none;border-radius:20px;}
.pcard:hover::after{opacity:1;}
.pcard-overlay-btn{position:absolute;bottom:0;left:0;right:0;background:linear-gradient(to top,rgba(0,0,0,.7),transparent);padding:1rem;display:flex;align-items:center;justify-content:center;opacity:0;transition:opacity .3s;border-radius:0 0 20px 20px;}
.pcard:hover .pcard-overlay-btn{opacity:1;}
.pob-txt{color:#fff;font-size:.8rem;font-weight:700;background:var(--or);padding:7px 18px;border-radius:20px;}

.hidden{display:none!important;}
.enterprise-banner{background:linear-gradient(135deg,#0A0806,#1A1010);border:1.5px solid var(--or);border-radius:16px;padding:1.2rem 1.5rem;margin-bottom:2rem;display:flex;align-items:center;gap:1rem;flex-wrap:wrap;}
.eb-icon{width:48px;height:48px;background:linear-gradient(135deg,var(--or),var(--or2));border-radius:12px;display:flex;align-items:center;justify-content:center;font-size:1.5rem;flex-shrink:0;}
.eb-text{flex:1;}.eb-text h3{font-family:'Instrument Serif',serif;font-size:1.1rem;font-style:italic;color:#fff;margin-bottom:.2rem;}
.eb-text p{font-size:.78rem;color:rgba(255,255,255,.6);line-height:1.5;}
.eb-btn{background:var(--or);color:#fff;border:none;padding:8px 16px;border-radius:20px;font-size:.78rem;font-weight:700;cursor:pointer;white-space:nowrap;transition:all .2s;flex-shrink:0;}
.eb-btn:hover{background:var(--or-dark);}
.music-chip{background:rgba(255,255,255,.08);border:1px solid rgba(255,255,255,.15);border-radius:8px;padding:6px 8px;cursor:pointer;transition:all .2s;text-align:left;}
.music-chip:hover,.music-chip.selected{background:rgba(29,185,84,.25);border-color:#1DB954;}
.music-chip-title{font-size:.72rem;font-weight:600;color:#fff;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;}
.music-chip-artist{font-size:.62rem;color:rgba(255,255,255,.55);}
.deezer-result{display:flex;align-items:center;gap:.5rem;padding:6px 8px;background:rgba(255,255,255,.06);border-radius:8px;cursor:pointer;transition:all .2s;border:1px solid transparent;margin-bottom:.3rem;}
.deezer-result:hover{background:rgba(29,185,84,.15);border-color:rgba(29,185,84,.3);}
.deezer-result-title{font-size:.78rem;font-weight:600;color:#fff;}
.deezer-result-artist{font-size:.68rem;color:rgba(255,255,255,.55);}

@media(max-width:768px){
  .hero-inner{grid-template-columns:1fr;}
  .hero{padding:2rem 16px 3rem;}
  .hero h1{font-size:1.8rem;}
  .hero-sub{font-size:.88rem;}
  .hero-stats{gap:1rem;}
  .hero-stat-num{font-size:1.2rem;}
  .footer-inner{grid-template-columns:1fr;}
  .main{padding:1.5rem 12px 3rem;}
  .cat-section-header{flex-wrap:wrap;gap:.5rem;}
  .cat-section-title{font-size:1.2rem;}
  .pcard-img{height:150px;}
  .pcard-name{font-size:.82rem;}
  .pcard-price{font-size:.85rem;}
  .nav-inner{padding:0 12px;}
  .nav-logo-text{font-size:1.2rem;}
  .nav-cart-btn{padding:8px 14px;font-size:.78rem;}
  .topbar{font-size:.68rem;padding:6px 8px;}
  .pay-banner-inner{gap:.8rem;padding:10px 12px;justify-content:flex-start;overflow-x:auto;}
  .pay-item{font-size:.72rem;white-space:nowrap;}
  .modal-box{border-radius:16px 16px 0 0;position:fixed;bottom:0;left:0;right:0;max-height:94vh;max-width:100%;margin:0;}
  .modal-ov{align-items:flex-end;padding:0;}
  .modal-top{padding:1rem 1.2rem;}
  .modal-body{padding:1rem 1.2rem;gap:1rem;}
  .cart-drawer{width:100vw;}
  .pay-modal{border-radius:16px 16px 0 0;position:fixed;bottom:0;left:0;right:0;max-height:92vh;width:100%;}
  .pay-modal-ov{align-items:flex-end;padding:0;}
  .f-sec{padding:.9rem;}
  .country-select{width:108px!important;font-size:.74rem!important;}
  .phone-number-input{font-size:.85rem!important;}
  .succ-screen{padding:1rem .5rem;}
  .buyer-modal{border-radius:16px 16px 0 0;position:fixed;bottom:0;left:0;right:0;max-width:100%;}
  .buyer-modal-ov{align-items:flex-end;padding:0;}
  .cat-tabs{gap:.4rem;padding-bottom:.4rem;}
  .cat-tab{padding:8px 14px;font-size:.78rem;}
}
</style>
</head>
<body>

<div class="topbar">🇸🇳 Diadieuf · Vœux, Fêtes & Cadeaux d'Entreprise · Orange Money · Wave · Carte bancaire · WhatsApp gratuit</div>

<!-- NAV -->
<nav>
  <div class="nav-inner">
    <div class="nav-logo" onclick="scrollToTop()">
      <div class="nav-logo-icon">🎴</div>
      <div class="nav-logo-text">Diad<span>ieuf</span></div>
    </div>
    <div class="nav-right">
      <span class="nav-flag">🇸🇳</span>
      <button class="nav-cart-btn" onclick="openCart()">
        🛍️ Panier
        <span class="cbadge" id="cart-count">0</span>
      </button>
    </div>
  </div>
</nav>

<!-- HERO -->
<div class="hero">
  <div class="hero-inner">
    <div>
      <div class="hero-tag">✦ Boutique sénégalaise de cartes</div>
      <h1>Diadieuf — <strong>Merci</strong> en wolof<br>pour chaque moment.</h1>
      <p class="hero-sub">Offrez des cartes photoréalistes avec votre message, votre musique et un cadeau en FCFA. Le receveur peut aussi vous répondre avec une <strong>carte de remerciement</strong> 🙏</p>
      <div class="hero-actions">
        <button class="btn-white" onclick="document.getElementById('catalogue').scrollIntoView({behavior:'smooth'})">Voir les cartes →</button>
        <button class="btn-outline" onclick="openCart()">Mon panier</button>
      </div>
    </div>
    <div>
      <div class="hero-stats">
        <div class="hero-stat"><span class="hero-stat-num">32+</span><span class="hero-stat-lbl">Cartes uniques</span></div>
        <div class="hero-stat"><span class="hero-stat-num">8</span><span class="hero-stat-lbl">Occasions</span></div>
        <div class="hero-stat"><span class="hero-stat-num">100%</span><span class="hero-stat-lbl">Sénégalais</span></div>
      </div>
    </div>
  </div>
</div>

<!-- PAY BANNER -->
<div class="pay-banner">
  <div class="pay-banner-inner">
    <div class="pay-item"><div class="pi pi-or">🟠</div> Orange Money</div>
    <div class="pay-item"><div class="pi pi-wv">🌊</div> Wave</div>
    <div class="pay-item"><div class="pi pi-cb">💳</div> Carte bancaire</div>
    <div class="pay-item"><div class="pi pi-visa">VISA</div> Visa / Mastercard</div>
    <div class="pay-item">🔒 Paiement 100% sécurisé</div>
  </div>
</div>

<!-- CATALOGUE PRINCIPAL -->
<div class="main" id="catalogue">

  <!-- TABS -->
  <div class="cat-tabs" id="cat-tabs"></div>

  <!-- TOUTES LES SECTIONS -->
  <div id="all-sections"></div>

</div>

<!-- FOOTER -->
<footer>
  <div class="footer-inner">
    <div class="footer-brand">
      <div class="fb-logo">Diad<span>ieuf</span></div>
      <p>Boutique sénégalaise de cartes de vœux photoréalistes. Payez en FCFA avec Orange Money, Wave ou carte bancaire.</p>
    </div>
    <div class="footer-links">
      <h4>Navigation</h4>
      <a onclick="scrollToTop()">Accueil</a>
      <a onclick="document.getElementById('catalogue').scrollIntoView({behavior:'smooth'})">Catalogue</a>
      <a onclick="openCart()">Mon panier</a>
    </div>
    <div class="footer-links">
      <h4>Contact</h4>
      <a>WhatsApp : +221 77 000 00 00</a>
      <a>contact@diadieuf.sn</a>
      <a>Dakar, Sénégal 🇸🇳</a>
    </div>
  </div>
  <div class="footer-bottom">
    <span>© 2026 Diadieuf — Tous droits réservés</span>
    <span>Fait avec ❤️ au Sénégal 🇸🇳</span>
  </div>
</footer>

<!-- DRAWER PANIER -->
<div class="cart-overlay" id="cart-overlay" onclick="closeCart()"></div>
<div class="cart-drawer" id="cart-drawer">
  <div class="cart-header">
    <h3>🛍️ Mon Panier</h3>
    <button class="cart-close" onclick="closeCart()">×</button>
  </div>
  <div class="cart-items-list" id="cart-items-list"></div>
  <div class="cart-footer" id="cart-footer"></div>
</div>

<!-- MODAL ÉDITEUR -->
<div class="modal-ov" id="editor-modal">
  <div class="modal-box">
    <div class="modal-top">
      <h2>Personnaliser ma carte</h2>
      <button class="modal-close" onclick="closeEditor()">×</button>
    </div>
    <div class="modal-body">
      <!-- Colonne gauche : aperçu -->
      <div>
        <div class="flip-scene" onclick="toggleFlip()">
          <div class="flip-inner" id="flip-inner">
            <div class="flip-f" id="flip-f">
              <div id="recto-svg"></div>
              <div class="recto-ol">
                <div class="ro-title" id="ro-title"></div>
                <div class="ro-msg" id="ro-msg"></div>
                <div class="ro-gift" id="ro-gift"></div>
                <div class="ro-music" id="ro-music"></div>
                <div class="ro-sig" id="ro-sig"></div>
              </div>
            </div>
            <div class="flip-b" id="flip-b">
              <div id="verso-svg-wrap"></div>
              <div style="position:absolute;bottom:0;left:0;right:0;padding:.8rem;background:linear-gradient(to top,rgba(0,0,0,.7),transparent);text-align:center;">
                <div style="font-family:'Instrument Serif',serif;font-style:italic;color:#fff;font-size:.9rem;" id="verso-card-name"></div>
                <div style="font-size:.6rem;color:rgba(255,255,255,.5);">Diadieuf · Sénégal 🇸🇳</div>
              </div>
            </div>
          </div>
        </div>
        <div class="flip-actions">
          <button class="fa-btn" onclick="toggleFlip()">🔄 Verso</button>
          <button class="fa-btn primary" onclick="saveToGalleryFromEditor()">📸 Garder</button>
        </div>
        <!-- VERSO THEMES -->
        <div style="margin-top:1rem;">
          <div style="font-size:.75rem;font-weight:700;color:var(--txt2);margin-bottom:.5rem;">🌍 Thème du verso</div>
          <div class="verso-grid" id="verso-grid"></div>
        </div>
      </div>
      <!-- Colonne droite : formulaire -->
      <div>
        <div class="f-sec">
          <div class="f-sec-title">📝 Votre message</div>
          <div class="fg"><label>Titre / Vœu</label><input type="text" id="e-title" placeholder="Ex: Joyeux Anniversaire !" oninput="updatePreview()"></div>
          <div class="fg"><label>Message</label><textarea id="e-msg" rows="3" placeholder="Votre message..." oninput="updatePreview()"></textarea></div>
          <div class="fg"><label>Signature</label><input type="text" id="e-sig" placeholder="— De la part de..." oninput="updatePreview()"></div>
        </div>

        <!-- MUSIQUE -->
        <div class="music-info-box" style="margin-bottom:.9rem;">
          <div class="mib-title">🎵 Musique de votre carte</div>
          <div class="mib-sub">4 titres inclus gratuitement · Recherche personnalisée +500 F CFA</div>
          <div id="music-suggestions" style="display:grid;grid-template-columns:1fr 1fr;gap:.4rem;margin-bottom:.7rem;"></div>
          <div style="display:flex;align-items:center;gap:.5rem;margin:.5rem 0;">
            <div style="flex:1;height:1px;background:rgba(255,255,255,.15);"></div>
            <span style="font-size:.68rem;color:rgba(255,255,255,.4);">ou rechercher</span>
            <div style="flex:1;height:1px;background:rgba(255,255,255,.15);"></div>
          </div>
          <div style="display:flex;gap:.4rem;margin-bottom:.5rem;">
            <input type="text" id="music-search-input" placeholder="🔍 Artiste ou titre... (+500 F CFA)"
              style="flex:1;background:rgba(255,255,255,.08);border:1px solid rgba(255,255,255,.2);border-radius:8px;padding:8px 10px;color:#fff;font-family:'Plus Jakarta Sans',sans-serif;font-size:.8rem;outline:none;"
              oninput="onMusicSearch(this.value)">
          </div>
          <div id="deezer-results"></div>
          <div class="music-track-display" id="music-track-display" style="display:none;margin-top:.5rem;">
            <div class="mtd-icon" id="mtd-icon">🎵</div>
            <div class="mtd-info">
              <div class="mtd-name" id="mtd-name">—</div>
              <div class="mtd-artist" id="mtd-artist">—</div>
            </div>
            <div style="display:flex;align-items:center;gap:.4rem;">
              <div class="np-anim"><div class="np-b"></div><div class="np-b"></div><div class="np-b"></div></div>
              <button onclick="clearMusicSelection()" style="background:rgba(255,255,255,.15);border:none;color:#fff;border-radius:6px;padding:2px 7px;cursor:pointer;font-size:.68rem;">✕</button>
            </div>
          </div>
        </div>

        <!-- CADEAU FINANCIER -->
        <div class="f-sec" style="background:linear-gradient(135deg,#FFFBF0,#FFF5E0);border:1px solid #E8C060;">
          <div class="f-sec-title">💰 Cadeau financier <span style="font-size:.65rem;color:var(--txt2);font-weight:400;">(optionnel)</span></div>
          <div class="gift-toggle-row" onclick="toggleGift()">
            <div class="tgsw" id="gift-sw"></div>
            <span class="gift-lbl" id="gift-lbl">Ajouter un cadeau en FCFA</span>
          </div>
          <div class="gift-body" id="gift-body">
            <div class="ops">
              <div class="op-btn" id="op-or" onclick="selOp('orange')"><div class="op-icon">🟠</div><div class="op-name" style="color:var(--or);">Orange Money</div></div>
              <div class="op-btn" id="op-wv" onclick="selOp('wave')"><div class="op-icon">🌊</div><div class="op-name" style="color:var(--blue);">Wave</div></div>
            </div>
            <div class="amts">
              <div class="achip" onclick="pickAmt(1000,this)">1 000 F</div>
              <div class="achip" onclick="pickAmt(2000,this)">2 000 F</div>
              <div class="achip" onclick="pickAmt(5000,this)">5 000 F</div>
              <div class="achip" onclick="pickAmt(10000,this)">10 000 F</div>
              <div class="achip" onclick="pickAmt(25000,this)">25 000 F</div>
              <div class="achip" onclick="pickAmt(50000,this)">50 000 F</div>
            </div>
            <div class="fg" style="margin:0;"><input type="number" id="gift-custom" placeholder="Montant personnalisé (FCFA)" min="500" oninput="customAmt()"></div>
            <div class="fg" style="margin:0;"><label>N° téléphone bénéficiaire</label>
              <div class="phone-field">
                <select class="country-select" id="gift-country" onchange="updatePhonePreview('gift')" style="width:130px;height:46px;font-size:.78rem;">
                  <option value="+221" selected>🇸🇳 +221</option>
                  <option value="+33">🇫🇷 +33</option>
                  <option value="+32">🇧🇪 +32</option>
                  <option value="+41">🇨🇭 +41</option>
                  <option value="+1">🇺🇸 +1</option>
                  <option value="+44">🇬🇧 +44</option>
                  <option value="+225">🇨🇮 +225</option>
                  <option value="+223">🇲🇱 +223</option>
                  <option value="+224">🇬🇳 +224</option>
                  <option value="+222">🇲🇷 +222</option>
                  <option value="+220">🇬🇲 +220</option>
                </select>
                <input type="tel" class="phone-number-input" id="gift-phone" placeholder="77 123 45 67" oninput="updatePhonePreview('gift');updatePreview()" style="height:46px;">
              </div>
              <div class="phone-preview" id="gift-phone-preview">Numéro : <span>—</span></div>
            </div>
          </div>
        </div>

        <!-- LIVRAISON -->
        <div class="f-sec">
          <div class="f-sec-title">📬 Infos du receveur</div>
          <div class="fg">
            <label>Prénom et nom du receveur *</label>
            <input type="text" id="e-recip" placeholder="Ex: Mamadou Diallo">
          </div>
          <div class="fg">
            <label>Téléphone du receveur *</label>
            <div class="phone-field">
              <select class="country-select" id="recip-country" onchange="updatePhonePreview('recip')" style="width:130px;height:46px;font-size:.78rem;">
                <option value="+221" selected>🇸🇳 +221</option>
                <option value="+33">🇫🇷 +33</option>
                <option value="+32">🇧🇪 +32</option>
                <option value="+41">🇨🇭 +41</option>
                <option value="+1">🇺🇸 +1</option>
                <option value="+44">🇬🇧 +44</option>
                <option value="+225">🇨🇮 +225</option>
                <option value="+223">🇲🇱 +223</option>
                <option value="+224">🇬🇳 +224</option>
                <option value="+222">🇲🇷 +222</option>
                <option value="+220">🇬🇲 +220</option>
                <option value="+245">🇬🇼 +245</option>
                <option value="+212">🇲🇦 +212</option>
                <option value="+216">🇹🇳 +216</option>
                <option value="+234">🇳🇬 +234</option>
                <option value="+233">🇬🇭 +233</option>
              </select>
              <input type="tel" class="phone-number-input" id="recip-phone" placeholder="77 123 45 67" oninput="updatePhonePreview('recip')">
            </div>
            <div class="phone-preview" id="recip-phone-preview">Numéro : <span>—</span></div>
          </div>
          <div class="fg">
            <label>Email du receveur (pour notification)</label>
            <input type="email" id="recip-email" placeholder="Ex: mamadou@gmail.com">
          </div>
          <div class="fg">
            <label>Mode d'envoi</label>
            <select id="e-del" onchange="onDelChg()">
              <option value="sms">📱 SMS (gratuit)</option>
              <option value="whatsapp">💬 WhatsApp (gratuit)</option>
              <option value="postal">📬 Courrier Dakar (+2 000 F)</option>
            </select>
          </div>
          <div class="fg hidden" id="addr-grp"><label>Adresse postale</label><textarea id="e-addr" rows="2" placeholder="Quartier, Rue, Dakar, Sénégal"></textarea></div>
        </div>

        <button class="add-to-cart-btn" onclick="addToCart()">
          🛒 Ajouter au panier — <span id="editor-total">2 500 F CFA</span>
        </button>
      </div>
    </div>
  </div>
</div>

<!-- MODAL PAIEMENT -->
<div class="pay-modal-ov" id="pay-modal">
  <div class="pay-modal" id="pay-modal-body">
    <div class="pay-modal-header">
      <h3>💳 Paiement sécurisé</h3>
      <button class="modal-close" onclick="closePay()">×</button>
    </div>
    <div class="pay-modal-body" id="pay-modal-content"></div>
  </div>
</div>

<!-- MODAL ACHETEUR -->
<div class="buyer-modal-ov" id="buyer-modal">
  <div class="buyer-modal">
    <div class="buyer-modal-top">
      <h3>👤 Vos coordonnées</h3>
      <button class="modal-close" onclick="closeBuyerModal()">×</button>
    </div>
    <div class="buyer-modal-body">
      <div class="buyer-note">📋 Ces informations sont nécessaires pour envoyer votre carte et confirmer votre commande.</div>

      <div class="fg">
        <label>Votre prénom et nom *</label>
        <input type="text" id="buyer-name" placeholder="Ex: Amadou Diallo" required>
      </div>

      <div class="fg">
        <label>Votre numéro de téléphone *</label>
        <div class="phone-field">
          <select class="country-select" id="buyer-country" onchange="updatePhonePreview('buyer')">
            <option value="+221" data-flag="🇸🇳" selected>🇸🇳 +221 Sénégal</option>
            <option value="+33" data-flag="🇫🇷">🇫🇷 +33 France</option>
            <option value="+32" data-flag="🇧🇪">🇧🇪 +32 Belgique</option>
            <option value="+41" data-flag="🇨🇭">🇨🇭 +41 Suisse</option>
            <option value="+1" data-flag="🇺🇸">🇺🇸 +1 USA/Canada</option>
            <option value="+44" data-flag="🇬🇧">🇬🇧 +44 Royaume-Uni</option>
            <option value="+225" data-flag="🇨🇮">🇨🇮 +225 Côte d'Ivoire</option>
            <option value="+223" data-flag="🇲🇱">🇲🇱 +223 Mali</option>
            <option value="+224" data-flag="🇬🇳">🇬🇳 +224 Guinée</option>
            <option value="+222" data-flag="🇲🇷">🇲🇷 +222 Mauritanie</option>
            <option value="+220" data-flag="🇬🇲">🇬🇲 +220 Gambie</option>
            <option value="+245" data-flag="🇬🇼">🇬🇼 +245 Guinée-Bissau</option>
            <option value="+238" data-flag="🇨🇻">🇨🇻 +238 Cap-Vert</option>
            <option value="+212" data-flag="🇲🇦">🇲🇦 +212 Maroc</option>
            <option value="+216" data-flag="🇹🇳">🇹🇳 +216 Tunisie</option>
            <option value="+213" data-flag="🇩🇿">🇩🇿 +213 Algérie</option>
            <option value="+234" data-flag="🇳🇬">🇳🇬 +234 Nigeria</option>
            <option value="+233" data-flag="🇬🇭">🇬🇭 +233 Ghana</option>
          </select>
          <input type="tel" class="phone-number-input" id="buyer-phone" placeholder="77 123 45 67" oninput="updatePhonePreview('buyer')">
        </div>
        <div class="phone-preview" id="buyer-phone-preview">Numéro complet : <span>—</span></div>
      </div>

      <div class="fg">
        <label>Votre adresse email (optionnel)</label>
        <input type="email" id="buyer-email" placeholder="Ex: amadou@gmail.com">
      </div>

      <button class="buyer-confirm-btn" onclick="confirmBuyer()">Continuer vers le paiement →</button>
    </div>
  </div>
</div>

<div class="toast" id="toast"><div class="toast-dot"></div><span id="toast-msg"></span></div>


<script>
// ══ FORMAT ══
const fmt = n => new Intl.NumberFormat('fr-SN').format(Math.round(n)) + ' F CFA';
const fmtS = n => new Intl.NumberFormat('fr-SN').format(Math.round(n)) + ' F';

// ══ SVG PHOTORÉALISTES ══
function svgAnniv1(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="a1g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#FF8C00"/><stop offset="100%" stop-color="#FF4400"/></linearGradient></defs><rect width="300" height="400" fill="url(#a1g)"/><circle cx="150" cy="160" r="90" fill="rgba(255,255,255,.08)"/><circle cx="150" cy="160" r="65" fill="rgba(255,255,255,.06)"/><ellipse cx="150" cy="370" rx="140" ry="25" fill="rgba(0,0,0,.15)"/><rect x="85" y="230" width="130" height="80" rx="8" fill="#F8C8A0"/><rect x="85" y="230" width="130" height="28" rx="8" fill="#F0A060"/><ellipse cx="150" cy="228" rx="65" ry="12" fill="#E89050"/><circle cx="120" cy="215" r="4" fill="#FFD700"/><circle cx="150" cy="210" r="4" fill="#FF6B6B"/><circle cx="180" cy="215" r="4" fill="#6BCB77"/><rect x="118" y="196" width="5" height="22" rx="2" fill="#FF9900"/><rect x="148" y="191" width="5" height="22" rx="2" fill="#FF6B6B"/><rect x="178" y="196" width="5" height="22" rx="2" fill="#FFD700"/><ellipse cx="60" cy="120" rx="22" ry="28" fill="#FF6B6B" opacity=".9"/><ellipse cx="100" cy="95" rx="22" ry="28" fill="#FFD93D" opacity=".9"/><ellipse cx="200" cy="90" rx="22" ry="28" fill="#6BCB77" opacity=".9"/><ellipse cx="240" cy="110" rx="22" ry="28" fill="#4D96FF" opacity=".9"/><line x1="60" y1="148" x2="65" y2="230" stroke="#FF6B6B" stroke-width="1.5"/><line x1="100" y1="123" x2="105" y2="230" stroke="#FFD93D" stroke-width="1.5"/><line x1="200" y1="118" x2="195" y2="230" stroke="#6BCB77" stroke-width="1.5"/><line x1="240" y1="138" x2="235" y2="230" stroke="#4D96FF" stroke-width="1.5"/><circle cx="50" cy="60" r="4" fill="#FFD700" opacity=".7"/><circle cx="250" cy="50" r="3" fill="#FF6B6B" opacity=".7"/><circle cx="30" cy="200" r="3" fill="#6BCB77" opacity=".6"/><circle cx="270" cy="180" r="4" fill="#4D96FF" opacity=".7"/></svg>`;}

function svgAnniv2(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="a2g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#0A0A20"/><stop offset="100%" stop-color="#1A0830"/></linearGradient></defs><rect width="300" height="400" fill="url(#a2g)"/><circle cx="50" cy="40" r="2" fill="#fff" opacity=".8"/><circle cx="200" cy="25" r="1.5" fill="#FFD700" opacity=".9"/><circle cx="270" cy="55" r="2" fill="#fff" opacity=".6"/><circle cx="120" cy="30" r="1" fill="#fff" opacity=".7"/><rect x="0" y="280" width="300" height="120" fill="#1A0A05"/><rect x="20" y="250" width="25" height="50" fill="#2A1A0A"/><rect x="60" y="240" width="18" height="60" fill="#221408"/><rect x="140" y="235" width="22" height="65" fill="#2A1A08"/><rect x="200" y="248" width="30" height="52" fill="#221408"/><rect x="250" y="258" width="20" height="42" fill="#1E1208"/><rect x="27" y="258" width="4" height="4" rx="1" fill="#FFD700" opacity=".7"/><rect x="148" y="243" width="4" height="4" rx="1" fill="#FFD700" opacity=".8"/><rect x="208" y="256" width="4" height="4" rx="1" fill="#FFD700" opacity=".6"/><rect x="100" y="205" width="100" height="75" fill="#2A180A"/><polygon points="150,165 120,205 180,205" fill="#3A2A10"/><rect x="145" y="150" width="10" height="18" fill="#C8922A"/><circle cx="150" cy="148" r="5" fill="#C8922A"/><g opacity=".9"><line x1="60" y1="130" x2="35" y2="85" stroke="#FFD700" stroke-width="2"/><line x1="60" y1="130" x2="85" y2="85" stroke="#FFD700" stroke-width="2"/><line x1="60" y1="130" x2="60" y2="78" stroke="#FFD700" stroke-width="2"/><line x1="60" y1="130" x2="25" y2="108" stroke="#FFD700" stroke-width="2"/><circle cx="35" cy="85" r="3" fill="#FFD700"/><circle cx="85" cy="85" r="3" fill="#FFD700"/><circle cx="60" cy="78" r="3" fill="#FFD700"/></g><g opacity=".9"><line x1="230" y1="110" x2="205" y2="68" stroke="#FF6B6B" stroke-width="2"/><line x1="230" y1="110" x2="255" y2="68" stroke="#FF6B6B" stroke-width="2"/><line x1="230" y1="110" x2="230" y2="62" stroke="#FF6B6B" stroke-width="2"/><line x1="230" y1="110" x2="195" y2="90" stroke="#FF6B6B" stroke-width="2"/><line x1="230" y1="110" x2="265" y2="90" stroke="#FF6B6B" stroke-width="2"/><circle cx="205" cy="68" r="3" fill="#FF6B6B"/><circle cx="255" cy="68" r="3" fill="#FF6B6B"/><circle cx="230" cy="62" r="3" fill="#FF6B6B"/></g></svg>`;}

function svgAnniv3(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="a3g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#F8F0E8"/><stop offset="100%" stop-color="#E8D8C0"/></linearGradient><pattern id="wax3" width="40" height="40" patternUnits="userSpaceOnUse"><circle cx="20" cy="20" r="8" fill="none" stroke="#C8922A" stroke-width="1.5" opacity=".2"/><circle cx="0" cy="0" r="8" fill="none" stroke="#C8922A" stroke-width="1.5" opacity=".15"/><circle cx="40" cy="40" r="8" fill="none" stroke="#C8922A" stroke-width="1.5" opacity=".15"/></pattern></defs><rect width="300" height="400" fill="url(#a3g)"/><rect width="300" height="400" fill="url(#wax3)"/><rect x="55" y="285" width="190" height="8" rx="4" fill="#8B6040"/><rect x="70" y="200" width="160" height="90" rx="6" fill="#F8D8B0"/><rect x="70" y="200" width="160" height="30" rx="6" fill="#E8B880"/><rect x="58" y="222" width="184" height="72" rx="6" fill="#FAE8C8"/><rect x="120" y="160" width="60" height="45" rx="4" fill="#F0D0A0"/><rect x="120" y="160" width="60" height="16" rx="4" fill="#E0B080"/><rect x="108" y="172" width="84" height="33" rx="4" fill="#F8E0B8"/><rect x="138" y="136" width="8" height="28" rx="4" fill="#F8F0E0"/><ellipse cx="142" cy="134" rx="5" ry="7" fill="#FF8800" opacity=".9"/><rect x="155" y="140" width="8" height="24" rx="4" fill="#F8F0E0"/><ellipse cx="159" cy="138" rx="5" ry="7" fill="#FF8800" opacity=".8"/><g transform="translate(230,240)"><ellipse cx="0" cy="-15" rx="10" ry="14" fill="#E8A0C0" transform="rotate(-20)"/><ellipse cx="0" cy="-15" rx="10" ry="14" fill="#F0A8C8" transform="rotate(60)"/><ellipse cx="0" cy="-15" rx="10" ry="14" fill="#E890B0" transform="rotate(140)"/><circle r="7" fill="#FFD700"/></g><g transform="translate(75,250)"><ellipse cx="0" cy="-12" rx="9" ry="12" fill="#C8E0A0" transform="rotate(-30)"/><ellipse cx="0" cy="-12" rx="9" ry="12" fill="#C8E8A8" transform="rotate(60)"/><ellipse cx="0" cy="-12" rx="9" ry="12" fill="#B8D890" transform="rotate(150)"/><circle r="6" fill="#FFD700"/></g><rect x="35" y="300" width="230" height="70" fill="rgba(200,146,42,.08)" rx="4"/></svg>`;}

function svgAnniv4(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="a4g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#FFF5CC"/><stop offset="100%" stop-color="#FFE080"/></linearGradient></defs><rect width="300" height="400" fill="url(#a4g)"/><circle cx="150" cy="80" r="60" fill="#FF8C00" opacity=".2"/><circle cx="150" cy="100" r="45" fill="#FF6600" opacity=".2"/><rect x="0" y="250" width="300" height="150" fill="#8B6040"/><ellipse cx="150" cy="270" rx="150" ry="20" fill="#C06020" opacity=".5"/><rect x="35" y="180" width="18" height="90" fill="#6B4020"/><ellipse cx="44" cy="175" rx="35" ry="28" fill="#4A7020"/><ellipse cx="25" cy="182" rx="18" ry="15" fill="#3A6018"/><rect x="248" y="200" width="14" height="70" fill="#6B4020"/><ellipse cx="255" cy="196" rx="28" ry="22" fill="#4A7020"/><rect x="100" y="230" width="100" height="60" fill="#C8905A"/><polygon points="100,230 200,230 150,195" fill="#A07030"/><rect x="135" y="260" width="30" height="30" fill="#7A4820"/><ellipse cx="115" cy="238" rx="8" ry="9" fill="#5A3010"/><rect x="108" y="246" width="14" height="20" rx="3" fill="#7A4020"/><ellipse cx="185" cy="236" rx="9" ry="10" fill="#5A3010"/><rect x="177" y="245" width="16" height="22" rx="3" fill="#8A5030"/><ellipse cx="150" cy="244" rx="6" ry="7" fill="#7A4820"/><rect x="145" y="250" width="10" height="14" rx="2" fill="#9A6040"/><circle cx="55" cy="55" r="2" fill="#FFD700" opacity=".8"/><circle cx="250" cy="45" r="2" fill="#FFD700" opacity=".7"/></svg>`;}

function svgMar1(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="m1g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#1A0A2E"/><stop offset="50%" stop-color="#2A1848"/><stop offset="100%" stop-color="#1A0A20"/></linearGradient></defs><rect width="300" height="400" fill="url(#m1g)"/><circle cx="50" cy="40" r="2" fill="#fff" opacity=".7"/><circle cx="250" cy="30" r="2" fill="#FFD700" opacity=".8"/><circle cx="160" cy="20" r="1.5" fill="#fff" opacity=".6"/><ellipse cx="150" cy="160" rx="75" ry="85" fill="rgba(200,146,42,.08)"/><ellipse cx="118" cy="180" rx="16" ry="17" fill="#C8905A"/><path d="M100,195 Q95,258 92,318 L148,318 Q145,258 140,195 Z" fill="#E8601A" opacity=".95"/><line x1="100" y1="210" x2="138" y2="210" stroke="#FFD700" stroke-width="1.5" opacity=".6"/><line x1="97" y1="230" x2="141" y2="230" stroke="#FFD700" stroke-width="1.5" opacity=".6"/><ellipse cx="118" cy="172" rx="20" ry="8" fill="#E8601A"/><path d="M100,168 Q118,153 136,168 Q136,173 118,171 Q100,173 100,168 Z" fill="#E8601A"/><ellipse cx="182" cy="178" rx="16" ry="17" fill="#C09060"/><path d="M162,193 Q157,256 154,316 L212,316 Q210,256 203,193 Z" fill="#F8F0E8" opacity=".95"/><line x1="162" y1="205" x2="202" y2="205" stroke="#C8922A" stroke-width="1.5" opacity=".5"/><line x1="160" y1="225" x2="204" y2="225" stroke="#C8922A" stroke-width="1.5" opacity=".5"/><ellipse cx="182" cy="170" rx="18" ry="7" fill="#F8F0E8"/><ellipse cx="182" cy="166" rx="15" ry="5" fill="#F0E8E0"/><path d="M82,352 Q150,338 218,352" stroke="#FFB8D8" stroke-width="3" fill="none" opacity=".6"/><circle cx="82" cy="352" r="5" fill="#FFB8D8" opacity=".7"/><circle cx="150" cy="338" r="5" fill="#FFD700" opacity=".7"/><circle cx="218" cy="352" r="5" fill="#FFB8D8" opacity=".7"/></svg>`;}

function svgMar2(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="m2g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#FFF0F8"/><stop offset="100%" stop-color="#FFD8F0"/></linearGradient></defs><rect width="300" height="400" fill="url(#m2g)"/><rect x="0" y="300" width="300" height="100" fill="#5A9040"/><rect x="110" y="240" width="80" height="160" rx="5" fill="#E8D8B0"/><rect x="90" y="200" width="10" height="100" rx="5" fill="#8B6040"/><rect x="200" y="200" width="10" height="100" rx="5" fill="#8B6040"/><path d="M90,200 Q150,158 210,200" fill="none" stroke="#8B6040" stroke-width="10"/><circle cx="90" cy="200" r="10" fill="#FF8BC0"/><circle cx="130" cy="170" r="9" fill="#FFD700"/><circle cx="150" cy="163" r="10" fill="#FF8BC0"/><circle cx="170" cy="170" r="9" fill="#6BCB77"/><circle cx="210" cy="200" r="10" fill="#FF8BC0"/><ellipse cx="115" cy="158" rx="15" ry="16" fill="#D4A870"/><rect x="100" y="173" width="30" height="50" rx="5" fill="#FFB8D8"/><path d="M100,185 Q90,220 85,240 L115,240 Z" fill="#FFB8D8"/><path d="M130,185 Q140,220 145,240 L115,240 Z" fill="#FFB8D8"/><path d="M100,153 Q115,138 130,153 Q130,158 115,157 Q100,158 100,153 Z" fill="rgba(255,255,255,.8)"/><ellipse cx="185" cy="155" rx="15" ry="16" fill="#C09060"/><rect x="170" y="170" width="30" height="50" rx="4" fill="#2A3A5A"/><rect x="175" y="170" width="8" height="50" fill="#fff" opacity=".4"/><path d="M142,152 Q148,144 152,152 Q158,144 162,152 Q162,160 152,167 Q142,160 142,152 Z" fill="#FF6B6B" opacity=".9"/></svg>`;}

function svgMar3(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="m3g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#F8EEE0"/><stop offset="100%" stop-color="#EED8C0"/></linearGradient></defs><rect width="300" height="400" fill="url(#m3g)"/><rect x="55" y="295" width="190" height="8" rx="4" fill="#8B6040"/><rect x="60" y="195" width="28" height="95" rx="6" fill="#2A6020"/><rect x="65" y="178" width="18" height="22" rx="4" fill="#3A7030"/><rect x="68" y="170" width="12" height="12" rx="3" fill="#2A5020"/><ellipse cx="74" cy="169" rx="8" ry="4" fill="#D4A800"/><g transform="translate(200,240)"><ellipse cx="0" cy="-15" rx="10" ry="14" fill="#E8A0C0" transform="rotate(-20)"/><ellipse cx="0" cy="-15" rx="10" ry="14" fill="#F0A8C8" transform="rotate(60)"/><ellipse cx="0" cy="-15" rx="10" ry="14" fill="#E890B0" transform="rotate(140)"/><circle r="7" fill="#FFD700"/></g><g transform="translate(240,250)"><ellipse cx="0" cy="-12" rx="8" ry="12" fill="#C8E0A0" transform="rotate(-30)"/><ellipse cx="0" cy="-12" rx="8" ry="12" fill="#C8E8A8" transform="rotate(60)"/><ellipse cx="0" cy="-12" rx="8" ry="12" fill="#B8D890" transform="rotate(150)"/><circle r="5" fill="#FFD700"/></g><polygon points="195,295 205,195 215,195" fill="rgba(200,240,255,0.5)" stroke="#B0D0E0" stroke-width="1"/><ellipse cx="205" cy="193" rx="12" ry="5" fill="rgba(200,240,255,0.4)" stroke="#B0D0E0" stroke-width="1"/><rect x="110" y="110" width="80" height="100" rx="4" fill="rgba(200,146,42,.2)"/><rect x="115" y="115" width="70" height="90" rx="3" fill="#F8F0E0"/><ellipse cx="150" cy="150" rx="26" ry="30" fill="#D4A870"/><ellipse cx="150" cy="140" rx="20" ry="20" fill="#C09060"/><path d="M105,195 Q150,208 195,195" stroke="#C8922A" stroke-width="3" fill="none"/></svg>`;}

function svgMar4(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="m4g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#FFFEF8"/><stop offset="100%" stop-color="#FFF8E0"/></linearGradient></defs><rect width="300" height="400" fill="url(#m4g)"/><path d="M150,80 Q200,40 250,80 Q250,180 150,220 Q50,180 50,80 Q100,40 150,80 Z" fill="none" stroke="#C8922A" stroke-width="1.5" opacity=".3"/><g transform="translate(150,180)"><ellipse cx="0" cy="-40" rx="28" ry="32" fill="#E03060" transform="rotate(0)"/><ellipse cx="0" cy="-40" rx="24" ry="28" fill="#C82050" transform="rotate(60)"/><ellipse cx="0" cy="-40" rx="20" ry="24" fill="#D02858" transform="rotate(120)"/><ellipse cx="0" cy="-40" rx="16" ry="20" fill="#E03868" transform="rotate(180)"/><ellipse cx="0" cy="-40" rx="12" ry="16" fill="#C82048" transform="rotate(240)"/><circle r="14" fill="#C01840"/><circle r="8" fill="#A01030"/></g><line x1="150" y1="220" x2="150" y2="330" stroke="#3A6020" stroke-width="4"/><ellipse cx="125" cy="265" rx="22" ry="10" fill="#4A7828" transform="rotate(-30,125,265)"/><ellipse cx="175" cy="295" rx="22" ry="10" fill="#3A6820" transform="rotate(30,175,295)"/><rect x="50" y="340" width="7" height="35" rx="3" fill="#F8F0E0"/><ellipse cx="53.5" cy="338" rx="4" ry="6" fill="#FF8800" opacity=".8"/><rect x="243" y="340" width="7" height="35" rx="3" fill="#F8F0E0"/><ellipse cx="246.5" cy="338" rx="4" ry="6" fill="#FF8800" opacity=".8"/><path d="M55,80 Q58,73 62,80 Q66,73 69,80 Q69,88 62,94 Q55,88 55,80 Z" fill="#E03060" opacity=".7"/><path d="M232,85 Q234,80 237,85 Q240,80 242,85 Q242,91 237,96 Q232,91 232,85 Z" fill="#E03060" opacity=".7"/></svg>`;}

function svgNais1(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="n1g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#E8F5FF"/><stop offset="100%" stop-color="#C8E8FF"/></linearGradient></defs><rect width="300" height="400" fill="url(#n1g)"/><ellipse cx="70" cy="65" rx="50" ry="24" fill="white" opacity=".8"/><ellipse cx="100" cy="52" rx="35" ry="18" fill="white" opacity=".9"/><ellipse cx="230" cy="75" rx="55" ry="26" fill="white" opacity=".7"/><path d="M20,200 Q150,60 280,200" fill="none" stroke="#FF8080" stroke-width="7" opacity=".4"/><path d="M35,200 Q150,80 265,200" fill="none" stroke="#FFB840" stroke-width="7" opacity=".4"/><path d="M50,200 Q150,98 250,200" fill="none" stroke="#FFE840" stroke-width="7" opacity=".4"/><path d="M65,200 Q150,114 235,200" fill="none" stroke="#80E080" stroke-width="7" opacity=".4"/><path d="M78,200 Q150,128 222,200" fill="none" stroke="#80B0FF" stroke-width="7" opacity=".4"/><path d="M70,320 Q150,290 230,320 Q230,360 150,370 Q70,360 70,320 Z" fill="#F8E0C0"/><path d="M70,320 Q150,308 230,320" fill="none" stroke="#D4A870" stroke-width="3"/><ellipse cx="150" cy="335" rx="30" ry="22" fill="#F8E0D0"/><ellipse cx="150" cy="318" rx="22" ry="22" fill="#F0D0B8"/><path d="M139,317 Q143,314 147,317" fill="none" stroke="#8B6040" stroke-width="1.5"/><path d="M153,317 Q157,314 161,317" fill="none" stroke="#8B6040" stroke-width="1.5"/><path d="M143,323 Q150,328 157,323" fill="none" stroke="#C09070" stroke-width="1.5"/><path d="M75,338 Q150,325 225,338 Q220,370 150,375 Q80,370 75,338 Z" fill="#B8D8F8"/><circle cx="50" cy="140" r="14" fill="#FFE860" opacity=".6"/><circle cx="255" cy="150" r="11" fill="#FFE860" opacity=".5"/></svg>`;}

function svgNais2(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="n2g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#E0EEFF"/><stop offset="100%" stop-color="#C0D8FF"/></linearGradient></defs><rect width="300" height="400" fill="url(#n2g)"/><circle cx="150" cy="120" r="50" fill="#FFE860" opacity=".3"/><ellipse cx="150" cy="280" rx="90" ry="14" fill="rgba(0,0,0,.08)"/><ellipse cx="150" cy="230" rx="55" ry="40" fill="#F0F0F0"/><ellipse cx="110" cy="215" rx="30" ry="28" fill="#F0F0F0"/><ellipse cx="90" cy="200" rx="22" ry="20" fill="#E8E0D8"/><ellipse cx="80" cy="196" rx="12" ry="10" fill="#D8D0C8"/><ellipse cx="68" cy="190" rx="8" ry="12" fill="#E0D8D0" transform="rotate(-20,68,190)"/><circle cx="84" cy="195" r="4" fill="#3A2A10"/><circle cx="85" cy="194" r="1.5" fill="#fff"/><ellipse cx="76" cy="202" rx="5" ry="3" fill="#C8A090"/><path d="M95,186 Q100,172 108,178" stroke="#C8B080" stroke-width="3" fill="none" stroke-linecap="round"/><rect x="110" y="262" width="12" height="35" rx="6" fill="#D8D0C8"/><rect x="130" y="265" width="12" height="35" rx="6" fill="#D8D0C8"/><rect x="155" y="265" width="12" height="35" rx="6" fill="#D8D0C8"/><rect x="175" y="262" width="12" height="35" rx="6" fill="#D8D0C8"/><circle cx="240" cy="210" r="18" fill="#FFB8D8"/><rect x="238" y="225" width="4" height="20" rx="2" fill="#E8A0C0"/><circle cx="240" cy="210" r="12" fill="#FF90C0" opacity=".5"/><circle cx="60" cy="200" r="5" fill="#B0C8E0"/><ellipse cx="240" cy="140" rx="14" ry="12" fill="#B0C8E0"/><circle cx="240" cy="135" r="3" fill="#3A5070"/></svg>`;}

function svgNais3(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="n3g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#FFF5F0"/><stop offset="100%" stop-color="#FFE0D8"/></linearGradient></defs><rect width="300" height="400" fill="url(#n3g)"/><circle cx="50" cy="80" r="35" fill="#FFD060" opacity=".4"/><circle cx="250" cy="90" r="30" fill="#FFD060" opacity=".3"/><path d="M40,180 Q150,100 260,180" fill="none" stroke="#FFB8D8" stroke-width="40" opacity=".3"/><rect x="80" y="290" width="140" height="8" rx="4" fill="#8B6040"/><rect x="90" y="240" width="120" height="55" rx="6" fill="#F8D8B0"/><rect x="90" y="240" width="120" height="22" rx="6" fill="#E8B880"/><ellipse cx="150" cy="238" rx="62" ry="11" fill="#D4A060"/><rect x="130" y="205" width="8" height="38" rx="4" fill="#F8F0E0"/><ellipse cx="134" cy="203" rx="5" ry="7" fill="#FF9900"/><rect x="162" y="210" width="8" height="33" rx="4" fill="#F8F0E0"/><ellipse cx="166" cy="208" rx="5" ry="7" fill="#FF6B6B"/><g transform="translate(90,265)"><ellipse cx="0" cy="-12" rx="9" ry="11" fill="#FFB8D8" transform="rotate(0)"/><ellipse cx="0" cy="-12" rx="9" ry="11" fill="#FFA8C8" transform="rotate(72)"/><ellipse cx="0" cy="-12" rx="9" ry="11" fill="#FFB8D8" transform="rotate(144)"/><circle r="6" fill="#FFD700"/></g><g transform="translate(210,260)"><ellipse cx="0" cy="-12" rx="9" ry="11" fill="#B8D8FF" transform="rotate(0)"/><ellipse cx="0" cy="-12" rx="9" ry="11" fill="#C8E8FF" transform="rotate(72)"/><ellipse cx="0" cy="-12" rx="9" ry="11" fill="#B0D0FF" transform="rotate(144)"/><circle r="6" fill="#FFD700"/></g><circle cx="40" cy="340" r="4" fill="#FFB8D8" opacity=".7"/><circle cx="80" cy="360" r="3" fill="#FFB8D8" opacity=".6"/><circle cx="220" cy="345" r="4" fill="#B8D8FF" opacity=".7"/><circle cx="265" cy="358" r="3" fill="#B8D8FF" opacity=".6"/></svg>`;}

function svgNais4(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="n4g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#E8FFE8"/><stop offset="100%" stop-color="#C8F0C8"/></linearGradient></defs><rect width="300" height="400" fill="url(#n4g)"/><ellipse cx="60" cy="65" rx="45" ry="22" fill="white" opacity=".8"/><ellipse cx="240" cy="70" rx="50" ry="24" fill="white" opacity=".7"/><ellipse cx="150" cy="110" rx="70" ry="50" fill="rgba(100,200,100,.15)"/><rect x="75" y="300" width="150" height="70" rx="10" fill="#A8D890"/><path d="M75,300 Q150,280 225,300 L225,320 Q150,305 75,320 Z" fill="#90C878"/><ellipse cx="150" cy="298" rx="75" ry="14" fill="#78B060"/><ellipse cx="150" cy="230" rx="45" ry="55" fill="#F0F8F0"/><ellipse cx="150" cy="195" rx="32" ry="35" fill="#E8F0E8"/><ellipse cx="150" cy="182" rx="25" ry="26" fill="#D8E8D8"/><path d="M135,180 Q143,175 150,180 Q157,175 165,180" fill="none" stroke="#8B6040" stroke-width="2"/><path d="M143,188 Q150,193 157,188" fill="none" stroke="#C09070" stroke-width="1.5"/><ellipse cx="150" cy="295" rx="40" ry="18" fill="#D8F0D8"/><circle cx="88" cy="158" r="6" fill="#FFB8D8" opacity=".8"/><circle cx="212" cy="158" r="6" fill="#B8D8FF" opacity=".8"/></svg>`;}

function svgCond1(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="c1g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#E8EEF8"/><stop offset="100%" stop-color="#C8D8EC"/></linearGradient></defs><rect width="300" height="400" fill="url(#c1g)"/><ellipse cx="80" cy="80" rx="60" ry="30" fill="white" opacity=".6"/><ellipse cx="130" cy="65" rx="50" ry="25" fill="white" opacity=".7"/><ellipse cx="220" cy="85" rx="55" ry="28" fill="white" opacity=".5"/><path d="M130,120 Q150,100 170,120 Q150,108 130,120 Z" fill="white"/><ellipse cx="150" cy="120" rx="22" ry="10" fill="white"/><path d="M135,125 Q125,138 118,132 Q128,128 135,125 Z" fill="white"/><path d="M165,125 Q175,138 182,132 Q172,128 165,125 Z" fill="white"/><circle cx="143" cy="118" r="3" fill="#5A7090"/><rect x="70" y="260" width="8" height="60" rx="4" fill="#F8F0E0"/><ellipse cx="74" cy="258" rx="5" ry="7" fill="#FF8800" opacity=".9"/><ellipse cx="74" cy="258" rx="3" ry="4" fill="#FFD700"/><rect x="140" y="250" width="10" height="70" rx="5" fill="#F8F0E0"/><ellipse cx="145" cy="248" rx="6" ry="8" fill="#FF8800" opacity=".9"/><ellipse cx="145" cy="248" rx="4" ry="5" fill="#FFD700"/><rect x="222" y="260" width="8" height="60" rx="4" fill="#F8F0E0"/><ellipse cx="226" cy="258" rx="5" ry="7" fill="#FF8800" opacity=".9"/><g transform="translate(110,300)"><ellipse cx="0" cy="-10" rx="8" ry="10" fill="white" transform="rotate(0)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="white" transform="rotate(60)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="white" transform="rotate(120)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="white" transform="rotate(180)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="white" transform="rotate(240)"/><circle r="6" fill="#F0F0E8"/></g><g transform="translate(195,295)"><ellipse cx="0" cy="-10" rx="8" ry="10" fill="white" transform="rotate(0)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="white" transform="rotate(60)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="white" transform="rotate(120)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="white" transform="rotate(180)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="white" transform="rotate(240)"/><circle r="6" fill="#F0F0E8"/></g><rect x="110" y="340" width="80" height="50" rx="6" fill="#2A4A2A"/><rect x="113" y="343" width="74" height="44" rx="4" fill="#3A5A3A"/><ellipse cx="150" cy="365" rx="20" ry="18" fill="none" stroke="#C8922A" stroke-width="1.5" opacity=".6"/><line x1="130" y1="365" x2="170" y2="365" stroke="#C8922A" stroke-width="1" opacity=".5"/><line x1="150" y1="347" x2="150" y2="383" stroke="#C8922A" stroke-width="1" opacity=".5"/></svg>`;}

function svgCond2(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="c2g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#F5F0EC"/><stop offset="100%" stop-color="#E5D8CC"/></linearGradient></defs><rect width="300" height="400" fill="url(#c2g)"/><rect x="0" y="260" width="300" height="140" fill="#8B6040"/><ellipse cx="150" cy="262" rx="150" ry="15" fill="#C06020" opacity=".4"/><circle cx="150" cy="170" r="60" fill="#FF8C00" opacity=".2"/><circle cx="150" cy="185" r="45" fill="#FF6600" opacity=".15"/><rect x="35" y="180" width="18" height="90" fill="#6B4020"/><ellipse cx="44" cy="175" rx="32" ry="26" fill="#4A7020"/><rect x="248" y="200" width="14" height="68" fill="#6B4020"/><ellipse cx="255" cy="196" rx="26" ry="21" fill="#4A7020"/><rect x="100" y="240" width="100" height="58" fill="#C8905A"/><polygon points="100,240 200,240 150,205" fill="#A07030"/><rect x="135" y="268" width="30" height="30" fill="#7A4820"/><ellipse cx="115" cy="245" rx="8" ry="9" fill="#5A3010"/><rect x="108" y="253" width="14" height="20" rx="3" fill="#7A4020"/><ellipse cx="185" cy="243" rx="9" ry="10" fill="#5A3010"/><rect x="177" y="251" width="16" height="22" rx="3" fill="#8A5030"/><ellipse cx="150" cy="248" rx="6" ry="7" fill="#7A4820"/><rect x="145" y="254" width="10" height="14" rx="2" fill="#9A6040"/><circle cx="55" cy="55" r="2" fill="#FFD700" opacity=".8"/><circle cx="250" cy="45" r="2" fill="#FFD700" opacity=".7"/><circle cx="150" cy="30" r="1.5" fill="#fff" opacity=".6"/></svg>`;}

function svgCond3(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="c3g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#1A1A2A"/><stop offset="50%" stop-color="#2A2A3A"/><stop offset="100%" stop-color="#1A1A2A"/></linearGradient></defs><rect width="300" height="400" fill="url(#c3g)"/><circle cx="150" cy="130" r="65" fill="#FFF8E0" opacity=".12"/><circle cx="150" cy="130" r="50" fill="#FFF8E0" opacity=".1"/><path d="M112,110 Q150,140 188,110 Q188,80 150,70 Q112,80 112,110 Z" fill="white" opacity=".85"/><path d="M128,128 Q142,110 150,108 Q158,110 172,128 Q160,130 150,128 Q140,130 128,128 Z" fill="white" opacity=".6"/><circle cx="135" cy="118" r="3" fill="#3A3A4A" opacity=".5"/><circle cx="165" cy="118" r="3" fill="#3A3A4A" opacity=".5"/><rect x="55" y="260" width="8" height="60" rx="4" fill="#E8E0D0" opacity=".7"/><ellipse cx="59" cy="258" rx="5" ry="7" fill="#FF8800" opacity=".7"/><rect x="147" y="250" width="6" height="70" rx="3" fill="#E8E0D0" opacity=".8"/><ellipse cx="150" cy="248" rx="4" ry="6" fill="#FFD700" opacity=".8"/><rect x="237" y="260" width="8" height="60" rx="4" fill="#E8E0D0" opacity=".7"/><ellipse cx="241" cy="258" rx="5" ry="7" fill="#FF8800" opacity=".7"/><path d="M30,280 Q60,260 90,270 Q70,275 50,290 Z" fill="#6A9040" opacity=".5"/><path d="M210,280 Q240,260 270,270 Q250,275 230,290 Z" fill="#6A9040" opacity=".5"/><circle cx="50" cy="50" r="2.5" fill="#FFD700" opacity=".6"/><circle cx="250" cy="40" r="2" fill="#FFD700" opacity=".5"/><circle cx="150" cy="30" r="2" fill="#fff" opacity=".4"/></svg>`;}

function svgCond4(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="c4g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#F0F4F8"/><stop offset="100%" stop-color="#D8E8F4"/></linearGradient></defs><rect width="300" height="400" fill="url(#c4g)"/><path d="M100,160 Q150,100 200,160 Q200,260 150,300 Q100,260 100,160 Z" fill="rgba(200,220,240,.4)"/><rect x="130" y="320" width="40" height="50" fill="#8B6040" opacity=".6"/><ellipse cx="150" cy="320" rx="50" ry="12" fill="#A08060" opacity=".5"/><g transform="translate(150,200)"><ellipse cx="0" cy="-20" rx="15" ry="18" fill="white" transform="rotate(0)"/><ellipse cx="0" cy="-20" rx="15" ry="18" fill="rgba(255,255,255,.9)" transform="rotate(45)"/><ellipse cx="0" cy="-20" rx="15" ry="18" fill="white" transform="rotate(90)"/><ellipse cx="0" cy="-20" rx="15" ry="18" fill="rgba(255,255,255,.9)" transform="rotate(135)"/><ellipse cx="0" cy="-20" rx="15" ry="18" fill="white" transform="rotate(180)"/><ellipse cx="0" cy="-20" rx="15" ry="18" fill="rgba(255,255,255,.9)" transform="rotate(225)"/><circle r="10" fill="#F0F0E8"/></g><rect x="70" y="280" width="8" height="55" rx="4" fill="#F8F0E0" opacity=".8"/><ellipse cx="74" cy="278" rx="5" ry="7" fill="#FF8800" opacity=".7"/><rect x="222" y="280" width="8" height="55" rx="4" fill="#F8F0E0" opacity=".8"/><ellipse cx="226" cy="278" rx="5" ry="7" fill="#FF8800" opacity=".7"/><path d="M55,160 Q70,140 90,148 Q80,158 55,160 Z" fill="#6A9040" opacity=".6"/><path d="M245,155 Q260,135 280,145 Q268,155 245,155 Z" fill="#6A9040" opacity=".6"/><circle cx="80" cy="80" r="3" fill="#A0B8D0" opacity=".7"/><circle cx="220" cy="75" r="2.5" fill="#A0B8D0" opacity=".6"/></svg>`;}

function svgTab1(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="t1g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#E8F5E0"/><stop offset="100%" stop-color="#C8E8A0"/></linearGradient></defs><rect width="300" height="400" fill="url(#t1g)"/><ellipse cx="200" cy="80" rx="40" ry="25" fill="white" opacity=".7"/><circle cx="60" cy="60" r="35" fill="#FFD060" opacity=".5"/><ellipse cx="150" cy="230" rx="55" ry="40" fill="#F0F0F0"/><ellipse cx="110" cy="215" rx="30" ry="28" fill="#F0F0F0"/><ellipse cx="90" cy="200" rx="22" ry="20" fill="#E8E0D8"/><ellipse cx="80" cy="196" rx="12" ry="10" fill="#D8D0C8"/><ellipse cx="68" cy="190" rx="8" ry="12" fill="#E0D8D0" transform="rotate(-20,68,190)"/><circle cx="84" cy="195" r="4" fill="#3A2A10"/><circle cx="85" cy="194" r="1.5" fill="#fff"/><path d="M95,186 Q100,172 108,178" stroke="#C8B080" stroke-width="3" fill="none" stroke-linecap="round"/><rect x="110" y="262" width="12" height="35" rx="6" fill="#D8D0C8"/><rect x="130" y="265" width="12" height="35" rx="6" fill="#D8D0C8"/><rect x="155" y="265" width="12" height="35" rx="6" fill="#D8D0C8"/><rect x="175" y="262" width="12" height="35" rx="6" fill="#D8D0C8"/><ellipse cx="200" cy="228" rx="12" ry="10" fill="#F0F0F0"/><ellipse cx="55" cy="240" rx="12" ry="13" fill="#C09060"/><rect x="44" y="252" width="22" height="40" rx="4" fill="#FF8C20"/><ellipse cx="240" cy="238" rx="12" ry="13" fill="#C8906A"/><rect x="229" y="250" width="22" height="40" rx="4" fill="#20A0FF"/><rect x="0" y="300" width="300" height="100" fill="#7AB840"/><polygon points="240,50 242,43 244,50 251,50 245,54 247,61 240,56 233,61 235,54 229,50" fill="#FFD700" transform="scale(0.7) translate(200,20)"/><path d="M245,50 Q262,40 278,50 Q262,36 245,50 Z" fill="#FFD700" transform="scale(0.8) translate(40,15)"/></svg>`;}

function svgTab2(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="t2g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#FFF8E0"/><stop offset="100%" stop-color="#FFE8A0"/></linearGradient></defs><rect width="300" height="400" fill="url(#t2g)"/><circle cx="150" cy="120" r="70" fill="#FF8800" opacity=".2"/><rect x="0" y="290" width="300" height="110" fill="#7AB840"/><rect x="20" y="260" width="25" height="55" fill="#6B4020"/><ellipse cx="32" cy="256" rx="30" ry="24" fill="#4A7020"/><rect x="256" y="275" width="22" height="40" fill="#6B4020"/><ellipse cx="267" cy="272" rx="28" ry="22" fill="#4A7020"/><rect x="90" y="250" width="120" height="65" fill="#C8905A"/><polygon points="90,250 210,250 150,210" fill="#A07030"/><rect x="126" y="278" width="48" height="37" fill="#7A4820"/><ellipse cx="110" cy="256" rx="9" ry="10" fill="#8A5030"/><rect x="102" y="265" width="16" height="22" rx="3" fill="#7A4020"/><ellipse cx="190" cy="254" rx="9" ry="10" fill="#8A5030"/><rect x="182" y="264" width="16" height="22" rx="3" fill="#7A4020"/><ellipse cx="150" cy="257" rx="7" ry="8" fill="#7A4820"/><rect x="144" y="264" width="12" height="16" rx="2" fill="#9A6040"/><rect x="130" y="185" width="40" height="30" rx="5" fill="#C09060"/><ellipse cx="150" cy="183" rx="22" ry="20" fill="#C8906A"/><ellipse cx="150" cy="172" rx="15" ry="15" fill="#C09060"/><rect x="144" y="155" width="12" height="20" rx="6" fill="#F8F0E0"/><polygon points="250,55 252,48 254,55 261,55 255,59 257,66 250,61 243,66 245,59 239,55" fill="#FFD700"/></svg>`;}

function svgTab3(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="t3g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#0A0820"/><stop offset="50%" stop-color="#1A1240"/><stop offset="100%" stop-color="#0A0420"/></linearGradient></defs><rect width="300" height="400" fill="url(#t3g)"/><circle cx="150" cy="100" r="55" fill="#FFF8E0" opacity=".25"/><circle cx="150" cy="100" r="42" fill="#0A0820" opacity=".8"/><polygon points="190,65 193,55 196,65 206,65 198,71 201,81 193,75 185,81 188,71 180,65" fill="#FFD700" opacity=".9"/><rect x="50" y="240" width="200" height="120" fill="#1A100A"/><rect x="80" y="210" width="140" height="50" fill="#221408"/><rect x="60" y="160" width="20" height="100" fill="#2A1810"/><polygon points="60,160 80,160 70,140" fill="#3A2418"/><circle cx="70" cy="139" r="5" fill="#C8922A"/><rect x="220" y="160" width="20" height="100" fill="#2A1810"/><polygon points="220,160 240,160 230,140" fill="#3A2418"/><circle cx="230" cy="139" r="5" fill="#C8922A"/><ellipse cx="150" cy="210" rx="45" ry="30" fill="#2A1808"/><rect x="145" y="180" width="10" height="32" fill="#C8922A"/><circle cx="150" cy="178" r="6" fill="#C8922A"/><rect x="90" y="248" width="12" height="18" rx="3" fill="#FFD700" opacity=".7"/><rect x="120" y="245" width="12" height="22" rx="3" fill="#FFD700" opacity=".6"/><rect x="168" y="245" width="12" height="22" rx="3" fill="#FFD700" opacity=".6"/><rect x="198" y="248" width="12" height="18" rx="3" fill="#FFD700" opacity=".7"/><circle cx="40" cy="40" r="2" fill="#fff" opacity=".7"/><circle cx="200" cy="30" r="1.5" fill="#FFD700" opacity=".9"/><circle cx="270" cy="55" r="2" fill="#fff" opacity=".6"/></svg>`;}

function svgTab4(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="t4g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#E0F0E8"/><stop offset="100%" stop-color="#B8E0C8"/></linearGradient></defs><rect width="300" height="400" fill="url(#t4g)"/><rect x="0" y="280" width="300" height="120" fill="#5A8040"/><ellipse cx="150" cy="280" rx="150" ry="18" fill="#4A7030" opacity=".7"/><rect x="40" y="210" width="220" height="12" rx="6" fill="#8B6040"/><rect x="55" y="175" width="190" height="40" rx="6" fill="#D4B060"/><ellipse cx="150" cy="174" rx="97" ry="14" fill="#C8A050"/><rect x="80" y="145" width="140" height="32" rx="6" fill="#E8C870"/><ellipse cx="150" cy="144" rx="72" ry="12" fill="#D4B060"/><rect x="100" y="118" width="100" height="30" rx="5" fill="#F0D880"/><ellipse cx="150" cy="117" rx="52" ry="11" fill="#DCC860"/><ellipse cx="150" cy="116" rx="30" ry="10" fill="#C8B040"/><rect x="145" y="90" width="10" height="30" rx="5" fill="#F8F0E0"/><ellipse cx="150" cy="88" rx="6" ry="8" fill="#FF8800" opacity=".9"/><path d="M90,210 Q150,195 210,210" stroke="#8B6040" stroke-width="4" fill="none"/><polygon points="255,55 257,48 259,55 266,55 260,59 262,66 255,61 248,66 250,59 244,55" fill="#FFD700" opacity=".9"/><path d="M40,65 Q55,55 70,65 Q55,50 40,65 Z" fill="#FFE880" opacity=".8"/></svg>`;}

function svgKor1(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="k1g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#0A0820"/><stop offset="50%" stop-color="#1A1240"/><stop offset="100%" stop-color="#0A0420"/></linearGradient></defs><rect width="300" height="400" fill="url(#k1g)"/><circle cx="150" cy="130" r="80" fill="#FFF8E0" opacity=".12"/><circle cx="150" cy="130" r="60" fill="#0A0820" opacity=".85"/><path d="M113,110 Q138,140 165,108 Q140,130 113,110 Z" fill="#FFF8E0" opacity=".9"/><polygon points="200,68 203,58 206,68 216,68 208,74 211,84 203,78 195,84 198,74 190,68" fill="#FFD700" opacity=".9"/><circle cx="40" cy="40" r="2" fill="#fff" opacity=".8"/><circle cx="260" cy="50" r="2" fill="#FFD700" opacity=".7"/><circle cx="130" cy="25" r="1.5" fill="#fff" opacity=".6"/><rect x="50" y="240" width="200" height="120" fill="#1A100A"/><rect x="80" y="210" width="140" height="50" fill="#221408"/><rect x="60" y="162" width="20" height="98" fill="#2A1810"/><polygon points="60,162 80,162 70,142" fill="#3A2418"/><circle cx="70" cy="141" r="5" fill="#C8922A"/><rect x="220" y="162" width="20" height="98" fill="#2A1810"/><polygon points="220,162 240,162 230,142" fill="#3A2418"/><circle cx="230" cy="141" r="5" fill="#C8922A"/><ellipse cx="150" cy="210" rx="42" ry="28" fill="#2A1808"/><rect x="145" y="182" width="10" height="30" fill="#C8922A"/><circle cx="150" cy="180" r="6" fill="#C8922A"/><rect x="92" y="248" width="12" height="18" rx="3" fill="#FFD700" opacity=".7"/><rect x="122" y="245" width="12" height="22" rx="3" fill="#FFD700" opacity=".6"/><rect x="166" y="245" width="12" height="22" rx="3" fill="#FFD700" opacity=".6"/><rect x="196" y="248" width="12" height="18" rx="3" fill="#FFD700" opacity=".7"/><path d="M55,225 Q135,215 205,225" stroke="#FFF8E0" stroke-width="1.5" fill="none" opacity=".3"/></svg>`;}

function svgKor2(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="k2g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#1A1030"/><stop offset="100%" stop-color="#2A1840"/></linearGradient></defs><rect width="300" height="400" fill="url(#k2g)"/><circle cx="50" cy="50" r="2" fill="#fff" opacity=".7"/><circle cx="250" cy="38" r="1.5" fill="#FFD700" opacity=".8"/><circle cx="170" cy="22" r="2" fill="#fff" opacity=".6"/><line x1="45" y1="90" x2="50" y2="170" stroke="#C8922A" stroke-width="1.5" opacity=".5"/><ellipse cx="50" cy="175" rx="14" ry="18" fill="#FF8800" opacity=".4"/><ellipse cx="50" cy="175" rx="9" ry="12" fill="#FFD700" opacity=".5"/><line x1="255" y1="90" x2="250" y2="170" stroke="#C8922A" stroke-width="1.5" opacity=".5"/><ellipse cx="250" cy="175" rx="14" ry="18" fill="#FF8800" opacity=".4"/><ellipse cx="250" cy="175" rx="9" ry="12" fill="#FFD700" opacity=".5"/><g transform="translate(60,240)"><ellipse cx="0" cy="0" rx="22" ry="15" fill="#2A1000"/><ellipse cx="-5" cy="-20" rx="10" ry="15" fill="#2A1000"/><rect x="-3" y="-32" width="6" height="14" rx="3" fill="#2A1000"/><line x1="-10" y1="12" x2="-14" y2="30" stroke="#2A1000" stroke-width="3"/><line x1="2" y1="13" x2="-2" y2="32" stroke="#2A1000" stroke-width="3"/><line x1="10" y1="12" x2="14" y2="30" stroke="#2A1000" stroke-width="3"/><line x1="18" y1="10" x2="22" y2="30" stroke="#2A1000" stroke-width="3"/></g><g transform="translate(115,248)"><ellipse cx="0" cy="0" rx="20" ry="13" fill="#2A1000"/><ellipse cx="-4" cy="-18" rx="9" ry="13" fill="#2A1000"/><rect x="-2" y="-28" width="5" height="12" rx="2" fill="#2A1000"/><line x1="-8" y1="11" x2="-12" y2="27" stroke="#2A1000" stroke-width="3"/><line x1="8" y1="11" x2="12" y2="27" stroke="#2A1000" stroke-width="3"/></g><rect x="0" y="300" width="300" height="100" fill="#3A1800"/><path d="M0,280 Q70,265 140,278 Q210,292 300,275 L300,400 L0,400 Z" fill="#2A1200"/><ellipse cx="150" cy="355" rx="120" ry="12" fill="#1A0A00" opacity=".5"/><path d="M70,290 Q150,280 230,290" stroke="#FFD700" stroke-width="1" fill="none" opacity=".2"/></svg>`;}

function svgKor3(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="k3g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#2A1840"/><stop offset="100%" stop-color="#1A1030"/></linearGradient></defs><rect width="300" height="400" fill="url(#k3g)"/><path d="M0,180 Q150,120 300,180 L300,400 L0,400 Z" fill="#1A0A05" opacity=".7"/><circle cx="150" cy="130" r="70" fill="#FFF8E0" opacity=".1"/><rect x="60" y="150" width="180" height="130" fill="#2A1808" opacity=".9"/><rect x="80" y="120" width="140" height="50" fill="#221408" opacity=".9"/><rect x="55" y="155" width="20" height="130" fill="#2A1810"/><polygon points="55,155 75,155 65,135" fill="#3A2418"/><circle cx="65" cy="134" r="5" fill="#C8922A"/><rect x="225" y="155" width="20" height="130" fill="#2A1810"/><polygon points="225,155 245,155 235,135" fill="#3A2418"/><circle cx="235" cy="134" r="5" fill="#C8922A"/><ellipse cx="150" cy="150" rx="45" ry="30" fill="#2A1808"/><rect x="145" y="120" width="10" height="32" fill="#C8922A"/><circle cx="150" cy="118" r="6" fill="#C8922A"/><rect x="88" y="200" width="12" height="20" rx="3" fill="#FFD700" opacity=".8"/><rect x="118" y="197" width="12" height="24" rx="3" fill="#FFD700" opacity=".7"/><rect x="170" y="197" width="12" height="24" rx="3" fill="#FFD700" opacity=".7"/><rect x="200" y="200" width="12" height="20" rx="3" fill="#FFD700" opacity=".8"/><path d="M112,108 Q136,140 162,106 Q136,128 112,108 Z" fill="#FFF8E0" opacity=".8"/><polygon points="198,65 201,55 204,65 214,65 206,71 209,81 201,75 193,81 196,71 188,65" fill="#FFD700" opacity=".8"/><circle cx="45" cy="40" r="1.5" fill="#fff" opacity=".6"/><circle cx="265" cy="48" r="2" fill="#FFD700" opacity=".6"/></svg>`;}

function svgKor4(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="k4g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#F8F0E8"/><stop offset="100%" stop-color="#EAD8C0"/></linearGradient></defs><rect width="300" height="400" fill="url(#k4g)"/><pattern id="pk4" width="40" height="40" patternUnits="userSpaceOnUse"><circle cx="20" cy="20" r="8" fill="none" stroke="#C8922A" stroke-width="1.2" opacity=".18"/><circle cx="0" cy="0" r="6" fill="none" stroke="#C8922A" stroke-width="1" opacity=".12"/><circle cx="40" cy="40" r="6" fill="none" stroke="#C8922A" stroke-width="1" opacity=".12"/></pattern><rect width="300" height="400" fill="url(#pk4)"/><rect x="60" y="260" width="180" height="115" rx="4" fill="rgba(200,146,42,.05)"/><g transform="translate(90,310)"><ellipse cx="0" cy="-10" rx="8" ry="10" fill="#FFB8D8" transform="rotate(0)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="#FFA8C8" transform="rotate(72)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="#FFB8D8" transform="rotate(144)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="#FFC8D8" transform="rotate(216)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="#FFB0D0" transform="rotate(288)"/><circle r="6" fill="#FFD700"/></g><g transform="translate(210,305)"><ellipse cx="0" cy="-10" rx="8" ry="10" fill="#C8E0A0" transform="rotate(0)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="#C8E8A8" transform="rotate(72)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="#B8D890" transform="rotate(144)"/><circle r="6" fill="#FFD700"/></g><rect x="110" y="185" width="80" height="55" rx="6" fill="#D4B060" opacity=".8"/><ellipse cx="150" cy="184" rx="42" ry="12" fill="#C8A050"/><rect x="100" y="155" width="100" height="35" rx="6" fill="#E8C870" opacity=".9"/><ellipse cx="150" cy="154" rx="52" ry="12" fill="#D4B060"/><ellipse cx="150" cy="152" rx="32" ry="11" fill="#C8A040"/><rect x="146" y="128" width="8" height="27" rx="4" fill="#F8F0E0"/><ellipse cx="150" cy="126" rx="5" ry="7" fill="#FF8800" opacity=".9"/><path d="M108,185 Q150,172 192,185" stroke="#8B6040" stroke-width="3" fill="none"/></svg>`;}

function svgTam1(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="tm1g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#3A1A00"/><stop offset="50%" stop-color="#6A3A10"/><stop offset="100%" stop-color="#2A1000"/></linearGradient></defs><rect width="300" height="400" fill="url(#tm1g)"/><ellipse cx="150" cy="350" rx="60" ry="15" fill="#FF4400" opacity=".3"/><path d="M130,280 Q150,220 170,280 Q165,250 150,240 Q135,250 130,280 Z" fill="#FF6600"/><path d="M138,280 Q150,235 162,280 Q158,258 150,250 Q142,258 138,280 Z" fill="#FF9900"/><path d="M143,275 Q150,248 157,275 Q154,262 150,258 Q146,262 143,275 Z" fill="#FFD700"/><ellipse cx="90" cy="310" rx="40" ry="15" fill="#8B6040"/><path d="M50,300 Q90,290 130,300 Q130,320 90,325 Q50,320 50,300 Z" fill="#C09060"/><ellipse cx="90" cy="299" rx="38" ry="13" fill="#D4B060" opacity=".9"/><ellipse cx="90" cy="300" rx="30" ry="8" fill="#E8C880" opacity=".8"/><ellipse cx="210" cy="310" rx="40" ry="15" fill="#8B6040"/><path d="M170,300 Q210,290 250,300 Q250,320 210,325 Q170,320 170,300 Z" fill="#C09060"/><ellipse cx="210" cy="299" rx="38" ry="13" fill="#D4B060" opacity=".9"/><ellipse cx="210" cy="300" rx="30" ry="8" fill="#E8C880" opacity=".8"/><ellipse cx="60" cy="255" rx="12" ry="13" fill="#8B5030"/><path d="M48,267 Q42,300 45,310 L75,310 Q78,300 72,267 Z" fill="#C8902A"/><line x1="45" y1="260" x2="35" y2="310" stroke="#6B4020" stroke-width="3"/><ellipse cx="115" cy="248" rx="12" ry="13" fill="#C09060"/><path d="M103,260 Q97,295 100,305 L130,305 Q133,295 127,260 Z" fill="#E06020"/><ellipse cx="185" cy="248" rx="13" ry="14" fill="#A07040"/><path d="M172,261 Q166,296 170,308 L200,308 Q204,296 198,261 Z" fill="#F0F0E0"/><ellipse cx="240" cy="258" rx="10" ry="11" fill="#C89060"/><path d="M230,268 Q225,295 228,303 L252,303 Q255,295 250,268 Z" fill="#60A8E0"/><circle cx="150" cy="30" r="2.5" fill="#FFD700" opacity=".9"/><circle cx="80" cy="50" r="2" fill="#fff" opacity=".7"/><circle cx="220" cy="45" r="2" fill="#fff" opacity=".6"/></svg>`;}

function svgTam2(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="tm2g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#2A1800"/><stop offset="50%" stop-color="#5A3010"/><stop offset="100%" stop-color="#1A0A00"/></linearGradient></defs><rect width="300" height="400" fill="url(#tm2g)"/><circle cx="150" cy="120" r="60" fill="#FF8800" opacity=".25"/><circle cx="150" cy="130" r="45" fill="#FF6600" opacity=".2"/><circle cx="150" cy="140" r="30" fill="#FF4400" opacity=".15"/><rect x="0" y="290" width="300" height="110" fill="#3A1E00"/><ellipse cx="150" cy="295" rx="150" ry="15" fill="#4A2800" opacity=".7"/><rect x="35" y="185" width="18" height="125" fill="#6B4020"/><ellipse cx="44" cy="180" rx="32" ry="26" fill="#4A7020"/><rect x="248" y="200" width="14" height="100" fill="#6B4020"/><ellipse cx="255" cy="196" rx="26" ry="21" fill="#4A7020"/><rect x="100" y="255" width="100" height="58" fill="#C8905A"/><polygon points="100,255 200,255 150,215" fill="#A07030"/><rect x="135" y="278" width="30" height="30" fill="#7A4820"/><ellipse cx="115" cy="260" rx="8" ry="9" fill="#5A3010"/><rect x="108" y="268" width="14" height="20" rx="3" fill="#7A4020"/><ellipse cx="185" cy="258" rx="9" ry="10" fill="#5A3010"/><rect x="177" y="266" width="16" height="22" rx="3" fill="#8A5030"/><ellipse cx="150" cy="263" rx="6" ry="7" fill="#7A4820"/><rect x="145" y="269" width="10" height="14" rx="2" fill="#9A6040"/><circle cx="55" cy="55" r="2" fill="#FFD700" opacity=".8"/><circle cx="250" cy="45" r="2" fill="#FFD700" opacity=".7"/></svg>`;}

function svgTam3(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="tm3g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#FF8C00"/><stop offset="30%" stop-color="#CC5500"/><stop offset="70%" stop-color="#8B3A00"/><stop offset="100%" stop-color="#3A1A00"/></linearGradient></defs><rect width="300" height="400" fill="url(#tm3g)"/><circle cx="150" cy="150" r="80" fill="#FF8800" opacity=".25"/><circle cx="150" cy="160" r="60" fill="#FF6600" opacity=".2"/><path d="M0,280 Q68,220 135,250 Q202,280 270,240 L270,360 L0,360 Z" fill="#8B5020"/><path d="M0,310 Q70,260 140,290 Q210,320 270,280 L270,360 L0,360 Z" fill="#A06030"/><path d="M0,335 Q90,305 180,325 Q225,335 270,315 L270,360 L0,360 Z" fill="#B87040"/><rect x="205" y="200" width="10" height="80" fill="#4A2A00"/><path d="M210,200 Q235,180 220,200 Q240,175 215,198" fill="#3A6020" stroke="#3A6020" stroke-width="2"/><path d="M210,200 Q185,180 200,200 Q180,175 205,198" fill="#4A7030" stroke="#4A7030" stroke-width="2"/><path d="M0,280 Q50,260 90,268 Q70,274 50,288 Z" fill="#6A9040" opacity=".5"/><g transform="translate(60,240)"><ellipse cx="0" cy="0" rx="22" ry="15" fill="#2A1000" opacity=".8"/><ellipse cx="-5" cy="-20" rx="10" ry="15" fill="#2A1000" opacity=".8"/><rect x="-3" y="-32" width="6" height="14" rx="3" fill="#2A1000" opacity=".8"/><line x1="-10" y1="12" x2="-14" y2="30" stroke="#2A1000" stroke-width="3" opacity=".8"/><line x1="10" y1="12" x2="14" y2="30" stroke="#2A1000" stroke-width="3" opacity=".8"/></g><circle cx="50" cy="50" r="2.5" fill="#FFD700" opacity=".8"/><circle cx="250" cy="40" r="2" fill="#FFD700" opacity=".7"/><circle cx="150" cy="30" r="1.5" fill="#fff" opacity=".6"/></svg>`;}

function svgTam4(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="tm4g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#FFF8DC"/><stop offset="100%" stop-color="#FFE8A0"/></linearGradient></defs><rect width="300" height="400" fill="url(#tm4g)"/><rect x="0" y="270" width="300" height="130" fill="#7AB840"/><ellipse cx="150" cy="272" rx="150" ry="18" fill="#5A9030" opacity=".6"/><rect x="40" y="220" width="220" height="12" rx="6" fill="#8B6040"/><rect x="55" y="182" width="190" height="42" rx="6" fill="#D4B060"/><ellipse cx="150" cy="181" rx="97" ry="14" fill="#C8A050"/><rect x="80" y="150" width="140" height="35" rx="6" fill="#E8C870"/><ellipse cx="150" cy="149" rx="72" ry="13" fill="#D4B060"/><rect x="100" y="122" width="100" height="30" rx="5" fill="#F0D880"/><ellipse cx="150" cy="121" rx="52" ry="11" fill="#DCC860"/><ellipse cx="150" cy="119" rx="30" ry="10" fill="#C8B040"/><rect x="145" y="93" width="10" height="30" rx="5" fill="#F8F0E0"/><ellipse cx="150" cy="91" rx="6" ry="8" fill="#FF8800" opacity=".9"/><path d="M90,220 Q150,205 210,220" stroke="#8B6040" stroke-width="4" fill="none"/><ellipse cx="55" cy="240" rx="12" ry="13" fill="#C09060"/><rect x="44" y="252" width="22" height="25" rx="4" fill="#FF8C20"/><ellipse cx="240" cy="238" rx="12" ry="13" fill="#C8906A"/><rect x="229" y="250" width="22" height="25" rx="4" fill="#3070C0"/><circle cx="55" cy="55" r="2" fill="#FFD700" opacity=".8"/><circle cx="250" cy="48" r="2" fill="#FFD700" opacity=".7"/></svg>`;}

function svgAmour1(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="am1g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#1A0820"/><stop offset="50%" stop-color="#2A0A10"/><stop offset="100%" stop-color="#3A1828"/></linearGradient><radialGradient id="glo" cx="50%" cy="55%" r="45%"><stop offset="0%" stop-color="rgba(220,80,80,.3)"/><stop offset="100%" stop-color="transparent"/></radialGradient></defs><rect width="300" height="400" fill="url(#am1g)"/><rect width="300" height="400" fill="url(#glo)"/><circle cx="30" cy="30" r="2" fill="#fff" opacity=".7"/><circle cx="70" cy="20" r="1.5" fill="#FFD700" opacity=".8"/><circle cx="240" cy="25" r="2" fill="#fff" opacity=".6"/><g transform="translate(150,180)"><ellipse cx="0" cy="-40" rx="28" ry="32" fill="#E03060" transform="rotate(0)"/><ellipse cx="0" cy="-40" rx="24" ry="28" fill="#C82050" transform="rotate(60)"/><ellipse cx="0" cy="-40" rx="20" ry="24" fill="#D02858" transform="rotate(120)"/><ellipse cx="0" cy="-40" rx="16" ry="20" fill="#E03868" transform="rotate(180)"/><ellipse cx="0" cy="-40" rx="12" ry="16" fill="#C82048" transform="rotate(240)"/><circle r="14" fill="#C01840"/><circle r="8" fill="#A01030"/></g><line x1="150" y1="220" x2="150" y2="330" stroke="#3A6020" stroke-width="4"/><ellipse cx="125" cy="265" rx="22" ry="10" fill="#4A7828" transform="rotate(-30,125,265)"/><ellipse cx="175" cy="295" rx="22" ry="10" fill="#3A6820" transform="rotate(30,175,295)"/><path d="M55,80 Q58,73 62,80 Q66,73 69,80 Q69,88 62,94 Q55,88 55,80 Z" fill="#E03060" opacity=".8"/><path d="M230,90 Q232,85 235,90 Q238,85 240,90 Q240,96 235,101 Q230,96 230,90 Z" fill="#E03060" opacity=".7"/><rect x="45" y="312" width="7" height="40" rx="3" fill="#F8F0E0"/><ellipse cx="48.5" cy="310" rx="4" ry="6" fill="#FF8800" opacity=".8"/><rect x="248" y="312" width="7" height="40" rx="3" fill="#F8F0E0"/><ellipse cx="251.5" cy="310" rx="4" ry="6" fill="#FF8800" opacity=".8"/></svg>`;}

function svgAmour2(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="am2g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#FFFEF5"/><stop offset="100%" stop-color="#FFF5DC"/></linearGradient></defs><rect width="300" height="400" fill="url(#am2g)"/><circle cx="150" cy="180" r="100" fill="rgba(220,80,80,.06)"/><g transform="translate(150,170)"><path d="M0,-55 Q22,-70 30,-45 Q40,-20 0,10 Q-40,-20 -30,-45 Q-22,-70 0,-55 Z" fill="#E03060"/><path d="M0,-45 Q18,-58 24,-37 Q32,-15 0,8 Q-32,-15 -24,-37 Q-18,-58 0,-45 Z" fill="#C82050"/><path d="M0,-35 Q14,-46 18,-29 Q24,-10 0,6 Q-24,-10 -18,-29 Q-14,-46 0,-35 Z" fill="#D02858"/></g><line x1="150" y1="220" x2="150" y2="330" stroke="#3A6020" stroke-width="4"/><ellipse cx="125" cy="265" rx="22" ry="10" fill="#4A7828" transform="rotate(-30,125,265)"/><ellipse cx="175" cy="295" rx="22" ry="10" fill="#3A6820" transform="rotate(30,175,295)"/><rect x="45" y="315" width="7" height="38" rx="3" fill="#F8F0E0"/><ellipse cx="48.5" cy="313" rx="4" ry="6" fill="#FF8800" opacity=".8"/><rect x="248" y="315" width="7" height="38" rx="3" fill="#F8F0E0"/><ellipse cx="251.5" cy="313" rx="4" ry="6" fill="#FF8800" opacity=".8"/><path d="M70,70 Q73,63 77,70 Q81,63 84,70 Q84,78 77,84 Q70,78 70,70 Z" fill="#E03060" opacity=".7"/><path d="M218,75 Q220,70 223,75 Q226,70 228,75 Q228,81 223,86 Q218,81 218,75 Z" fill="#E03060" opacity=".6"/><ellipse cx="80" cy="350" rx="6" ry="3" fill="#E03060" transform="rotate(-20,80,350)" opacity=".5"/><ellipse cx="220" cy="345" rx="6" ry="3" fill="#E03060" transform="rotate(10,220,345)" opacity=".5"/></svg>`;}

function svgAmour3(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="am3g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#FFE8F0"/><stop offset="100%" stop-color="#FFD0E0"/></linearGradient></defs><rect width="300" height="400" fill="url(#am3g)"/><path d="M0,0 L300,0 L300,200 Q150,160 0,200 Z" fill="rgba(220,80,80,.06)"/><rect x="30" y="290" width="240" height="90" rx="8" fill="rgba(220,80,80,.04)"/><g transform="translate(100,140)"><ellipse cx="0" cy="-10" rx="9" ry="11" fill="#FFB8D8" transform="rotate(0)"/><ellipse cx="0" cy="-10" rx="9" ry="11" fill="#FFA8C8" transform="rotate(72)"/><ellipse cx="0" cy="-10" rx="9" ry="11" fill="#FFB8D8" transform="rotate(144)"/><ellipse cx="0" cy="-10" rx="9" ry="11" fill="#FFC8D8" transform="rotate(216)"/><ellipse cx="0" cy="-10" rx="9" ry="11" fill="#FFB0D0" transform="rotate(288)"/><circle r="7" fill="#FFD700"/></g><g transform="translate(200,150)"><ellipse cx="0" cy="-10" rx="9" ry="11" fill="#E03060" transform="rotate(0)"/><ellipse cx="0" cy="-10" rx="9" ry="11" fill="#C82050" transform="rotate(72)"/><ellipse cx="0" cy="-10" rx="9" ry="11" fill="#D02858" transform="rotate(144)"/><ellipse cx="0" cy="-10" rx="9" ry="11" fill="#E03060" transform="rotate(216)"/><ellipse cx="0" cy="-10" rx="9" ry="11" fill="#C82050" transform="rotate(288)"/><circle r="7" fill="#FFD700"/></g><g transform="translate(150,230)"><ellipse cx="0" cy="-14" rx="12" ry="15" fill="#E03060" transform="rotate(0)"/><ellipse cx="0" cy="-14" rx="12" ry="15" fill="#C82050" transform="rotate(60)"/><ellipse cx="0" cy="-14" rx="12" ry="15" fill="#D02858" transform="rotate(120)"/><ellipse cx="0" cy="-14" rx="12" ry="15" fill="#E03868" transform="rotate(180)"/><ellipse cx="0" cy="-14" rx="12" ry="15" fill="#C82048" transform="rotate(240)"/><ellipse cx="0" cy="-14" rx="12" ry="15" fill="#D82858" transform="rotate(300)"/><circle r="10" fill="#A01030"/></g><path d="M150,244 L150,320" stroke="#3A6020" stroke-width="4"/><ellipse cx="128" cy="278" rx="20" ry="9" fill="#4A7828" transform="rotate(-30,128,278)"/><ellipse cx="172" cy="302" rx="20" ry="9" fill="#3A6820" transform="rotate(30,172,302)"/></svg>`;}

function svgAmour4(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="am4g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#0A0820"/><stop offset="100%" stop-color="#180A28"/></linearGradient></defs><rect width="300" height="400" fill="url(#am4g)"/><circle cx="30" cy="30" r="1.5" fill="#fff" opacity=".6"/><circle cx="270" cy="25" r="2" fill="#FFD700" opacity=".7"/><circle cx="150" cy="18" r="1.5" fill="#fff" opacity=".5"/><ellipse cx="150" cy="350" rx="90" ry="12" fill="#E03060" opacity=".2"/><g transform="translate(150,190)"><ellipse cx="0" cy="-45" rx="32" ry="36" fill="#E03060" transform="rotate(0)"/><ellipse cx="0" cy="-45" rx="28" ry="32" fill="#C82050" transform="rotate(40)"/><ellipse cx="0" cy="-45" rx="24" ry="28" fill="#D02858" transform="rotate(80)"/><ellipse cx="0" cy="-45" rx="20" ry="24" fill="#E03868" transform="rotate(120)"/><ellipse cx="0" cy="-45" rx="16" ry="20" fill="#C82048" transform="rotate(160)"/><ellipse cx="0" cy="-45" rx="12" ry="16" fill="#D82858" transform="rotate(200)"/><ellipse cx="0" cy="-45" rx="8" ry="12" fill="#E04070" transform="rotate(240)"/><circle r="16" fill="#C01840"/><circle r="9" fill="#A01030"/></g><line x1="150" y1="235" x2="150" y2="345" stroke="#3A6020" stroke-width="5"/><ellipse cx="122" cy="278" rx="24" ry="11" fill="#4A7828" transform="rotate(-30,122,278)"/><ellipse cx="178" cy="310" rx="24" ry="11" fill="#3A6820" transform="rotate(30,178,310)"/><path d="M58,85 Q62,78 66,85 Q70,78 73,85 Q73,94 66,100 Q58,94 58,85 Z" fill="#E03060" opacity=".8"/><path d="M228,92 Q231,86 234,92 Q238,86 241,92 Q241,98 234,104 Q228,98 228,92 Z" fill="#E03060" opacity=".7"/></svg>`;}

// ══ VERSO SVG ══
const VERSO=[
  {id:'wakanda',name:'Wakanda',svg:()=>`<svg viewBox="0 0 270 360" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="vw" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#1A0A2E"/><stop offset="50%" stop-color="#2D1B4E"/><stop offset="100%" stop-color="#0A1628"/></linearGradient></defs><rect width="270" height="360" fill="url(#vw)"/><circle cx="135" cy="180" r="90" fill="none" stroke="#C8922A" stroke-width="1" opacity=".3"/><circle cx="135" cy="180" r="60" fill="none" stroke="#E8C060" stroke-width="1" opacity=".2"/><path d="M135,90 L155,170 L240,180 L155,190 L135,270 L115,190 L30,180 L115,170 Z" fill="none" stroke="#C8922A" stroke-width="1.5" opacity=".35"/><polygon points="135,130 115,165 135,175 155,165" fill="#4040C0" opacity=".6"/><polygon points="135,130 155,165 135,155 115,165" fill="#6060E0" opacity=".5"/><polygon points="135,175 115,165 135,185 155,165" fill="#2020A0" opacity=".7"/><pattern id="cir" width="30" height="30" patternUnits="userSpaceOnUse"><line x1="0" y1="15" x2="30" y2="15" stroke="#C8922A" stroke-width=".5" opacity=".12"/><line x1="15" y1="0" x2="15" y2="30" stroke="#C8922A" stroke-width=".5" opacity=".12"/></pattern><rect width="270" height="360" fill="url(#cir)"/><circle cx="40" cy="50" r="2" fill="#C8922A" opacity=".5"/><circle cx="230" cy="60" r="2" fill="#C8922A" opacity=".4"/></svg>`},
  {id:'savane',name:'Savane',svg:()=>`<svg viewBox="0 0 270 360" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="vs" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#FF6600"/><stop offset="40%" stop-color="#CC4400"/><stop offset="70%" stop-color="#8B3000"/><stop offset="100%" stop-color="#2A1000"/></linearGradient></defs><rect width="270" height="360" fill="url(#vs)"/><circle cx="135" cy="160" r="65" fill="#FF8800" opacity=".4"/><rect x="25" y="200" width="18" height="120" fill="#1A0A00"/><ellipse cx="34" cy="195" rx="35" ry="28" fill="#2A1A00"/><rect x="228" y="215" width="14" height="105" fill="#1A0A00"/><ellipse cx="235" cy="210" rx="28" ry="22" fill="#2A1A00"/><g transform="translate(100,200)"><rect x="0" y="0" width="8" height="50" rx="4" fill="#1A0A00"/><rect x="-5" y="-40" width="5" height="45" rx="2" fill="#1A0A00" transform="rotate(10)"/><ellipse cx="0" cy="-42" rx="10" ry="8" fill="#1A0A00" transform="rotate(10)"/><line x1="-2" y1="45" x2="-5" y2="70" stroke="#1A0A00" stroke-width="4"/><line x1="5" y1="45" x2="8" y2="70" stroke="#1A0A00" stroke-width="4"/></g><rect x="0" y="300" width="270" height="60" fill="#2A1400"/><ellipse cx="135" cy="302" rx="135" ry="10" fill="#3A1E00"/></svg>`},
  {id:'ocean',name:'Océan',svg:()=>`<svg viewBox="0 0 270 360" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="vo" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#001A3D"/><stop offset="50%" stop-color="#003366"/><stop offset="100%" stop-color="#001A3D"/></linearGradient></defs><rect width="270" height="360" fill="url(#vo)"/><circle cx="80" cy="80" r="30" fill="#FFF8E0" opacity=".25"/><circle cx="80" cy="80" r="22" fill="#FFF8E0" opacity=".3"/><path d="M0,200 Q45,185 90,200 Q135,215 180,200 Q225,185 270,200 L270,360 L0,360 Z" fill="#002244"/><path d="M0,225 Q45,212 90,225 Q135,238 180,225 Q225,212 270,225 L270,360 L0,360 Z" fill="#001A38"/><path d="M70,215 Q135,210 200,215" stroke="#FFF8E0" stroke-width="1.5" fill="none" opacity=".3"/><path d="M70,230 Q135,225 200,230" stroke="#FFF8E0" stroke-width="1" fill="none" opacity=".2"/><path d="M70,215 Q135,200 200,215 Q200,225 135,228 Q70,225 70,215 Z" fill="#6B3A10"/><rect x="100" y="195" width="5" height="28" fill="#4A2A08"/><path d="M105,195 L158,210 L105,215 Z" fill="#FF8C00" opacity=".9"/><circle cx="50" cy="40" r="1.5" fill="#fff" opacity=".7"/><circle cx="220" cy="32" r="1.5" fill="#FFD700" opacity=".8"/></svg>`},
  {id:'jungle',name:'Forêt',svg:()=>`<svg viewBox="0 0 270 360" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="vj" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#0A2A0A"/><stop offset="50%" stop-color="#1A4A1A"/><stop offset="100%" stop-color="#051005"/></linearGradient></defs><rect width="270" height="360" fill="url(#vj)"/><path d="M135,0 L100,200" stroke="rgba(255,220,100,.12)" stroke-width="20"/><path d="M135,0 L170,200" stroke="rgba(255,220,100,.10)" stroke-width="15"/><ellipse cx="20" cy="180" rx="50" ry="20" fill="#2A6020" transform="rotate(-30,20,180)"/><ellipse cx="250" cy="160" rx="50" ry="20" fill="#3A7030" transform="rotate(30,250,160)"/><ellipse cx="30" cy="280" rx="60" ry="22" fill="#1E5018" transform="rotate(-20,30,280)"/><ellipse cx="250" cy="270" rx="55" ry="20" fill="#2A6028" transform="rotate(20,250,270)"/><circle cx="110" cy="160" r="3" fill="#AAFFAA" opacity=".7"/><circle cx="160" cy="140" r="2" fill="#AAFFAA" opacity=".6"/><circle cx="140" cy="200" r="3" fill="#AAFFAA" opacity=".5"/></svg>`},
  {id:'desert',name:'Sahara',svg:()=>`<svg viewBox="0 0 270 360" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="vd" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#FF8C00"/><stop offset="30%" stop-color="#CC5500"/><stop offset="70%" stop-color="#8B3A00"/><stop offset="100%" stop-color="#3A1A00"/></linearGradient></defs><rect width="270" height="360" fill="url(#vd)"/><circle cx="135" cy="120" r="80" fill="#FF8800" opacity=".25"/><path d="M0,280 Q68,220 135,250 Q202,280 270,240 L270,360 L0,360 Z" fill="#8B5020"/><path d="M0,310 Q70,260 140,290 Q210,320 270,280 L270,360 L0,360 Z" fill="#A06030"/><rect x="205" y="200" width="10" height="80" fill="#4A2A00"/><path d="M210,200 Q235,180 220,200 Q240,175 215,198" fill="#3A6020" stroke="#3A6020" stroke-width="2"/><circle cx="50" cy="50" r="2.5" fill="#FFD700" opacity=".7"/><circle cx="220" cy="40" r="2" fill="#FFD700" opacity=".6"/></svg>`},
  {id:'cosmos',name:'Cosmos',svg:()=>`<svg viewBox="0 0 270 360" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="vc" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#000010"/><stop offset="50%" stop-color="#0A0030"/><stop offset="100%" stop-color="#100020"/></linearGradient><radialGradient id="neb" cx="50%" cy="45%" r="50%"><stop offset="0%" stop-color="rgba(100,40,200,.25)"/><stop offset="100%" stop-color="transparent"/></radialGradient></defs><rect width="270" height="360" fill="url(#vc)"/><rect width="270" height="360" fill="url(#neb)"/><circle cx="25" cy="30" r="1.5" fill="#fff" opacity=".8"/><circle cx="100" cy="20" r="1.5" fill="#FFD700" opacity=".8"/><circle cx="180" cy="30" r="1.5" fill="#fff" opacity=".7"/><circle cx="245" cy="35" r="2" fill="#C8A0FF" opacity=".7"/><circle cx="135" cy="180" r="65" fill="#1A0A4A"/><circle cx="135" cy="180" r="65" fill="none" stroke="#C8922A" stroke-width="1" opacity=".3"/><path d="M125,145 Q145,140 152,155 Q158,168 155,185 Q152,200 145,210 Q138,220 130,215 Q118,205 115,190 Q112,175 115,162 Q118,150 125,145 Z" fill="#4A8A20" opacity=".7"/><circle cx="135" cy="180" r="70" fill="none" stroke="rgba(100,160,255,.25)" stroke-width="7"/><ellipse cx="135" cy="180" rx="95" ry="18" fill="none" stroke="rgba(200,146,42,.25)" stroke-width="7"/></svg>`},
];

// ══ DATA CARTES ══
const CATS=[
  {id:'Anniversaire',icon:'🎂',label:'Anniversaire'},
  {id:'Mariage',icon:'💍',label:'Mariage'},
  {id:'Naissance',icon:'👶',label:'Naissance'},
  {id:'Condoléances',icon:'🕊️',label:'Condoléances'},
  {id:'Noel',icon:'🎄',label:'Noël'},
  {id:'Paques',icon:'🐣',label:'Pâques'},
  {id:'FeteTravail',icon:'✊',label:'Fête du Travail'},
  {id:'FinAnnee',icon:'🎆',label:'Fin d'Année'},
  {id:'SaintValentin',icon:'💖',label:'Saint-Valentin'},
  {id:'Tabaski',icon:'🐑',label:'Tabaski'},
  {id:'Korité',icon:'🌙',label:'Korité'},
  {id:'Tamkharit',icon:'🔥',label:'Tamkharit'},
  {id:'Amour',icon:'💝',label:'Amour'},
  {id:'Entreprise',icon:'🏢',label:'Entreprise'},
  {id:'Remerciement',icon:'🙏',label:'Remerciement'},
];

const CARDS=[
  // ANNIVERSAIRE
  {id:1,cat:'Anniversaire',name:'Fête en couleurs',music:{t:'Happy Birthday',a:'Stevie Wonder'},price:2500,badge:'pb-new',svgFn:svgAnniv1,title:'Joyeux Anniversaire !',msg:'Que cette journée soit aussi belle et lumineuse que tu l\'es. Puisse chaque vœu s\'exaucer !'},
  {id:2,cat:'Anniversaire',name:'Nuit de Dakar',music:{t:'Celebrate',a:'Kool & The Gang'},price:3500,badge:'pb-best',svgFn:svgAnniv2,title:'Joyeux Anniversaire !',msg:'Cette nuit t\'appartient ! Que chaque moment soit mémorable et plein de joie.'},
  {id:3,cat:'Anniversaire',name:'Élégance & Or',music:{t:'Beautiful Day',a:'U2'},price:4500,badge:'pb-prem',svgFn:svgAnniv3,title:'Joyeux Anniversaire !',msg:'Que cette belle journée soit à la hauteur de la personne extraordinaire que vous êtes.'},
  {id:4,cat:'Anniversaire',name:'Coucher de soleil',music:{t:'Africa',a:'Toto'},price:3000,badge:null,svgFn:svgAnniv4,title:'Joyeux Anniversaire !',msg:'Une vie bien remplie mérite une célébration tout aussi belle. Longue vie et santé !'},
  // MARIAGE
  {id:5,cat:'Mariage',name:'Grand Boubou',music:{t:'All You Need Is Love',a:'The Beatles'},price:5000,badge:'pb-prem',svgFn:svgMar1,title:'Félicitations aux mariés !',msg:'Vous unissez vos vies dans la tradition et la modernité. Félicitations du fond du cœur.'},
  {id:6,cat:'Mariage',name:'Jardin fleuri',music:{t:'Can You Feel The Love',a:'Elton John'},price:3500,badge:'pb-new',svgFn:svgMar2,title:'Félicitations aux mariés !',msg:'L\'amour est la plus belle aventure. Que votre voyage commence dans la joie !'},
  {id:7,cat:'Mariage',name:'Soirée élégante',music:{t:'A Thousand Years',a:'Christina Perri'},price:4000,badge:'pb-best',svgFn:svgMar3,title:'Félicitations aux mariés !',msg:'Ce soir, deux vies ne font qu\'une. Que votre bonheur dure pour toujours.'},
  {id:8,cat:'Mariage',name:'Rose éternelle',music:{t:'La Vie en Rose',a:'Louis Armstrong'},price:4200,badge:null,svgFn:svgMar4,title:'Félicitations aux mariés !',msg:'Que Dieu bénisse cette union et qu\'elle soit source de bonheur pour toute la famille.'},
  // NAISSANCE
  {id:9,cat:'Naissance',name:'Arc-en-ciel',music:{t:'What A Wonderful World',a:'Louis Armstrong'},price:2500,badge:'pb-new',svgFn:svgNais1,title:'Bienvenue dans notre monde !',msg:'Ce petit être merveilleux va illuminer votre vie. Félicitations à toute la famille !'},
  {id:10,cat:'Naissance',name:'Doux bienvenu',music:{t:'You Are My Sunshine',a:'Ray Charles'},price:3000,badge:'pb-best',svgFn:svgNais2,title:'Bienvenue dans notre monde !',msg:'La vie vient de vous offrir son plus beau cadeau. Longue vie et santé au nouveau-né !'},
  {id:11,cat:'Naissance',name:'Fête rose',music:{t:'Baby',a:'Justin Bieber'},price:2000,badge:null,svgFn:svgNais3,title:'Bienvenue dans notre monde !',msg:'Un bébé est une bénédiction de Dieu. Félicitations aux heureux parents !'},
  {id:12,cat:'Naissance',name:'Herbe verte',music:{t:'Pure Imagination',a:'Gene Wilder'},price:2500,badge:null,svgFn:svgNais4,title:'Bienvenue dans notre monde !',msg:'La naissance d\'un enfant est le plus beau des cadeaux. Bonne santé à ce petit ange !'},
  // CONDOLÉANCES
  {id:13,cat:'Condoléances',name:'Colombe blanche',music:{t:'Hallelujah',a:'Leonard Cohen'},price:3500,badge:null,svgFn:svgCond1,title:'Nos sincères condoléances',msg:'Nous partageons votre douleur en ces moments difficiles. Nos condoléances les plus sincères.'},
  {id:14,cat:'Condoléances',name:'Lumière douce',music:{t:'Ave Maria',a:'Schubert'},price:3000,badge:null,svgFn:svgCond2,title:'Nos sincères condoléances',msg:'Que l\'âme du disparu repose en paix. Nous prions pour vous et votre famille.'},
  {id:15,cat:'Condoléances',name:'Nuit apaisée',music:{t:'Tears in Heaven',a:'Eric Clapton'},price:3500,badge:null,svgFn:svgCond3,title:'Nos sincères condoléances',msg:'Dans ces moments de tristesse, nous sommes à vos côtés. Que Dieu vous donne la force.'},
  {id:16,cat:'Condoléances',name:'Paix et prières',music:{t:'Amazing Grace',a:'Traditional'},price:3000,badge:null,svgFn:svgCond4,title:'Nos sincères condoléances',msg:'Que l\'Éternel accueille l\'âme du défunt dans Sa miséricorde. Inna lillahi wa inna ilayhi rajioun.'},
  // TABASKI
  {id:17,cat:'Tabaski',name:'Prairie verte',music:{t:'Tabaski',a:'Youssou N\'Dour'},price:2000,badge:'pb-new',svgFn:svgTab1,title:'Bonne Fête de Tabaski !',msg:'Aïd Adha Moubarak ! Que cette fête bénie vous apporte joie, paix et prospérité.'},
  {id:18,cat:'Tabaski',name:'Village fête',music:{t:'Immigrés',a:'Youssou N\'Dour'},price:3000,badge:'pb-best',svgFn:svgTab2,title:'Bonne Fête de Tabaski !',msg:'Que le sacrifice d\'Abraham soit une source d\'inspiration pour toute la famille.'},
  {id:19,cat:'Tabaski',name:'Grande mosquée',music:{t:'Allah Wakbar',a:'Salif Keita'},price:3500,badge:null,svgFn:svgTab3,title:'Bonne Fête de Tabaski !',msg:'Que Dieu accepte votre sacrifice et vous comble de Ses grâces en ce jour béni.'},
  {id:20,cat:'Tabaski',name:'Mouton festif',music:{t:'Fête africaine',a:'Ismael Lô'},price:2500,badge:null,svgFn:svgTab4,title:'Bonne Fête de Tabaski !',msg:'Aïd Moubarak à vous et toute votre famille ! Que cette fête soit pleine de bénédictions.'},
  // KORITÉ
  {id:21,cat:'Korité',name:'Mosquée de nuit',music:{t:'Allahu Akbar',a:'Islamic Nasheed'},price:3500,badge:'pb-new',svgFn:svgKor1,title:'Bonne Fête de Korité !',msg:'Aïd el-Fitr Moubarak ! Fin du Ramadan bénie pour vous et tous vos proches.'},
  {id:22,cat:'Korité',name:'Nuit de Dakar',music:{t:'Nuit de Ramadan',a:'Collectif'},price:3000,badge:'pb-best',svgFn:svgKor2,title:'Bonne Fête de Korité !',msg:'Que cette Korité marque la fin d\'un mois béni et le début d\'une année prospère.'},
  {id:23,cat:'Korité',name:'Grande prière',music:{t:'Salat',a:'Hadj Omar'},price:4000,badge:null,svgFn:svgKor3,title:'Bonne Fête de Korité !',msg:'Que Dieu récompense vos efforts du Ramadan et vous accorde Sa bénédiction infinie.'},
  {id:24,cat:'Korité',name:'Motifs wax',music:{t:'Salam Alaykoum',a:'Collectif'},price:2500,badge:null,svgFn:svgKor4,title:'Bonne Fête de Korité !',msg:'Bonne fête à vous et vos proches ! Que la paix et la joie règnent dans votre foyer.'},
  // TAMKHARIT
  {id:25,cat:'Tamkharit',name:'Feu de famille',music:{t:'Tamkharit',a:'Super Étoile'},price:3000,badge:'pb-new',svgFn:svgTam1,title:'Joyeux Tamkharit !',msg:'Que cette belle tradition nous rappelle la force de notre culture. Bonne fête à tous !'},
  {id:26,cat:'Tamkharit',name:'Village de nuit',music:{t:'Afriki',a:'Youssou N\'Dour'},price:3500,badge:'pb-best',svgFn:svgTam2,title:'Joyeux Tamkharit !',msg:'Bonne année islamique ! Que ce Tamkharit rassemble toute la famille dans la joie.'},
  {id:27,cat:'Tamkharit',name:'Sahara festif',music:{t:'Sawale',a:'Baaba Maal'},price:3000,badge:null,svgFn:svgTam3,title:'Joyeux Tamkharit !',msg:'Que les traditions de nos ancêtres nous guident et que l\'amour familial soit notre force.'},
  {id:28,cat:'Tamkharit',name:'Bouillie dorée',music:{t:'Diouma',a:'Ismael Lô'},price:2500,badge:null,svgFn:svgTam4,title:'Joyeux Tamkharit !',msg:'Que la bouillie de Tamkharit soit symbole de douceur et de partage pour toute la famille !'},
  // AMOUR
  {id:29,cat:'Amour',name:'Rose de nuit',music:{t:'Je t\'aime... moi non plus',a:'Gainsbourg'},price:4200,badge:'pb-new',svgFn:svgAmour1,title:'Je t\'aime ❤️',msg:'Tu es la lumière de ma vie, la rose dans mon jardin. Je t\'aime infiniment.'},
  {id:30,cat:'Amour',name:'Cœur pur',music:{t:'My Heart Will Go On',a:'Céline Dion'},price:3800,badge:'pb-best',svgFn:svgAmour2,title:'Tu comptes pour moi',msg:'Chaque jour à tes côtés est un cadeau précieux. Notre amour est notre force.'},
  {id:31,cat:'Amour',name:'Jardin floral',music:{t:'At Last',a:'Etta James'},price:3500,badge:null,svgFn:svgAmour3,title:'Mon amour pour toi',msg:'Comme une fleur qui s\'épanouit, notre amour grandit chaque jour davantage.'},
  {id:32,cat:'Amour',name:'Flamme éternelle',music:{t:'Endless Love',a:'Lionel Richie'},price:4000,badge:null,svgFn:svgAmour4,title:'Pour toujours',msg:'Notre amour est une flamme qui ne s\'éteint jamais. Pour toujours et à jamais.'},
];

// ══ SVG REMERCIEMENT ══
function svgRem1(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="r1g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#FFF8F0"/><stop offset="100%" stop-color="#FFE8D0"/></linearGradient></defs><rect width="300" height="400" fill="url(#r1g)"/><pattern id="pr1" width="50" height="50" patternUnits="userSpaceOnUse"><circle cx="25" cy="25" r="10" fill="none" stroke="#C8922A" stroke-width="1" opacity=".15"/></pattern><rect width="300" height="400" fill="url(#pr1)"/><circle cx="150" cy="160" r="80" fill="rgba(242,90,10,.06)"/><g transform="translate(150,155)"><path d="M0,-55 C15,-55 30,-40 30,-25 C30,-10 15,5 0,20 C-15,5 -30,-10 -30,-25 C-30,-40 -15,-55 0,-55Z" fill="#F25A0A" opacity=".9"/><path d="M0,-45 C12,-45 24,-33 24,-20 C24,-7 12,5 0,18 C-12,5 -24,-7 -24,-20 C-24,-33 -12,-45 0,-45Z" fill="#FF7A30" opacity=".8"/><path d="M0,-35 C9,-35 18,-26 18,-16 C18,-6 9,3 0,13 C-9,3 -18,-6 -18,-16 C-18,-26 -9,-35 0,-35Z" fill="#FFD700" opacity=".9"/></g><text x="150" y="268" text-anchor="middle" font-family="serif" font-style="italic" font-size="22" fill="#C8922A" opacity=".9">Diadieuf !</text><text x="150" y="292" text-anchor="middle" font-family="serif" font-size="12" fill="#8B6040" opacity=".7">Merci du fond du cœur</text><g transform="translate(80,320)"><ellipse cx="0" cy="-10" rx="9" ry="11" fill="#FFB8D8" transform="rotate(0)"/><ellipse cx="0" cy="-10" rx="9" ry="11" fill="#FFA8C8" transform="rotate(72)"/><ellipse cx="0" cy="-10" rx="9" ry="11" fill="#FFB8D8" transform="rotate(144)"/><circle r="6" fill="#FFD700"/></g><g transform="translate(220,325)"><ellipse cx="0" cy="-10" rx="9" ry="11" fill="#C8E0A0" transform="rotate(0)"/><ellipse cx="0" cy="-10" rx="9" ry="11" fill="#B8D890" transform="rotate(120)"/><ellipse cx="0" cy="-10" rx="9" ry="11" fill="#C8E8A8" transform="rotate(240)"/><circle r="6" fill="#FFD700"/></g><circle cx="50" cy="60" r="3" fill="#F25A0A" opacity=".3"/><circle cx="250" cy="55" r="3" fill="#F25A0A" opacity=".25"/><circle cx="40" cy="300" r="2.5" fill="#C8922A" opacity=".3"/><circle cx="262" cy="295" r="2.5" fill="#C8922A" opacity=".25"/></svg>`;}

function svgRem2(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="r2g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#0A0820"/><stop offset="50%" stop-color="#1A1040"/><stop offset="100%" stop-color="#0A0518"/></linearGradient></defs><rect width="300" height="400" fill="url(#r2g)"/><circle cx="40" cy="40" r="2" fill="#fff" opacity=".7"/><circle cx="260" cy="30" r="1.5" fill="#FFD700" opacity=".8"/><circle cx="150" cy="20" r="1.5" fill="#fff" opacity=".6"/><circle cx="80" cy="70" r="1" fill="#FFD700" opacity=".5"/><circle cx="220" cy="65" r="1" fill="#fff" opacity=".4"/><g transform="translate(150,150)"><circle r="55" fill="none" stroke="#C8922A" stroke-width="1" opacity=".3"/><circle r="38" fill="none" stroke="#E8C060" stroke-width="1" opacity=".2"/><path d="M0,-45 L12,-15 L45,-15 L20,5 L30,35 L0,15 L-30,35 L-20,5 L-45,-15 L-12,-15 Z" fill="none" stroke="#C8922A" stroke-width="1.5" opacity=".4"/><text x="0" y="8" text-anchor="middle" font-family="serif" font-style="italic" font-size="18" fill="#E8C060" opacity=".9">Merci</text></g><text x="150" y="242" text-anchor="middle" font-family="serif" font-style="italic" font-size="20" fill="#C8922A" opacity=".9">Diadieuf !</text><text x="150" y="265" text-anchor="middle" font-family="serif" font-size="11" fill="rgba(255,255,255,.5)">Votre geste m'a touché le cœur</text><line x1="80" y1="278" x2="220" y2="278" stroke="#C8922A" stroke-width="1" opacity=".3"/><circle cx="40" cy="300" r="2" fill="#C8922A" opacity=".4"/><circle cx="260" cy="300" r="2" fill="#C8922A" opacity=".4"/><circle cx="150" cy="340" r="3" fill="#E8C060" opacity=".5"/></svg>`;}

function svgRem3(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="r3g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#E8F8E8"/><stop offset="100%" stop-color="#C8ECC8"/></linearGradient></defs><rect width="300" height="400" fill="url(#r3g)"/><ellipse cx="60" cy="70" rx="50" ry="24" fill="white" opacity=".7"/><ellipse cx="240" cy="75" rx="55" ry="26" fill="white" opacity=".6"/><circle cx="150" cy="120" r="55" fill="rgba(0,166,81,.1)"/><g transform="translate(150,140)"><path d="M-5,-60 L5,-60 L5,-10 L20,-25 L15,-18 L5,0 L5,40 L-5,40 L-5,0 L-15,-18 L-20,-25 L-5,-10 Z" fill="#00A651" opacity=".8"/><ellipse cx="-20" cy="-40" rx="18" ry="22" fill="#2A8A20" opacity=".7" transform="rotate(-30,-20,-40)"/><ellipse cx="20" cy="-40" rx="18" ry="22" fill="#3A9A30" opacity=".7" transform="rotate(30,20,-40)"/><ellipse cx="-30" cy="-20" rx="15" ry="18" fill="#4A8A30" opacity=".6" transform="rotate(-50,-30,-20)"/><ellipse cx="30" cy="-20" rx="15" ry="18" fill="#3A7A20" opacity=".6" transform="rotate(50,30,-20)"/></g><text x="150" y="235" text-anchor="middle" font-family="serif" font-style="italic" font-size="22" fill="#2A6A20" opacity=".9">Diadieuf !</text><text x="150" y="258" text-anchor="middle" font-family="serif" font-size="11" fill="#4A8A40" opacity=".8">Que Dieu vous bénisse</text><path d="M65,300 Q150,285 235,300" stroke="#4A8A40" stroke-width="1.5" fill="none" opacity=".4"/><g transform="translate(90,330)"><ellipse cx="0" cy="-10" rx="8" ry="10" fill="#90E890" transform="rotate(0)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="#80D880" transform="rotate(72)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="#90E890" transform="rotate(144)"/><circle r="6" fill="#FFD700"/></g><g transform="translate(210,330)"><ellipse cx="0" cy="-10" rx="8" ry="10" fill="#FFB8D8" transform="rotate(0)"/><ellipse cx="0" cy="-10" rx="8" ry="10" fill="#FFA8C8" transform="rotate(120)"/><circle r="6" fill="#FFD700"/></g></svg>`;}

function svgRem4(){return`<svg viewBox="0 0 300 400" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="r4g" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#3A1A00"/><stop offset="50%" stop-color="#6A3A10"/><stop offset="100%" stop-color="#2A1000"/></linearGradient></defs><rect width="300" height="400" fill="url(#r4g)"/><circle cx="150" cy="30" r="2.5" fill="#FFD700" opacity=".9"/><circle cx="80" cy="50" r="2" fill="#fff" opacity=".7"/><circle cx="220" cy="45" r="2" fill="#fff" opacity=".6"/><circle cx="40" cy="80" r="1.5" fill="#FFD700" opacity=".5"/><circle cx="265" cy="70" r="1.5" fill="#fff" opacity=".5"/><path d="M130,280 Q150,220 170,280 Q165,250 150,240 Q135,250 130,280 Z" fill="#FF6600"/><path d="M138,280 Q150,235 162,280 Q158,258 150,250 Q142,258 138,280 Z" fill="#FF9900"/><path d="M143,275 Q150,248 157,275 Q154,262 150,258 Q146,262 143,275 Z" fill="#FFD700"/><text x="150" y="185" text-anchor="middle" font-family="serif" font-style="italic" font-size="26" fill="#FFD700" opacity=".95">Diadieuf !</text><text x="150" y="210" text-anchor="middle" font-family="serif" font-size="12" fill="rgba(255,255,255,.65)">Merci pour votre générosité</text><line x1="70" y1="222" x2="230" y2="222" stroke="#C8922A" stroke-width="1" opacity=".35"/><ellipse cx="60" cy="245" rx="12" ry="13" fill="#8B5030"/><path d="M48,257 Q42,290 45,300 L75,300 Q78,290 72,257 Z" fill="#C8902A"/><ellipse cx="150" cy="243" rx="12" ry="13" fill="#C09060"/><path d="M138,256 Q132,291 136,301 L164,301 Q168,291 162,256 Z" fill="#E06020"/><ellipse cx="240" cy="245" rx="12" ry="13" fill="#A07040"/><path d="M228,258 Q222,293 226,303 L254,303 Q258,293 252,258 Z" fill="#F0F0E0"/><ellipse cx="150" cy="350" rx="60" ry="12" fill="#FF4400" opacity=".2"/></svg>`;}


// ── NOËL ──
CARDS.push(
  {id:37,cat:'Noel',name:'Nuit étoilée',music:{t:'Jingle Bells',a:'Frank Sinatra'},price:2500,badge:'pb-new',svgFn:svgAnniv2,title:'Joyeux Noël !',msg:'Que cette nuit magique vous apporte joie, paix et bonheur. Passez un merveilleux Noël en famille !'},
  {id:38,cat:'Noel',name:'Père Noël africain',music:{t:'Last Christmas',a:'Wham!'},price:3000,badge:'pb-best',svgFn:svgAnniv1,title:'Joyeux Noël !',msg:'Que la magie de Noël illumine votre foyer et apporte le bonheur à toute la famille !'},
  {id:39,cat:'Noel',name:'Sapins dorés',music:{t:'White Christmas',a:'Bing Crosby'},price:3500,badge:'pb-prem',svgFn:svgAnniv3,title:'Joyeux Noël !',msg:'En ce jour de fête, nous vous souhaitons amour, paix et prospérité pour toute l'année !'},
  {id:40,cat:'Noel',name:'Étoile de Bethléem',music:{t:'Silent Night',a:'Traditional'},price:2000,badge:null,svgFn:svgKor1,title:'Joyeux Noël !',msg:'Que l'étoile de Noël guide vos pas vers le bonheur et la réussite !'}
);
// ── PÂQUES ──
CARDS.push(
  {id:41,cat:'Paques',name:'Aube de Pâques',music:{t:'Hallelujah',a:'Leonard Cohen'},price:2500,badge:'pb-new',svgFn:svgNais1,title:'Joyeuses Pâques !',msg:'En ce jour de résurrection et d'espoir, nous vous souhaitons une belle fête de Pâques !'},
  {id:42,cat:'Paques',name:'Œufs colorés',music:{t:'Here Comes The Sun',a:'The Beatles'},price:2000,badge:null,svgFn:svgAnniv1,title:'Joyeuses Pâques !',msg:'Que cette belle fête printanière vous apporte joie, renouveau et beaucoup de bonheur !'},
  {id:43,cat:'Paques',name:'Printemps fleuri',music:{t:'Morning Has Broken',a:'Cat Stevens'},price:3000,badge:'pb-best',svgFn:svgNais3,title:'Joyeuses Pâques !',msg:'Pâques est le symbole du renouveau. Que cette fête vous apporte espoir et nouvelles opportunités !'},
  {id:44,cat:'Paques',name:'Colombe de paix',music:{t:'Amazing Grace',a:'Traditional'},price:2500,badge:null,svgFn:svgCond1,title:'Joyeuses Pâques !',msg:'En ce jour béni, que la paix et la joie habitent votre cœur et votre foyer !'}
);
// ── FÊTE DU TRAVAIL ──
CARDS.push(
  {id:45,cat:'FeteTravail',name:'1er Mai solidaire',music:{t:'We Are The World',a:'USA for Africa'},price:2000,badge:'pb-new',svgFn:svgAnniv4,title:'Bonne Fête du Travail !',msg:'En ce 1er Mai, nous célébrons votre engagement et votre dévouement !'},
  {id:46,cat:'FeteTravail',name:'Force ouvrière',music:{t:'Imagine',a:'John Lennon'},price:2500,badge:null,svgFn:svgAnniv3,title:'Bonne Fête du Travail !',msg:'Le travail est la dignité de l'homme. Nous saluons votre courage et votre persévérance !'},
  {id:47,cat:'FeteTravail',name:'Mains unies',music:{t:'Stand By Me',a:'Ben E. King'},price:2000,badge:'pb-best',svgFn:svgMar1,title:'Bonne Fête du Travail !',msg:'Ensemble nous sommes plus forts ! Bonne fête à tous les travailleurs du Sénégal !'},
  {id:48,cat:'FeteTravail',name:'Avenir radieux',music:{t:'A New Day Has Come',a:'Céline Dion'},price:3000,badge:null,svgFn:svgAnniv2,title:'Bonne Fête du Travail !',msg:'Que vos efforts d'aujourd'hui bâtissent le monde de demain !'}
);
// ── FIN D'ANNÉE ──
CARDS.push(
  {id:49,cat:'FinAnnee',name:'Feux d'artifice',music:{t:'Auld Lang Syne',a:'Traditional'},price:3500,badge:'pb-new',svgFn:svgAnniv2,title:'Bonne Année !',msg:'Une nouvelle année commence ! Que 2026 vous apporte santé, bonheur, succès et prospérité !'},
  {id:50,cat:'FinAnnee',name:'Champagne doré',music:{t:'New Year's Day',a:'U2'},price:3000,badge:'pb-best',svgFn:svgMar3,title:'Bonne Année !',msg:'L'année se termine, une nouvelle aventure commence ! Bonne et heureuse année à vous !'},
  {id:51,cat:'FinAnnee',name:'Nuit de gala',music:{t:'Celebration',a:'Kool & The Gang'},price:4000,badge:'pb-prem',svgFn:svgKor3,title:'Meilleurs Vœux !',msg:'En cette fin d'année, merci pour votre confiance et bonne année à vous et vos proches !'},
  {id:52,cat:'FinAnnee',name:'Étoiles et vœux',music:{t:'Simply The Best',a:'Tina Turner'},price:2500,badge:null,svgFn:svgKor1,title:'Bonne Année !',msg:'Que les étoiles guident vos pas vers un futur radieux. Excellente année à vous !'}
);
// ── SAINT-VALENTIN ──
CARDS.push(
  {id:53,cat:'SaintValentin',name:'Rose rouge',music:{t:'My Valentine',a:'Paul McCartney'},price:4500,badge:'pb-prem',svgFn:svgAmour4,title:'Bonne Saint-Valentin !',msg:'En ce jour de l'amour, je veux te dire combien tu comptes pour moi. Je t'aime !'},
  {id:54,cat:'SaintValentin',name:'Cœurs enflammés',music:{t:'La Vie en Rose',a:'Édith Piaf'},price:3800,badge:'pb-best',svgFn:svgAmour1,title:'Bonne Saint-Valentin !',msg:'L'amour est la plus belle aventure. Merci d'être là à mes côtés chaque jour !'},
  {id:55,cat:'SaintValentin',name:'Nuit romantique',music:{t:'Fly Me To The Moon',a:'Frank Sinatra'},price:4200,badge:null,svgFn:svgAmour3,title:'Je t'aime ❤️',msg:'Cette nuit est pour toi, mon amour. Que notre histoire continue d'écrire les plus belles pages !'},
  {id:56,cat:'SaintValentin',name:'Lettre d'amour',music:{t:'She's The One',a:'Robbie Williams'},price:3500,badge:'pb-new',svgFn:svgAmour2,title:'Mon cœur est à toi',msg:'Les mots ne suffisent pas pour décrire ce que tu représentes pour moi !'}
);
// ── ENTREPRISE ──
CARDS.push(
  {id:57,cat:'Entreprise',name:'Excellence corporate',music:{t:'Simply The Best',a:'Tina Turner'},price:5000,badge:'pb-prem',svgFn:svgAnniv3,title:'Félicitations !',msg:'Votre engagement et votre professionnalisme sont une source d'inspiration pour toute l'équipe !'},
  {id:58,cat:'Entreprise',name:'Vœux professionnels',music:{t:'Eye of the Tiger',a:'Survivor'},price:4500,badge:'pb-best',svgFn:svgMar3,title:'Meilleurs Vœux Professionnels',msg:'Au nom de toute l'équipe, nous vous adressons nos meilleurs vœux pour la nouvelle année !'},
  {id:59,cat:'Entreprise',name:'Merci équipe',music:{t:'You've Got A Friend',a:'James Taylor'},price:4000,badge:null,svgFn:svgAnniv4,title:'Merci à notre équipe !',msg:'Votre travail et votre dévouement font la force de notre entreprise. Un grand merci !'},
  {id:60,cat:'Entreprise',name:'Succès partagé',music:{t:'We Are The Champions',a:'Queen'},price:5000,badge:'pb-new',svgFn:svgAnniv2,title:'Bravo à toute l'équipe !',msg:'Ce succès est le vôtre ! Ensemble, nous avons accompli quelque chose d'exceptionnel !'}
);

// AJOUT DES CARTES REMERCIEMENT
CARDS.push(
  {id:33,cat:'Remerciement',name:'Cœur de gratitude',music:{t:'Thank You',a:'Dido'},price:1500,badge:'pb-new',svgFn:svgRem1,title:'Diadieuf — Merci !',msg:'Votre geste m\'a profondément touché. Je vous adresse toute ma reconnaissance et ma gratitude sincère.'},
  {id:34,cat:'Remerciement',name:'Étoiles de Dakar',music:{t:'Merci',a:'Youssou N\'Dour'},price:2000,badge:'pb-best',svgFn:svgRem2,title:'Diadieuf — Merci !',msg:'Que Dieu vous récompense pour votre générosité. Votre attention m\'a touché le cœur.'},
  {id:35,cat:'Remerciement',name:'Jardin vert',music:{t:'Grateful',a:'Naughty Boy'},price:1500,badge:null,svgFn:svgRem3,title:'Diadieuf — Merci !',msg:'Que Dieu vous bénisse pour votre bonté. Votre cadeau restera gravé dans ma mémoire.'},
  {id:36,cat:'Remerciement',name:'Feu de joie',music:{t:'Beautiful',a:'James Blunt'},price:2000,badge:null,svgFn:svgRem4,title:'Diadieuf — Merci !',msg:'Votre générosité illumine ma journée. Merci du fond du cœur pour tout ce que vous avez fait.'}
);

const TITLES={
  Anniversaire:'Joyeux Anniversaire !',Mariage:'Félicitations aux mariés !',
  Naissance:'Bienvenue dans notre monde !',Condoléances:'Nos sincères condoléances',
  Noel:'Joyeux Noël !',Paques:'Joyeuses Pâques !',
  FeteTravail:'Bonne Fête du Travail !',FinAnnee:'Bonne Année !',
  SaintValentin:'Bonne Saint-Valentin !',Tabaski:'Bonne Fête de Tabaski !',
  Korité:'Bonne Fête de Korité !',Tamkharit:'Joyeux Tamkharit !',
  Amour:'Je t\'aime ❤️',Entreprise:'Félicitations !',Remerciement:'Diadieuf — Merci !',
};

// ══ STATE ══
let cart=[],currentCard=null,selectedVerso=VERSO[0],isFlipped=false;
let giftOn=false,giftOp=null,giftAmt=0,payMethod=null;
let buyerName='',buyerPhone='',buyerEmail='';

// ══ INIT ══
function buildCatTabs(){
  const tabs=document.getElementById('cat-tabs');
  tabs.innerHTML=`<div class="cat-tab on" onclick="scrollToCat('all',this)">🌟 Tout voir</div>`+
    CATS.map(c=>`<div class="cat-tab" onclick="scrollToCat('${c.id}',this)">${c.icon} ${c.label}</div>`).join('');
}

function buildAllSections(){
  const cont=document.getElementById('all-sections');
  cont.innerHTML=CATS.map(c=>{
    const cards=CARDS.filter(x=>x.cat===c.id);
    const isRem=c.id==='Remerciement';
    const isEnt=c.id==='Entreprise';
    const banner=isEnt?`<div class="enterprise-banner">
      <div class="eb-icon">🏢</div>
      <div class="eb-text">
        <h3>Cadeaux d'Entreprise & Gouvernement</h3>
        <p>Commandes en volume · Cartes pour fonctionnaires · Fête du Travail · Vœux institutionnels · Devis personnalisé</p>
      </div>
      <button class="eb-btn" onclick="window.location.href='mailto:diadieuf.senegal@gmail.com?subject=Commande%20Entreprise%20Diadieuf'">📧 Nous contacter</button>
    </div>`:isRem?`<div class="remerciement-banner">
      <div class="rb-icon">🙏</div>
      <div class="rb-text">
        <h3>Vous avez reçu une carte ? Répondez avec un Remerciement !</h3>
        <p>Le receveur peut à son tour envoyer une belle carte de remerciement à l'expéditeur — avec musique et cadeau financier si souhaité.</p>
      </div>
    </div>`:'';
    return `${banner}<div class="cat-section" id="sec-${c.id}">
      <div class="cat-section-header">
        <div class="cat-section-icon">${c.icon}</div>
        <div class="cat-section-title">${c.label}</div>
        <div class="cat-section-count">${cards.length} cartes</div>
      </div>
      <div class="cards-row">
        ${cards.map(card=>`
          <div class="pcard" onclick="openEditor(${card.id})">
            <div class="pcard-img" style="position:relative;">
              ${card.svgFn()}
              ${card.badge?`<div class="pcard-badge ${card.badge}">${card.badge==='pb-new'?'Nouveau':card.badge==='pb-best'?'Best':card.badge==='pb-prem'?'Premium':''}</div>`:''}
              <div class="pcard-music">🎵 ${card.music.t}</div>
              <div class="pcard-overlay-btn"><span class="pob-txt">✨ Personnaliser</span></div>
            </div>
            <div class="pcard-info">
              <div class="pcard-name">${card.name}</div>
              <div class="pcard-cat">${card.cat} · ${card.music.a}</div>
              <div class="pcard-foot">
                <span class="pcard-price">${fmtS(card.price)}</span>
                <button class="pcard-add" onclick="event.stopPropagation();quickAdd(${card.id})">+</button>
              </div>
            </div>
          </div>`).join('')}
      </div>
    </div>`;
  }).join('');
}

function scrollToCat(cat,el){
  document.querySelectorAll('.cat-tab').forEach(t=>t.classList.remove('on'));
  el.classList.add('on');
  if(cat==='all'){window.scrollTo({top:document.getElementById('catalogue').offsetTop-80,behavior:'smooth'});}
  else{const s=document.getElementById('sec-'+cat);if(s)s.scrollIntoView({behavior:'smooth',block:'start'});}
}

function scrollToTop(){window.scrollTo({top:0,behavior:'smooth'});}

// ══ ÉDITEUR ══
function openEditor(id){
  currentCard=CARDS.find(c=>c.id===id);if(!currentCard)return;
  isFlipped=false;giftOn=false;giftOp=null;giftAmt=0;selectedVerso=VERSO[0];
  document.getElementById('flip-inner').classList.remove('flipped');
  document.getElementById('gift-sw').classList.remove('on');
  document.getElementById('gift-lbl').textContent='Ajouter un cadeau en FCFA';
  document.getElementById('gift-body').classList.remove('open');
  document.querySelectorAll('.achip').forEach(c=>c.classList.remove('on'));
  document.getElementById('gift-custom').value='';
  document.getElementById('gift-phone').value='';
  document.getElementById('op-or').classList.remove('sel-or');
  document.getElementById('op-wv').classList.remove('sel-wv');
  document.getElementById('addr-grp').classList.add('hidden');
  document.getElementById('e-del').value='sms';
  document.getElementById('e-recip').value='';
  if(document.getElementById('recip-phone')) document.getElementById('recip-phone').value='';
  if(document.getElementById('recip-email')) document.getElementById('recip-email').value='';
  if(document.getElementById('recip-phone-preview')) document.getElementById('recip-phone-preview').innerHTML='Numéro : <span>—</span>';
  document.getElementById('e-title').value=currentCard.title;
  document.getElementById('e-msg').value=currentCard.msg;
  document.getElementById('e-sig').value='— Avec toute mon affection';
  document.getElementById('mtd-name').textContent=currentCard.music.t;
  document.getElementById('mtd-artist').textContent=currentCard.music.a;
  buildVersoGrid();buildMusicSuggestions();updatePreview();updateEditorTotal();
  document.getElementById('editor-modal').classList.add('open');
  document.body.style.overflow='hidden';
}
function closeEditor(){document.getElementById('editor-modal').classList.remove('open');document.body.style.overflow='';}

function buildVersoGrid(){
  document.getElementById('verso-grid').innerHTML=VERSO.map(v=>`
    <div class="vt ${v.id===selectedVerso.id?'on':''}" onclick="pickVerso('${v.id}',this)">
      <div class="vt-img">${v.svg()}</div>
      <div class="vt-name">${v.name}</div>
    </div>`).join('');
}
function pickVerso(id,el){selectedVerso=VERSO.find(v=>v.id===id)||VERSO[0];document.querySelectorAll('.vt').forEach(v=>v.classList.remove('on'));el.classList.add('on');updatePreview();}

function toggleFlip(){isFlipped=!isFlipped;document.getElementById('flip-inner').classList.toggle('flipped',isFlipped);}

function updatePreview(){
  if(!currentCard)return;
  document.getElementById('recto-svg').innerHTML=currentCard.svgFn();
  document.getElementById('ro-title').textContent=document.getElementById('e-title').value||currentCard.title;
  document.getElementById('ro-msg').textContent=document.getElementById('e-msg').value||currentCard.msg;
  document.getElementById('ro-sig').textContent=document.getElementById('e-sig').value||'— Avec amour';
  document.getElementById('ro-music').textContent='🎵 '+currentCard.music.t+' · '+currentCard.music.a;
  // gift
  const rg=document.getElementById('ro-gift');
  if(giftOn&&giftAmt>0&&giftOp){
    rg.textContent=`🎁 ${fmtS(giftAmt)} · ${giftOp==='orange'?'Orange Money':'Wave'}`;
    rg.className='ro-gift show '+(giftOp==='orange'?'ro-gift-or':'ro-gift-wv');
  }else{rg.className='ro-gift';}
  // verso
  document.getElementById('verso-svg-wrap').innerHTML=selectedVerso.svg();
  document.getElementById('verso-card-name').textContent=currentCard.name+' · '+currentCard.cat;
}

function onDelChg(){const v=document.getElementById('e-del').value;document.getElementById('addr-grp').classList.toggle('hidden',v!=='postal');updateEditorTotal();}
function updateEditorTotal(){if(!currentCard)return;const d=document.getElementById('e-del')?.value==='postal'?2000:0;const mf=musicCustom?500:0;const f=Math.round((currentCard.price+d)*0.03);document.getElementById('editor-total').textContent=fmt(currentCard.price+d+mf+f+(giftOn?giftAmt:0));}

// GIFT
function toggleGift(){giftOn=!giftOn;document.getElementById('gift-sw').classList.toggle('on',giftOn);document.getElementById('gift-lbl').textContent=giftOn?'Cadeau activé ✓':'Ajouter un cadeau en FCFA';document.getElementById('gift-body').classList.toggle('open',giftOn);if(!giftOn){giftAmt=0;giftOp=null;document.querySelectorAll('.achip').forEach(c=>c.classList.remove('on'));document.getElementById('gift-custom').value='';}updatePreview();updateEditorTotal();}
function selOp(op){giftOp=op;document.getElementById('op-or').className='op-btn'+(op==='orange'?' sel-or':'');document.getElementById('op-wv').className='op-btn'+(op==='wave'?' sel-wv':'');updatePreview();}
function pickAmt(a,el){giftAmt=a;document.querySelectorAll('.achip').forEach(c=>c.classList.remove('on'));el.classList.add('on');document.getElementById('gift-custom').value='';updatePreview();updateEditorTotal();}
function customAmt(){giftAmt=parseInt(document.getElementById('gift-custom').value)||0;document.querySelectorAll('.achip').forEach(c=>c.classList.remove('on'));updatePreview();updateEditorTotal();}

function saveToGalleryFromEditor(){showToast('📸 Carte sauvegardée !');}

// ══ PANIER ══
function addToCart(){
  if(!currentCard)return;
  if(giftOn&&!giftOp){showToast('Choisissez Orange Money ou Wave.');return;}
  if(giftOn&&giftAmt<500){showToast('Montant minimum : 500 F CFA.');return;}
  const del=document.getElementById('e-del').value;const delC=del==='postal'?2000:0;const mFee=musicCustom?500:0;const fee=Math.round((currentCard.price+delC)*0.03);
  const recipPhone=getFullPhone('recip-country','recip-phone');
  const recipEmail=document.getElementById('recip-email')?.value.trim()||'';
  cart.push({id:Date.now(),card:{...currentCard},title:document.getElementById('e-title').value||currentCard.title,msg:document.getElementById('e-msg').value,sig:document.getElementById('e-sig').value,verso:selectedVerso.id,recip:document.getElementById('e-recip').value,recipPhone,recipEmail,delivery:del,delC,cardPrice:currentCard.price,fee,gift:giftOn?{op:giftOp,amount:giftAmt,phone:getFullPhone('gift-country','gift-phone')}:null,music:selectedTrack?{...selectedTrack,custom:musicCustom}:null,musicFee:mFee,total:currentCard.price+delC+mFee+fee+(giftOn?giftAmt:0)});
  updateBadge();closeEditor();showToast('✅ Carte ajoutée au panier !');
}

function quickAdd(id){
  const c=CARDS.find(x=>x.id===id);if(!c)return;const fee=Math.round(c.price*0.03);
  cart.push({id:Date.now(),card:{...c},title:c.title,msg:c.msg,sig:'— Avec amour',verso:'wakanda',recip:'',delivery:'sms',delC:0,cardPrice:c.price,fee,gift:null,total:c.price+fee});
  updateBadge();showToast('✅ Ajouté ! Cliquez pour personnaliser.');
}

function removeFromCart(id){cart=cart.filter(i=>i.id!==id);renderCart();}
function updateBadge(){document.getElementById('cart-count').textContent=cart.length;}

// ══ DRAWER PANIER ══
function openCart(){renderCart();document.getElementById('cart-overlay').classList.add('open');document.getElementById('cart-drawer').classList.add('open');document.body.style.overflow='hidden';}
function closeCart(){document.getElementById('cart-overlay').classList.remove('open');document.getElementById('cart-drawer').classList.remove('open');document.body.style.overflow='';}

const delLabels={sms:'SMS',whatsapp:'WhatsApp',postal:'Courrier postal'};
function renderCart(){
  const list=document.getElementById('cart-items-list');
  const footer=document.getElementById('cart-footer');
  if(!cart.length){
    list.innerHTML=`<div class="cart-empty"><div class="cei">🛍️</div><p>Votre panier est vide.<br>Choisissez une carte !</p></div>`;
    footer.innerHTML='';return;
  }
  list.innerHTML=cart.map(item=>`
    <div class="cart-item">
      <div class="ci-thumb">${item.card.svgFn()}</div>
      <div class="ci-info">
        <div class="ci-name">${item.title}</div>
        <div class="ci-meta">${item.card.cat} · ${delLabels[item.delivery]||item.delivery}${item.recip?' · Pour : <strong>'+item.recip+'</strong>':''}${item.recipPhone?' · 📱 '+item.recipPhone:''}</div>
        <div class="ci-tags">
          <div class="ci-tag ci-tag-mu">🎵 ${item.card.music.t}</div>
          ${item.gift?`<div class="ci-tag ${item.gift.op==='orange'?'ci-tag-or':'ci-tag-wv'}">🎁 ${fmtS(item.gift.amount)}</div>`:''}
        </div>
      </div>
      <div class="ci-right">
        <div class="ci-price">${fmtS(item.total)}</div>
        <button class="ci-del" onclick="removeFromCart(${item.id})">✕</button>
      </div>
    </div>`).join('');
  const cT=cart.reduce((s,i)=>s+i.cardPrice,0);
  const gT=cart.reduce((s,i)=>s+(i.gift?i.gift.amount:0),0);
  const dT=cart.reduce((s,i)=>s+i.delC,0);
  const fT=cart.reduce((s,i)=>s+i.fee,0);
  const tot=cT+gT+dT+fT;
  footer.innerHTML=`
    <div class="cart-summary-rows">
      <div class="cs-row"><span>Cartes (${cart.length})</span><span>${fmtS(cT)}</span></div>
      ${gT?`<div class="cs-row"><span>Cadeaux financiers</span><span>${fmtS(gT)}</span></div>`:''}
      <div class="cs-row"><span>Livraison</span><span>${dT?fmtS(dT):'Gratuit'}</span></div>
      <div class="cs-row"><span>Frais service (3%)</span><span>${fmtS(fT)}</span></div>
      <div class="cs-row tot"><span>Total</span><span>${fmt(tot)}</span></div>
    </div>
    <button class="checkout-btn" onclick="openBuyerModal()">💳 Commander & Payer</button>`;
}

// ══ PHONE HELPERS ══
function updatePhonePreview(context){
  if(context==='buyer'){
    const code=document.getElementById('buyer-country')?.value||'+221';
    const num=document.getElementById('buyer-phone')?.value||'';
    const prev=document.getElementById('buyer-phone-preview');
    if(prev) prev.innerHTML=`Numéro complet : <span>${num?code+' '+num:'—'}</span>`;
  } else if(context==='gift'){
    const code=document.getElementById('gift-country')?.value||'+221';
    const num=document.getElementById('gift-phone')?.value||'';
    const prev=document.getElementById('gift-phone-preview');
    if(prev) prev.innerHTML=`Numéro : <span>${num?code+' '+num:'—'}</span>`;
  } else if(context==='recip'){
    const code=document.getElementById('recip-country')?.value||'+221';
    const num=document.getElementById('recip-phone')?.value||'';
    const prev=document.getElementById('recip-phone-preview');
    if(prev) prev.innerHTML=`Numéro : <span>${num?code+' '+num:'—'}</span>`;
  } else if(context==='co'){
    const code=document.getElementById('co-country')?.value||'+221';
    const num=document.getElementById('co-num')?.value||'';
    const prev=document.getElementById('co-phone-preview');
    if(prev) prev.innerHTML=`Numéro complet : <span>${num?code+' '+num:'—'}</span>`;
  }
}

function getFullPhone(countryId, numberId){
  const code=document.getElementById(countryId)?.value||'+221';
  const num=document.getElementById(numberId)?.value?.trim()||'';
  return num ? code+' '+num : '';
}

// ══ BUYER MODAL ══
function openBuyerModal(){
  if(!cart.length){showToast('Panier vide !');return;}
  if(buyerName) document.getElementById('buyer-name').value=buyerName;
  if(buyerPhone){
    // extract number without code
    const parts=buyerPhone.split(' ');
    if(parts.length>1) document.getElementById('buyer-phone').value=parts.slice(1).join(' ');
  }
  if(buyerEmail) document.getElementById('buyer-email').value=buyerEmail;
  updatePhonePreview('buyer');
  document.getElementById('buyer-modal').classList.add('open');
  document.body.style.overflow='hidden';
}
function closeBuyerModal(){document.getElementById('buyer-modal').classList.remove('open');document.body.style.overflow='';}
function confirmBuyer(){
  const name=document.getElementById('buyer-name').value.trim();
  const num=document.getElementById('buyer-phone').value.trim();
  if(!name){showToast('Veuillez entrer votre nom.');return;}
  if(!num){showToast('Veuillez entrer votre numéro de téléphone.');return;}
  buyerName=name;
  buyerPhone=getFullPhone('buyer-country','buyer-phone');
  buyerEmail=document.getElementById('buyer-email').value.trim();
  closeBuyerModal();
  openPayModal();
}

// ══ MODAL PAIEMENT ══
function openPayModal(){
  payMethod=null;
  const tot=cart.reduce((s,i)=>s+i.total,0);
  document.getElementById('pay-modal-content').innerHTML=buildPayStep1(tot);
  document.getElementById('pay-modal').classList.add('open');
  document.body.style.overflow='hidden';
}
function closePay(){document.getElementById('pay-modal').classList.remove('open');document.body.style.overflow='';}

function buildPayStep1(tot){
  return `
    <div class="pay-steps"><div class="ps active"></div><div class="ps"></div><div class="ps"></div></div>
    <p style="font-size:.85rem;font-weight:600;color:var(--txt2);margin-bottom:.9rem;">Choisissez votre mode de paiement</p>
    <div class="pay-methods-grid">
      <div class="pmb" id="pmb-or" onclick="selPayM('orange')"><div class="pmb-icon">🟠</div><div class="pmb-name">Orange Money</div></div>
      <div class="pmb" id="pmb-wv" onclick="selPayM('wave')"><div class="pmb-icon">🌊</div><div class="pmb-name">Wave</div></div>
      <div class="pmb" id="pmb-cb" onclick="selPayM('card')"><div class="pmb-icon">💳</div><div class="pmb-name">Carte bancaire</div></div>
    </div>
    <div id="pay-method-form"></div>
    <div class="pay-secure-badges">
      <div class="psb">🔒 SSL</div>
      <div class="psb">✅ 3D Secure</div>
      <div class="psb">🏦 Certifié</div>
    </div>
    <div class="pay-total-row"><span class="ptr-lbl">Total à payer</span><span class="ptr-amt" id="pay-total-disp">${fmt(tot)}</span></div>
    <button class="pay-confirm-btn" onclick="proceedPayment()">Continuer →</button>`;
}

function selPayM(m){
  payMethod=m;
  document.querySelectorAll('.pmb').forEach(b=>b.classList.remove('on'));
  document.getElementById('pmb-'+m)?.classList.add('on');
  // Afficher form selon méthode
  const f=document.getElementById('pay-method-form');
  if(m==='orange'||m==='wave'){
    const label=m==='orange'?'Orange Money':'Wave';
    const icon=m==='orange'?'🟠':'🌊';
    f.innerHTML=`
      <div class="pay-info-box">${icon} Entrez votre numéro ${label} pour recevoir la confirmation de paiement.</div>
      <div class="fg"><label>Prénom et nom</label><input type="text" id="co-name" placeholder="Amadou Diallo" value="${buyerName}"></div>
      <div class="fg">
        <label>Numéro ${label}</label>
        <div class="phone-field">
          <select class="country-select" id="co-country" onchange="updatePhonePreview('co')" style="min-width:120px;height:44px;">
            <option value="+221" selected>🇸🇳 +221</option>
            <option value="+33">🇫🇷 +33</option>
            <option value="+32">🇧🇪 +32</option>
            <option value="+41">🇨🇭 +41</option>
            <option value="+1">🇺🇸 +1</option>
            <option value="+44">🇬🇧 +44</option>
            <option value="+225">🇨🇮 +225</option>
            <option value="+223">🇲🇱 +223</option>
            <option value="+220">🇬🇲 +220</option>
          </select>
          <input type="tel" class="phone-number-input" id="co-num" placeholder="77 000 00 00" oninput="updatePhonePreview('co')">
        </div>
        <div class="phone-preview" id="co-phone-preview">Numéro complet : <span>—</span></div>
      </div>`;
  } else if(m==='card'){
    f.innerHTML=`
      <div class="card-form">
        <div class="card-preview-box">
          <div class="card-logos">
            <div class="cl-circle" style="background:#EB001B;"></div>
            <div class="cl-circle" style="background:#F79E1B;margin-left:-8px;"></div>
          </div>
          <div class="cpb-chip"></div>
          <div class="cpb-num" id="cpb-num">•••• •••• •••• ••••</div>
          <div class="cpb-row">
            <div><div class="cpb-label">TITULAIRE</div><div class="cpb-val" id="cpb-name">VOTRE NOM</div></div>
            <div><div class="cpb-label">EXPIRE</div><div class="cpb-val" id="cpb-exp">MM/AA</div></div>
          </div>
          <div class="cpb-visa">VISA</div>
        </div>
        <div class="fg"><label>Numéro de carte</label><input type="text" id="card-num" placeholder="1234 5678 9012 3456" maxlength="19" oninput="fmtCard(this);document.getElementById('cpb-num').textContent=this.value||'•••• •••• •••• ••••'"></div>
        <div class="fg"><label>Nom sur la carte</label><input type="text" id="card-name" placeholder="AMADOU DIALLO" oninput="this.value=this.value.toUpperCase();document.getElementById('cpb-name').textContent=this.value||'VOTRE NOM'"></div>
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:.7rem;">
          <div class="fg"><label>Expiration</label><input type="text" id="card-exp" placeholder="MM/AA" maxlength="5" oninput="fmtExp(this);document.getElementById('cpb-exp').textContent=this.value||'MM/AA'"></div>
          <div class="fg"><label>CVV</label><input type="text" id="card-cvv" placeholder="123" maxlength="3"></div>
        </div>
      </div>
      <div class="pay-secure-badges">
        <div class="psb">🔒 SSL 256-bit</div>
        <div class="psb">✅ 3D Secure</div>
        <div class="psb">💳 Visa/Mastercard</div>
      </div>`;
  }
}

function fmtCard(el){let v=el.value.replace(/\D/g,'').substring(0,16);el.value=v.replace(/(.{4})/g,'$1 ').trim();}
function fmtExp(el){let v=el.value.replace(/\D/g,'');if(v.length>=2)v=v.substring(0,2)+'/'+v.substring(2,4);el.value=v;}

function proceedPayment(){
  if(!payMethod){showToast('Choisissez un mode de paiement.');return;}
  if(payMethod==='orange'||payMethod==='wave'){
    const name=document.getElementById('co-name')?.value.trim();
    const num=document.getElementById('co-num')?.value.trim();
    if(!name||!num){showToast('Renseignez votre nom et numéro.');return;}
  } else if(payMethod==='card'){
    const num=document.getElementById('card-num')?.value.trim();
    const name=document.getElementById('card-name')?.value.trim();
    const exp=document.getElementById('card-exp')?.value.trim();
    const cvv=document.getElementById('card-cvv')?.value.trim();
    if(!num||!name||!exp||!cvv){showToast('Remplissez tous les champs de la carte.');return;}
  }
  showSuccessScreen();
}

// ══ BREVO EMAIL INTEGRATION ══
// ⚠️ REMPLACEZ LE TEXTE CI-DESSOUS PAR VOTRE CLE BREVO
// Votre cle commence par xkeysib- et se trouve sur app.brevo.com
const BREVO_API_KEY = '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';
const DIADIEUF_EMAIL = 'diadieuf.senegal@gmail.com';
const DIADIEUF_NAME = 'Diadieuf — Cartes de Voeux';

async function sendBrevoEmail({toEmail, toName, subject, htmlContent}){
  if(!BREVO_API_KEY || BREVO_API_KEY === 'PLACEHOLDER_ONLY'){
    console.warn('⚠️ Clé Brevo manquante — email non envoyé à : '+toEmail);
    return false;
  }
  try {
    const res = await fetch('https://api.brevo.com/v3/smtp/email', {
      method: 'POST',
      headers: {
        'Content-Type': 'application/json',
        'api-key': BREVO_API_KEY
      },
      body: JSON.stringify({
        sender: { name: DIADIEUF_NAME, email: DIADIEUF_EMAIL },
        to: [{ email: toEmail, name: toName||toEmail }],
        subject: subject,
        htmlContent: htmlContent
      })
    });
    if(!res.ok){
      const err = await res.text();
      console.error('Brevo erreur '+res.status+':', err);
      return false;
    }
    console.log('✅ Email envoyé à '+toEmail);
    return true;
  } catch(e) {
    console.error('Brevo fetch erreur:', e);
    return false;
  }
}

function buildEmailAcheteur(ref, tot, opLabel, cartItems, buyerN, buyerP){
  const lignes = cartItems.map(item=>`
    <tr>
      <td style="padding:10px;border-bottom:1px solid #f0e8e0;">
        <strong>${item.title}</strong><br>
        <span style="font-size:12px;color:#888;">${item.card.cat} · 🎵 ${item.card.music.t} · ${item.card.music.a}</span>
        ${item.gift?`<br><span style="font-size:12px;color:#F25A0A;">🎁 Cadeau : ${fmtS(item.gift.amount)} (${item.gift.op==='orange'?'Orange Money':'Wave'})</span>`:''}
        ${item.recip?`<br><span style="font-size:12px;color:#666;">📬 Pour : ${item.recip}${item.recipPhone?' · '+item.recipPhone:''}</span>`:''}
      </td>
      <td style="padding:10px;border-bottom:1px solid #f0e8e0;text-align:right;font-weight:700;color:#F25A0A;">
        ${fmtS(item.total)}
      </td>
    </tr>`).join('');
  return `
  <!DOCTYPE html>
  <html>
  <body style="margin:0;padding:0;background:#F5F2EF;font-family:'Helvetica Neue',Arial,sans-serif;">
    <div style="max-width:580px;margin:0 auto;background:#fff;border-radius:16px;overflow:hidden;margin-top:20px;">
      <!-- HEADER -->
      <div style="background:linear-gradient(135deg,#C04500,#F25A0A);padding:32px 24px;text-align:center;">
        <div style="font-size:32px;margin-bottom:8px;">🎴</div>
        <h1 style="color:#fff;font-family:Georgia,serif;font-style:italic;font-size:28px;margin:0;">Diadieuf</h1>
        <p style="color:rgba(255,255,255,.85);font-size:13px;margin:6px 0 0;">Cartes de Vœux Sénégalaises 🇸🇳</p>
      </div>
      <!-- BODY -->
      <div style="padding:28px 24px;">
        <h2 style="color:#0A0806;font-size:20px;margin-bottom:6px;">Merci ${buyerN} ! ✅</h2>
        <p style="color:#6A5E50;font-size:14px;line-height:1.6;margin-bottom:20px;">
          Votre commande a bien été confirmée. Voici votre récapitulatif.
        </p>
        <!-- REF BOX -->
        <div style="background:#FFF0E8;border-radius:12px;padding:14px 18px;margin-bottom:20px;display:flex;justify-content:space-between;align-items:center;">
          <span style="font-size:13px;color:#6A5E50;">Référence commande</span>
          <strong style="color:#F25A0A;font-size:15px;">${ref}</strong>
        </div>
        <!-- ARTICLES -->
        <table style="width:100%;border-collapse:collapse;margin-bottom:20px;">
          <thead>
            <tr style="background:#FFF0E8;">
              <th style="padding:10px;text-align:left;font-size:12px;color:#6A5E50;text-transform:uppercase;letter-spacing:.06em;">Carte</th>
              <th style="padding:10px;text-align:right;font-size:12px;color:#6A5E50;text-transform:uppercase;letter-spacing:.06em;">Prix</th>
            </tr>
          </thead>
          <tbody>${lignes}</tbody>
          <tfoot>
            <tr>
              <td style="padding:14px 10px;font-weight:800;font-size:16px;">TOTAL</td>
              <td style="padding:14px 10px;text-align:right;font-weight:800;font-size:16px;color:#F25A0A;">${fmtS(tot)}</td>
            </tr>
          </tfoot>
        </table>
        <!-- PAIEMENT -->
        <div style="background:#F5F2EF;border-radius:12px;padding:14px 18px;margin-bottom:20px;">
          <p style="margin:0;font-size:13px;color:#6A5E50;">💳 Paiement via <strong>${opLabel}</strong></p>
          <p style="margin:4px 0 0;font-size:13px;color:#6A5E50;">📱 Téléphone : <strong>${buyerP}</strong></p>
        </div>
        <!-- REMERCIEMENT CTA -->
        <div style="background:linear-gradient(135deg,#1A0A2E,#2D1B4E);border-radius:12px;padding:18px;text-align:center;margin-bottom:20px;">
          <p style="color:#fff;font-size:13px;margin:0 0 10px;">🙏 Le receveur peut vous envoyer une carte de remerciement !</p>
          <a href="https://diadieuf.vercel.app" style="background:#F25A0A;color:#fff;padding:10px 22px;border-radius:20px;text-decoration:none;font-size:13px;font-weight:700;">Visiter Diadieuf →</a>
        </div>
        <p style="color:#B0A898;font-size:12px;text-align:center;margin:0;">
          Des questions ? Contactez-nous : ${DIADIEUF_EMAIL}<br>
          Diadieuf — Dakar, Sénégal 🇸🇳
        </p>
      </div>
    </div>
  </body>
  </html>`;
}

function buildEmailReceveur(ref, senderName, cardTitle, cardCat, recipN){
  return `
  <!DOCTYPE html>
  <html>
  <body style="margin:0;padding:0;background:#F5F2EF;font-family:'Helvetica Neue',Arial,sans-serif;">
    <div style="max-width:580px;margin:0 auto;background:#fff;border-radius:16px;overflow:hidden;margin-top:20px;">
      <div style="background:linear-gradient(135deg,#C04500,#F25A0A);padding:32px 24px;text-align:center;">
        <div style="font-size:40px;margin-bottom:8px;">💌</div>
        <h1 style="color:#fff;font-family:Georgia,serif;font-style:italic;font-size:26px;margin:0;">Vous avez reçu une carte !</h1>
        <p style="color:rgba(255,255,255,.85);font-size:13px;margin:6px 0 0;">Diadieuf · Cartes de Vœux 🇸🇳</p>
      </div>
      <div style="padding:28px 24px;">
        <h2 style="color:#0A0806;font-size:18px;">Bonjour ${recipN} 👋</h2>
        <p style="color:#6A5E50;font-size:14px;line-height:1.7;">
          <strong>${senderName}</strong> vous a envoyé une belle carte de vœux via <strong>Diadieuf</strong> !
        </p>
        <div style="background:#FFF0E8;border-radius:12px;padding:18px;margin:20px 0;text-align:center;">
          <div style="font-size:36px;margin-bottom:8px;">🎴</div>
          <p style="font-family:Georgia,serif;font-style:italic;font-size:18px;color:#0A0806;margin:0 0 4px;">${cardTitle}</p>
          <p style="font-size:13px;color:#6A5E50;margin:0;">Catégorie : ${cardCat}</p>
        </div>
        <div style="text-align:center;margin:24px 0;">
          <a href="https://diadieuf.vercel.app" style="background:#F25A0A;color:#fff;padding:14px 32px;border-radius:30px;text-decoration:none;font-size:15px;font-weight:700;display:inline-block;">
            🙏 Répondre avec un Remerciement
          </a>
        </div>
        <p style="color:#B0A898;font-size:12px;text-align:center;">
          Diadieuf — Cartes de Vœux Sénégalaises · Dakar 🇸🇳
        </p>
      </div>
    </div>
  </body>
  </html>`;
}

function buildEmailAdmin(ref, tot, opLabel, buyerN, buyerP, buyerMail, cartItems){
  const lignes = cartItems.map(i=>`
    <tr>
      <td style="padding:8px;border-bottom:1px solid #eee;">${i.title} (${i.card.cat})</td>
      <td style="padding:8px;border-bottom:1px solid #eee;">${i.recip||'—'}${i.recipPhone?' · '+i.recipPhone:''}</td>
      <td style="padding:8px;border-bottom:1px solid #eee;text-align:right;color:#F25A0A;font-weight:700;">${fmtS(i.total)}</td>
    </tr>`).join('');
  return `
  <!DOCTYPE html><html><body style="font-family:Arial,sans-serif;background:#f5f5f5;">
  <div style="max-width:560px;margin:20px auto;background:#fff;border-radius:12px;overflow:hidden;">
    <div style="background:#0A0806;padding:20px 24px;display:flex;align-items:center;gap:12px;">
      <span style="font-size:24px;">🔔</span>
      <div>
        <h2 style="color:#F25A0A;margin:0;font-size:18px;">Nouvelle commande Diadieuf !</h2>
        <p style="color:#888;margin:4px 0 0;font-size:12px;">Réf : ${ref}</p>
      </div>
    </div>
    <div style="padding:20px 24px;">
      <div style="background:#FFF0E8;border-radius:10px;padding:14px;margin-bottom:16px;">
        <p style="margin:0 0 6px;font-size:14px;"><strong>👤 Acheteur :</strong> ${buyerN}</p>
        <p style="margin:0 0 6px;font-size:14px;"><strong>📱 Téléphone :</strong> ${buyerP}</p>
        ${buyerMail?`<p style="margin:0 0 6px;font-size:14px;"><strong>📧 Email :</strong> ${buyerMail}</p>`:''}
        <p style="margin:0;font-size:14px;"><strong>💳 Paiement :</strong> ${opLabel}</p>
      </div>
      <table style="width:100%;border-collapse:collapse;margin-bottom:16px;">
        <thead><tr style="background:#f5f5f5;">
          <th style="padding:8px;text-align:left;font-size:12px;">Carte</th>
          <th style="padding:8px;text-align:left;font-size:12px;">Receveur</th>
          <th style="padding:8px;text-align:right;font-size:12px;">Prix</th>
        </tr></thead>
        <tbody>${lignes}</tbody>
      </table>
      <div style="background:#F25A0A;border-radius:10px;padding:14px;text-align:center;">
        <p style="color:#fff;font-weight:800;font-size:18px;margin:0;">TOTAL : ${fmtS(tot)}</p>
      </div>
    </div>
  </div>
  </body></html>`;
}

async function sendAllEmails(ref, tot, opLabel, cartSnapshot, buyerN, buyerP, buyerMail){
  // 1. Email à l'acheteur
  if(buyerMail){
    await sendBrevoEmail({
      toEmail: buyerMail,
      toName: buyerN,
      subject: `✅ Commande confirmée — ${ref} | Diadieuf`,
      htmlContent: buildEmailAcheteur(ref, tot, opLabel, cartSnapshot, buyerN, buyerP)
    });
  }

  // 2. Email aux receveurs (un par carte)
  for(const item of cartSnapshot){
    if(item.recipEmail){
      await sendBrevoEmail({
        toEmail: item.recipEmail,
        toName: item.recip||'',
        subject: `💌 ${buyerN} vous a envoyé une carte | Diadieuf`,
        htmlContent: buildEmailReceveur(ref, buyerN, item.title, item.card.cat, item.recip||'')
      });
    }
  }

  // 3. Email admin (vous)
  await sendBrevoEmail({
    toEmail: DIADIEUF_EMAIL,
    toName: 'Diadieuf Admin',
    subject: `🔔 Nouvelle commande ${ref} — ${fmtS(tot)} | Diadieuf`,
    htmlContent: buildEmailAdmin(ref, tot, opLabel, buyerN, buyerP, buyerMail, cartSnapshot)
  });
}

function showSuccessScreen(){
  const tot=cart.reduce((s,i)=>s+i.total,0);
  const ref='DDUF-'+Math.random().toString(36).substring(2,8).toUpperCase();
  const fullPayPhone=(payMethod==='orange'||payMethod==='wave')?getFullPhone('co-country','co-num'):'';
  const opLabel=payMethod==='orange'?'🟠 Orange Money':payMethod==='wave'?'🌊 Wave':'💳 Carte bancaire';
  const cartSnapshot=[...cart];

  // Envoi emails Brevo
  sendAllEmails(ref, tot, opLabel, cartSnapshot, buyerName, buyerPhone, buyerEmail)
    .then(()=>console.log('✅ Emails Brevo envoyés'))
    .catch(e=>console.error('Erreur emails:',e));

  // Afficher les cartes achetées avec leur message
  const cartesHTML = cartSnapshot.map(item=>`
    <div style="background:#fff;border-radius:14px;padding:1rem;margin-bottom:.8rem;border:1.5px solid var(--border);text-align:left;">
      <div style="display:flex;align-items:center;gap:.8rem;margin-bottom:.6rem;">
        <div style="width:48px;height:64px;border-radius:8px;overflow:hidden;flex-shrink:0;">${item.card.svgFn()}</div>
        <div>
          <div style="font-weight:700;font-size:.9rem;color:var(--ink);">${item.title}</div>
          <div style="font-size:.75rem;color:var(--txt2);">${item.card.cat} · 🎵 ${item.card.music.t}</div>
          ${item.recip?`<div style="font-size:.75rem;color:var(--or);font-weight:600;">📬 Pour : ${item.recip}${item.recipPhone?' · '+item.recipPhone:''}</div>`:''}
        </div>
      </div>
      ${item.msg?`<div style="font-size:.82rem;color:var(--txt2);font-style:italic;border-left:3px solid var(--or);padding-left:.7rem;line-height:1.6;">"${item.msg}"</div>`:''}
      ${item.sig?`<div style="font-size:.78rem;color:var(--txt2);text-align:right;margin-top:.4rem;">${item.sig}</div>`:''}
      ${item.gift?`<div style="margin-top:.5rem;padding:4px 10px;border-radius:10px;background:var(--or-light);color:var(--or);font-size:.75rem;font-weight:700;display:inline-block;">🎁 Cadeau : ${fmtS(item.gift.amount)} · ${item.gift.op==='orange'?'Orange Money':'Wave'}</div>`:''}
    </div>`).join('');

  document.getElementById('pay-modal-content').innerHTML=`
    <div class="succ-screen">
      <div class="succ-icon">✅</div>
      <h3>Merci ${buyerName} !</h3>
      <div class="succ-ref">${ref}</div>
      <p style="margin-bottom:.8rem;">Paiement de <strong>${fmt(tot)}</strong> via <strong>${opLabel}</strong> accepté.<br>
      📱 <strong>${buyerPhone}</strong>${fullPayPhone?' · Paiement sur : '+fullPayPhone:''}</p>
      <div style="text-align:left;margin-bottom:1rem;">
        <div style="font-size:.82rem;font-weight:700;color:var(--or-dark);margin-bottom:.6rem;">🎴 Vos cartes :</div>
        ${cartesHTML}
      </div>
      <button class="pay-confirm-btn" onclick="afterOrder()">✓ Retour à la boutique</button>
    </div>`;
  cart=[];updateBadge();buyerName='';buyerPhone='';buyerEmail='';
}

function afterOrder(){closePay();closeCart();}

// ══ TOAST ══
function showToast(msg){const t=document.getElementById('toast');document.getElementById('toast-msg').textContent=msg;t.classList.add('show');setTimeout(()=>t.classList.remove('show'),3200);}

// ══ INIT ══

// ══ SUGGESTIONS MUSIQUE PAR CATÉGORIE ══
const MUSIC_BY_CAT={
  Anniversaire:[{t:'Happy Birthday',a:'Stevie Wonder'},{t:'Celebrate',a:'Kool & The Gang'},{t:'Beautiful Day',a:'U2'},{t:'Africa',a:'Toto'}],
  Mariage:[{t:'All You Need Is Love',a:'The Beatles'},{t:'A Thousand Years',a:'Christina Perri'},{t:'La Vie en Rose',a:'Édith Piaf'},{t:'Can You Feel The Love',a:'Elton John'}],
  Naissance:[{t:'What A Wonderful World',a:'Louis Armstrong'},{t:'You Are My Sunshine',a:'Ray Charles'},{t:'Pure Imagination',a:'Gene Wilder'},{t:'Baby',a:'Justin Bieber'}],
  Condoléances:[{t:'Hallelujah',a:'Leonard Cohen'},{t:'Ave Maria',a:'Schubert'},{t:'Amazing Grace',a:'Traditional'},{t:'Tears in Heaven',a:'Eric Clapton'}],
  Noel:[{t:'Jingle Bells',a:'Frank Sinatra'},{t:'White Christmas',a:'Bing Crosby'},{t:'Last Christmas',a:'Wham!'},{t:'Silent Night',a:'Traditional'}],
  Paques:[{t:'Hallelujah',a:'Leonard Cohen'},{t:'Here Comes The Sun',a:'The Beatles'},{t:'Morning Has Broken',a:'Cat Stevens'},{t:'Amazing Grace',a:'Traditional'}],
  FeteTravail:[{t:'We Are The World',a:'USA for Africa'},{t:'Imagine',a:'John Lennon'},{t:'Stand By Me',a:'Ben E. King'},{t:'A New Day Has Come',a:'Céline Dion'}],
  FinAnnee:[{t:'Auld Lang Syne',a:'Traditional'},{t:"New Year's Day",a:'U2'},{t:'Celebration',a:'Kool & The Gang'},{t:'Simply The Best',a:'Tina Turner'}],
  SaintValentin:[{t:'My Valentine',a:'Paul McCartney'},{t:'La Vie en Rose',a:'Édith Piaf'},{t:'Fly Me To The Moon',a:'Frank Sinatra'},{t:"She's The One",a:'Robbie Williams'}],
  Tabaski:[{t:'Tabaski',a:"Youssou N'Dour"},{t:'Immigrés',a:"Youssou N'Dour"},{t:'Allah Wakbar',a:'Salif Keita'},{t:'Fête africaine',a:'Ismaël Lô'}],
  Korité:[{t:'Salam Alaykoum',a:'Collectif'},{t:'Nuit de Ramadan',a:'Collectif'},{t:'Salat',a:'Hadj Omar'},{t:'Allah Wakbar',a:'Salif Keita'}],
  Tamkharit:[{t:'Tamkharit',a:'Super Étoile'},{t:'Afriki',a:"Youssou N'Dour"},{t:'Sawale',a:'Baaba Maal'},{t:'Diouma',a:'Ismaël Lô'}],
  Amour:[{t:'Endless Love',a:'Lionel Richie'},{t:'My Heart Will Go On',a:'Céline Dion'},{t:'At Last',a:'Etta James'},{t:"Je t'aime",a:'Gainsbourg'}],
  Entreprise:[{t:'Simply The Best',a:'Tina Turner'},{t:'Eye of the Tiger',a:'Survivor'},{t:'We Are The Champions',a:'Queen'},{t:"You've Got A Friend",a:'James Taylor'}],
  Remerciement:[{t:'Thank You',a:'Dido'},{t:'Merci',a:"Youssou N'Dour"},{t:'Grateful',a:'Naughty Boy'},{t:'Beautiful',a:'James Blunt'}],
};

let selectedTrack=null, musicCustom=false, musicTimeout=null, currentAudio=null;

function buildMusicSuggestions(){
  if(!currentCard)return;
  const suggs=MUSIC_BY_CAT[currentCard.cat]||MUSIC_BY_CAT['Anniversaire'];
  const cont=document.getElementById('music-suggestions');
  if(!cont)return;
  cont.innerHTML=suggs.map((s,i)=>`
    <div class="music-chip" id="mchip-${i}" onclick="pickSuggestion(${i})">
      <div class="music-chip-title">🎵 ${s.t}</div>
      <div class="music-chip-artist">${s.a}</div>
    </div>`).join('');
  pickSuggestion(0);
}

function pickSuggestion(i){
  if(!currentCard)return;
  const suggs=MUSIC_BY_CAT[currentCard.cat]||MUSIC_BY_CAT['Anniversaire'];
  selectedTrack={...suggs[i]};musicCustom=false;
  document.querySelectorAll('.music-chip').forEach((c,j)=>c.classList.toggle('selected',j===i));
  document.getElementById('music-search-input').value='';
  document.getElementById('deezer-results').innerHTML='';
  showSelectedTrack();updatePreview();updateEditorTotal();
}

function onMusicSearch(q){
  clearTimeout(musicTimeout);
  if(!q||q.length<2){document.getElementById('deezer-results').innerHTML='';return;}
  musicTimeout=setTimeout(()=>fetchDeezer(q),700);
}

async function fetchDeezer(q){
  const cont=document.getElementById('deezer-results');
  cont.innerHTML='<div style="color:rgba(255,255,255,.5);font-size:.75rem;padding:.3rem 0;">🔍 Recherche...</div>';
  try{
    const res=await fetch(`https://corsproxy.io/?https://api.deezer.com/search?q=${encodeURIComponent(q)}&limit=5&output=json`);
    const data=await res.json();
    if(data.data&&data.data.length){
      cont.innerHTML=data.data.map(tr=>`
        <div class="deezer-result" onclick="pickDeezer('${tr.title.replace(/'/g,"\'")}','${tr.artist.name.replace(/'/g,"\'")}','${tr.preview||''}')">
          <div style="font-size:1rem;">🎵</div>
          <div style="flex:1;">
            <div class="deezer-result-title">${tr.title}</div>
            <div class="deezer-result-artist">${tr.artist.name}</div>
          </div>
          ${tr.preview?`<button onclick="event.stopPropagation();playPreview('${tr.preview}')" style="background:rgba(29,185,84,.3);border:none;color:#1DB954;border-radius:6px;padding:3px 8px;cursor:pointer;font-size:.68rem;white-space:nowrap;">▶ 30s</button>`:''}
        </div>`).join('');
    }else{
      cont.innerHTML=showManualInput(q);
    }
  }catch(e){
    cont.innerHTML=showManualInput(q);
  }
}

function showManualInput(q){
  return `<div style="background:rgba(255,255,255,.06);border-radius:8px;padding:.6rem;">
    <div style="font-size:.72rem;color:rgba(255,255,255,.5);margin-bottom:.4rem;">Entrez manuellement :</div>
    <div style="display:flex;gap:.3rem;">
      <input type="text" id="m-title" value="${q}" placeholder="Titre" style="flex:1;background:rgba(255,255,255,.08);border:1px solid rgba(255,255,255,.2);border-radius:6px;padding:5px 8px;color:#fff;font-size:.75rem;outline:none;">
      <input type="text" id="m-artist" placeholder="Artiste" style="flex:1;background:rgba(255,255,255,.08);border:1px solid rgba(255,255,255,.2);border-radius:6px;padding:5px 8px;color:#fff;font-size:.75rem;outline:none;">
      <button onclick="pickManual()" style="background:#1DB954;color:#fff;border:none;border-radius:6px;padding:5px 10px;cursor:pointer;font-size:.72rem;font-weight:700;">OK</button>
    </div>
  </div>`;
}

function pickManual(){
  const t=document.getElementById('m-title')?.value.trim();
  const a=document.getElementById('m-artist')?.value.trim();
  if(t)pickDeezer(t,a||'','');
}

function pickDeezer(title,artist,preview){
  selectedTrack={t:title,a:artist,preview};musicCustom=true;
  document.querySelectorAll('.music-chip').forEach(c=>c.classList.remove('selected'));
  document.getElementById('deezer-results').innerHTML='';
  document.getElementById('music-search-input').value='';
  showSelectedTrack();updatePreview();updateEditorTotal();
  showToast('🎵 '+title+' sélectionné ! +500 F CFA');
}

function playPreview(url){
  if(currentAudio){currentAudio.pause();currentAudio=null;return;}
  currentAudio=new Audio(url);currentAudio.play();
  currentAudio.onended=()=>{currentAudio=null;};
}

function clearMusicSelection(){
  selectedTrack=null;musicCustom=false;
  document.getElementById('music-track-display').style.display='none';
  document.querySelectorAll('.music-chip').forEach(c=>c.classList.remove('selected'));
  updatePreview();updateEditorTotal();
}

function showSelectedTrack(){
  if(!selectedTrack)return;
  const d=document.getElementById('music-track-display');
  if(d){
    d.style.display='flex';
    document.getElementById('mtd-name').textContent=selectedTrack.t;
    document.getElementById('mtd-artist').textContent=selectedTrack.a+(musicCustom?' · +500 F CFA':'');
    document.getElementById('mtd-icon').textContent=musicCustom?'🎧':'🎵';
  }
}

buildCatTabs();
buildAllSections();
</script>
</body>
</html>
