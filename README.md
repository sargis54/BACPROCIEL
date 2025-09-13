<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title data-fr="Bac Pro CIEL" data-en="CIEL Vocational High School">Bac Pro CIEL</title>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
<style>
    #map {
  height: 400px; /* obligatoire pour que la carte apparaisse */
  width: 100%;
  border-radius: 12px;
  box-shadow: 0 3px 6px rgba(0,0,0,.1);
}

html{scroll-behavior:smooth;}
body{font-family:sans-serif;margin:0;color:#222;background:linear-gradient(135deg,#07c,#6a11cb,#2575fc);background-attachment:fixed;}
header{background:rgba(0,0,0,.6);color:#fff;padding:15px;text-align:center;position:sticky;top:0;z-index:1000;backdrop-filter:blur(8px);}
#btnLang{position:absolute;top:10px;left:10px;}
header h1{margin:0;}
nav a{color:#fff;margin:0 10px;text-decoration:none;font-weight:bold;position:relative;}
nav a::after{content:"";position:absolute;left:0;bottom:-3px;width:0;height:2px;background:#57ffab;transition:.3s;}
nav a:hover::after{width:100%;}
section{background:rgba(255,255,255,.9);padding:30px;margin:30px auto;border-radius:15px;box-shadow:0 6px 15px rgba(0,0,0,.15);max-width:900px;animation:fadeIn 1s;}
h2{color:#07c;margin-top:0;}
.grid{display:grid;grid-template-columns:1fr 1fr;gap:20px;}
@media(max-width:700px){.grid{grid-template-columns:1fr;}}
.card{background:#f9f9f9;padding:20px;border-radius:12px;box-shadow:0 3px 6px rgba(0,0,0,.1);transition:.3s;}
.card:hover{transform:translateY(-5px);box-shadow:0 8px 20px rgba(0,0,0,.2);}
.btn{background:#07c;color:#fff;padding:10px 18px;border-radius:8px;text-decoration:none;display:inline-block;margin-top:10px;transition:.3s;border:none;cursor:pointer;}
.btn:hover{background:#005fa3;transform:scale(1.05);}
.slogan{text-align:center;font-weight:bold;margin:20px 0;font-size:1.4em;transition:.5s;color:#333;}
input,textarea{width:100%;margin:8px 0;padding:10px;border:1px solid #ccc;border-radius:6px;font-size:1rem;}
footer{background:rgba(0,0,0,.8);color:#fff;text-align:center;padding:15px;margin-top:40px;}
@keyframes fadeIn{from{opacity:0;transform:translateY(20px);}to{opacity:1;transform:translateY(0);}}
</style>
<link rel="stylesheet" href="https://unpkg.com/leaflet/dist/leaflet.css" />
<script src="https://unpkg.com/leaflet/dist/leaflet.js"></script>

</head>
<body>

<header>
<button id="btnLang" class="btn">EN</button>
<h1 data-fr="Bac Pro CIEL" data-en="CIEL Vocational High School">Bac Pro CIEL</h1>
<nav>
  <a href="#presentation" data-fr="Présentation" data-en="Presentation">Présentation</a>
  <a href="#competences" data-fr="Compétences" data-en="Skills">Compétences</a>
  <a href="#Etudes sup" data-fr="Etudes sup" data-en="Higher Education">Etudes sup</a>
  <a href="#Paroles d'élèves" data-fr="Paroles d'élèves" data-en="Student Words">Paroles d'élèves</a>
  <a href="#contact" data-fr="Contact" data-en="Contact">Contact</a>
</nav>
</header>

<section id="presentation">
<h2 data-fr="Présentation" data-en="Presentation"><i class="fa-solid fa-graduation-cap"></i> Présentation</h2>
<p data-fr="Le Bac Pro CIEL forme des techniciens en numérique, réseaux et électronique."
   data-en="The CIEL Vocational High School trains technicians in digital, networks, and electronics.">
   Le <b>Bac Pro CIEL</b> forme des techniciens en numérique, réseaux et électronique.
</p>
<video controls width="800">
  <source src="https://vr.lycee-cormontaigne-metz.fr/ciel.mp4?_=1" type="video/webm" />
</video>
</section>

<section id="carte">
    <h2 data-fr="Carte des lycées et stages CIEL" data-en="Map of CIEL High Schools and Internships">
      <i class="fa-solid fa-map-marker-alt"></i> Carte des lycées CIEL
    </h2>
    <div id="map" style="height: 400px;"></div>
  </section>
  
<section id="competences">
<h2 data-fr="Compétences" data-en="Skills"><i class="fa-solid fa-bolt"></i> Compétences</h2>
<div class="grid">
  <div class="card" data-fr="Installer et sécuriser des équipements" data-en="Install and secure equipment">
    <i class="fa-solid fa-shield-halved"></i> Installer et sécuriser des équipements
  </div>
  <div class="card" data-fr="Diagnostiquer et réparer" data-en="Diagnose and repair">
    <i class="fa-solid fa-screwdriver-wrench"></i> Diagnostiquer et réparer
  </div>
  <div class="card" data-fr="Mettre en œuvre des réseaux" data-en="Implement networks">
    <i class="fa-solid fa-network-wired"></i> Mettre en œuvre des réseaux
  </div>
  <div class="card" data-fr="Intervenir en domotique et IoT" data-en="Work in home automation and IoT">
    <i class="fa-solid fa-house-signal"></i> Intervenir en domotique et IoT
  </div>
</div>
</section>

<section id="Etudes sup">
<h2 data-fr="Etudes sup" data-en="Higher Education"><i class="fa-solid fa-road"></i> Etudes sup</h2>
<div class="grid">
  <div class="card">
    <b data-fr="Pro" data-en="Pro">Pro</b>
    <ul>
      <li data-fr="Technicien réseaux" data-en="Network technician">Technicien réseaux</li>
      <li data-fr="Domoticien" data-en="Home automation specialist">Domoticien</li>
    </ul>
  </div>
  <div class="card">
    <b data-fr="Études" data-en="Studies">Études</b>
    <ul>
      <li data-fr="BTS SN" data-en="BTS Digital Systems">BTS SN</li>
      <li data-fr="BTS Cybersécurité" data-en="BTS Cybersecurity">BTS Cybersécurité</li>
    </ul>
  </div>
</div>
</section>

<section>
<h2 data-fr="Slogans" data-en="Slogans"><i class="fa-solid fa-lightbulb"></i> Slogans</h2>
<div class="slogan" id="slogan" data-fr="Connecte ton avenir avec le Bac Pro CIEL."
     data-en="Connect your future with the CIEL Vocational High School.">
     Connecte ton avenir avec le Bac Pro CIEL.
</div>
</section>

<section id="Paroles d'élèves">
<h2 data-fr="Paroles d'élèves" data-en="Student Words"><i class="fa-solid fa-user"></i> Paroles d'élèves</h2>
<div class="grid">
  <div class="card">
    <h3>Sargis G.</h3>
    <p data-fr="Le Bac Pro CIEL m'a permis de comprendre le monde numérique."
       data-en="The CIEL Bac Pro allowed me to understand the digital world.">
       Le Bac Pro CIEL m'a permis de comprendre le monde numérique.
    </p>
    <button class="btn" onclick="afficherEleve('Sargis')">Voir témoignage</button>
  </div>
  <div class="card">
    <h3>Tom O.</h3>
    <p data-fr="J'adore apprendre à installer des systèmes domotiques."
       data-en="I love learning to install home automation systems.">
       J'adore apprendre à installer des systèmes domotiques.
    </p>
    <button class="btn" onclick="afficherEleve('Tom')">Voir témoignage</button>
  </div>
</div>
</section>

<div id="modalEleve" style="display:none;position:fixed;top:0;left:0;width:100vw;height:100vh;background:rgba(0,0,0,0.7);z-index:2000;">
  <div style="background:#fff;margin:50px auto;padding:20px;border-radius:10px;max-width:600px;position:relative;">
    <span onclick="fermerModal()" style="position:absolute;top:10px;right:15px;cursor:pointer;font-size:1.5em;">&times;</span>
    <div id="contenuEleve"></div>
  </div>
</div>

<script>
const profils = {
  Sargis: { nom:"Sargis", texte: {
    fr:`<p>Bonjour, je m'appelle <strong>Sargis</strong> et je suis en Terminale Bac Pro CIEL.</p>
        <p>J’ai choisi cette filière car je suis passionné par l’informatique et les nouvelles technologies. J’ai appris à installer des systèmes, sécuriser des réseaux et même programmer un peu en Python.</p>
        <p>Mon stage en entreprise m’a permis de travailler sur de vrais projets. J’ai pu installer une caméra IP dans une maison connectée, ce qui m’a beaucoup plu.</p>
        <p>Après le bac, je souhaite poursuivre en <strong>BTS Systèmes Numériques</strong> pour approfondir mes connaissances.</p>
        <p><em>"CIEL, c’est une voie concrète vers les métiers du futur."</em></p>`,
    en:`<p>Hello, my name is <strong>Sargis</strong> and I am in the final year of CIEL Vocational High School.</p>
        <p>I chose this program because I am passionate about IT and new technologies. I learned to install systems, secure networks, and even program a bit in Python.</p>
        <p>My internship allowed me to work on real projects. I installed an IP camera in a smart home, which I really enjoyed.</p>
        <p>After graduation, I plan to continue with a <strong>BTS Digital Systems</strong> to deepen my knowledge.</p>
        <p><em>"CIEL is a concrete path to future careers."</em></p>` }},
  Tom: { nom:"Tom", texte: {
    fr:`<p>Je suis <strong>Tom</strong> et j’ai rejoint le Bac Pro CIEL après la 3e.</p>
        <p>Ce que j'aime le plus, c’est la domotique : contrôler des lumières ou des volets avec une appli, c’est trop stylé !</p>
        <p>Grâce à cette formation, j’ai appris à intervenir sur des équipements électroniques, mais aussi à comprendre comment tout est relié en réseau.</p>
        <p>Plus tard, j’aimerais devenir technicienne en automatisme.</p>
        <p><em>"CIEL m’a donné confiance en moi."</em></p>`,
    en:`<p>I am <strong>Tom</strong> and I joined the CIEL Bac Pro after 9th grade.</p>
        <p>What I like most is home automation: controlling lights or shutters with an app is so cool!</p>
        <p>Thanks to this training, I learned to work on electronic equipment and understand how everything is connected in a network.</p>
        <p>Later, I would like to become an automation technician.</p>
        <p><em>"CIEL gave me confidence in myself."</em></p>` }}
};

let currentLang='fr';

function afficherEleve(prenom){
  const eleve=profils[prenom];
  document.getElementById("contenuEleve").innerHTML=`<h2>${eleve.nom}</h2>`+eleve.texte[currentLang];
  document.getElementById("modalEleve").style.display="block";
}
function fermerModal(){ document.getElementById("modalEleve").style.display="none"; }

// Slogans
const slogans = {fr:["Connecte ton avenir avec le Bac Pro CIEL.","Ton futur dans le numérique commence ici.","CIEL : maîtrise les réseaux, sécurise le futur."],
                 en:["Connect your future with the CIEL Vocational High School.","Your future in digital starts here.","CIEL: master networks, secure the future."]};
let i=0, el=document.getElementById("slogan");
setInterval(()=>{
  el.style.opacity=0;
  setTimeout(()=>{
    i=(i+1)%slogans[currentLang].length;
    el.innerHTML=slogans[currentLang][i];
    el.style.opacity=1;
  },400);
},3000);

// Changement de langue
const btnLang=document.getElementById('btnLang');
btnLang.addEventListener('click',()=>{
  currentLang=currentLang==='fr'?'en':'fr';
  btnLang.textContent=currentLang==='fr'?'EN':'FR';
  document.querySelectorAll('[data-fr]').forEach(el=>el.innerHTML=el.dataset[currentLang]);
});

// Footer year
document.getElementById("year").textContent=new Date().getFullYear();
</script>

<section id="contact">
<h2 data-fr="Contact" data-en="Contact"><i class="fa-solid fa-envelope"></i> Contact</h2>
<form onsubmit="event.preventDefault();alert(currentLang==='fr'?'Merci !':'Thank you!');">
<input type="text" placeholder="Nom" required>
<input type="email" placeholder="Email" required>
<textarea rows="3" placeholder="Message"></textarea>
<button class="btn" data-fr="Envoyer" data-en="Send">Envoyer</button>
</form>
</section>

<footer>© <span id="year"></span> <span data-fr="Bac Pro CIEL" data-en="CIEL Vocational High School">Bac Pro CIEL</span></footer>

<script>
    const map = L.map('map').setView([46.603354, 1.888334], 6); // Centré sur la France
  
    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
    }).addTo(map);
  
    const etablissements = [
      {
        nom: 'Lycée Louise Michel',
        ville: 'Ruffec',
        coord: [45.946, 0.289],
        type: 'Lycée',
      
      },
      {
        nom: 'Lycée Rompsay',
        ville: 'La Rochelle',
        coord: [46.158, -1.153],
        type: 'Lycée',
      
      },
      {
        nom: 'Lycée Paule Pignolet',
        ville: 'Les Trois-Bassins',
        coord: [-21.175, 55.267],
        type: 'Lycée',
      
      },
      {
        nom: 'Lycée Rompsay',
        ville: 'La Rochelle',
        coord: [46.158, -1.153],
        type: 'Lycée',
    
      },
    {
        nom: 'Lycée des Métiers Pierre-André Chabanne',
        ville: 'Angoulême',
        coord: [45.648, 0.163],
        type: 'Lycée',
    
    },
    {
        nom: 'Lycée polyvalent Clément Ader',
        ville: 'Toulouse',
        coord: [43.604, 1.444],
        type: 'Lycée',
  
    },
    {
        nom: 'Lycée de l\'Essouriau',
        ville: 'Saint-Amand-les-Eaux',
        coord: [50.396, 3.417],
        type: 'Lycée',
    },
    {
        nom: 'Lycée Gutenberg',
        ville: 'Paris',
        coord: [48.855, 2.381],
        type: 'Lycée',
 
    },
    {
        nom: 'Lycée Saint-Nicolas',
        ville: 'Paris',
        coord: [48.868, 2.331],
        type: 'Lycée',
  },
    {
        nom: 'Lycée Joséphine Baker',
        ville: 'Paris',
        coord: [48.832, 2.358],
        type: 'Lycée',
        
    },
    {
        nom: 'Lycée Kastler',
        ville: 'Strasbourg',
        coord: [48.586, 7.748],
        type: 'Lycée',
        
    },
    {
        nom: 'Lycée Marius Bouvier',
        ville: 'Lyon',
        coord: [45.748, 4.846],
        type: 'Lycée',
       
    },
    {
        nom: 'Lycée Jeannette-Verdier',
        ville: 'Montargis',
        coord: [47.993, 2.729],
        type: 'Lycée',
     
    },
    {
        nom: 'Lycée Georges-Baumont',
        ville: 'Saint-Dié-des-Vosges',
        coord: [48.276, 6.950],
        type: 'Lycée',
    
    },
    {
        nom: 'Lycée Louis de Cormontaigne',
        ville: 'Metz',
        coord: [49.124353, 6.163330],
        type: 'Lycée',
   
    }
    
];

      
      // Ajoutez d'autres établissements ici
    ;
  
    etablissements.forEach(etab => {
      L.marker(etab.coord)
        .addTo(map)
        .bindPopup(`<strong>${etab.nom}</strong><br>${etab.ville}<br><em>${etab.type}</em><br>${etab.description}`);
    });
</script>
  
</body>
</html>
