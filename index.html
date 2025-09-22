<html lang="en-us"><script src="https://pygame-web.github.io/archives/0.9/pythons.js" type=module id=site data-LINES=50 data-CONSOLE=25 data-python=python3.12 data-os=vtx,fs,snd,gui async defer>#<!--

print("""
Loading pacman_complete from pacman_complete.apk
    Pygbag Version : 0.9.3
    Template Version : 0.9.0
    Python  : 3.12
    CDN URL : https://pygame-web.github.io/archives/0.9/
    Screen  : 1280x720
    Title   : pacman_complete
    Folder  : pacman_complete
    Authors : pgw
    SPDX-License-Identifier: cookiecutter.spdx

""")


# screen pixels (real, hardware)
WIDTH=1024  # 1280
HEIGHT=600  # 720

# reference/idealized screen pixels
REFX = 1980
REFY = 1080

def u(real, ref, v):
    if abs(v)<0.9999999:
        result = int( (float(real)/100.0) * (v*1000))
        if v<0:
            return real-result
        return result
    return int( (real/ref) * v )

def ux(*argv):
    global WIDTH, REFX
    acc = 0
    for v in argv:
        acc += u(WIDTH, REFX, v)
    return acc

def uy(*argv):
    global HEIGHT, REFY
    acc = 0
    for v in argv:
        acc += u(HEIGHT, REFY, v)
    return acc




# do not rename
async def custom_site():

    import sys
    import asyncio
    import platform
    import json
    from pathlib import Path



    import embed


    platform.document.body.style.background = "#7f7f7f"

    import pygame

    def compose():
        pygame.display.update()
        window.chromakey(None, *screen.get_colorkey(), 40)

    pygame.init()
    pygame.font.init()

    screen = pygame.display.set_mode([ux(.100),uy(.100)], pygame.SRCALPHA, 32)
    screen.set_colorkey( (0,0,0,0), pygame.RLEACCEL )
    screen.fill( (0,0,0,0) )

    compose()

    platform.window.transfer.hidden = true
    platform.window.canvas.style.visibility = "visible"



    apk = "pacman_complete.apk"

    bundle = "pacman_complete"

    # the C or js loader could do that but be explicit.
    appdir = Path(f"/data/data/{bundle}") # /data/data/pacman_complete
    appdir.mkdir()


    # mount apk

    cfg = {
        "io": "url",
        "type":"mount",
        "mount" : {
            "point" : appdir.as_posix(),
            "path" : "/",
        },
        "path" : f"/ => {appdir.as_posix()}",
    }


    track = platform.window.MM.prepare(apk, json.dumps(cfg))

    marginx = ux(.020) # 20%
    marginy = uy(.045) # 45%


    def pg_bar(pos):
        nonlocal marginx, marginy
        # resolution of progress bar, recalculate since it may not be know yet.
        total = track.len or 10  # avoid div0
        slot = ux(.060)/ total # 60%

        pygame.draw.rect(screen,(10,10,10),( marginx-ux(10), marginy-uy(10), (total*slot)+ux(20), uy(110) ) )
        pygame.draw.rect(screen,(0,255,0), ( marginx, marginy, track.pos*slot, uy(90)) )

    # wait until zip mount + overlayfs is complete
    while not track.ready:
        pg_bar(track.pos)
        compose()
        await asyncio.sleep(.1)

    # fill it up in case it was cached and instant download
    pg_bar(track.len)
    compose()


    # preloader will change dir and prepend it to sys.path
    platform.run_main(PyConfig, loaderhome= appdir / "assets", loadermain=None)


    # wait preloading complete
    # that includes images and wasm compilation of bundled modules
    while embed.counter()<0:
        await asyncio.sleep(.1)

    main = appdir / "assets" / "main.py"

    # start async top level machinery and add a console.
    await TopLevel_async_handler.start_toplevel(platform.shell, console=window.python.config.debug)

    # now that apk is mounted we have access to font cache
    # but we need to fill __file__ that is not yet set
    __import__(__name__).__file__ = str(main)


    # now make a prompt
    fnt = pygame.sysfont.SysFont("freesans",  uy(80) )

    def ui_callback(pkg, error=None):
        nonlocal fnt
        if error:
            prompt = fnt.render(f"{error}", True, "black")
        else:
            prompt = fnt.render(f"Setting [{pkg}] up", True, "black")
        pg_bar(track.len)
        screen.blit(prompt, ( marginx+ ux(80), marginy - uy(10) ) )
        compose()

    # test/wait if user media interaction required
    if not platform.window.MM.UME:

        # now make a prompt
        fnt = pygame.sysfont.SysFont("freesans",  uy(80) )
        prompt = fnt.render("Ready to start !", True, "blue")
        pg_bar(track.len)
        screen.blit(prompt, ( marginx+ ux(80), marginy - uy(10) ) )
        compose()
        print("""
        * Waiting for media user engagement : please click/touch page *
    """)
        while not platform.window.MM.UME:
            await asyncio.sleep(.1)

    # cleanup
    screen.fill( (0,0,0,0) )
    pygame.display.flip()

    await shell.runpy(main, callback=ui_callback)



