<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#07090f">
<title>MNEMO — Multi-Deck Flashcards</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Share+Tech+Mono&family=Syne:wght@400;600;700;800&display=swap" rel="stylesheet">
<style>
:root {
  --bg:         #07090f;
  --bg2:        #0b0e1a;
  --surface:    #0e1220;
  --surface2:   #131829;
  --surface3:   #192035;
  --border:     #1c2840;
  --border2:    #243250;
  --glow:       #00f5c8;
  --glow-dim:   rgba(0,245,200,.12);
  --glow-faint: rgba(0,245,200,.05);
  --violet:     #7b5fff;
  --vio-dim:    rgba(123,95,255,.12);
  --danger:     #ff4d6d;
  --dan-dim:    rgba(255,77,109,.1);
  --text:       #c4d4ee;
  --text-mid:   #6a82a8;
  --text-dim:   #3a4f70;
  --mono:       'Share Tech Mono', monospace;
  --sans:       'Syne', sans-serif;
  --rad:        12px;
  --rad-lg:     18px;
}
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{background:var(--bg);color:var(--text);font-family:var(--sans);min-height:100vh;display:flex;flex-direction:column;overflow-x:hidden}
body::before{content:'';position:fixed;inset:0;background-image:linear-gradient(rgba(0,245,200,.025) 1px,transparent 1px),linear-gradient(90deg,rgba(0,245,200,.025) 1px,transparent 1px);background-size:44px 44px;pointer-events:none;z-index:0}
body::after{content:'';position:fixed;top:-30%;right:-15%;width:55%;height:70%;background:radial-gradient(ellipse,rgba(123,95,255,.06) 0%,transparent 68%);pointer-events:none;z-index:0}

/* ── APP GRID ── */
#app{position:relative;z-index:1;display:grid;grid-template-columns:260px 1fr;grid-template-rows:56px 1fr;min-height:100vh}

/* ── TOPNAV ── */
#topnav{grid-column:1/-1;display:flex;align-items:center;gap:16px;padding:0 24px;background:rgba(7,9,15,.85);backdrop-filter:blur(12px);border-bottom:1px solid var(--border);position:sticky;top:0;z-index:50}
.logo{font-family:var(--mono);font-size:1.05rem;letter-spacing:.22em;color:var(--glow);text-shadow:0 0 16px rgba(0,245,200,.45);flex-shrink:0}
.logo em{color:var(--violet);font-style:normal}
.nav-sep{flex:1}
.nav-tag{font-family:var(--mono);font-size:.65rem;letter-spacing:.14em;color:var(--text-dim);text-transform:uppercase}

