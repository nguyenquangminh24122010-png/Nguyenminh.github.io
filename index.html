<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Nminh Lock Pro</title>
<style>
  :root{
    --cyan:#39e6e6;
    --cyan-soft:rgba(57,230,230,.12);
    --text:#eaf2f2;
    --text-dim:#7e93a0;
    --danger:#ff5c5c;
    --gold:#ffd700;
    --panel-border:rgba(57,230,230,0.2);
  }
  *{box-sizing:border-box;margin:0;padding:0;}
  html,body{height:100%;font-family:'Segoe UI',system-ui,sans-serif;color:var(--text);background:#020408;overflow:hidden;}

  /* ===== GALAXY ===== */
  #galaxy{position:fixed;inset:0;pointer-events:none;z-index:0;}
  .nebula{position:fixed;pointer-events:none;z-index:0;border-radius:50%;filter:blur(80px);animation:nebulaPulse 8s ease-in-out infinite alternate;}
  .nebula1{width:600px;height:400px;top:-100px;left:-100px;background:radial-gradient(ellipse,rgba(80,20,160,0.35),transparent 70%);}
  .nebula2{width:500px;height:500px;bottom:-150px;right:-100px;background:radial-gradient(ellipse,rgba(20,60,180,0.3),transparent 70%);animation-delay:3s;}
  .nebula3{width:300px;height:300px;top:40%;left:40%;background:radial-gradient(ellipse,rgba(57,230,230,0.07),transparent 70%);animation-delay:5s;}
  @keyframes nebulaPulse{from{opacity:.7;transform:scale(1);}to{opacity:1;transform:scale(1.1);}}
  .star-shoot{position:fixed;z-index:0;pointer-events:none;width:2px;height:2px;background:#fff;border-radius:50%;box-shadow:0 0 4px #fff,0 0 10px rgba(57,230,230,0.6);animation:shoot linear infinite;opacity:0;}
  @keyframes shoot{0%{opacity:0;transform:translate(0,0) rotate(-45deg) scaleX(1);}5%{opacity:1;}15%{opacity:0;transform:translate(200px,200px) rotate(-45deg) scaleX(80);}100%{opacity:0;}}
  #snow,#petals{position:fixed;inset:0;pointer-events:none;z-index:1;}

  /* ===== INTRO SCREEN ===== */
  #intro{
    position:fixed;inset:0;z-index:100;
    display:flex;flex-direction:column;align-items:center;justify-content:center;gap:0;
    background:radial-gradient(ellipse at 50% 40%, #060a14 0%, #020408 65%, #000102 100%);
    transition:opacity 0.9s ease, filter 0.9s ease;
  }
  #intro.hide{opacity:0;filter:blur(6px);pointer-events:none;}

  /* Sweeping security ring behind everything */
  .intro-ring-orbit{position:absolute;width:260px;height:260px;border-radius:50%;display:flex;align-items:center;justify-content:center;}
  .intro-ring-orbit::before{
    content:'';position:absolute;inset:0;border-radius:50%;
    border:1px solid rgba(57,230,230,0.14);
  }
  .intro-ring-orbit::after{
    content:'';position:absolute;inset:-1px;border-radius:50%;
    border:1.5px solid transparent;
    border-top-color:var(--cyan);
    border-right-color:rgba(57,230,230,0.5);
    opacity:0;
    animation:ringSweep 1.8s ease-out 0.05s forwards, ringFade .6s ease 2.6s forwards;
  }
  @keyframes ringSweep{
    0%{transform:rotate(-90deg) scale(.82);opacity:0;}
    12%{opacity:1;}
    100%{transform:rotate(640deg) scale(1);opacity:1;}
  }
  @keyframes ringFade{to{opacity:0;}}

  .intro-ring-tick{position:absolute;width:3px;height:3px;border-radius:50%;background:var(--cyan);opacity:0;box-shadow:0 0 6px var(--cyan);animation:tickPop .4s ease forwards;}

  /* Crown: assembles from light instead of just popping in */
  .intro-crown-wrap{position:relative;width:64px;height:64px;margin-bottom:14px;display:flex;align-items:center;justify-content:center;}
  .intro-crown{
    font-size:38px;line-height:1;
    opacity:0;filter:drop-shadow(0 0 0px var(--gold));
    animation:crownAssemble 0.9s cubic-bezier(0.16,1,0.3,1) 0.15s forwards;
  }
  @keyframes crownAssemble{
    0%{opacity:0;transform:scale(2.4) translateY(10px);filter:drop-shadow(0 0 0px var(--gold)) blur(6px);}
    55%{opacity:1;filter:drop-shadow(0 0 22px var(--gold)) blur(0px);}
    100%{opacity:1;transform:scale(1) translateY(0);filter:drop-shadow(0 0 10px var(--gold)) blur(0px);}
  }
  .crown-spark{position:absolute;width:2px;height:2px;border-radius:50%;background:var(--gold);box-shadow:0 0 5px var(--gold);opacity:0;animation:sparkOut .6s ease-out 0.5s forwards;}

  /* Title: soft reveal + gleam sweep, no harsh typewriter cursor */
  .intro-title-wrap{position:relative;overflow:hidden;padding:0 4px;}
  .intro-title{
    font-size:30px;font-weight:800;letter-spacing:7px;
    text-transform:uppercase;color:var(--cyan);
    text-shadow:0 0 30px rgba(57,230,230,0.55),0 0 60px rgba(57,230,230,0.25);
    opacity:0;
    transform:translateY(10px);
    animation:titleRise .7s cubic-bezier(0.16,1,0.3,1) 0.85s forwards;
  }
  @keyframes titleRise{to{opacity:1;transform:translateY(0);}}
  .intro-title-wrap::after{
    content:'';position:absolute;top:0;left:-60%;width:40%;height:100%;
    background:linear-gradient(100deg,transparent,rgba(255,255,255,0.55),transparent);
    transform:skewX(-18deg);
    opacity:0;
    animation:gleam .9s ease 1.55s forwards;
  }
  @keyframes gleam{
    0%{left:-60%;opacity:0;}
    15%{opacity:.9;}
    60%{opacity:.5;}
    100%{left:130%;opacity:0;}
  }

  .intro-sub{
    margin-top:10px;
    font-size:11.5px;letter-spacing:3.5px;color:var(--text-dim);text-transform:uppercase;
    opacity:0;
    animation:fadeUp 0.6s ease 1.95s forwards;
  }
  @keyframes fadeUp{from{opacity:0;transform:translateY(8px);}to{opacity:1;transform:translateY(0);}}

  .intro-status{
    display:flex;align-items:center;gap:7px;
    margin-top:22px;
    font-size:10.5px;letter-spacing:1.5px;color:var(--text-dim);
    opacity:0;animation:fadeUp 0.4s ease 2.2s forwards;
  }
  .intro-status .dot{width:5px;height:5px;border-radius:50%;background:var(--cyan);box-shadow:0 0 6px var(--cyan);animation:dotPulse 1.1s ease-in-out infinite;}
  @keyframes dotPulse{0%,100%{opacity:.35;transform:scale(.8);}50%{opacity:1;transform:scale(1.15);}}
  .intro-status-text{position:relative;min-width:128px;text-align:left;}
  .intro-status-text span{position:absolute;left:0;top:0;white-space:nowrap;opacity:0;animation:statusSwap 2.4s steps(1) 2.2s infinite;}
  .intro-status-text span:nth-child(1){animation-delay:2.2s;}
  .intro-status-text span:nth-child(2){animation-delay:3.0s;}
  .intro-status-text span:nth-child(3){animation-delay:3.8s;}
  @keyframes statusSwap{0%{opacity:1;}32%{opacity:1;}38%{opacity:0;}100%{opacity:0;}}

  .intro-bar-wrap{
    width:176px;height:2px;background:rgba(57,230,230,0.13);border-radius:2px;overflow:hidden;
    margin-top:14px;
    opacity:0;animation:fadeUp 0.4s ease 2.2s forwards;
  }
  .intro-bar{
    height:100%;width:0;border-radius:2px;
    background:linear-gradient(90deg,rgba(57,230,230,0.4),var(--cyan));
    box-shadow:0 0 10px var(--cyan);
    animation:loadBar 1.9s cubic-bezier(0.4,0,0.2,1) 2.35s forwards;
  }
  @keyframes loadBar{from{width:0;}to{width:100%;}}

  /* ===== APP WRAPPER ===== */
  #app{
    position:relative;z-index:2;
    display:flex;align-items:center;justify-content:center;
    width:100%;height:100%;
    opacity:0;transition:opacity 0.6s ease;
  }
  #app.show{opacity:1;}

  /* ===== PAGES ===== */
  .page{
    display:none;width:330px;
    background:rgba(13,18,32,0.82);
    border:1px solid var(--panel-border);
    border-radius:18px;padding:34px 26px;
    text-align:center;position:relative;
    box-shadow:0 0 40px rgba(57,230,230,0.08),0 0 80px rgba(80,20,160,0.15),inset 0 0 30px rgba(57,230,230,0.03);
    backdrop-filter:blur(16px);
    animation:smoothFade 0.45s cubic-bezier(0.34,1.56,0.64,1) forwards;
  }
  .page.active{display:block;}
  @keyframes smoothFade{from{opacity:0;transform:scale(0.95) translateY(14px);filter:blur(4px);}to{opacity:1;transform:scale(1) translateY(0);filter:blur(0);}}

  .crown-badge{position:absolute;top:-18px;left:50%;transform:translateX(-50%);font-size:26px;filter:drop-shadow(0 0 8px var(--gold));animation:crownFloat 3s ease-in-out infinite;}
  @keyframes crownFloat{0%,100%{transform:translateX(-50%) translateY(0);}50%{transform:translateX(-50%) translateY(-5px);}}

  .brand{font-size:11px;letter-spacing:3px;color:var(--text-dim);text-transform:uppercase;margin-bottom:6px;margin-top:8px;}
  h1{font-size:22px;letter-spacing:1px;color:var(--cyan);margin-bottom:24px;text-transform:uppercase;text-shadow:0 0 20px rgba(57,230,230,0.35);}

  .btn{width:100%;padding:13px;border-radius:10px;background:transparent;color:var(--cyan);border:1.5px solid var(--cyan);font-weight:600;font-size:14px;letter-spacing:.5px;cursor:pointer;text-transform:uppercase;transition:all 0.25s ease;}
  .btn:hover{background:rgba(57,230,230,0.12);box-shadow:0 0 20px rgba(57,230,230,0.25);}
  .btn:active{transform:scale(0.97);}

  .hint{margin-top:14px;font-size:12px;color:var(--text-dim);}
  .blink{animation:blink 2s ease-in-out infinite;}
  @keyframes blink{50%{opacity:.2;}}

  .icon-wrap{position:relative;width:84px;height:84px;margin:0 auto 20px;display:flex;align-items:center;justify-content:center;}
  .icon-ring{position:absolute;inset:0;border:1.5px solid var(--cyan);border-radius:50%;opacity:.35;animation:pulseRing 2.6s ease infinite;}
  .icon-ring.delay{animation-delay:1.3s;}
  @keyframes pulseRing{0%{transform:scale(.7);opacity:.5;}100%{transform:scale(1.35);opacity:0;}}
  .icon-core{position:relative;z-index:1;width:54px;height:54px;border-radius:50%;background:rgba(13,18,32,0.9);border:1.5px solid var(--cyan);display:flex;align-items:center;justify-content:center;box-shadow:0 0 22px rgba(57,230,230,0.2);}
  .icon-core svg{width:24px;height:24px;}
  .tagline{font-size:12.5px;color:var(--text-dim);line-height:1.6;margin:-12px 0 22px;}

  .input-key{width:100%;padding:13px;margin-bottom:14px;background:rgba(57,230,230,0.04);color:var(--text);border:1.5px solid rgba(57,230,230,0.2);border-radius:10px;text-align:center;font-size:15px;outline:none;transition:all 0.25s ease;}
  .input-key:focus{border-color:var(--cyan);box-shadow:0 0 14px rgba(57,230,230,0.18);}
  .error{color:var(--danger);font-size:12px;margin-top:10px;display:none;}

  .setting-row{display:flex;justify-content:space-between;align-items:center;background:rgba(57,230,230,0.04);border:1px solid rgba(57,230,230,0.1);border-radius:10px;padding:11px 14px;margin-bottom:9px;}
  .setting-name{font-size:13.5px;font-weight:600;display:flex;align-items:center;gap:7px;}

  .toggle{width:44px;height:24px;border-radius:12px;background:rgba(255,255,255,0.1);position:relative;cursor:pointer;transition:background-color 0.3s ease,transform 0.1s ease;flex-shrink:0;border:1px solid rgba(57,230,230,0.15);}
  .toggle.on{background:var(--cyan);}
  .toggle:active{transform:scale(0.92);}
  .toggle .knob{width:18px;height:18px;border-radius:50%;background:#fff;position:absolute;top:2px;left:2px;transition:left 0.3s cubic-bezier(0.34,1.56,0.64,1);box-shadow:0 1px 4px rgba(0,0,0,0.4);}
  .toggle.on .knob{left:22px;}

  .back-link{display:inline-block;margin-top:14px;font-size:12px;color:var(--text-dim);cursor:pointer;transition:color 0.2s;}
  .back-link:hover{color:var(--cyan);}

  /* ===== CODE MODAL ===== */
  .modal-overlay{position:fixed;inset:0;z-index:999;background:rgba(2,4,8,0.88);backdrop-filter:blur(8px);display:flex;align-items:center;justify-content:center;animation:fadeIn 0.25s ease;}
  @keyframes fadeIn{from{opacity:0;}to{opacity:1;}}
  .modal-box{width:340px;max-width:92vw;background:rgba(10,14,28,0.96);border-radius:16px;border:1px solid rgba(57,230,230,0.25);box-shadow:0 0 50px rgba(57,230,230,0.1),0 0 100px rgba(80,20,160,0.2);overflow:hidden;display:flex;flex-direction:column;animation:modalPop 0.35s cubic-bezier(0.34,1.56,0.64,1);}
  @keyframes modalPop{from{transform:scale(0.85);opacity:0;}to{transform:scale(1);opacity:1;}}
  .modal-header{padding:14px 18px 12px;border-bottom:1px solid rgba(57,230,230,0.12);display:flex;align-items:center;gap:10px;}
  .modal-title-icon{font-size:20px;}
  .modal-title-text{font-size:13px;font-weight:700;letter-spacing:0.5px;color:var(--cyan);}
  .modal-status-badge{margin-left:auto;font-size:11px;font-weight:600;padding:3px 10px;border-radius:20px;letter-spacing:0.5px;}
  .badge-on{background:rgba(77,255,145,0.15);color:#4dff91;border:1px solid rgba(77,255,145,0.3);}
  .badge-off{background:rgba(255,107,107,0.15);color:#ff6b6b;border:1px solid rgba(255,107,107,0.3);}
  .modal-code-area{height:200px;overflow:hidden;position:relative;background:rgba(0,0,0,0.3);}
  .modal-code-area::before,.modal-code-area::after{content:'';position:absolute;left:0;right:0;height:40px;z-index:2;pointer-events:none;}
  .modal-code-area::before{top:0;background:linear-gradient(to bottom,rgba(10,14,28,0.95),transparent);}
  .modal-code-area::after{bottom:0;background:linear-gradient(to top,rgba(10,14,28,0.95),transparent);}
  .code-scroll-inner{position:absolute;bottom:0;left:0;right:0;padding:10px 14px;font-family:'Courier New',monospace;font-size:11.5px;line-height:1.85;white-space:pre-wrap;word-break:break-all;}
  .modal-footer{padding:14px 18px;border-top:1px solid rgba(57,230,230,0.12);display:flex;align-items:center;justify-content:center;gap:10px;opacity:0;transition:opacity 0.5s ease;min-height:54px;}
  .modal-footer.show{opacity:1;}
  .footer-icon{font-size:22px;animation:popIn 0.5s cubic-bezier(0.34,1.56,0.64,1);}
  .footer-msg{font-size:13px;font-weight:600;letter-spacing:0.5px;}
  @keyframes popIn{from{transform:scale(0);opacity:0;}to{transform:scale(1);opacity:1;}}
  @keyframes shake{0%,100%{transform:translateX(0);}20%{transform:translateX(-8px);}40%{transform:translateX(8px);}60%{transform:translateX(-5px);}80%{transform:translateX(5px);}}
</style>
</head>
<body>

<!-- Galaxy bg -->
<canvas id="galaxy"></canvas>
<div class="nebula nebula1"></div>
<div class="nebula nebula2"></div>
<div class="nebula nebula3"></div>
<div class="star-shoot" style="top:10%;left:20%;animation-duration:6s;animation-delay:0s;"></div>
<div class="star-shoot" style="top:30%;left:60%;animation-duration:8s;animation-delay:2.5s;"></div>
<div class="star-shoot" style="top:60%;left:10%;animation-duration:7s;animation-delay:5s;"></div>
<div class="star-shoot" style="top:5%;left:80%;animation-duration:5s;animation-delay:1.5s;"></div>
<div class="star-shoot" style="top:80%;left:50%;animation-duration:9s;animation-delay:4s;"></div>
<canvas id="snow"></canvas>
<canvas id="petals"></canvas>

<!-- ===== INTRO ===== -->
<div id="intro">
  <div class="intro-ring-orbit" id="ringOrbit"></div>

  <div class="intro-crown-wrap">
    <div class="intro-crown">👑</div>
  </div>

  <div class="intro-title-wrap">
    <div class="intro-title">NMINH LOCK</div>
  </div>
  <div class="intro-sub">Hệ thống bảo mật</div>

  <div class="intro-bar-wrap">
    <div class="intro-bar"></div>
  </div>
  <div class="intro-status">
    <span class="dot"></span>
    <span class="intro-status-text">
      <span>Đang xác thực thiết bị...</span>
      <span>Đang thiết lập kết nối an toàn...</span>
      <span>Sẵn sàng</span>
    </span>
  </div>
</div>

<!-- ===== APP ===== -->
<div id="app">

<!-- PAGE 1 -->
<div id="page1" class="page active">
  <div class="crown-badge">👑</div>
  <div class="brand">App by Nminh</div>
  <div class="icon-wrap">
    <div class="icon-ring"></div><div class="icon-ring delay"></div>
    <div class="icon-core">
      <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" style="color:var(--cyan)">
        <rect x="4" y="11" width="16" height="9" rx="2"/><path d="M8 11V7a4 4 0 0 1 8 0v4"/>
      </svg>
    </div>
  </div>
  <h1>Nminh Lock</h1>
  <div class="tagline">Khóa truy cập an toàn cho thiết bị của bạn</div>
  <button class="btn" onclick="goTo('page2')">Bấm vào để kích hoạt</button>
  <div class="hint blink">✦ Hệ thống đang chờ lệnh... ✦</div>
</div>

<!-- PAGE 2 -->
<div id="page2" class="page">
  <div class="crown-badge">👑</div>
  <div class="brand">Xác thực</div>
  <h1>Nhập Key</h1>
  <input type="text" id="keyInput" class="input-key" placeholder="Nhập key tại đây...">
  <button class="btn" onclick="checkKey()">Xác Nhận</button>
  <div id="errorMsg" class="error">❌ Key không hợp lệ. Vui lòng thử lại!</div>
</div>

<!-- PAGE 3 -->
<div id="page3" class="page">
  <div class="crown-badge">👑</div>
  <div class="brand">Bảng điều khiển</div>
  <h1>Nminh Lock</h1>
  <div class="setting-row">
    <span class="setting-name">🌙 Chế Độ Tối</span>
    <div class="toggle on" id="themeToggle" onclick="handleToggle(this,'Chế Độ Tối','theme')"><div class="knob"></div></div>
  </div>
  <div class="setting-row">
    <span class="setting-name">🍃 Nhẹ Tâm</span>
    <div class="toggle" onclick="handleToggle(this,'Nhẹ Tâm','relax')"><div class="knob"></div></div>
  </div>
  <div class="setting-row">
    <span class="setting-name">📉 Giảm FPS</span>
    <div class="toggle" onclick="handleToggle(this,'Giảm FPS','fps')"><div class="knob"></div></div>
  </div>
  <div class="setting-row">
    <span class="setting-name">⚙️ Tối Ưu Máy</span>
    <div class="toggle" onclick="handleToggle(this,'Tối Ưu Máy','optimize')"><div class="knob"></div></div>
  </div>
  <div class="setting-row">
    <span class="setting-name">🎯 Tăng Nhạy</span>
    <div class="toggle" onclick="handleToggle(this,'Tăng Nhạy','sens')"><div class="knob"></div></div>
  </div>
  <div class="setting-row">
    <span class="setting-name">📳 Fix Rung</span>
    <div class="toggle" onclick="handleToggle(this,'Fix Rung','vibration')"><div class="knob"></div></div>
  </div>
  <div class="setting-row">
    <span class="setting-name">🖱️ Bật DPI</span>
    <div class="toggle" onclick="handleToggle(this,'Bật DPI','dpi')"><div class="knob"></div></div>
  </div>
  <div style="margin-top:10px;font-size:11px;color:var(--text-dim)">Slot đã dùng: <span id="slotCount">-- / 200</span></div>
  <span class="back-link" onclick="goTo('page1')">↩ Đăng xuất</span>
</div>

<!-- PAGE FULL -->
<div id="pageFull" class="page">
  <div class="crown-badge">👑</div>
  <div class="brand">Thông báo hệ thống</div>
  <div class="icon-wrap">
    <div class="icon-ring"></div><div class="icon-ring delay"></div>
    <div class="icon-core">
      <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" style="color:var(--danger)">
        <circle cx="12" cy="12" r="10"/><line x1="12" y1="8" x2="12" y2="12"/><line x1="12" y1="16" x2="12.01" y2="16"/>
      </svg>
    </div>
  </div>
  <h1 style="color:var(--danger)">Hết Slot</h1>
  <div class="tagline">Hệ thống đã đạt giới hạn <strong style="color:var(--cyan)">200 người dùng</strong>.<br>Vui lòng liên hệ admin để mở thêm.</div>
  <span class="back-link" onclick="goTo('page1')">← Quay lại</span>
</div>

</div><!-- end #app -->

<script>
/* ===== CONFIG — ĐỔI KEY Ở ĐÂY ===== */
const CORRECT_KEY = "nminh-key";
const MAX_USERS   = 200;

/* ===== SLOT ===== */
const STORAGE_KEY="nminh_lock_slots", MY_SLOT_KEY="nminh_lock_my_slot";
function getSlots(){try{return JSON.parse(localStorage.getItem(STORAGE_KEY)||'[]');}catch{return[];}}
function saveSlots(a){localStorage.setItem(STORAGE_KEY,JSON.stringify(a));}
function claimSlot(){
  const slots=getSlots(),my=localStorage.getItem(MY_SLOT_KEY);
  if(my&&slots.includes(my)) return true;
  if(slots.length>=MAX_USERS) return false;
  const id='u_'+Date.now()+'_'+Math.random().toString(36).slice(2,7);
  slots.push(id);saveSlots(slots);localStorage.setItem(MY_SLOT_KEY,id);return true;
}
function slotsUsed(){return getSlots().length;}

/* ===== INTRO ===== */
// Tạo các đốm sáng nhỏ chạy quanh viền vòng bảo mật + tia sáng bung ra từ vương miện
(function buildIntroFx(){
  const orbit=document.getElementById('ringOrbit');
  const R=130;
  for(let i=0;i<5;i++){
    const tick=document.createElement('div');
    tick.className='intro-ring-tick';
    const angle=(i/5)*Math.PI*2 - Math.PI/2;
    const x=130+R*Math.cos(angle), y=130+R*Math.sin(angle);
    tick.style.left=x+'px';tick.style.top=y+'px';
    tick.style.animationDelay=(0.3+i*0.32)+'s';
    orbit.appendChild(tick);
  }
  const crownWrap=document.querySelector('.intro-crown-wrap');
  for(let i=0;i<8;i++){
    const spark=document.createElement('div');
    spark.className='crown-spark';
    const angle=(i/8)*Math.PI*2;
    spark.style.left='50%';spark.style.top='50%';
    spark.style.setProperty('--dx',(Math.cos(angle)*34)+'px');
    spark.style.setProperty('--dy',(Math.sin(angle)*34)+'px');
    spark.style.animation='sparkOut .55s ease-out '+(0.45+Math.random()*0.1)+'s forwards';
    spark.style.transform='translate(-50%,-50%)';
    crownWrap.appendChild(spark);
  }
})();
</script>
<style>
  @keyframes sparkOut{
    0%{opacity:1;transform:translate(-50%,-50%) translate(0,0) scale(1);}
    100%{opacity:0;transform:translate(-50%,-50%) translate(var(--dx,20px),var(--dy,20px)) scale(0);}
  }
  @keyframes tickPop{0%{opacity:0;transform:scale(0);}40%{opacity:1;transform:scale(1.4);}100%{opacity:0;transform:scale(.6);}}
</style>
<script>
// Intro tự biến mất sau 3.4 giây — nhanh, dứt khoát, không kéo dài
window.addEventListener('load',()=>{
  setTimeout(()=>{
    const intro=document.getElementById('intro');
    const app=document.getElementById('app');
    intro.classList.add('hide');
    app.classList.add('show');
    setTimeout(()=>{ intro.style.display='none'; }, 900);
  }, 3400);
});

/* ===== NAV ===== */
function goTo(id){
  document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
  const el=document.getElementById(id);
  el.style.animation='none';void el.offsetWidth;el.style.animation='';
  el.classList.add('active');
  if(id==='page2') setTimeout(()=>document.getElementById('keyInput').focus(),60);
  if(id==='page3') document.getElementById('slotCount').textContent=slotsUsed()+' / '+MAX_USERS;
}

/* ===== AUTH ===== */
function checkKey(){
  const val=document.getElementById('keyInput').value.trim();
  const err=document.getElementById('errorMsg');
  if(val===CORRECT_KEY){
    if(!claimSlot()){err.style.display='none';document.getElementById('keyInput').value='';goTo('pageFull');return;}
    err.style.display='none';document.getElementById('keyInput').value='';goTo('page3');
  } else {
    err.style.display='block';
    const inp=document.getElementById('keyInput');
    inp.style.animation='none';void inp.offsetWidth;inp.style.animation='shake 0.4s ease';
  }
}
document.getElementById('keyInput').addEventListener('keypress',e=>{if(e.key==='Enter'){e.preventDefault();checkKey();}});

/* ===== TOGGLE CONFIG ===== */
const TOGGLE_CONFIG={
  theme:{color:'#c8a0ff',icon:'🌙',offIcon:'☀️',lines:['[THEME] Khởi tạo engine chủ đề...','[GPU]   Tải shader bảng màu tối: depth_blur=3.2px','[CSS]   Áp dụng biến --bg=#020408 --panel=#0d1220','[LAYER] Thiết lập nebula opacity=0.35 blend=screen','[FONT]  antialiasing=lcd subpixel=off hinting=auto','[SYNC]  GPU vsync=true refresh=144hz framebuffer=swap','[CACHE] Ghi theme → key="nminh_dark_v4" scope=session','[DONE]  Chủ đề tối đã được áp dụng thành công ✓']},
  relax:{color:'#7fffb0',icon:'🍃',offIcon:'⚡',lines:['[INIT]  Khởi động module Nhẹ Tâm...','[NEURO] Điều chỉnh sóng não: freq=0.5Hz amplitude=low','[ALERT] Tắt thông báo ưu tiên: queue=clear mode=silent','[SYNC]  Đồng bộ hơi thở: inhale=4s hold=4s exhale=6s','[BIO]   Chặn cortisol threshold=auto HRV_sensor=active','[AUDIO] Tải âm thanh môi trường: rain+pink_noise vol=28%','[LIGHT] Bộ lọc ánh sáng xanh: temp=3200K strength=80%','[DONE]  Chế độ Nhẹ Tâm đã kích hoạt thành công ✓']},
  fps:{color:'#ffdd55',icon:'📉',offIcon:'🔥',lines:['[INIT]  Khởi động bộ giới hạn FPS...','[DISP]  Đặt giới hạn: cap=30fps vsync=adaptive','[REND]  Giảm độ phân giải: scale=0.75x DLSS=quality','[LOD]   Điều chỉnh chi tiết: near=80 far=200 shadow=512','[PART]  Giới hạn particle: max=256 physics_hz=20Hz','[CULL]  Bật tối ưu render: frustum=on occlusion=on','[TEMP]  Giám sát nhiệt độ: max=72°C fan=aggressive','[DONE]  Chế độ Giảm FPS đã áp dụng thành công ✓']},
  optimize:{color:'#55ccff',icon:'⚙️',offIcon:'🛑',lines:['[INIT]  Bắt đầu quét tiến trình hệ thống...','[PROC]  Dọn tiến trình zombie: 14 đã tắt idle=trimmed','[MEM]   Defrag bộ nhớ: huge_pages=on swap=zstd 4096MB','[CPU]   Ghim CPU: isolcpus=2,3 nohz_full=on rcu=enabled','[CACHE] Xả cache: L1=clean L2=clean L3=warm TLB=flush','[IO]    Tối ưu ổ đĩa: mq-deadline queue=64 ncq=on','[NET]   Tinh chỉnh mạng: tcp_bbr=on rmem=16MB wmem=16MB','[DONE]  Tối Ưu Máy hoàn tất thành công ✓']},
  sens:{color:'#ff9966',icon:'🎯',offIcon:'🔕',lines:['[INIT]  Khởi động module tăng độ nhạy...','[INPUT] Đặt tốc độ poll: rate=8000Hz latency=0.125ms','[RAW]   Kích hoạt raw input: bypass=true accel=false','[DPI]   Áp dụng profile: 800dpi step=50 snap=disabled','[USB]   Ưu tiên USB IRQ: priority=99 affinity=cpu0','[HID]   Bộ lọc HID: driver=hidraw buffer=1 mode=direct','[CLICK] Debounce=0ms pre_travel=0.2mm actuation=47g','[DONE]  Tăng Nhạy đã kích hoạt thành công ✓']},
  vibration:{color:'#ff80c0',icon:'📳',offIcon:'🔔',lines:['[INIT]  Khởi động module Fix Rung...','[HAL]   Kết nối HAL haptic: driver=ff_memless override=on','[MOTOR] Tắt motor rung: duty_cycle=0% carrier=200Hz','[FF]    Chặn force feedback: rumble=off periodic=off','[PAD]   Tắt rung tay cầm: left=0x00 right=0x00 trim=0','[TOUCH] Vô hiệu hóa phản hồi cảm ứng: amplitude=0','[SYS]   Ghi đè pattern rung hệ thống: pattern=null','[DONE]  Fix Rung đã áp dụng thành công ✓']},
  dpi:{color:'#80d8ff',icon:'🖱️',offIcon:'🖥️',lines:['[INIT]  Khởi động DPI Engine...','[DRV]   Tải driver: libinput backend=evdev mode=raw','[PTR]   Tốc độ con trỏ: scale=1.0x accel_profile=flat','[DPI1]  Stage 1 → 800dpi  sens=1.000 LED=#ff0000','[DPI2]  Stage 2 → 1200dpi sens=1.000 LED=#00ff00','[DPI3]  Stage 3 → 1600dpi sens=1.000 LED=#0000ff','[DPI4]  Stage 4 → 3200dpi sens=1.000 LED=#ffffff','[DONE]  DPI đã bật và cấu hình thành công ✓']},
};

/* ===== TOGGLE ===== */
let effectRunning=false;
function handleToggle(el,name,type){
  if(effectRunning) return;
  el.classList.toggle('on');
  showCodeModal(name,el.classList.contains('on'),type);
}
function showCodeModal(name,isOn,type){
  effectRunning=true;
  const cfg=TOGGLE_CONFIG[type]||TOGGLE_CONFIG.optimize;
  const overlay=document.createElement('div'); overlay.className='modal-overlay';
  const box=document.createElement('div'); box.className='modal-box';
  const header=document.createElement('div'); header.className='modal-header';
  header.innerHTML=`<span class="modal-title-icon">${isOn?cfg.icon:cfg.offIcon}</span><span class="modal-title-text">Đang ${isOn?'bật':'tắt'}: ${name}</span><span class="modal-status-badge ${isOn?'badge-on':'badge-off'}">${isOn?'● ĐANG BẬT':'○ ĐANG TẮT'}</span>`;
  const codeArea=document.createElement('div'); codeArea.className='modal-code-area';
  const codeInner=document.createElement('div'); codeInner.className='code-scroll-inner';
  codeInner.style.color=cfg.color;
  codeInner.style.transform='translateY(100%)';
  codeInner.style.transition='none';
  codeInner.textContent=cfg.lines.map((l,i)=>`[+${String(i*200).padStart(4,'0')}ms] ${l}`).join('\n');
  codeArea.appendChild(codeInner);
  const footer=document.createElement('div'); footer.className='modal-footer';
  footer.innerHTML=`<span class="footer-icon">${isOn?'✅':'❌'}</span><span class="footer-msg" style="color:${isOn?'#4dff91':'#ff6b6b'}">${isOn?'Bật thành công!':'Đã tắt!'} — ${name}</span>`;
  box.appendChild(header);box.appendChild(codeArea);box.appendChild(footer);
  overlay.appendChild(box);document.body.appendChild(overlay);
  requestAnimationFrame(()=>requestAnimationFrame(()=>{
    const endY=Math.min(0,(codeArea.clientHeight||200)-codeInner.scrollHeight-20);
    codeInner.style.transition='transform 2s linear';
    codeInner.style.transform=`translateY(${endY}px)`;
  }));
  setTimeout(()=>footer.classList.add('show'),2050);
  setTimeout(()=>{
    overlay.style.transition='opacity 0.35s ease';overlay.style.opacity='0';
    setTimeout(()=>{overlay.remove();effectRunning=false;},350);
  },3500);
}

/* ===== GALAXY ===== */
const gC=document.getElementById('galaxy'),gCtx=gC.getContext('2d');
let gW,gH,stars=[];
function resizeAll(){
  gW=gC.width=window.innerWidth;gH=gC.height=window.innerHeight;
  document.getElementById('snow').width=gW;document.getElementById('snow').height=gH;
  pC.width=gW;pC.height=gH;
}
window.addEventListener('resize',()=>{resizeAll();makeStars(220);});
function makeStars(n){stars=[];for(let i=0;i<n;i++)stars.push({x:Math.random()*gW,y:Math.random()*gH,r:Math.random()*1.2+0.2,op:Math.random()*0.8+0.2,ts:Math.random()*0.02+0.005,to:Math.random()*Math.PI*2,c:['#fff','#adf','#ffe','#ccf'][Math.floor(Math.random()*4)]});}
let gT=0;
function drawGalaxy(){gCtx.clearRect(0,0,gW,gH);gT+=0.016;stars.forEach(s=>{const tw=0.5+0.5*Math.sin(gT*s.ts*60+s.to);gCtx.globalAlpha=s.op*tw;gCtx.fillStyle=s.c;gCtx.beginPath();gCtx.arc(s.x,s.y,s.r,0,Math.PI*2);gCtx.fill();});gCtx.globalAlpha=1;requestAnimationFrame(drawGalaxy);}

/* ===== SNOW ===== */
const sC=document.getElementById('snow'),sCtx=sC.getContext('2d');let flakes=[];
function makeSnow(){flakes=[];for(let i=0;i<40;i++)flakes.push({x:Math.random()*gW,y:Math.random()*gH,r:Math.random()*1.4+0.4,sp:Math.random()*0.4+0.2,d:Math.random()*10,op:Math.random()*0.25+0.1});}
function drawSnow(){sCtx.clearRect(0,0,gW,gH);sCtx.fillStyle='#fff';flakes.forEach(f=>{sCtx.globalAlpha=f.op;sCtx.beginPath();sCtx.arc(f.x,f.y,f.r,0,Math.PI*2);sCtx.fill();f.y+=f.sp;f.x+=Math.sin(f.d)*0.2;f.d+=0.01;if(f.y>gH){f.y=-5;f.x=Math.random()*gW;}if(f.x>gW)f.x=0;if(f.x<0)f.x=gW;});sCtx.globalAlpha=1;requestAnimationFrame(drawSnow);}

/* ===== PETALS ===== */
const pC=document.getElementById('petals'),pCtx=pC.getContext('2d');let petals=[];
const PC=['rgba(255,182,193,0.7)','rgba(255,153,168,0.6)','rgba(255,200,210,0.65)','rgba(255,220,228,0.55)'];
function mkP(){return{x:Math.random()*gW,y:-20,s:Math.random()*6+4,sy:Math.random()*1+0.4,sx:Math.random()*0.6-0.3,r:Math.random()*Math.PI*2,rs:(Math.random()-0.5)*0.035,sw:Math.random()*2+1,so:Math.random()*Math.PI*2,c:PC[Math.floor(Math.random()*PC.length)],op:Math.random()*0.5+0.35};}
function initPetals(n){petals=[];for(let i=0;i<n;i++){const p=mkP();p.y=Math.random()*gH;petals.push(p);}}
let pT=0;
function drawPetals(){pCtx.clearRect(0,0,gW,gH);pT++;if(pT%20===0&&petals.length<45)petals.push(mkP());petals.forEach((p,i)=>{p.y+=p.sy;p.x+=p.sx+Math.sin(pT*0.015+p.so)*p.sw*0.035;p.r+=p.rs;pCtx.save();pCtx.translate(p.x,p.y);pCtx.rotate(p.r);pCtx.globalAlpha=p.op;pCtx.fillStyle=p.c;for(let k=0;k<5;k++){pCtx.save();pCtx.rotate((k/5)*Math.PI*2);pCtx.beginPath();pCtx.ellipse(0,-p.s*0.55,p.s*0.3,p.s*0.65,0,0,Math.PI*2);pCtx.fill();pCtx.restore();}pCtx.restore();if(p.y>gH+20||p.x<-30||p.x>gW+30)petals[i]=mkP();});requestAnimationFrame(drawPetals);}

/* ===== INIT ===== */
resizeAll();makeStars(220);makeSnow();initPetals(18);
drawGalaxy();drawSnow();drawPetals();
</script>
</body>
</html>