import asyncio

asyncio.run( custom_site() )












# BEGIN BLOCK
#
# now this is the html part you can (and should) customize
# It is not mandatory : pygame-script when it reads the first line (also called
# shebang ) of above code create absolute minimal widget set
# required for running with default rules
#
# do not alter that comment block it is separating python code from html code
# =============================================================================
# --></script><head>
<link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap" rel="stylesheet"><!--
//=============================================================================
//
//
//
//
//
//
//

    {%- if cookiecutter.comment != "" -%}
{{cookiecutter.comment}}
    {% endif %}

--><script type="application/javascript">
// END BLOCK



// this dict is available under PyConfig.config from __main__

config = {
    xtermjs : "1" ,
    _sdl2 : "canvas",
    user_canvas : 0,
    user_canvas_managed : 0,
    ume_block : 1,
    can_close : 0,
    archive : "pacman_complete",
    gui_debug : 3,
    cdn : "https://pygame-web.github.io/archives/0.9/",
    autorun : 0,
    PYBUILD : "3.12"
}

</script>

    <title>pacman_complete</title>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
    <meta name="viewport" content="height=device-height, initial-scale=1.0">
    <meta name="mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-capable" content="yes"/>

    <link rel="prefetch" href="https://pygame-web.github.io/archives/0.9/pythonrc.py">
    <link rel="prefetch" href="https://pygame-web.github.io/archives/0.9/vt/xterm.js">
    <link rel="prefetch" href="https://pygame-web.github.io/archives/0.9/vt/xterm-addon-image.js">
    <link rel="prefetch" href="https://pygame-web.github.io/archives/0.9/vt/xterm-addon-image.js">


    <link rel="icon" type="image/png" href="favicon.png" sizes="16x16">

    <style>
        #status {
            display: inline-block;
            vertical-align: top;
            margin-top: 20px;
            margin-left: 30px;
            font-weight: bold;
            color: rgb(120, 120, 120);
        }

        #progress {
            height: 20px;
            width: 300px;
        }

        div.emscripten { text-align: center; }
        div.emscripten_border { border: 1px solid black; }
        div.thick_border { border: 4px solid black; }

        /* the canvas *must not* have any border or padding, or mouse coords will be wrong */
        /* average size of droid screen 470dp x 320dp  */
        canvas.emscripten {
            border: 0px none;
            background-color: transparent;
            width: 100%;
            height: 100%;
            z-index: 5;

            padding: 0;
            margin: 0 auto;

            position: absolute;
            top: 0;
            bottom: 0;
            left: 0;
            right: 0;
        }

        body {
            font-family: arial;
            margin: 0;
            padding: none;
            background-color:powderblue;
        }

        .topright{
           position:absolute;
           top:0px;
           right:0px;
        }

        .bottomright {
            position:absolute;
            top: 40%;
            right: 0px;
        }

        .center {
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .trinfo{
           position:relative;
           right:0px;
           border: 1px solid black;
        }

        .framed{
           position:relative;
           top:150px;
           right:10px;
           border: 1px solid black;
        }
    
/* === 8-bit Pac-Man UI skin === */
:root { --pm-yellow:#ffd400; --pm-dark:#0b0b0b; --pm-grey:#1a1a1a; }
#scoreCard{ background:var(--pm-grey); border:4px solid var(--pm-dark); box-shadow:0 0 0 4px #fff inset; font-family:'Press Start 2P', system-ui, monospace; }
#scoreCard h3{ color:#fff; text-shadow:2px 2px 0 #000; font-family:'Press Start 2P', system-ui, monospace; }
.ui-btn.pixel, #dpad .pixel{ 
  font-family:'Press Start 2P', system-ui, monospace;
  border-radius:0 !important;
  border:4px solid var(--pm-dark) !important;
  background:var(--pm-yellow) !important;
  color:#000;
  image-rendering: pixelated;
  box-shadow: 
    0 4px 0 0 #000,               /* hard drop */
    inset 0 -4px 0 0 #c5a800,     /* bottom shade */
    inset 0 4px 0 0 #ffe768;      /* top light */
}
.ui-btn.pixel:active, #dpad .pixel:active{ 
  transform: translateY(2px);
  box-shadow: 
    0 2px 0 0 #000,
    inset 0 -2px 0 0 #c5a800,
    inset 0 2px 0 0 #ffe768;
}
#dpad{ filter: drop-shadow(0 6px 0 #000); }
#dpad .pixel{ width:48px;height:48px; }
#scoreModal{ backdrop-filter: blur(0px); } /* keep crisp */
#scoresList li{ color:#fff; font-family:'Press Start 2P', system-ui, monospace; font-size:12px; }
@media (max-width:420px){
  #scoresList li{ font-size:10px; }
}