/* ── SIDEBAR ── */
#sidebar{grid-row:2;background:var(--bg2);border-right:1px solid var(--border);display:flex;flex-direction:column;overflow-y:auto;position:sticky;top:56px;height:calc(100vh - 56px)}
.sb-header{padding:18px 16px 10px;display:flex;align-items:center;justify-content:space-between}
.sb-title{font-family:var(--mono);font-size:.65rem;letter-spacing:.16em;color:var(--text-dim);text-transform:uppercase}
#project-list{flex:1;overflow-y:auto;padding:4px 8px;display:flex;flex-direction:column;gap:4px}
.proj-item{display:flex;align-items:center;gap:10px;padding:10px 12px;border-radius:9px;border:1px solid transparent;cursor:pointer;transition:all .18s;background:transparent}
.proj-item:hover{background:var(--surface);border-color:var(--border)}
.proj-item.active{background:var(--glow-dim);border-color:rgba(0,245,200,.25)}
.proj-item.active .proj-name{color:var(--glow)}
.proj-ring{width:30px;height:30px;flex-shrink:0}
.proj-meta{flex:1;min-width:0}
.proj-name{font-size:.85rem;font-weight:700;color:var(--text);white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
.proj-count{font-family:var(--mono);font-size:.63rem;color:var(--text-dim);margin-top:2px}
.proj-del{opacity:0;background:none;border:none;color:var(--danger);cursor:pointer;font-size:.9rem;padding:3px 5px;border-radius:4px;transition:opacity .15s,background .15s;flex-shrink:0}
.proj-item:hover .proj-del{opacity:.55}
.proj-del:hover{opacity:1!important;background:var(--dan-dim)}
.sb-footer{padding:12px 8px;border-top:1px solid var(--border)}

/* ── MAIN ── */
#main{grid-row:2;padding:32px 40px 60px;display:flex;flex-direction:column;gap:24px;min-width:0}

/* ── WELCOME ── */
#welcome{display:flex;flex-direction:column;align-items:center;justify-content:center;flex:1;gap:20px;text-align:center;padding:40px 20px}
.wg{font-size:4rem;filter:drop-shadow(0 0 24px rgba(0,245,200,.35));animation:pulse 3s ease-in-out infinite}
@keyframes pulse{0%,100%{filter:drop-shadow(0 0 18px rgba(0,245,200,.3))}50%{filter:drop-shadow(0 0 32px rgba(0,245,200,.55))}}
.wt{font-size:1.8rem;font-weight:800;background:linear-gradient(135deg,var(--glow) 0%,var(--violet) 100%);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text}
.ws{font-size:.9rem;color:var(--text-mid);max-width:380px;line-height:1.7}

/* ── PROJECT VIEW ── */
#project-view{display:flex;flex-direction:column;gap:22px}
.pv-header{display:flex;align-items:center;gap:14px;flex-wrap:wrap}
.pv-title-wrap{flex:1;min-width:0}
.pv-title{font-size:1.5rem;font-weight:800;color:var(--text);white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
.pv-sub{font-family:var(--mono);font-size:.68rem;color:var(--text-dim);letter-spacing:.1em;margin-top:3px}

/* ── STATS ── */
.stats-row{display:grid;grid-template-columns:repeat(4,1fr);gap:10px}
.stat-card{background:var(--surface);border:1px solid var(--border);border-radius:var(--rad);padding:14px 16px;display:flex;flex-direction:column;gap:4px}
.stat-lbl{font-family:var(--mono);font-size:.6rem;letter-spacing:.14em;color:var(--text-dim);text-transform:uppercase}
.stat-val{font-size:1.6rem;font-weight:800;color:var(--text);line-height:1}
.sv-g{color:var(--glow)}.sv-v{color:var(--violet)}.sv-d{color:var(--danger)}

/* ── PROGRESS ── */
.prog-row{display:flex;flex-direction:column;gap:7px}
.prog-labels{display:flex;justify-content:space-between;font-family:var(--mono);font-size:.68rem;color:var(--text-mid)}
.prog-track{height:4px;background:var(--surface3);border-radius:99px;overflow:hidden}
.prog-fill{height:100%;background:linear-gradient(90deg,var(--violet),var(--glow));border-radius:99px;transition:width .45s cubic-bezier(.4,0,.2,1);box-shadow:0 0 10px rgba(0,245,200,.3)}

/* ── CARD ── */
.card-area{display:flex;flex-direction:column;align-items:center;gap:20px}
.card-scene{width:100%;max-width:580px;height:300px;perspective:1400px;cursor:pointer}
.card-inner{width:100%;height:100%;position:relative;transform-style:preserve-3d;transition:transform .52s cubic-bezier(.4,0,.2,1)}
.card-inner.flipped{transform:rotateY(180deg)}
.card-face{position:absolute;inset:0;backface-visibility:hidden;-webkit-backface-visibility:hidden;border-radius:var(--rad-lg);display:flex;flex-direction:column;align-items:center;justify-content:center;padding:36px;text-align:center;border:1px solid var(--border);overflow:hidden;background:var(--surface)}
.card-face::before{content:'';position:absolute;inset:0;background:radial-gradient(ellipse at 50% -10%,rgba(0,245,200,.06) 0%,transparent 60%);pointer-events:none}
.card-back{background:var(--surface2);transform:rotateY(180deg)}
.card-back::before{background:radial-gradient(ellipse at 50% 110%,rgba(123,95,255,.1) 0%,transparent 60%)}
.card-badge{position:absolute;top:14px;right:16px;font-family:var(--mono);font-size:.65rem;color:var(--text-dim);letter-spacing:.08em}
.card-tag{font-family:var(--mono);font-size:.63rem;letter-spacing:.18em;color:var(--text-dim);text-transform:uppercase;margin-bottom:12px}
.card-back .card-tag{color:var(--violet)}
.card-text{font-size:1.2rem;font-weight:700;line-height:1.55;color:var(--text)}
.card-back .card-text{color:var(--glow)}
.card-hint{position:absolute;bottom:14px;font-family:var(--mono);font-size:.62rem;color:var(--text-dim);letter-spacing:.08em}

/* ── CONTROLS ── */
.card-controls{display:flex;align-items:center;gap:10px;flex-wrap:wrap;justify-content:center}
.nav-btn{background:var(--surface);border:1px solid var(--border);color:var(--text-mid);border-radius:9px;width:44px;height:44px;display:flex;align-items:center;justify-content:center;font-size:1.1rem;cursor:pointer;transition:all .18s;flex-shrink:0}
.nav-btn:hover:not(:disabled){border-color:var(--border2);color:var(--text);background:var(--surface2)}
.nav-btn:disabled{opacity:.3;cursor:not-allowed}
.act-btn{font-family:var(--mono);font-size:.78rem;letter-spacing:.06em;padding:11px 24px;border-radius:9px;border:1px solid transparent;cursor:pointer;transition:all .2s;text-transform:uppercase}
.btn-got{background:var(--glow-dim);border-color:var(--glow);color:var(--glow)}
.btn-got:hover{background:rgba(0,245,200,.2);box-shadow:0 0 20px rgba(0,245,200,.2);transform:translateY(-1px)}
.btn-study{background:var(--dan-dim);border-color:var(--danger);color:var(--danger)}
.btn-study:hover{background:rgba(255,77,109,.18);box-shadow:0 0 20px rgba(255,77,109,.18);transform:translateY(-1px)}
.btn-flip{background:var(--vio-dim);border-color:var(--violet);color:var(--violet)}
.btn-flip:hover{background:rgba(123,95,255,.2);box-shadow:0 0 20px rgba(123,95,255,.2)}
.judge-btns{display:none;gap:10px}
.judge-btns.vis{display:flex}

/* ── COMPLETE ── */
#complete-screen{display:none;flex-direction:column;align-items:center;gap:18px;padding:40px 20px;text-align:center}
#complete-screen.vis{display:flex}
.cg{font-size:3.5rem;filter:drop-shadow(0 0 22px rgba(0,245,200,.5))}
.ct{font-size:1.9rem;font-weight:800;background:linear-gradient(135deg,var(--glow),var(--violet));-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text}
.ci{font-family:var(--mono);font-size:.83rem;color:var(--text-mid);line-height:2.1}
.ci b{color:var(--glow)}

/* ── UPLOAD ── */
.drop-zone{border:1.5px dashed var(--border2);border-radius:var(--rad-lg);padding:36px 24px;text-align:center;cursor:pointer;transition:all .22s;background:var(--surface);position:relative;overflow:hidden}
.drop-zone:hover,.drop-zone.dragover{border-color:var(--glow);background:var(--glow-faint);box-shadow:0 0 30px rgba(0,245,200,.07),inset 0 0 30px rgba(0,245,200,.03)}
.dz-icon{font-size:2rem;margin-bottom:8px;display:block}
.drop-zone p{font-size:.88rem;color:var(--text-mid);line-height:1.6}
.drop-zone strong{color:var(--glow)}
.fmt-hint{font-family:var(--mono);font-size:.68rem;color:var(--text-dim);background:var(--surface2);border:1px solid var(--border);border-radius:7px;padding:8px 14px;line-height:1.8;text-align:left}
.fmt-hint b{color:var(--violet)}

/* ── BUTTONS ── */
.btn{font-family:var(--mono);font-size:.75rem;letter-spacing:.07em;padding:9px 16px;border-radius:8px;border:1px solid var(--border);background:transparent;color:var(--text-mid);cursor:pointer;transition:all .18s;text-transform:uppercase;display:inline-flex;align-items:center;gap:6px}
.btn:hover{border-color:var(--border2);color:var(--text);background:var(--surface2)}
.btn-acc{border-color:var(--glow);color:var(--glow);background:var(--glow-dim)}
.btn-acc:hover{background:rgba(0,245,200,.18);box-shadow:0 0 14px rgba(0,245,200,.15)}
.btn-sm{padding:6px 12px;font-size:.68rem}

/* ── MODAL ── */
.modal-ov{display:none;position:fixed;inset:0;z-index:200;background:rgba(7,9,15,.8);backdrop-filter:blur(6px);align-items:center;justify-content:center}
.modal-ov.open{display:flex}
.modal{background:var(--surface);border:1px solid var(--border2);border-radius:var(--rad-lg);padding:32px;width:min(500px,92vw);display:flex;flex-direction:column;gap:20px;box-shadow:0 30px 80px rgba(0,0,0,.6),0 0 40px rgba(0,245,200,.04);animation:su .25s cubic-bezier(.4,0,.2,1)}
@keyframes su{from{opacity:0;transform:translateY(18px)}to{opacity:1;transform:translateY(0)}}
.modal-title{font-size:1.15rem;font-weight:800;color:var(--glow)}
.field{display:flex;flex-direction:column;gap:7px}
.field label{font-family:var(--mono);font-size:.65rem;letter-spacing:.12em;color:var(--text-dim);text-transform:uppercase}
.field input{background:var(--surface2);border:1px solid var(--border2);border-radius:8px;color:var(--text);font-family:var(--sans);font-size:.9rem;padding:10px 14px;outline:none;transition:border-color .18s,box-shadow .18s}
.field input:focus{border-color:var(--glow);box-shadow:0 0 0 3px rgba(0,245,200,.08)}
.modal-actions{display:flex;gap:10px;justify-content:flex-end}

/* ── TOAST ── */
.toast{position:fixed;bottom:24px;left:50%;transform:translateX(-50%) translateY(16px);background:var(--surface2);border:1px solid var(--border2);border-radius:8px;padding:11px 22px;font-family:var(--mono);font-size:.78rem;color:var(--text);opacity:0;transition:opacity .28s,transform .28s;pointer-events:none;z-index:300;white-space:nowrap}
.toast.err{border-color:var(--danger);color:var(--danger)}
.toast.ok{border-color:var(--glow);color:var(--glow)}
.toast.show{opacity:1;transform:translateX(-50%) translateY(0)}

/* ── EMPTY STATE ── */
.empty-sidebar{font-family:var(--mono);font-size:.68rem;color:var(--text-dim);padding:12px;line-height:1.7}

::-webkit-scrollbar{width:4px}::-webkit-scrollbar-track{background:transparent}::-webkit-scrollbar-thumb{background:var(--border);border-radius:99px}

@media(max-width:680px){
  #app{grid-template-columns:1fr}
  #sidebar{display:none}
  #main{padding:20px 16px 40px}
  .stats-row{grid-template-columns:repeat(2,1fr)}
  .card-scene{height:240px}
  .card-text{font-size:1rem}
}
</style>
</head>
<body>
<div id="app">

  <!-- TOPNAV -->
  <nav id="topnav">
    <div class="logo">MN<em>EM</em>O</div>
    <span class="nav-sep"></span>
    <span class="nav-tag" id="nav-ctx">/ select a deck</span>
  </nav>

  <!-- SIDEBAR -->
  <aside id="sidebar">
    <div class="sb-header">
      <span class="sb-title">Decks</span>
      <button class="btn btn-sm btn-acc" id="btn-new">+ New</button>
    </div>
    <div id="project-list"></div>
    <div class="sb-footer">
      <div style="font-family:var(--mono);font-size:.6rem;color:var(--text-dim);padding:4px 8px;line-height:1.8;">
        Stored locally.<br>No account needed.
      </div>
    </div>
  </aside>

  <!-- MAIN -->
  <main id="main">

    <!-- WELCOME -->
    <div id="welcome">
      <div class="wg">◈</div>
      <div class="wt">Welcome to MNEMO</div>
      <div class="ws">Create a deck, import a CSV, and start studying. Everything lives in your browser — works fully offline.</div>
      <button class="btn btn-acc" id="btn-new-welcome">+ Create your first deck</button>
    </div>

    <!-- PROJECT VIEW -->
    <div id="project-view" style="display:none">

      <div class="pv-header">
        <div class="pv-title-wrap">
          <div class="pv-title" id="pv-title">—</div>
          <div class="pv-sub"  id="pv-sub">0 cards</div>
        </div>
        <button class="btn btn-sm" id="btn-shuffle">⇄ Shuffle</button>
        <button class="btn btn-sm" id="btn-reset">↺ Reset</button>
        <button class="btn btn-sm" id="btn-reimport">⬆ Import CSV</button>
      </div>

      <div class="stats-row">
        <div class="stat-card"><div class="stat-lbl">Total</div><div class="stat-val" id="s-total">0</div></div>
        <div class="stat-card"><div class="stat-lbl">Remaining</div><div class="stat-val sv-g" id="s-remain">0</div></div>
        <div class="stat-card"><div class="stat-lbl">Got It</div><div class="stat-val sv-v" id="s-got">0</div></div>
        <div class="stat-card"><div class="stat-lbl">Review</div><div class="stat-val sv-d" id="s-review">0</div></div>
      </div>

      <div class="prog-row" id="prog-row">
        <div class="prog-labels">
          <span id="prog-lbl">Card 1 of 1</span>
          <span id="prog-pct">0%</span>
        </div>
        <div class="prog-track"><div class="prog-fill" id="prog-fill" style="width:0%"></div></div>
      </div>

      <!-- UPLOAD AREA -->
      <div id="upload-area" style="display:none;flex-direction:column;gap:12px;">
        <div class="drop-zone" id="drop-zone">
          <span class="dz-icon">⬡</span>
          <p><strong>Drop CSV here</strong> or click to browse</p>
          <p>NotebookLM export or any two-column CSV</p>
        </div>
        <input type="file" id="file-input" accept=".csv" style="display:none">
        <div class="fmt-hint"><b>FORMAT</b> — two columns, no header needed:<br><code>Question text, Answer text</code></div>
      </div>

      <!-- CARD STAGE -->
      <div id="card-stage" style="display:none">
        <div class="card-area">

          <div class="card-scene" id="card-scene" onclick="flipCard()">
            <div class="card-inner" id="card-inner">
              <div class="card-face">
                <div class="card-badge" id="badge-f">1 / 1</div>
                <div class="card-tag">Question</div>
                <div class="card-text" id="cf-text">—</div>
                <div class="card-hint">tap to reveal ↗</div>
              </div>
              <div class="card-face card-back">
                <div class="card-badge" id="badge-b">1 / 1</div>
                <div class="card-tag">Answer</div>
                <div class="card-text" id="cb-text">—</div>
                <div class="card-hint">↗ tap to flip back</div>
              </div>
            </div>
          </div>

          <div class="card-controls">
            <button class="nav-btn" id="btn-prev" onclick="navCard(-1)" title="Prev (←)">←</button>
            <button class="act-btn btn-flip" onclick="flipCard()">Flip</button>
            <div class="judge-btns" id="judge-btns">
              <button class="act-btn btn-study" onclick="judgeCard(false)">✗ Again</button>
              <button class="act-btn btn-got"   onclick="judgeCard(true)">✓ Got It</button>
            </div>
            <button class="nav-btn" id="btn-next" onclick="navCard(1)"  title="Next (→)">→</button>
          </div>

        </div>
      </div>

      <!-- COMPLETE -->
      <div id="complete-screen">
        <div class="cg">◈</div>
        <div class="ct">Round Complete</div>
        <div class="ci" id="ci"></div>
        <div style="display:flex;gap:10px;flex-wrap:wrap;justify-content:center">
          <button class="btn" id="btn-missed">↺ Study Missed</button>
          <button class="btn btn-acc" id="btn-restart">⟳ Full Restart</button>
        </div>
      </div>

    </div><!-- /project-view -->
  </main>
</div><!-- /app -->

<!-- NEW DECK MODAL -->
<div class="modal-ov" id="modal-ov">
  <div class="modal">
    <div class="modal-title">New Deck</div>
    <div class="field">
      <label>Deck Name</label>
      <input type="text" id="m-name" placeholder="e.g. Biology Chapter 4" maxlength="60">
    </div>
    <div class="field">
      <label>Icon (emoji, optional)</label>
      <input type="text" id="m-icon" placeholder="📚" maxlength="4">
    </div>
    <div class="modal-actions">
      <button class="btn" id="m-cancel">Cancel</button>
      <button class="btn btn-acc" id="m-create">Create Deck</button>
    </div>
  </div>
</div>

<div class="toast" id="toast"></div>

<script>
/* ══════════════════════════════════════════════════
   STORAGE
══════════════════════════════════════════════════ */
const KEY = 'mnemo_v3';
function load()    { try { return JSON.parse(localStorage.getItem(KEY)) || {}; } catch { return {}; } }
function save(d)   { try { localStorage.setItem(KEY, JSON.stringify(d)); } catch { toast('Storage full', 'err'); } }

/* ══════════════════════════════════════════════════
   STATE
══════════════════════════════════════════════════ */
let projects = load();   // { [id]: { name, icon, cards, session } }
let activeId = null;

const proj    = () => projects[activeId];
const session = () => proj()?.session;

/* ══════════════════════════════════════════════════
   HELPERS
══════════════════════════════════════════════════ */
const $ = id => document.getElementById(id);
function esc(s){ return s.replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;'); }

let _tt;
function toast(msg, type='ok'){
  const el=$('toast'); el.textContent=msg;
  el.className=`toast ${type} show`;
  clearTimeout(_tt); _tt=setTimeout(()=>el.className='toast',3000);
}

function shuffle(arr){
  for(let i=arr.length-1;i>0;i--){
    const j=Math.floor(Math.random()*(i+1));
    [arr[i],arr[j]]=[arr[j],arr[i]];
  }
}

/* ══════════════════════════════════════════════════
   SIDEBAR
══════════════════════════════════════════════════ */
function renderSidebar(){
  const list = $('project-list');
  list.innerHTML = '';
  const ids = Object.keys(projects);
  if(!ids.length){
    list.innerHTML = '<div class="empty-sidebar">No decks yet.<br>Hit + New to begin.</div>';
    return;
  }
  ids.forEach(id => {
    const p = projects[id];
    const total   = p.cards.length;
    const gotCnt  = p.session ? Object.values(p.session.judgements||{}).filter(Boolean).length : 0;
    const pct     = total ? Math.round((gotCnt/total)*100) : 0;
    const r=11, circ=2*Math.PI*r, dash=circ*pct/100;

    const el = document.createElement('div');
    el.className = 'proj-item' + (id===activeId?' active':'');
    el.dataset.id = id;
    el.innerHTML = `
      <svg class="proj-ring" viewBox="0 0 30 30">
        <circle cx="15" cy="15" r="${r}" fill="none" stroke="var(--border)" stroke-width="2.2"/>
        <circle cx="15" cy="15" r="${r}" fill="none" stroke="var(--glow)" stroke-width="2.2"
          stroke-dasharray="${dash} ${circ}" stroke-dashoffset="${circ/4}"
          stroke-linecap="round" style="transition:stroke-dasharray .4s"/>
        <text x="15" y="15" text-anchor="middle" dominant-baseline="central"
          font-family="var(--mono)" font-size="6.5" fill="var(--text-mid)">${pct}%</text>
      </svg>
      <div class="proj-meta">
        <div class="proj-name">${p.icon||'📋'} ${esc(p.name)}</div>
        <div class="proj-count">${total} card${total!==1?'s':''}</div>
      </div>
      <button class="proj-del" title="Delete">✕</button>`;
    el.querySelector('.proj-del').addEventListener('click', e => { e.stopPropagation(); deleteProj(id); });
    el.addEventListener('click', () => openProj(id));
    list.appendChild(el);
  });
}

/* ══════════════════════════════════════════════════
   PROJECT CRUD
══════════════════════════════════════════════════ */
function createProj(name, icon){
  const id = 'p_'+Date.now();
  projects[id] = { name, icon: icon||'📋', cards: [], session: null };
  save(projects);
  renderSidebar();
  openProj(id);
}

function deleteProj(id){
  if(!confirm(`Delete deck "${projects[id]?.name}"?`)) return;
  delete projects[id];
  save(projects);
  if(activeId===id){ activeId=null; showWelcome(); }
  renderSidebar();
}

function openProj(id){
  activeId = id;
  const p = proj();
  $('welcome').style.display       = 'none';
  $('project-view').style.display  = 'flex';
  $('nav-ctx').textContent         = '/ '+p.name;
  $('pv-title').textContent        = `${p.icon} ${p.name}`;
  $('pv-sub').textContent          = `${p.cards.length} card${p.cards.length!==1?'s':''}`;
  renderSidebar();
  if(!p.cards.length){ showUpload(); return; }
  if(!p.session) initSession(p.cards.map((_,i)=>i));
  restoreView();
}

function showWelcome(){
  $('welcome').style.display       = '';
  $('project-view').style.display  = 'none';
  $('nav-ctx').textContent         = '/ select a deck';
}

/* ══════════════════════════════════════════════════
   SESSION
══════════════════════════════════════════════════ */
/*  { queue:[idx…], pos:0, got:0, studyAgain:0,
      judgements:{idx:bool}, missed:[idx…],
      flipped:false, done:false }           */
function initSession(indices){
  proj().session = {
    queue:[...indices], pos:0, got:0, studyAgain:0,
    judgements:{}, missed:[], flipped:false, done:false
  };
  save(projects);
}

function restoreView(){
  const s = session();
  $('upload-area').style.display  = 'none';
  $('card-stage').style.display   = s.done ? 'none' : '';
  $('complete-screen').className  = s.done ? 'vis' : '';
  if(!s.done){ showCard(); updateStats(); }
  else        showComplete();
}

function showUpload(){
  $('upload-area').style.display  = 'flex';
  $('card-stage').style.display   = 'none';
  $('complete-screen').className  = '';
}

/* ══════════════════════════════════════════════════
   CARD RENDER
══════════════════════════════════════════════════ */
let flipped = false;

function showCard(){
  const s = session(), p = proj();
  flipped = s.flipped||false;
  $('card-inner').classList.toggle('flipped', flipped);
  $('judge-btns').classList.toggle('vis', flipped);

  const card = p.cards[s.queue[s.pos]];
  $('cf-text').textContent = card.front;
  $('cb-text').textContent = card.back;
  const badge = `${s.pos+1} / ${s.queue.length}`;
  $('badge-f').textContent = badge;
  $('badge-b').textContent = badge;

  $('btn-prev').disabled = s.pos === 0;
  $('btn-next').disabled = s.pos === s.queue.length-1;

  const pct = Math.round((s.pos/s.queue.length)*100);
  $('prog-fill').style.width  = pct+'%';
  $('prog-lbl').textContent   = `Card ${s.pos+1} of ${s.queue.length}`;
  $('prog-pct').textContent   = pct+'%';
}

window.flipCard = function(){
  const s=session(); if(!s||s.done) return;
  flipped = !flipped;
  $('card-inner').classList.toggle('flipped', flipped);
  $('judge-btns').classList.toggle('vis', flipped);
  s.flipped = flipped;
  save(projects);
};

window.navCard = function(dir){
  const s=session(); if(!s||s.done) return;
  const np = s.pos+dir;
  if(np<0||np>=s.queue.length) return;
  s.pos = np; s.flipped = false; flipped = false;
  save(projects); showCard();
};

window.judgeCard = function(wasGot){
  const s=session(); if(!s||s.done) return;
  const idx = s.queue[s.pos];
  const prev = s.judgements[idx];
  if(prev===true)  s.got--;
  if(prev===false) s.studyAgain--;
  if(wasGot) s.got++; else s.studyAgain++;
  s.judgements[idx] = wasGot;
  s.missed = wasGot ? s.missed.filter(m=>m!==idx)
                    : s.missed.includes(idx) ? s.missed : [...s.missed, idx];
  updateStats();
  if(s.pos < s.queue.length-1){
    s.pos++; s.flipped = false; flipped = false;
    save(projects); showCard();
  } else {
    s.done = true; save(projects); showComplete();
  }
};

/* ══════════════════════════════════════════════════
   STATS
══════════════════════════════════════════════════ */
function updateStats(){
  const s=session(), p=proj(); if(!s) return;
  $('s-total').textContent  = p.cards.length;
  $('s-remain').textContent = Math.max(0, s.queue.length-s.pos-1);
  $('s-got').textContent    = s.got;
  $('s-review').textContent = s.studyAgain;
}

/* ══════════════════════════════════════════════════
   COMPLETE
══════════════════════════════════════════════════ */
function showComplete(){
  const s=session(), total=s.queue.length;
  const pct = total ? Math.round((s.got/total)*100) : 0;
  $('card-stage').style.display  = 'none';
  $('complete-screen').className = 'vis';
  $('ci').innerHTML = `<b>${s.got}</b> got it &nbsp;·&nbsp; <b>${s.studyAgain}</b> to review &nbsp;·&nbsp; <b>${pct}%</b> accuracy`;
  const mb=$('btn-missed');
  if(s.missed.length){ mb.style.display=''; mb.onclick=()=>{ initSession(s.missed); restoreView(); }; }
  else mb.style.display='none';
  $('btn-restart').onclick = ()=>{ initSession(proj().cards.map((_,i)=>i)); restoreView(); };
  renderSidebar();
}

/* ══════════════════════════════════════════════════
   DECK CONTROLS
══════════════════════════════════════════════════ */
$('btn-shuffle').onclick  = ()=>{ if(!activeId||!proj().cards.length) return; const idx=proj().cards.map((_,i)=>i); shuffle(idx); initSession(idx); restoreView(); toast('Shuffled ✓'); };
$('btn-reset').onclick    = ()=>{ if(!activeId) return; initSession(proj().cards.map((_,i)=>i)); restoreView(); toast('Session reset'); };
$('btn-reimport').onclick = ()=>{ if(!activeId) return; showUpload(); };

/* ══════════════════════════════════════════════════
   CSV
══════════════════════════════════════════════════ */
const dz=$('drop-zone'), fi=$('file-input');
dz.addEventListener('click', ()=>fi.click());
dz.addEventListener('dragover', e=>{ e.preventDefault(); dz.classList.add('dragover'); });
dz.addEventListener('dragleave', ()=>dz.classList.remove('dragover'));
dz.addEventListener('drop', e=>{ e.preventDefault(); dz.classList.remove('dragover'); if(e.dataTransfer.files[0]) readCSV(e.dataTransfer.files[0]); });
fi.addEventListener('change', ()=>{ if(fi.files[0]) readCSV(fi.files[0]); fi.value=''; });

function readCSV(file){
  if(!file.name.endsWith('.csv')){ toast('Need a .csv file','err'); return; }
  const r=new FileReader();
  r.onload=e=>{
    const cards=parseCSV(e.target.result);
    if(!cards.length){ toast('No cards found','err'); return; }
    const p=proj(); p.cards=cards; p.session=null;
    save(projects);
    $('pv-sub').textContent=`${cards.length} cards`;
    initSession(cards.map((_,i)=>i));
    restoreView();
    renderSidebar();
    toast(`Imported ${cards.length} cards ✓`);
  };
  r.readAsText(file);
}

function parseCSV(text){
  const cards=[];
  for(const line of text.trim().split(/\r?\n/)){
    if(!line.trim()) continue;
    const m=line.match(/^(?:"((?:[^"]|"")*)"|([^,]*)),(?:"((?:[^"]|"")*)"|(.*))/);
    if(m){
      const f=(m[1]!==undefined?m[1].replace(/""/g,'"'):m[2]||'').trim();
      const b=(m[3]!==undefined?m[3].replace(/""/g,'"'):m[4]||'').trim();
      if(f) cards.push({front:f,back:b});
    }
  }
  return cards;
}

/* ══════════════════════════════════════════════════
   MODAL
══════════════════════════════════════════════════ */
function openModal(){ $('m-name').value=''; $('m-icon').value=''; $('modal-ov').classList.add('open'); setTimeout(()=>$('m-name').focus(),60); }
function closeModal(){ $('modal-ov').classList.remove('open'); }

$('btn-new').onclick         = openModal;
$('btn-new-welcome').onclick = openModal;
$('m-cancel').onclick        = closeModal;
$('modal-ov').addEventListener('click', e=>{ if(e.target===$('modal-ov')) closeModal(); });
$('m-create').onclick = ()=>{
  const name=$('m-name').value.trim();
  if(!name){ toast('Please enter a name','err'); return; }
  closeModal();
  createProj(name, $('m-icon').value.trim());
  toast(`Deck created ✓`);
};
$('m-name').addEventListener('keydown', e=>{ if(e.key==='Enter') $('m-create').click(); });

/* ══════════════════════════════════════════════════
   KEYBOARD
══════════════════════════════════════════════════ */
document.addEventListener('keydown', e=>{
  if(!activeId||!session()||session().done) return;
  if(document.activeElement.tagName==='INPUT') return;
  if(e.key===' '||e.key==='Enter'){ e.preventDefault(); flipCard(); return; }
  if(e.key==='ArrowRight'){ flipped ? judgeCard(true)  : navCard(1);  return; }
  if(e.key==='ArrowLeft') { flipped ? judgeCard(false) : navCard(-1); return; }
});

/* ══════════════════════════════════════════════════
   INIT
══════════════════════════════════════════════════ */
renderSidebar();
const ids=Object.keys(projects);
if(ids.length) openProj(ids[ids.length-1]);
else showWelcome();
</script>
</body>
</html>
