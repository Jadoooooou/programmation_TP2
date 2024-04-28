let voiture1 = document.getElementById("voiture1");
let voiture2 = document.getElementById("voiture2");
let temps1 = 0;
let temps2 = 0;
const containerWidth = 900;
const voiture1Width = 175;
const voiture2Width = 195;
let translationX1 = 0;
let translationX2 = 0;

// compte à rebours

function compteARebour() {
  let decompte = 10;

  const decompteInterval = setInterval(function () {
    document.getElementById("decompte").value = decompte;
    decompte--;
    if (decompte < 0) {
      clearInterval(decompteInterval);
      document.getElementById("decompte").value = "GO!";
    }
  }, 1000);
}

// chronomètre

function chronometre() {
  setInterval(function () {
    temps1++;
    temps2++;
    document.getElementById("timer1").textContent = temps1;
    document.getElementById("timer2").textContent = temps2;
  }, 1000);
}

// déplacement

function aleatoireTranslationX(containerWidth, voiture1Width) {
  const maxTranslationX = containerWidth - voiture1Width;
  const aleatoire = Math.random() * maxTranslationX;
  const translationX = Math.floor(aleatoire);

  return translationX;
}

function deplacerVoiture() {
  translationX1 += aleatoireTranslationX(containerWidth, voiture1Width);
  translationX2 += aleatoireTranslationX(containerWidth, voiture2Width);

  if (translationX1 > containerWidth - voiture1Width)
    translationX1 = containerWidth - voiture1Width;
  if (translationX2 > containerWidth - voiture2Width)
    translationX2 = containerWidth - voiture2Width;

  voiture1.style.left = translationX1 + "10px";
  voiture2.style.left = translationX2 + "10px";
}

// démarrer la course

function demarrerCourse() {
  compteARebour();
  setTimeout(chronometre, 10000);
  setTimeout(function () {
    setInterval(deplacerVoiture, 1000);
  }, 10000);
}

function arreterCourse() {
  clearInterval()(deplacerVoiture);
}