</style>

    <script src="https://pygame-web.github.io/archives/0.9//browserfs.min.js"></script>

</head>

<body>

    <div id="transfer" align=center>
<!--        <div class="spinner" id='spinner'></div> -->
        <div class="emscripten" id="status">Downloading...</div>
        <div class="emscripten">
            <progress value="0" max="100" id="progress"></progress>
        </div>
    </div>


    <canvas class="emscripten" id="canvas"
width="1px"
height="1px"
    oncontextmenu="event.preventDefault()" tabindex=1>
    </canvas>

    <div id=html></div>

    <div id=crt  class=bottomright >

        <div id="system" hidden>
            <div class="button-container">
                <button id="aiostop" disabled>AIO ⏏︎</button>
                <button id="aiopaused_true" disabled>AIO ■</button>
                <button id="aiopaused_false" disabled>AIO ▶</button>
                <button id="pygame_mixer_music_pause" disabled>Music ■</button>
            </div>

            <div class="button-container">
                <div id=load_min>min</div>
                <div id=load_avg>avg</div>
                <div id=load_max>max</div>
              <button id="load_rst" disabled>RESET</button>
            </div>

            <div id="level">(battery level unknown)</div>
            <div id="stateBattery">(charging state unknown)</div>

        </div>

        <div id=box class="emscripten_border" hidden=true>

            <div id="info" class="trinfo"></div>

            <iframe id="iframe" class="framed" name="iframe"
width="470px" height="90%"
allowtransparency="true"
style="z-index: 10;"
style="background: #FFFFFF;"
frameborder="1"
                allowfullscreen="true"
                webkitallowfullscreen="true"
                msallowfullscreen="true"
                mozallowfullscreen="true"
                sandbox="allow-same-origin allow-top-navigation allow-scripts allow-pointer-lock"
                allow="autoplay; fullscreen *; geolocation; microphone; camera; midi; monetization; xr-spatial-tracking; gamepad; gyroscope; accelerometer; xr; cross-origin-isolated"
                src="https://pygame-web.github.io/archives/0.9/empty.html"
                scrolling="yes">
            </iframe>
        </div>

    </div>


    <div id="dlg" hidden>
        <input type="file" id="dlg_multifile" multiple accept="image/*">
        <label for="dlg_multifile">Select files</label>
    </div>

    <div id="pyconsole">
        <div id="terminal" tabIndex=1 align="left"></div>
    </div>

    <script type="application/javascript">

    async function custom_onload(debug_hidden) {
        // this is called before anything python is loaded
        // make your js customization here
        console.log(__FILE__, "custom_onload")

        pyconsole.hidden = debug_hidden
        system.hidden = debug_hidden
        transfer.hidden = debug_hidden
        info.hidden = debug_hidden
        box.hidden =  debug_hidden

    }

    function custom_prerun(){
        // no python main and no (MEMFS + VFS) yet.
        console.log(__FILE__, "custom_prerun")

    }

    function custom_postrun(){
        // python main and no VFS filesystem yet.
        console.log(__FILE__, "custom_postrun")

        // prevent ff horizontal scroll
        window.addEventListener("keydown", function(e) {
            if(["Space","ArrowUp","ArrowDown","ArrowLeft","ArrowRight"].indexOf(e.code) > -1) {
                if (!python.config.debug)
                    e.preventDefault();
            }
        }, false);

    }

    function debug() {
        // allow to gain access to dev tools from js console
        // but only on desktop. difficult to reach when in iframe
        python.config.debug = true
        custom_onload(false)
        Module.PyRun_SimpleString("shell.uptime()")
        window_resize()
    }

    function info_inline(data){
        document.getElementById("info").innerHTML = data
    }

    function info_online(url) {
        // display info about current APK
        fetch( url /*, options */)
            .then((response) => response.text())
            .then((html) => {
                info_inline(html);
        })
        .catch((error) => {
            console.warn(error);
        });
    }

    function frame_online(url) {
        window.frames["iframe"].location = url;
    }

    </script>


