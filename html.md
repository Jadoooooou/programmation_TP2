<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Course de Voitures</title>
    <link rel="stylesheet" href="course.css" />
    <script src="course.js"></script>
  </head>
  <body>
    <img src="./images/piston_cup_logo.png" id="imageLogo" />

    <h1>Course de Voitures - Piston Cup</h1>

    <div id="course-container">
      <div class="voiture">
        <img src="./images/voiture_01.png" id="voiture1" />
      </div>

      <div id="timer1" class="timer">00:00:00</div>

      <div class="voiture">
        <img src="./images/voiture_02.png" id="voiture2" />
      </div>

      <div id="timer2" class="timer">00:00:00</div>

      <img src="./images/circuit.png" id="imageCircuit" />

      <button type="button" onClick="demarrerCourse" id="startButton">
        Démarrer la Course
      </button>
      <input type="text" id="decompte" size="10" readonly />
    </div>
    <script src="course.js"></script>
  </body>
</html>
