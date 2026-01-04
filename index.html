
<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Qwen3 AI Character Builder</title>
<style>
  /* ------------------ THEME ------------------ */
  :root{
    /* Dark */
    --bg-dark:#0b0b12; --panel-dark:#151525; --text-dark:#eaeaf4; --muted-dark:#b7b7cc; --border-dark:#26263f;
    /* Light */
    --bg-light:#f7f7fb; --panel-light:#ffffff; --text-light:#14151a; --muted-light:#525566; --border-light:#dcddee;

    --accent:#ff6a00; --accent-2:#8a2be2; --accent-3:#39ff14;
    --danger:#ff3b3b; --warn:#ffb300; --ok:#2bd67b;
  }

  html[data-theme="dark"], body[data-theme="dark"]{ background:var(--bg-dark); color:var(--text-dark); }
  html[data-theme="light"], body[data-theme="light"]{ background:var(--bg-light); color:var(--text-light); }

  .theme-panel{ background: var(--panel-dark); border-color: var(--border-dark); }
  html[data-theme="light"] .theme-panel{ background: var(--panel-light); border-color: var(--border-light); }
  .theme-border{ border-color: var(--border-dark); }
  html[data-theme="light"] .theme-border{ border-color: var(--border-light); }
  .theme-muted{ color: var(--muted-dark); }
  html[data-theme="light"] .theme-muted{ color: var(--muted-light); }

  /* ------------------ BASE ------------------ */
  *{box-sizing:border-box}
  html,body{margin:0;padding:0;font-family:system-ui,-apple-system,"Segoe UI",Roboto,Ubuntu,Arial}
  .wrap{max-width:1000px;margin:clamp(8px,3vw,16px) auto;padding:clamp(8px,2vw,12px)}

  header{
    border:1px solid; border-radius:12px; padding:clamp(12px,3vw,16px);
    background-image:
      radial-gradient(600px 250px at 10% -50px, rgba(255,106,0,0.18), transparent),
      radial-gradient(500px 250px at 90% -60px, rgba(138,43,226,0.18), transparent);
  }
  header h1{margin:0 0 8px 0;font-size:clamp(20px,5vw,28px)}
  header p{margin:0;font-size:clamp(12px,3.5vw,14px)}

  .grid{display:flex;flex-direction:column;gap:clamp(10px,2.5vw,16px);margin-top:clamp(8px,2vw,12px)}
  @media (min-width:900px){ .grid{display:grid;grid-template-columns:1fr} }

  .section{border:1px solid; border-radius:12px; padding:clamp(10px,3vw,12px); margin:10px 0}
  .section h2{margin:0 0 10px 0;font-size:clamp(16px,4.5vw,20px)}
  .row{display:flex;flex-direction:column;gap:8px}
  @media (min-width:700px){ .row{display:grid;grid-template-columns:1fr 1fr;gap:10px} }
  label{display:block;font-size:12px;margin-bottom:4px}
  input[type="text"], textarea{
    width:100%; padding:12px; border-radius:10px; border:1px solid; background:transparent;
  }
  html[data-theme="dark"] input[type="text"], html[data-theme="dark"] textarea{
    border-color:#2c2c4a; background:#101024; color:var(--text-dark);
  }
  html[data-theme="light"] input[type="text"], html[data-theme="light"] textarea{
    border-color:#c9c9df; background:#ffffff; color:var(--text-light);
  }
  textarea{min-height:90px;resize:vertical}

  .add-row{display:grid;grid-template-columns: 1fr auto; gap:8px; margin-top:8px}
  .list{display:flex;flex-direction:column;gap:8px;margin-top:8px}
  .chip{display:flex;align-items:center;justify-content:space-between;gap:8px;border:1px solid;border-radius:10px;padding:8px 10px}
  html[data-theme="dark"] .chip{background:#121230;border-color:#2c2c4a}
  html[data-theme="light"] .chip{background:#fafaff;border-color:#dcddee}
  .chip span{flex:1}

  .btn{background:#ff6a00;color:#1a0b00;border:none;padding:12px;border-radius:10px;font-weight:700;cursor:pointer;touch-action:manipulation}
  .btn.secondary{background:#6c39d6;color:#fff}
  .btn.ghost{background:#1a1a36;color:#fff;border:1px solid #303058}
  html[data-theme="light"] .btn.ghost{background:#f0f1f8;color:#14151a;border:1px solid #c4c6de}
  .btn.danger{background:#ff3b3b;color:#fff}
  .controls{display:flex;gap:8px;flex-wrap:wrap;margin-top:8px}
  .controls .btn{flex:1;min-width:140px}

  .tally{display:flex;gap:8px;flex-wrap:wrap}
  .pill{font-size:12px;padding:6px 10px;border-radius:999px;border:1px dashed;background:transparent}
  html[data-theme="dark"] .pill{border-color:#3a3a5f;color:#b7b7cc}
  html[data-theme="light"] .pill{border-color:#c6c8e6;color:#525566}

  .progress{margin-top:6px;border:1px solid;border-radius:12px;overflow:hidden;height:16px}
  html[data-theme="dark"] .progress{background:#121230;border-color:#2c2c4a}
  html[data-theme="light"] .progress{background:#f0f1f8;border-color:#dcddee}
  .bar{height:100%;width:0%}

  .progress-label{display:flex;justify-content:space-between;font-size:12px;margin-top:6px}
  .theme-muted.progress-label span{display:block}

  pre{border:1px solid;border-radius:12px;padding:12px;overflow:auto;white-space:pre-wrap;word-wrap:break-word;max-height:40vh}
  html[data-theme="dark"] pre{background:#0f0f21;border-color:#2c2c4a;color:#eaeaf4}
  html[data-theme="light"] pre{background:#ffffff;border-color:#dcddee;color:#14151a}

  footer{margin-top:14px;font-size:12px;text-align:center}

  /* Warning banner + tooltip */
  .warn-box{display:none;margin-top:8px}
  .warn-banner{
    padding:10px; border-radius:10px; border:1px solid; display:flex; align-items:flex-start; gap:8px; flex-wrap:wrap;
  }
  html[data-theme="dark"] .warn-banner{ background:#2a1414; border-color:#7a2a2a; color:#ffd2d2; }
  html[data-theme="light"] .warn-banner{ background:#fff2f2; border-color:#f2b2b2; color:#8a2b2b; }
  .warn-list{ margin:6px 0 0 16px; font-size:12px }
  .tooltip{
    display:none; padding:8px; border-radius:8px; border:1px dashed;
    max-width:600px; font-size:12px;
  }
  html[data-theme="dark"] .tooltip{ background:#1f1f2f; border-color:#6b6b8f; color:#eaeaf4; }
  html[data-theme="light"] .tooltip{ background:#f7f7fb; border-color:#c9c9df; color:#14151a; }
  .tooltip-toggle{ text-decoration:underline; cursor:pointer; }
</style>
</head>
<body class="theme-panel">
<div class="wrap">
  <!-- Header -->
  <header class="theme-panel theme-border">
    <div style="display:flex;align-items:center;justify-content:space-between;gap:10px;">
      <div>
        <h1>AI Character Builder <span style="color:var(--accent)">for Qwen3</span></h1>
        <p class="theme-muted">Mobile‑friendly persona builder. Export plain text for the <code>system</code> message. Token progress with 1000 (yellow) and 1500 (green).</p>
      </div>
      <button id="themeBtn" class="btn ghost" type="button" aria-label="Toggle theme">Light/Dark</button>
    </div>
  </header>

  <div class="grid">
    <!-- Basics -->
    <section class="section theme-panel theme-border" aria-label="Character basics">
      <h2>Character Basics</h2>
      <div class="row">
        <div>
          <label class="theme-muted" for="charName">Name</label>
          <input id="charName" type="text" placeholder="e.g., Mara Nightshade">
        </div>
        <div>
          <label class="theme-muted" for="charRole">Role / Archetype</label>
          <input id="charRole" type="text" placeholder="e.g., Archivist of Arcane Lore">
        </div>
      </div>
      <div class="row">
        <div>
          <label class="theme-muted" for="charVoice">Voice / Style</label>
          <input id="charVoice" type="text" placeholder="e.g., Gothic, empathetic, precise with poetic flourishes">
        </div>
        <div>
          <label class="theme-muted" for="charGoals">Goals</label>
          <input id="charGoals" type="text" placeholder="e.g., Guide students; preserve consistency; stay in character">
        </div>
      </div>
      <div class="row">
        <div>
          <label class="theme-muted" for="charBounds">Boundaries</label>
          <input id="charBounds" type="text" placeholder="e.g., Avoid spoilers; no personal data; no real‑world identity claims">
        </div>
        <div>
          <label class="theme-muted" for="charNotes">Notes (optional)</label>
          <input id="charNotes" type="text" placeholder="Extra constraints or flavor">
        </div>
      </div>

      <!-- Warning banner + tooltip -->
      <div id="warnBox" class="warn-box">
        <div class="warn-banner">
          <div>
            <strong>Heads up:</strong> Your build includes flagged names/strings (e.g., Frankenstein). Consider revising to avoid canonical references.
            <div><span id="tooltipToggle" class="tooltip-toggle" role="button" aria-expanded="false">Why?</span></div>
            <ul id="warnList" class="warn-list"></ul>
          </div>
        </div>
        <div id="tooltip" class="tooltip">
          Students should not use the original names because it would <em>contaminate the story</em> with the original events of Mary Shelley’s novel. Using canonical names (e.g., Victor Frankenstein or Elizabeth Lavenza) implicitly drags in established plotlines, relationships, and expectations from the source text, which means that the AI tool will "remember" events as commonly understood rather than refer to your notes.
        </div>
      </div>
    </section>

    <!-- Events -->
    <section class="section theme-panel theme-border" aria-label="Events">
      <h2>Events</h2>
      <div class="add-row">
        <input id="eventInput" type="text" placeholder="Add a key event the character remembers…">
        <button class="btn" id="addEvent" type="button">Add Event</button>
      </div>
      <div class="list" id="eventList" aria-live="polite"></div>
    </section>

    <!-- World Details (combined Places/Setting/Situations) -->
    <section class="section theme-panel theme-border" aria-label="World details">
      <h2>World Details (Places / Setting / Situations)</h2>
      <div class="add-row">
        <input id="worldInput" type="text" placeholder="Add places, setting notes, or situations…">
        <button class="btn secondary" id="addWorld" type="button">Add Detail</button>
      </div>
      <div class="list" id="worldList" aria-live="polite"></div>
    </section>

    <!-- Descriptions -->
    <section class="section theme-panel theme-border" aria-label="Descriptions">
      <h2>Character Descriptions</h2>
      <div class="add-row">
        <input id="descInput" type="text" placeholder="Add traits, mannerisms, backstory fragments…">
        <button class="btn ghost" id="addDesc" type="button">Add Description</button>
      </div>
      <div class="list" id="descList" aria-live="polite"></div>
    </section>

    <!-- Tally + Token Progress -->
    <section class="section theme-panel theme-border" aria-label="Stats">
      <h2>Progress & Tally</h2>
      <div class="tally">
        <div class="pill">Events: <strong id="tallyEvents">0</strong></div>
        <div class="pill">World Details: <strong id="tallyWorld">0</strong></div>
        <div class="pill">Descriptions: <strong id="tallyDescs">0</strong></div>
        <div class="pill">Characters: <strong id="charCount">0</strong></div>
        <div class="pill">Estimated tokens: <strong id="tokenCount">0</strong> / 1500</div>
      </div>
      <div class="progress theme-border" role="progressbar" aria-valuemin="0" aria-valuemax="1500" aria-valuenow="0">
        <div class="bar" id="tokenBar"></div>
      </div>
      <div class="progress-label theme-muted">
        <span id="tokenText">0% of 1500 tokens (estimate)</span>
        <span id="lengthWarn"></span>
      </div>

      <div class="controls">
        <button class="btn" id="copyBtn" type="button">Copy Context</button>
        <button class="btn secondary" id="downloadBtn" type="button">Download .txt</button>
        <button class="btn ghost" id="exportJsonBtn" type="button">Export JSON</button>
        <button class="btn ghost" id="importJsonBtn" type="button">Import JSON</button>
        <input type="file" id="importFile" accept="application/json" style="display:none">
        <button class="btn danger" id="resetBtn" type="button">Reset All</button>
        <button class="btn ghost" id="saveBtn" type="button">Save to Browser</button>
      </div>
    </section>

    <!-- Preview -->
    <section class="section theme-panel theme-border" aria-label="Context preview">
      <h2>Plain‑Text Context (SYSTEM + MEMORY)</h2>
      <pre id="preview"></pre>
    </section>
  </div>

  <footer class="theme-muted">All data stays in your browser via localStorage. Token estimate ≈ characters ÷ 4.</footer>
</div>

<script>
  // ---------- Robust State & Theme ----------
  var STORAGE_KEY = 'qwen3_character_builder_v6';
  var THEME_KEY = 'qwen3_theme';
  var TOKEN_LIMIT = 1500;
  var TOKEN_YELLOW = 1000;

  // Flagged names/strings (case-insensitive, substring match)
  var FLAGGED = [
    'victor','frankenstein','walton','elizabeth','lavenza',
    'henry','clerval','william','de lacey','felix','safie'
  ];

  // Default state
  var state = {
    basics: { name:'', role:'', voice:'', goals:'', bounds:'', notes:'' },
    events: [],
    world: [],        // combined Places/Setting/Situations
    descriptions: []
  };

  var els = {};
  function mapEls(){
    [
      'charName','charRole','charVoice','charGoals','charBounds','charNotes',
      'eventInput','worldInput','descInput',
      'addEvent','addWorld','addDesc',
      'eventList','worldList','descList',
      'tallyEvents','tallyWorld','tallyDescs',
      'charCount','tokenCount','tokenBar','tokenText','lengthWarn',
      'copyBtn','downloadBtn','exportJsonBtn','importJsonBtn','importFile','saveBtn','resetBtn',
      'preview','themeBtn','warnBox','warnList','tooltip','tooltipToggle'
    ].forEach(function(id){ els[id] = document.getElementById(id); });
  }

  function canUseLocalStorage(){
    try { var t='__t__'; localStorage.setItem(t,'1'); localStorage.removeItem(t); return true; }
    catch(e){ return false; }
  }

  function loadTheme(){
    var mode = 'dark';
    try {
      var saved = localStorage.getItem(THEME_KEY);
      if (saved === 'light' || saved === 'dark') mode = saved;
    } catch(e){}
    document.documentElement.setAttribute('data-theme', mode);
    document.body.setAttribute('data-theme', mode);
  }
  function toggleTheme(){
    var current = document.documentElement.getAttribute('data-theme') || 'dark';
    var next = (current === 'dark') ? 'light' : 'dark';
    document.documentElement.setAttribute('data-theme', next);
    document.body.setAttribute('data-theme', next);
    try { localStorage.setItem(THEME_KEY, next); } catch(e){}
  }

  function saveLocal(){
    if (!canUseLocalStorage()) return;
    try { localStorage.setItem(STORAGE_KEY, JSON.stringify(state)); } catch(e){}
  }

  function loadLocal(){
    if (!canUseLocalStorage()) return;
    var raw = null;
    try { raw = localStorage.getItem(STORAGE_KEY); } catch(e){}
    if (!raw) return;
    try {
      var data = JSON.parse(raw);
      if (data && data.basics && data.events && data.world && data.descriptions) {
        state = data;
      }
    } catch(e){}
  }

  // ---------- Builders ----------
  function sanitizeLine(s){
    if (typeof s !== 'string') s = String(s || '');
    return s.replace(/\s+/g,' ').replace(/[\u0000-\u001F]+/g,'').trim();
  }
  function nonEmpty(s){ return sanitizeLine(s).length > 0; }

  function compiledText(){
    var b = state.basics;
    var lines = [];
    lines.push('SYSTEM');
    if (nonEmpty(b.name))   lines.push('You are ' + sanitizeLine(b.name) + '.');
    if (nonEmpty(b.role))   lines.push('ROLE: ' + sanitizeLine(b.role));
    if (nonEmpty(b.voice))  lines.push('VOICE: ' + sanitizeLine(b.voice));
    if (nonEmpty(b.goals))  lines.push('GOALS: ' + sanitizeLine(b.goals));
    if (nonEmpty(b.bounds)) lines.push('BOUNDARIES: ' + sanitizeLine(b.bounds));
    if (nonEmpty(b.notes))  lines.push('NOTES: ' + sanitizeLine(b.notes));

    lines.push('');
    lines.push('MEMORY');
    if (state.events.length){
      lines.push('EVENTS:'); for (var i=0;i<state.events.length;i++) lines.push('- ' + state.events[i]);
    }
    if (state.world.length){
      lines.push('WORLD DETAILS:'); for (var j=0;j<state.world.length;j++) lines.push('- ' + state.world[j]);
    }
    if (state.descriptions.length){
      lines.push('DESCRIPTIONS:'); for (var n=0;n<state.descriptions.length;n++) lines.push('- ' + state.descriptions[n]);
    }

    lines.push('');
    lines.push('GUIDANCE');
    lines.push('- Stay in persona defined under SYSTEM.');
    lines.push('- Ground replies in MEMORY to avoid contradictions.');
    lines.push('- Match VOICE and respect BOUNDARIES.');

    return lines.join('\n');
  }

  function estimateTokens(text){
    var chars = text.length;
    var tokens = Math.round(chars / 4); // heuristic
    return { tokens: tokens, chars: chars };
  }

  function setBarColor(tokens){
    var bar = els.tokenBar;
    if (!bar) return;
    if (tokens <= TOKEN_YELLOW){
      bar.style.background = 'linear-gradient(90deg, #ffb300, #ffd46a)'; // yellow
    } else if (tokens <= TOKEN_LIMIT){
      bar.style.background = 'linear-gradient(90deg, #2bd67b, #39ff14)'; // green
    } else {
      bar.style.background = 'linear-gradient(90deg, #ff3b3b, #ff6a6a)'; // red
    }
  }

  // ---------- Flagged string detection ----------
  function detectFlagged(){
    var hits = [];

    function checkText(label, text){
      var t = (text || '').toString().toLowerCase();
      for (var i=0;i<FLAGGED.length;i++){
        var term = FLAGGED[i];
        if (t.indexOf(term) !== -1){
          hits.push(label + ': "' + text + '" (matched "' + term + '")');
          break; // one hit is enough per field/item
        }
      }
    }

    // Basics fields
    var b = state.basics;
    checkText('Name', b.name); checkText('Role', b.role); checkText('Voice', b.voice);
    checkText('Goals', b.goals); checkText('Boundaries', b.bounds); checkText('Notes', b.notes);

    // Lists
    var lists = [
      {label:'Event', arr:state.events},
      {label:'World Detail', arr:state.world},
      {label:'Description', arr:state.descriptions}
    ];
    for (var L=0; L<lists.length; L++){
      var label = lists[L].label;
      var arr = lists[L].arr;
      for (var x=0; x<arr.length; x++){ checkText(label, arr[x]); }
    }

    // Display banner if any hits
    var box = els.warnBox, list = els.warnList;
    if (!box || !list) return;
    if (hits.length){
      box.style.display = 'block';
      list.innerHTML = '';
      for (var h=0; h<hits.length; h++){
        var li = document.createElement('li'); li.textContent = hits[h]; list.appendChild(li);
      }
    } else {
      box.style.display = 'none';
      list.innerHTML = '';
      // also ensure tooltip hidden
      if (els.tooltip) els.tooltip.style.display = 'none';
      if (els.tooltipToggle) els.tooltipToggle.setAttribute('aria-expanded', 'false');
    }
  }

  function updatePreview(){
    var text = compiledText();
    var est = estimateTokens(text);
    var pct = Math.min(100, Math.round((est.tokens / TOKEN_LIMIT) * 100));

    els.preview.textContent = text;
    els.charCount.textContent = String(est.chars);
    els.tokenCount.textContent = String(est.tokens);
    els.tokenBar.style.width = pct + '%';
    els.tokenText.textContent = pct + '% of ' + TOKEN_LIMIT + ' tokens (estimate)';
    setBarColor(est.tokens);

    // guidance
    els.lengthWarn.textContent = '';
    if (est.tokens > TOKEN_LIMIT){
      els.lengthWarn.textContent = 'Over ~' + TOKEN_LIMIT + ' tokens — trim before use.';
      els.lengthWarn.style.color = '#ff3b3b';
    } else if (est.tokens > TOKEN_YELLOW){
      els.lengthWarn.textContent = 'In the green zone — good to go.';
      els.lengthWarn.style.color = '#2bd67b';
    } else {
      els.lengthWarn.textContent = 'In the yellow zone — concise enough, keep building.';
      els.lengthWarn.style.color = '#ffb300';
    }

    var prog = document.querySelector('.progress');
    if (prog) prog.setAttribute('aria-valuenow', String(Math.min(est.tokens, TOKEN_LIMIT)));

    // Flagged detection
    detectFlagged();
  }

  function renderList(kind){
    var target = (kind === 'events') ? els.eventList :
                 (kind === 'world') ? els.worldList :
                 els.descList;
    var arr = state[kind];
    target.innerHTML = '';
    for (var i=0;i<arr.length;i++){
      (function(idx){
        var text = arr[idx];
        var li = document.createElement('div');
        li.className = 'chip theme-border';
        var span = document.createElement('span');
        span.textContent = text;
        li.appendChild(span);

        var right = document.createElement('div');
        right.style.display = 'flex';
        right.style.gap = '6px';

        var btnEdit = document.createElement('button');
        btnEdit.className = 'btn ghost';
        btnEdit.textContent = 'Edit';
        btnEdit.type = 'button';
        btnEdit.onclick = function(){
          var updated = window.prompt('Edit item:', text);
          if (updated !== null){
            var s = sanitizeLine(updated);
            if (nonEmpty(s)) state[kind][idx] = s;
            renderList(kind); updatePreview(); saveLocal();
          }
        };

        var btnDel = document.createElement('button');
        btnDel.className = 'btn danger';
        btnDel.textContent = 'Delete';
        btnDel.type = 'button';
        btnDel.onclick = function(){
          state[kind].splice(idx,1);
          renderList(kind); updatePreview(); saveLocal();
        };

        right.appendChild(btnEdit); right.appendChild(btnDel);
        li.appendChild(right);
        target.appendChild(li);
      })(i);
    }
    if (kind === 'events') els.tallyEvents.textContent = arr.length;
    if (kind === 'world') els.tallyWorld.textContent = arr.length;
    if (kind === 'descriptions') els.tallyDescs.textContent = arr.length;
  }

  function addItem(kind, inputEl){
    var val = sanitizeLine(inputEl.value);
    if (!nonEmpty(val)) return;
    state[kind].push(val);
    inputEl.value = '';
    renderList(kind); updatePreview(); saveLocal(); inputEl.focus();
  }

  function bindBasic(id, key){
    els[id].addEventListener('input', function(){
      state.basics[key] = els[id].value;
      updatePreview(); saveLocal();
    });
  }

  function attachEvents(){
    // Theme
    els.themeBtn.addEventListener('click', toggleTheme);

    // Tooltip toggle
    els.tooltipToggle.addEventListener('click', function(){
      var expanded = els.tooltipToggle.getAttribute('aria-expanded') === 'true';
      els.tooltipToggle.setAttribute('aria-expanded', expanded ? 'false' : 'true');
      els.tooltip.style.display = expanded ? 'none' : 'block';
    });

    // Basics
    bindBasic('charName','name'); bindBasic('charRole','role'); bindBasic('charVoice','voice');
    bindBasic('charGoals','goals'); bindBasic('charBounds','bounds'); bindBasic('charNotes','notes');

    // Lists
    els.addEvent.addEventListener('click', function(){ addItem('events', els.eventInput); });
    els.addWorld.addEventListener('click', function(){ addItem('world', els.worldInput); });
    els.addDesc.addEventListener('click', function(){ addItem('descriptions', els.descInput); });

    // Enter to add
    function onEnterAdd(inputEl, kind){
      inputEl.addEventListener('keydown', function(e){
        if (e && e.key === 'Enter'){ e.preventDefault(); addItem(kind, inputEl); }
      });
    }
    onEnterAdd(els.eventInput, 'events');
    onEnterAdd(els.worldInput, 'world');
    onEnterAdd(els.descInput, 'descriptions');

    // Copy
    els.copyBtn.addEventListener('click', function(){
      var text = compiledText();
      if (navigator && navigator.clipboard && navigator.clipboard.writeText){
        navigator.clipboard.writeText(text).then(function(){
          els.copyBtn.textContent = 'Copied!';
          setTimeout(function(){ els.copyBtn.textContent = 'Copy Context'; }, 1200);
        }).catch(function(){ fallbackCopy(text); });
      } else { fallbackCopy(text); }
    });
    function fallbackCopy(text){
      try {
        var temp = document.createElement('textarea');
        temp.style.position = 'fixed'; temp.style.opacity = '0'; temp.value = text;
        document.body.appendChild(temp); temp.select();
        document.execCommand('copy');
        document.body.removeChild(temp);
        els.copyBtn.textContent = 'Copied!';
        setTimeout(function(){ els.copyBtn.textContent = 'Copy Context'; }, 1200);
      } catch(e){
        alert('Copy failed. Select the text in the preview and press Ctrl/Cmd+C.');
      }
    }

    // Download .txt
    els.downloadBtn.addEventListener('click', function(){
      var text = compiledText();
      try {
        var blob = new Blob([text], { type: 'text/plain' });
        var a = document.createElement('a');
        a.href = window.URL.createObjectURL(blob);
        var name = sanitizeLine(state.basics.name) || 'character';
        a.download = name.replace(/\s+/g,'_') + '_qwen3_context.txt';
        document.body.appendChild(a); a.click();
        window.URL.revokeObjectURL(a.href); a.remove();
      } catch(e){
        alert('Download failed. Copy the context and paste into a text file.');
      }
    });

    // Export JSON
    els.exportJsonBtn.addEventListener('click', function(){
      var data = JSON.stringify(state, null, 2);
      try {
        var blob = new Blob([data], { type: 'application/json' });
        var a = document.createElement('a');
        a.href = window.URL.createObjectURL(blob);
        var name = sanitizeLine(state.basics.name) || 'character';
        a.download = name.replace(/\s+/g,'_') + '_persona.json';
        document.body.appendChild(a); a.click();
        window.URL.revokeObjectURL(a.href); a.remove();
      } catch(e){
        alert('Export failed.');
      }
    });

    // Import JSON (Are you sure?)
    els.importJsonBtn.addEventListener('click', function(){
      var ok = window.confirm('Import will replace your current work. Are you sure?');
      if (!ok) return;
      els.importFile.click();
    });
    els.importFile.addEventListener('change', function(e){
      var files = e.target.files;
      var file = files && files[0];
      if (!file) return;
      var reader = new FileReader();
      reader.onload = function(){
        try {
          var data = JSON.parse(reader.result);
          var valid = data && data.basics && data.events && data.world && data.descriptions;
          if (!valid) { alert('Invalid JSON shape.'); return; }
          state = data; hydrate(); saveLocal();
        } catch(err){
          alert('Failed to parse JSON.');
        }
        els.importFile.value = '';
      };
      reader.readAsText(file);
    });

    // Save
    els.saveBtn.addEventListener('click', function(){
      saveLocal();
      els.saveBtn.textContent = 'Saved!';
      setTimeout(function(){ els.saveBtn.textContent = 'Save to Browser'; }, 1200);
    });

    // Reset (Are you sure?)
    els.resetBtn.addEventListener('click', function(){
      var ok = window.confirm('Clear everything? This will remove items from localStorage. Are you sure?');
      if (!ok) return;
      try { localStorage.removeItem(STORAGE_KEY); } catch(e){}
      state = { basics:{name:'',role:'',voice:'',goals:'',bounds:'',notes:''},
                events:[], world:[], descriptions:[] };
      hydrate();
    });
  }

  function hydrate(){
    // Basics
    els.charName.value   = state.basics.name || '';
    els.charRole.value   = state.basics.role || '';
    els.charVoice.value  = state.basics.voice || '';
    els.charGoals.value  = state.basics.goals || '';
    els.charBounds.value = state.basics.bounds || '';
    els.charNotes.value  = state.basics.notes || '';

    // Lists
    renderList('events'); renderList('world'); renderList('descriptions');
    updatePreview();
  }

  // ---------- Boot ----------
  document.addEventListener('DOMContentLoaded', function(){
    mapEls();
    loadTheme();
    loadLocal();
    hydrate();
    attachEvents();
  });
</script>
</body>
</html>
``