<!-- === Highscores UI + Mobile Controls (Google Sheets) === -->
<style>
  :root { --ui-gap: 16px; }
  .ui-btn{position:fixed;z-index:20;font:600 14px/1.2 system-ui;padding:.6rem .9rem;border:none;border-radius:12px;box-shadow:0 6px 18px rgba(0,0,0,.25);background:#fff;cursor:pointer}
  #btnScores{right:var(--ui-gap);top:var(--ui-gap)}
  #btnSave{right:var(--ui-gap);top:calc(var(--ui-gap) + 48px)}
  #scoreModal{position:fixed;inset:0;display:none;place-items:center;background:rgba(0,0,0,.55);z-index:9999}
  #scoreCard{width:min(92vw,520px);max-height:80vh;overflow:auto;background:#111;color:#fff;border-radius:16px;padding:18px}
  #scoreCard h3{margin:.2rem 0 1rem;font:700 18px/1.2 system-ui}
  #scoresList{list-style:none;margin:0;padding:0}
  #scoresList li{display:flex;justify-content:space-between;gap:12px;padding:8px 10px;border-bottom:1px solid rgba(255,255,255,.10)}

  /* D‑pad responsive */
  #dpad{position:fixed;left:0;top:0;width:140px;height:140px;opacity:.9;z-index:9998;touch-action:none}
  #dpad button{position:absolute;width:48px;height:48px;border-radius:14px;border:none;box-shadow:0 6px 18px rgba(0,0,0,.25);background:#fff}
  #dpad [data-dir="up"]{left:46px;top:0}
  #dpad [data-dir="left"]{left:0;top:46px}
  #dpad [data-dir="right"]{right:0;top:46px}
  #dpad [data-dir="down"]{left:46px;bottom:0}

  /* Smaller phones */
  @media (max-width: 420px) {
    :root { --ui-gap: 10px; }
    #dpad{width:120px;height:120px}
    #dpad button{width:40px;height:40px;border-radius:12px}
    #dpad [data-dir="up"]{left:40px}
    #dpad [data-dir="left"]{top:40px}
    #dpad [data-dir="right"]{top:40px}
    #dpad [data-dir="down"]{left:40px}
    .ui-btn{font-size:12px;padding:.5rem .7rem}
  }

  /* Hide D‑pad on big screens (можно убрать если хочешь видеть и на десктопе) */
  @media (min-width: 900px) {
    #dpad{opacity:.8}
  }

/* === 8-bit Pac-Man UI skin === */
:root { --pm-yellow:#ffd400; --pm-dark:#0b0b0b; --pm-grey:#1a1a1a; }
#scoreCard{ background:var(--pm-grey); border:4px solid var(--pm-dark); box-shadow:0 0 0 4px #fff inset; font-family:'Press Start 2P', system-ui, monospace; }
#scoreCard h3{ color:#fff; text-shadow:2px 2px 0 #000; font-family:'Press Start 2P', system-ui, monospace; }
.ui-btn.pixel, #dpad .pixel{ 
  font-family:'Press Start 2P', system-ui, monospace;
  border-radius:0 !important;
  border:4px solid var(--pm-dark) !important;
  background:var(--pm-yellow) !important;
  color:#000;
  image-rendering: pixelated;
  box-shadow: 
    0 4px 0 0 #000,               /* hard drop */
    inset 0 -4px 0 0 #c5a800,     /* bottom shade */
    inset 0 4px 0 0 #ffe768;      /* top light */
}
.ui-btn.pixel:active, #dpad .pixel:active{ 
  transform: translateY(2px);
  box-shadow: 
    0 2px 0 0 #000,
    inset 0 -2px 0 0 #c5a800,
    inset 0 2px 0 0 #ffe768;
}
#dpad{ filter: drop-shadow(0 6px 0 #000); }
#dpad .pixel{ width:48px;height:48px; }
#scoreModal{ backdrop-filter: blur(0px); } /* keep crisp */
#scoresList li{ color:#fff; font-family:'Press Start 2P', system-ui, monospace; font-size:12px; }
@media (max-width:420px){
  #scoresList li{ font-size:10px; }
}

