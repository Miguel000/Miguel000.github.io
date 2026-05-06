---
layout: default
title: Miguel Hernández
---

<style>
.mh-tagline { color: #888; font-size: 14px; margin: 4px 0 0; }

.mh-nav {
  display: flex;
  gap: 0;
  margin: 22px 0 0;
  border-bottom: 1px solid #2a2a2a;
}
.mh-tab {
  background: none;
  border: none;
  border-bottom: 2px solid transparent;
  color: #666;
  cursor: pointer;
  font-family: Monaco, "Bitstream Vera Sans Mono", monospace;
  font-size: 13px;
  padding: 7px 18px 7px 0;
  margin-bottom: -1px;
  margin-right: 14px;
  transition: color .15s;
}
.mh-tab:hover { color: #bbb; }
.mh-tab.active { color: #9dbc98; border-bottom-color: #9dbc98; }

.mh-pane { display: none; padding-top: 16px; }
.mh-pane.active { display: block; }

/* ── Filter bars (shared by Talks + Blog) ── */
.mh-filters {
  display: flex;
  flex-wrap: wrap;
  gap: 6px;
  margin-bottom: 20px;
}
.mh-fbtn {
  background: none;
  border: 1px solid #2a2a2a;
  color: #666;
  cursor: pointer;
  font-family: Monaco, "Bitstream Vera Sans Mono", monospace;
  font-size: 12px;
  padding: 3px 10px;
  border-radius: 2px;
  transition: all .15s;
}
.mh-fbtn:hover { border-color: #555; color: #bbb; }
.mh-fbtn.active { border-color: #9dbc98; color: #9dbc98; }
.mh-fcount { color: #444; }

/* ── Talk list ── */
.mh-year-group { margin-bottom: 26px; }
.mh-group-heading {
  font-size: 11px;
  color: #444;
  text-transform: uppercase;
  letter-spacing: 3px;
  margin: 0 0 10px;
  padding-bottom: 5px;
  border-bottom: 1px solid #1e1e1e;
}
.mh-talk {
  padding: 8px 0 8px 14px;
  border-left: 2px solid #1e1e1e;
  margin: 5px 0;
  transition: border-color .15s;
}
.mh-talk:hover { border-left-color: #9dbc98; }
.mh-conf { color: #ddd; font-size: 13px; font-weight: bold; }
.mh-loc { color: #444; font-size: 12px; margin-left: 6px; font-weight: normal; }
.mh-title { color: #888; font-size: 13px; margin: 3px 0 4px; font-style: italic; }
.mh-row-links { display: flex; flex-wrap: wrap; gap: 10px; }
.mh-link { color: #63c0f5; font-size: 12px; text-decoration: none; }
.mh-link:hover { text-decoration: underline; }
.mh-badge {
  display: inline-block;
  font-size: 10px;
  padding: 1px 6px;
  border-radius: 2px;
  border: 1px solid;
  vertical-align: middle;
  margin-left: 6px;
}
.mh-badge-ws { color: #d29922; border-color: #5a3e00; background: #1a1200; }

/* ── Blog list ── */
.mh-blog-group { margin-bottom: 26px; }
.mh-blog-entry {
  padding: 8px 0 8px 14px;
  border-left: 2px solid #1e1e1e;
  margin: 5px 0;
  transition: border-color .15s;
}
.mh-blog-entry:hover { border-left-color: #63c0f5; }
.mh-blog-title { font-size: 13px; }
.mh-blog-title a { color: #63c0f5; text-decoration: none; }
.mh-blog-title a:hover { text-decoration: underline; }
.mh-blog-source {
  display: inline-block;
  font-size: 10px;
  color: #555;
  border: 1px solid #2a2a2a;
  border-radius: 2px;
  padding: 1px 6px;
  margin-left: 8px;
  vertical-align: middle;
}
.mh-blog-desc { color: #666; font-size: 12px; margin-top: 3px; }

/* ── OSS list ── */
.mh-oss-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 12px;
  padding-top: 4px;
}
.mh-oss-card {
  border: 1px solid #1e1e1e;
  border-radius: 4px;
  padding: 14px;
  transition: border-color .15s;
}
.mh-oss-card:hover { border-color: #9dbc98; }
.mh-oss-name { font-size: 14px; font-weight: bold; }
.mh-oss-name a { color: #9dbc98; text-decoration: none; }
.mh-oss-name a:hover { text-decoration: underline; }
.mh-oss-role {
  display: inline-block;
  font-size: 10px;
  color: #888;
  border: 1px solid #2a2a2a;
  border-radius: 2px;
  padding: 1px 6px;
  margin-left: 8px;
  vertical-align: middle;
}
.mh-oss-desc { color: #666; font-size: 12px; margin-top: 8px; line-height: 1.5; }

/* ── About ── */
.mh-about-links { list-style: none; padding: 0; margin: 12px 0 20px; }
.mh-about-links li { margin: 8px 0; font-size: 13px; }
.mh-about-links a { color: #63c0f5; }
.mh-about-section { margin-bottom: 20px; }
.mh-about-section h3 { font-size: 11px; text-transform: uppercase; letter-spacing: 2px; color: #444; margin: 0 0 10px; padding-bottom: 5px; border-bottom: 1px solid #1e1e1e; }
</style>

# Miguel Hernández

<p class="mh-tagline">Sr. Threat Research Engineer · Sysdig · Security researcher &amp; conference speaker</p>

<div class="mh-nav">
  <button class="mh-tab active" data-target="mh-talks">Talks</button>
  <button class="mh-tab" data-target="mh-blog">Blog</button>
  <button class="mh-tab" data-target="mh-oss">Open Source</button>
  <button class="mh-tab" data-target="mh-about">About</button>
</div>

<!-- ══════════════ TALKS ══════════════ -->
<div id="mh-talks" class="mh-pane active">
  <div class="mh-filters" id="mh-years"></div>
  <div id="mh-talk-list"></div>
</div>

<!-- ══════════════ BLOG ══════════════ -->
<div id="mh-blog" class="mh-pane">
  <div class="mh-filters" id="mh-platforms"></div>
  <div id="mh-blog-list"></div>
</div>

<!-- ══════════════ OPEN SOURCE ══════════════ -->
<div id="mh-oss" class="mh-pane">
  <div class="mh-oss-grid" id="mh-oss-grid"></div>
</div>

<!-- ══════════════ ABOUT ══════════════ -->
<div id="mh-about" class="mh-pane">

<div class="mh-about-section">
<h3>Contact</h3>
<ul class="mh-about-links">
  <li>📫 <a href="mailto:miguelhernandez2907@gmail.com">miguelhernandez2907@gmail.com</a></li>
  <li><a href="https://github.com/Miguel000">github.com/Miguel000</a></li>
</ul>
</div>

<div class="mh-about-section">
<h3>Repositories</h3>
<ul class="mh-about-links">
  <li><a href="https://github.com/Miguel000/MySecTalks">MySecTalks</a> — talk slides, recordings, and abstracts</li>
  <li><a href="https://github.com/Miguel000/BlogContent">BlogContent</a> — research posts and write-ups</li>
  <li><a href="https://github.com/Miguel000/OpenSourceTools">OpenSourceTools</a> — cybersecurity tools and contributions</li>
</ul>
</div>

<div class="mh-about-section">
<h3>Bio</h3>
<p style="color:#888;font-size:13px;line-height:1.6">
Miguel Hernández is a Sr. Threat Research Engineer at Sysdig with over a decade of experience in security research. He has spoken at major cybersecurity conferences across Europe including HITB, HackLu, DeepSec, RootedCon, and fwd:CloudSec EU. His research spans cloud-native threats, runtime detection with Falco, supply chain security, adversarial AI, and emerging threat intelligence.
</p>
</div>

</div>

<script>
/* ─── DATA ─── */
var TALKS = [
  {y:2026, conf:"T3chfest", loc:"Getafe, ES", title:"De Worms a typosquatting: ¿Qué ocurre con npm?"},
  {y:2025, conf:"fwd:CloudSec EU", loc:"London, UK", title:"Cloud Abuse at Scale: How Cybercriminals Exploit Free Tiers for Profit", video:"https://youtu.be/-a9Ts7AWT7I?t=4875"},
  {y:2025, conf:"DFeX 2025", loc:"", title:"From Research to Security: Real-World Threats and the Evolving Challenge of Detection"},
  {y:2025, conf:"Tardes de Ciberseguridad", loc:"", title:"Día a día de un investigador de ciberseguridad en Sysdig"},
  {y:2025, conf:"DevOps Zaragoza", loc:"Zaragoza, ES", title:"Robo de credenciales y el negocio del roleplay NSFW"},
  {y:2024, conf:"DeepSec", loc:"Vienna, AT", title:"Navigating the Storm: Emerging Threats in AWS Cloud Security"},
  {y:2024, conf:"HackLu", loc:"Luxembourg", title:"Insights from Modern Botnets"},
  {y:2024, conf:"DevOps Barcelona", loc:"Barcelona, ES", title:"Fortifying DevOps: Understanding and Fighting Botnet Threats", video:"https://www.youtube.com/watch?v=xD_cNBN_SbI"},
  {y:2024, conf:"KCD Austria", loc:"Vienna, AT", title:"Detecting Unexpected Behavior and Intrusions with Falco + Atomic Red Team", workshop:true},
  {y:2024, conf:"BSides Barcelona", loc:"Barcelona, ES", title:"Beyond Cryptominers: Unveiling the Depths of AWS Post-Exploitation Strategies"},
  {y:2023, conf:"HackInParis", loc:"Paris, FR", title:"Dig Deeper into OWASP Kubernetes"},
  {y:2023, conf:"RootedCon", loc:"Madrid, ES", title:"Offensive Artificial Intelligence — How to be prepared", workshop:true},
  {y:2023, conf:"KCD Spain", loc:"Spain", title:"OWASP Kubernetes", video:"https://www.youtube.com/watch?v=gJc8JIc2VvY"},
  {y:2023, conf:"SecAdmin", loc:"Spain", title:"Falco 101 — Detecting threats in real-time", workshop:true},
  {y:2023, conf:"EsLibre Zaragoza", loc:"Zaragoza, ES", title:"Introducción práctica a Runtime Security con Falco", workshop:true, video:"https://commons.wikimedia.org/wiki/File:EsLibre_2023_P46_-_Miguel_Hern%C3%A1ndez_Boza,_Vicente_J._Jim%C3%A9nez_Miras_-_Introducci%C3%B3n_pr%C3%A1ctica_a_Runtime_Security_con_Falco.webm"},
  {y:2022, conf:"KubeCon EU", loc:"Valencia, ES", title:"How Attackers Use Exposed Prometheus Server to Exploit Kubernetes Cluster", video:"https://www.youtube.com/watch?v=5cbbm_L6n7w"},
  {y:2022, conf:"DragonJar", loc:"Colombia", title:"Después de proteger la infraestructura y los datos, deberías preocuparte por tus modelos de IA", video:"https://www.youtube.com/watch?v=7uoWwFbc9g0"},
  {y:2022, conf:"KCD Spain", loc:"Spain", title:"Reforzando la seguridad de Kubernetes con gVisor y Falco", video:"https://www.youtube.com/watch?v=8N8IpToYOGM"},
  {y:2022, conf:"AllDayDevOps", loc:"Online", title:"Secure Your Prometheus Server From Indiscreet Eyes or Die by Metrics"},
  {y:2021, conf:"STIC CCN CERT", loc:"Spain", title:"Introduccion al Adversarial Machine Learning", video:"https://www.youtube.com/watch?v=jsDLt5gBnmY"},
  {y:2021, conf:"JNIC", loc:"Spain", title:"Estado del arte en generación y detección de contenido sintético. Limitaciones y oportunidades"},
  {y:2020, conf:"StandOff", loc:"Online", title:"Issues and limitations in generation and detection of synthetic data", video:"https://www.youtube.com/watch?v=SjeE2erDzFY"},
  {y:2020, conf:"Cybercamp", loc:"Spain", title:"Y se ARmo la marimorena! Seguridad en realidad aumentada", video:"https://www.youtube.com/watch?v=TJirrht7MuQ"},
  {y:2019, conf:"HITB", loc:"Amsterdam, NL", title:"DeepUnicode, problems with confusables", video:"https://www.youtube.com/watch?v=9SXRe0dWyxM"},
  {y:2019, conf:"STIC CCN CERT", loc:"Spain", title:"Protection against DeepFake"},
  {y:2019, conf:"Codemotion", loc:"Spain", title:"Blackmirror o realidad — OSINT + Face recognition"},
  {y:2019, conf:"Cybercamp", loc:"Spain", title:"DeepConfusables", video:"https://www.youtube.com/watch?v=8uVX9lEm4R0"},
  {y:2019, conf:"JNIC", loc:"Spain", title:"DeepConfusables: mejorando la detección de ataques basados en codificación Unicode"},
  {y:2019, conf:"RootedCon Valencia", loc:"Valencia, ES", title:"Playing with Mastodon for fun and profit"},
  {y:2017, conf:"Secrypt", loc:"", title:"(In) Security in Graph Databases"},
  {y:2017, conf:"Cybercamp", loc:"Spain", title:"Seguridad en redes sociales libres", video:"https://www.youtube.com/watch?v=ZfNzvBhsKIg"},
  {y:2017, conf:"JNIC", loc:"Spain", title:"Análisis de la seguridad de las bases de datos orientadas a grafos"},
  {y:2016, conf:"RootedCon", loc:"Madrid, ES", title:"(In) Security in Graph Databases", video:"https://www.youtube.com/watch?v=K0_GU8__3qw"},
  {y:2016, conf:"NoConName", loc:"Spain", title:"Seguridad en redes sociales libres"},
  {y:2016, conf:"NavajaNegra", loc:"Albacete, ES", title:"Espiando redes de microblogging"}
];

var BLOG = [
  {platform:"sysdig", src:"Sysdig Blog", title:"Attacker exploits misconfigured AI tool to run AI-generated payload", url:"https://www.sysdig.com/blog/attacker-exploits-misconfigured-ai-tool-to-run-ai-generated-payload", desc:"Accidental misconfigurations where systems like Open WebUI are exposed to the internet remain a serious problem."},
  {platform:"sysdig", src:"Sysdig Blog", title:"EMERALDWHALE: 15k Cloud credentials stolen targeting exposed Git config files", url:"https://www.sysdig.com/blog/emeraldwhale", desc:"Operation targeting exposed Git configurations resulting in more than 15,000 cloud service credentials stolen."},
  {platform:"sysdig", src:"Sysdig Blog", title:"LLMjacking targets DeepSeek", url:"http://sysdig.com/blog/llmjacking-targets-deepseek", desc:"LLMjacking proxy operators have expanded access to credentials and begun including new models like DeepSeek."},
  {platform:"sysdig", src:"Sysdig Blog", title:"The Growing Dangers of LLMjacking: Evolving Tactics and Evading Sanctions", url:"https://www.sysdig.com/blog/growing-dangers-of-llmjacking", desc:"LLMjacking describes an attacker obtaining access to an LLM illegally and reselling that access."},
  {platform:"sysdig", src:"Sysdig Blog", title:"CRYSTALRAY: Inside the Operations of a Rising Threat Actor Exploiting OSS Tools", url:"https://www.sysdig.com/blog/crystalray-rising-threat-actor-exploiting-oss-tools", desc:"CRYSTALRAY collects and sells credentials, deploys cryptominers, and maintains persistence in victim environments."},
  {platform:"sysdig", src:"Sysdig Blog", title:"DDoS-as-a-Service: The Rebirth Botnet", url:"https://www.sysdig.com/blog/ddos-as-a-service-the-rebirth-botnet", desc:"At the core of RebirthLtd's business is its DDoS botnet, rented out to whomever is willing to pay."},
  {platform:"sysdig", src:"Sysdig Blog", title:"RUBYCARP: A Detailed Analysis of a Sophisticated Decade-Old Botnet Group", url:"https://www.sysdig.com/blog/rubycarp-romanian-botnet-group", desc:"RUBYCARP is interested in cryptomining, DDoS, and phishing payloads for financial gain."},
  {platform:"sysdig", src:"Sysdig Blog", title:"SSH-Snake: New Self-Modifying Worm Threatens Networks", url:"https://sysdig.com/blog/ssh-snake/", desc:"Analysis of SSH-Snake, a self-replicating worm using SSH credentials to spread across networks."},
  {platform:"sysdig", src:"Sysdig Blog", title:"LABRAT: Stealthy Cryptojacking and Proxyjacking Campaign Targeting GitLab", url:"https://sysdig.com/blog/labrat-cryptojacking-proxyjacking-campaign/", desc:"A deep dive into a stealthy attack combining crypto- and proxyjacking targeting GitLab."},
  {platform:"sysdig", src:"Sysdig Blog", title:"Why Companies Still Struggle with Least Privilege in the Cloud", url:"https://sysdig.com/blog/identity-access-management-difficult-cloud/", desc:"Discussion on the persistent IAM challenges in cloud security."},
  {platform:"sysdig", src:"Sysdig Blog", title:"Securing SSH on EC2", url:"https://sysdig.com/blog/aws-secure-ssh-ec2-threats/", desc:"Best practices for hardening SSH access in AWS EC2 environments."},
  {platform:"bbva", src:"BBVA Next Tech", title:"Adversarial Machine Learning (Whitepaper)", url:"https://www.bbvanexttechnologies.com/wp-content/uploads/2020/11/whitepaper-adversarial-machine-learning.pdf", desc:"Techniques and threats related to adversarial ML. Co-referenced in offensive-ai-compilation."},
  {platform:"bbva", src:"BBVA Next Tech", title:"Contenido Sintético (Whitepaper)", url:"https://www.bbvanexttechnologies.com/wp-content/uploads/2020/11/whitepaper-contenido-sintetico.pdf", desc:"An overview of synthetic content and its implications for cybersecurity."},
  {platform:"media", src:"Aragón Radio", title:"Hackers vs ciberdelincuentes", url:"https://www.cartv.es/aragonradio/radio?play=podcast/104463", desc:"Discussion on the difference between hackers and cybercriminals."},
  {platform:"media", src:"Aragón Radio", title:"Ciberseguridad en verano", url:"https://www.cartv.es/aragonradio/radio?play=podcast/108338", desc:"How to stay cyber-safe during summer vacations."},
  {platform:"media", src:"Aragon Inteligencia", title:"Tardes de Ciberseguridad Unizar", url:"https://araintel.com/articulos/dia-a-dia-de-un-investigador-de-ciberseguridad-en-sysdig/", desc:"¿Cómo es el día a día de un investigador de ciberseguridad en Sysdig?"},
  {platform:"media", src:"Business Insider", title:"Detección de deepfakes", url:"https://www.businessinsider.es/consejos-2-expertos-ciberseguridad-detectar-deepfakes-831319", desc:"Tips from cybersecurity experts on detecting deepfakes."},
  {platform:"media", src:"Revista SIC", title:"Análisis de la seguridad de las bases de datos orientadas a grafos", url:"https://revistasic.es/archivo/index8463.html?option=com_content&view=article&id=1825&Itemid=1589", desc:"Research paper analyzing information leakage and design flaws in graph-oriented databases."},
  {platform:"academic", src:"SECRYPT", title:"(In) Security in Graph Databases — Analysis and Data Leaks", url:"https://press.um.si/index.php/ump/catalog/book/296", desc:"Review of the most widespread graph databases, detecting security problems and improper default configurations."},
  {platform:"academic", src:"CECC 2017", title:"Why Did I End Up Living in a Cave? Risks of IoT at home", url:"https://revistasic.es/archivo/index8463.html?option=com_content&view=article&id=1825&Itemid=1589", desc:""},
  {platform:"media", src:"El lado del mal", title:"Desenmascarar cuentas de Twitter a través de Sinfonier", url:"https://www.elladodelmal.com/2015/12/desenmascarar-cuentas-de-twitter-traves.html", desc:""}
];

var OSS = [
  {name:"GraFScaN", url:"https://github.com/Miguel000/GraFScaN", role:"Creator", desc:"Python tool to discover and fingerprint graph databases (Neo4j, JanusGraph) for red team reconnaissance and vulnerability assessment."},
  {name:"DeepConfusables", url:"https://github.com/jiep/deep-confusables-cli", role:"Creator", desc:"Combines ML and confusable character domains (homoglyphs) to analyze domain obfuscation attacks used in phishing and impersonation."},
  {name:"SpyScrap", url:"https://github.com/RuthGnz/SpyScrap", role:"Developer", desc:"Platform to analyze your digital fingerprint using OSINT techniques, browser fingerprinting, and facial recognition."},
  {name:"offensive-ai-compilation", url:"https://github.com/jiep/offensive-ai-compilation", role:"Maintainer", desc:"Curated list of tools, papers, and resources covering Offensive AI research."},
  {name:"Synthetic Content Toolkit", url:"https://github.com/Miguel000/tools-generation-detection-synthetic-content", role:"Co-Creator", desc:"Curated tools, papers, and resources focused on generation and detection of synthetic content — deepfakes, GANs, synthetic media."},
  {name:"Fake Video Forensics", url:"https://github.com/Miguel000/fakeVideoFoarensics", role:"Co-Creator", desc:"Detects fake faces in videos using models evolved from FaceForensics++. Handles DeepFakes, FaceSwap, and Face2Face generated content."}
];

/* ─── HELPERS ─── */
function esc(s) {
  return String(s).replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;').replace(/"/g,'&quot;');
}

/* ─── TALKS ─── */
var activeYear = 'all';
(function() {
  var years = [];
  TALKS.forEach(function(t){ if(years.indexOf(t.y)===-1) years.push(t.y); });
  years.sort(function(a,b){ return b-a; });

  function buildYearBtns() {
    var html = '<button class="mh-fbtn active" data-y="all">All <span class="mh-fcount">('+TALKS.length+')</span></button>';
    years.forEach(function(y){
      var c = TALKS.filter(function(t){ return t.y===y; }).length;
      html += '<button class="mh-fbtn" data-y="'+y+'">'+y+' <span class="mh-fcount">('+c+')</span></button>';
    });
    document.getElementById('mh-years').innerHTML = html;
    document.querySelectorAll('#mh-years .mh-fbtn').forEach(function(btn){
      btn.addEventListener('click', function(){
        activeYear = this.dataset.y === 'all' ? 'all' : parseInt(this.dataset.y);
        document.querySelectorAll('#mh-years .mh-fbtn').forEach(function(b){ b.classList.remove('active'); });
        this.classList.add('active');
        renderTalks();
      });
    });
  }

  function renderTalks() {
    var list = activeYear === 'all' ? TALKS : TALKS.filter(function(t){ return t.y===activeYear; });
    var grouped = {};
    list.forEach(function(t){ if(!grouped[t.y]) grouped[t.y]=[]; grouped[t.y].push(t); });
    var sortedY = Object.keys(grouped).map(Number).sort(function(a,b){ return b-a; });
    var html = '';
    sortedY.forEach(function(y){
      html += '<div class="mh-year-group">';
      if(activeYear==='all') html += '<div class="mh-group-heading">'+y+'</div>';
      grouped[y].forEach(function(t){
        html += '<div class="mh-talk">';
        html += '<div><span class="mh-conf">'+esc(t.conf)+'</span>';
        if(t.loc) html += '<span class="mh-loc">'+esc(t.loc)+'</span>';
        if(t.workshop) html += '<span class="mh-badge mh-badge-ws">workshop</span>';
        html += '</div>';
        html += '<div class="mh-title">'+esc(t.title)+'</div>';
        if(t.video) html += '<div class="mh-row-links"><a class="mh-link" href="'+t.video+'" target="_blank">▶ video</a></div>';
        html += '</div>';
      });
      html += '</div>';
    });
    document.getElementById('mh-talk-list').innerHTML = html;
  }

  buildYearBtns();
  renderTalks();
})();

/* ─── BLOG ─── */
(function(){
  var PLATFORMS = [
    {id:'all',   label:'All'},
    {id:'sysdig',label:'Sysdig Blog'},
    {id:'bbva',  label:'BBVA'},
    {id:'media', label:'Media'},
    {id:'academic', label:'Academic'}
  ];
  var activePlat = 'all';

  function buildPlatBtns() {
    var html = '';
    PLATFORMS.forEach(function(p){
      var c = p.id==='all' ? BLOG.length : BLOG.filter(function(b){ return b.platform===p.id; }).length;
      html += '<button class="mh-fbtn'+(p.id==='all'?' active':'')+'" data-p="'+p.id+'">'+esc(p.label)+' <span class="mh-fcount">('+c+')</span></button>';
    });
    document.getElementById('mh-platforms').innerHTML = html;
    document.querySelectorAll('#mh-platforms .mh-fbtn').forEach(function(btn){
      btn.addEventListener('click', function(){
        activePlat = this.dataset.p;
        document.querySelectorAll('#mh-platforms .mh-fbtn').forEach(function(b){ b.classList.remove('active'); });
        this.classList.add('active');
        renderBlog();
      });
    });
  }

  function renderBlog() {
    var list = activePlat==='all' ? BLOG : BLOG.filter(function(b){ return b.platform===activePlat; });
    var html = '';
    list.forEach(function(b){
      html += '<div class="mh-blog-entry">';
      html += '<div class="mh-blog-title"><a href="'+esc(b.url)+'" target="_blank">'+esc(b.title)+'</a>';
      html += '<span class="mh-blog-source">'+esc(b.src)+'</span></div>';
      if(b.desc) html += '<div class="mh-blog-desc">'+esc(b.desc)+'</div>';
      html += '</div>';
    });
    document.getElementById('mh-blog-list').innerHTML = html;
  }

  buildPlatBtns();
  renderBlog();
})();

/* ─── OSS ─── */
(function(){
  var html = '';
  OSS.forEach(function(p){
    html += '<div class="mh-oss-card">';
    html += '<div class="mh-oss-name"><a href="'+esc(p.url)+'" target="_blank">'+esc(p.name)+'</a>';
    html += '<span class="mh-oss-role">'+esc(p.role)+'</span></div>';
    html += '<div class="mh-oss-desc">'+esc(p.desc)+'</div>';
    html += '</div>';
  });
  document.getElementById('mh-oss-grid').innerHTML = html;
})();

/* ─── TABS ─── */
document.querySelectorAll('.mh-tab').forEach(function(btn){
  btn.addEventListener('click', function(){
    document.querySelectorAll('.mh-tab').forEach(function(b){ b.classList.remove('active'); });
    document.querySelectorAll('.mh-pane').forEach(function(p){ p.classList.remove('active'); });
    this.classList.add('active');
    document.getElementById(this.dataset.target).classList.add('active');
  });
});
</script>
