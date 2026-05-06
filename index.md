---
layout: default
title: Miguel Hernández
---

<style>
.mh-nav {
  display: flex;
  gap: 0;
  margin: 24px 0 0;
  border-bottom: 1px solid #333;
}
.mh-tab {
  background: none;
  border: none;
  border-bottom: 2px solid transparent;
  color: #888;
  cursor: pointer;
  font-family: Monaco, "Bitstream Vera Sans Mono", "Lucida Console", Terminal, monospace;
  font-size: 14px;
  padding: 8px 18px 8px 0;
  margin-bottom: -1px;
  margin-right: 18px;
  transition: color .15s;
}
.mh-tab:hover { color: #ccc; }
.mh-tab.active { color: #9dbc98; border-bottom-color: #9dbc98; }

.mh-pane { display: none; padding-top: 16px; }
.mh-pane.active { display: block; }

.mh-years {
  display: flex;
  flex-wrap: wrap;
  gap: 6px;
  margin-bottom: 20px;
}
.mh-yr {
  background: none;
  border: 1px solid #333;
  color: #888;
  cursor: pointer;
  font-family: Monaco, "Bitstream Vera Sans Mono", monospace;
  font-size: 12px;
  padding: 3px 10px;
  border-radius: 2px;
  transition: all .15s;
}
.mh-yr:hover { border-color: #666; color: #ccc; }
.mh-yr.active { border-color: #9dbc98; color: #9dbc98; }

.mh-year-group { margin-bottom: 28px; }
.mh-year-heading {
  font-size: 11px;
  color: #555;
  text-transform: uppercase;
  letter-spacing: 3px;
  margin: 0 0 10px;
  padding-bottom: 5px;
  border-bottom: 1px solid #222;
}
.mh-talk {
  padding: 9px 0 9px 14px;
  border-left: 2px solid #252525;
  margin: 5px 0;
  transition: border-color .15s;
}
.mh-talk:hover { border-left-color: #9dbc98; }
.mh-conf { color: #fff; font-size: 13px; font-weight: bold; }
.mh-loc { color: #555; font-size: 12px; margin-left: 6px; font-weight: normal; }
.mh-title { color: #aaa; font-size: 13px; margin: 3px 0 5px; font-style: italic; }
.mh-links { display: flex; flex-wrap: wrap; gap: 10px; margin-top: 2px; }
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
.mh-badge-ws { color: #d29922; border-color: #5a3e00; background: #2d2000; }
.mh-count { color: #555; font-size: 12px; margin-left: 4px; }

.mh-about-links { list-style: none; padding: 0; margin: 16px 0; }
.mh-about-links li { margin: 8px 0; }
.mh-about-links a { color: #63c0f5; }
</style>

# Miguel Hernández

Sr. Threat Research Engineer at Sysdig. Security researcher focused on cloud-native threats, runtime detection, and AI security. Speaker at cybersecurity conferences in Europe and Latin America since 2016.

<div class="mh-nav">
  <button class="mh-tab active" data-target="mh-talks">Talks</button>
  <button class="mh-tab" data-target="mh-about">About</button>
</div>

<div id="mh-talks" class="mh-pane active">
  <div class="mh-years" id="mh-years"></div>
  <div id="mh-list"></div>
</div>

<div id="mh-about" class="mh-pane">

**Contact:** [miguelhernandez2907@gmail.com](mailto:miguelhernandez2907@gmail.com)

<ul class="mh-about-links">
  <li><a href="https://github.com/Miguel000/MySecTalks">Conference talks</a> — slides, recordings, and abstracts</li>
  <li><a href="https://github.com/Miguel000/BlogContent">Blog content</a> — research posts and write-ups</li>
  <li><a href="https://github.com/Miguel000/OpenSourceTools">Open-source projects</a> — tools and contributions</li>
  <li><a href="https://github.com/Miguel000">GitHub profile</a></li>
</ul>

**Bio:** Miguel Hernández is a Sr. Threat Research Engineer at Sysdig with over a decade of experience in security research. He has spoken at major cybersecurity conferences across Europe including HITB, HackLu, DeepSec, RootedCon, and fwd:CloudSec EU. His research spans cloud-native threats, runtime detection with Falco, supply chain security, adversarial AI, and emerging threat intelligence.

</div>

<script>
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

var years = [];
TALKS.forEach(function(t){ if(years.indexOf(t.y) === -1) years.push(t.y); });
years.sort(function(a,b){ return b - a; });

var activeYear = 'all';

function buildYears() {
  var html = '<button class="mh-yr active" data-y="all">All <span class="mh-count">(' + TALKS.length + ')</span></button>';
  years.forEach(function(y) {
    var c = TALKS.filter(function(t){ return t.y === y; }).length;
    html += '<button class="mh-yr" data-y="' + y + '">' + y + ' <span class="mh-count">(' + c + ')</span></button>';
  });
  document.getElementById('mh-years').innerHTML = html;
  document.querySelectorAll('.mh-yr').forEach(function(btn) {
    btn.addEventListener('click', function() {
      activeYear = this.dataset.y === 'all' ? 'all' : parseInt(this.dataset.y);
      document.querySelectorAll('.mh-yr').forEach(function(b){ b.classList.remove('active'); });
      this.classList.add('active');
      renderList();
    });
  });
}

function esc(s) {
  return s.replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;');
}

function renderList() {
  var filtered = activeYear === 'all' ? TALKS : TALKS.filter(function(t){ return t.y === activeYear; });
  var grouped = {};
  filtered.forEach(function(t){ if(!grouped[t.y]) grouped[t.y]=[]; grouped[t.y].push(t); });
  var sortedYears = Object.keys(grouped).map(Number).sort(function(a,b){ return b-a; });

  var html = '';
  sortedYears.forEach(function(y) {
    html += '<div class="mh-year-group">';
    if(activeYear === 'all') html += '<div class="mh-year-heading">' + y + '</div>';
    grouped[y].forEach(function(t) {
      html += '<div class="mh-talk">';
      html += '<div><span class="mh-conf">' + esc(t.conf) + '</span>';
      if(t.loc) html += '<span class="mh-loc">' + esc(t.loc) + '</span>';
      if(t.workshop) html += '<span class="mh-badge mh-badge-ws">workshop</span>';
      html += '</div>';
      html += '<div class="mh-title">' + esc(t.title) + '</div>';
      var links = [];
      if(t.video) links.push('<a class="mh-link" href="' + t.video + '" target="_blank">▶ video</a>');
      if(t.slides) links.push('<a class="mh-link" href="' + t.slides + '" target="_blank">slides</a>');
      if(links.length) html += '<div class="mh-links">' + links.join('') + '</div>';
      html += '</div>';
    });
    html += '</div>';
  });
  document.getElementById('mh-list').innerHTML = html;
}

document.querySelectorAll('.mh-tab').forEach(function(btn) {
  btn.addEventListener('click', function() {
    document.querySelectorAll('.mh-tab').forEach(function(b){ b.classList.remove('active'); });
    document.querySelectorAll('.mh-pane').forEach(function(p){ p.classList.remove('active'); });
    this.classList.add('active');
    document.getElementById(this.dataset.target).classList.add('active');
  });
});

buildYears();
renderList();
</script>