</style>

<div id="nameBadge" class="ui-btn pixel" style="left:16px;top:16px;right:auto">👤 NAME: —</div>
<button id="btnScores" class="ui-btn pixel">🏆 High Scores</button>
<button id="btnChangeName" class="ui-btn pixel" style="top:calc(var(--ui-gap) + 48px);right:var(--ui-gap)">👤 Name</button>
<button id="btnSave" class="ui-btn pixel" title="Ручное сохранение для теста">💾 Save score</button>

<div id="scoreModal"><div id="scoreCard">
  <h3>High Scores</h3>
  <ul id="scoresList"><li>Loading…</li></ul>
  <div style="display:flex;gap:8px;justify-content:flex-end;margin-top:10px">
    <button class="ui-btn pixel" style="background:#ffd400;color:#000" onclick="document.getElementById('scoreModal').style.display='none'">Close</button>
  </div>
</div></div>

<!-- Name prompt at start -->
<div id="nameModal" style="position:fixed;inset:0;display:grid;place-items:center;background:rgba(0,0,0,.65);z-index:10000">
  <div style="background:#111;border:4px solid #000;box-shadow:0 0 0 4px #fff inset;border-radius:0;padding:18px;width:min(92vw,420px);color:#fff;font-family:'Press Start 2P', system-ui, monospace">
    <h3 style="margin:0 0 12px">ENTER NAME</h3>
    <input id="playerNameInput" maxlength="24" placeholder="PLAYER" 
      style="width:100%;padding:10px;border:4px solid #000;border-radius:0;font-family:'Press Start 2P', monospace;font-size:14px;background:#ffd400;color:#000;box-shadow:inset 0 -4px 0 #c5a800,inset 0 4px 0 #ffe768;">
    <div style="display:flex;gap:8px;justify-content:flex-end;margin-top:12px">
      <button id="nameOkBtn" class="ui-btn pixel" style="background:#ffd400;color:#000">OK</button>
    </div>
  </div>
</div>

<div id="dpad" aria-label="Touch controller">
  <button data-dir="up" class="pixel">▲</button>
  <button data-dir="left" class="pixel">◀</button>
  <button data-dir="right" class="pixel">▶</button>
  <button data-dir="down" class="pixel">▼</button>
</div>

<script>
const WEB_APP_URL = "https://script.google.com/a/macros/exactprosystems.com/s/AKfycbx4ngTsNYuRnVmPR9P8ZvsZbQzBqfm3YO7qToWXhel-3lHb2dKaHGU3EIe8vD0CWWvMoQ/exec";
const SECRET      = "CHANGE_ME_123";

/* Google Sheets API via Apps Script */
async function saveScoreOnline(name, score){
  try{
    await fetch(WEB_APP_URL, {
      method:"POST",
      headers:{"Content-Type":"application/json"},
      body:JSON.stringify({secret:SECRET, name, score, meta:{ua:navigator.userAgent}})
    });
  }catch(e){ console.warn('Save failed:', e.message); }
}
async function loadScoresOnline(limit=20){
  const r = await fetch(`${WEB_APP_URL}?top=${limit}`);
  return await r.json();
}

/* UI modal */
async function showScores(){
  const ul = document.getElementById('scoresList');
  ul.innerHTML = '<li>Loading…</li>';
  document.getElementById('scoreModal').style.display = 'grid';
  try{
    const data = await loadScoresOnline(20);
    ul.innerHTML = '';
    data.forEach((s,i)=>{
      const li = document.createElement('li');
      li.innerHTML = `<span>${i+1}. ${s.name}</span><strong>${s.score}</strong>`;
      ul.appendChild(li);
    });
  }catch(e){ ul.innerHTML = '<li>Не удалось загрузить</li>'; }
}
document.getElementById('btnScores').onclick = showScores;

/* Ручное сохранение (для теста) */
document.getElementById('btnSave').onclick = async () => {
  const name = localStorage.getItem('pacman_name') || prompt('Имя для рекорда?','Player');
  if (!name) return;
  localStorage.setItem('pacman_name', name);
  const score = Number(prompt('Сколько очков сохранить?','0'));
  if (!Number.isFinite(score)) return;
  await saveScoreOnline(name, score);
  showScores();
};

/* Автосохранение из Python (pygbag):
   В конце игры в Python вызвать:
   import platform
   platform.window.pacmanSaveScore(player_name, final_score)
*/
window.pacmanSaveScore = async function(name, score){
  const n = name || localStorage.getItem('pacman_name') || 'Player';
  await saveScoreOnline(n, Number(score)||0);
};

/* Touch controls → отправляем стрелки в canvas */
const canvas = document.getElementById('canvas');
function pressKey(code){
  const ev = new KeyboardEvent('keydown', {code, key: code.replace('Arrow',''), bubbles:true});
  canvas.dispatchEvent(ev); canvas.focus();
}
const map = { up:'ArrowUp', down:'ArrowDown', left:'ArrowLeft', right:'ArrowRight' };
document.querySelectorAll('#dpad [data-dir]').forEach(b=>{
  b.addEventListener('touchstart', e=>{ pressKey(map[e.currentTarget.dataset.dir]); e.preventDefault(); }, {passive:false});
});
/* свайпы для экрана */
let sx=0, sy=0;
window.addEventListener('touchstart', e=>{ sx=e.touches[0].clientX; sy=e.touches[0].clientY; }, {passive:true});
window.addEventListener('touchend', e=>{
  const dx=e.changedTouches[0].clientX-sx, dy=e.changedTouches[0].clientY-sy;
  if (Math.abs(dx)>Math.abs(dy)) pressKey(dx>0?'ArrowRight':'ArrowLeft');
  else pressKey(dy>0?'ArrowDown':'ArrowUp');
}, {passive:true});

// === Responsive canvas scaler (keeps aspect 1024x600) ===
(function(){
  const canvas = document.getElementById('canvas');
  canvas.style.imageRendering = 'pixelated';
  const TARGET_W = 1024, TARGET_H = 600; // from main.py
  function fit(){
    const vw = window.innerWidth, vh = window.innerHeight;
    const scale = Math.min(vw/TARGET_W, vh/TARGET_H);
    const w = Math.max( Math.floor(TARGET_W*scale), 320 );
    const h = Math.max( Math.floor(TARGET_H*scale), 240 );
    canvas.style.width = w + 'px';
    canvas.style.height = h + 'px';
    // keep centered
    canvas.style.left = ((vw - w)/2) + 'px';
    canvas.style.top  = ((vh - h)/2) + 'px';
    canvas.style.right = 'unset';
    canvas.style.bottom = 'unset';
  }
  window.addEventListener('resize', fit, {passive:true});
  window.addEventListener('orientationchange', fit, {passive:true});
  document.addEventListener('visibilitychange', fit);
  setTimeout(fit, 50);
  setTimeout(fit, 500);
  if (window.__positionDpad) setTimeout(window.__positionDpad, 520);
})();

// === Name handling robustness ===
(function(){
  const nameModal = document.getElementById('nameModal');
  const nameInput = document.getElementById('playerNameInput');
  const changeBtn = document.getElementById('btnChangeName');

  function stored(){
    try { return localStorage.getItem('pacman_name') || ''; } catch(_) { return ''; }
  }
  function saveName(val){
    try { localStorage.setItem('pacman_name', val); } catch(_) {}
  }
  function askIfMissing(){
    let n = stored().trim();
    if (!n){
      nameModal.style.display = 'grid';
      setTimeout(()=>nameInput && nameInput.focus(), 100);
    } else {
      nameModal.style.display = 'none';
    }
  }
  window.addEventListener('load', askIfMissing);

  // allow reopen/change name
  if (changeBtn){
    changeBtn.addEventListener('click', ()=>{
      nameModal.style.display = 'grid';
      nameInput.value = stored() || 'PLAYER';
      setTimeout(()=>nameInput && nameInput.select(), 50);
    });
  }

  // guard: if user closes modal without typing, keep asking
  const ok = document.getElementById('nameOkBtn');
  function commit(){
    const val = (nameInput.value || 'PLAYER').toUpperCase().slice(0,24);
    saveName(val);
    nameModal.style.display = 'none';
    document.getElementById('canvas').focus();
  }
  ok.addEventListener('click', commit);
  nameInput.addEventListener('keydown', (e)=>{ if(e.key==='Enter'){ e.preventDefault(); commit(); }});
  nameModal.addEventListener('click', (e)=>{
    // click backdrop does nothing — require explicit OK so имя точно сохранится
    if (e.target === nameModal){ /* ignore */ }
  });
})();

</script>
<!-- === /Highscores + Mobile === -->


<script>
// === Robust name persistence (localStorage + cookie fallback) ===
(function(){
  function setCookie(name, value, days){
    try{
      const d = new Date(); d.setTime(d.getTime() + (days*24*60*60*1000));
      document.cookie = name + "=" + encodeURIComponent(value) + ";expires=" + d.toUTCString() + ";path=/";
    }catch(_){}
  }
  function getCookie(name){
    try{
      const key = name + "=";
      const ca = document.cookie.split(';');
      for(let c of ca){
        while (c.charAt(0) === ' ') c = c.substring(1);
        if (c.indexOf(key) === 0) return decodeURIComponent(c.substring(key.length, c.length));
      }
    }catch(_){}
    return "";
  }
  window._getStoredName = function(){
    try{
      const ls = (localStorage.getItem('pacman_name') || '').trim();
      if (ls) return ls;
    }catch(_){}
    const ck = (getCookie('pacman_name') || '').trim();
    return ck || "";
  };
  window._setStoredName = function(val){
    const v = (val || 'PLAYER').toUpperCase().slice(0,24);
    try{ localStorage.setItem('pacman_name', v); }catch(_){}
    setCookie('pacman_name', v, 365*2);
    const badge = document.getElementById('nameBadge');
    if (badge){ badge.textContent = "👤 NAME: " + v; }
    return v;
  };

  // Initialize badge and enforce asking name if missing
  function initNameFlow(){
    const badge = document.getElementById('nameBadge');
    const n = _getStoredName();
    if (badge){ badge.textContent = "👤 NAME: " + (n || "—"); }
    const modal = document.getElementById('nameModal');
    const input = document.getElementById('playerNameInput');
    const okBtn = document.getElementById('nameOkBtn');
    function ensure(){
      const cur = _getStoredName();
      if (!cur){
        if (modal){ modal.style.display = 'grid'; }
        if (input){ input.value = 'PLAYER'; setTimeout(()=>input.focus(), 50); }
      }else{
        if (modal){ modal.style.display = 'none'; }
      }
    }
    if (okBtn){
      okBtn.onclick = function(){
        const v = (input && input.value ? input.value : 'PLAYER');
        _setStoredName(v);
        if (modal) modal.style.display = 'none';
        document.getElementById('canvas')?.focus(); if(window.__positionDpad) setTimeout(window.__positionDpad, 50);
      };
    }
    window.addEventListener('load', ensure);
  }
  initNameFlow();

  // Override JS bridge to ALWAYS use stored name
  window.pacmanSaveScore = async function(_name, score){
    const n = _getStoredName() || (_name ? String(_name).toUpperCase() : 'PLAYER');
    try{
      await saveScoreOnline(n, Number(score)||0);
    }catch(e){ console.warn('Save failed:', e.message); }
  };

  // Also wire "Name" button if present
  const changeBtn = document.getElementById('btnChangeName');
  if (changeBtn){
    changeBtn.onclick = function(){
      const modal = document.getElementById('nameModal');
      const input = document.getElementById('playerNameInput');
      if (modal) modal.style.display = 'grid';
      if (input){ input.value = _getStoredName() || 'PLAYER'; setTimeout(()=>input.focus(), 50); }
    };
  }
})();
</script>

</body>
</html>
