* {
  margin: 0;
}

body {
  background-color: #efefef;
  font-family: Arial, sans-serif;
  text-align: center;
}

#imageLogo {
  width: 400px;
  height: 150px;
  margin-right: 20px;
  margin-left: auto;
  margin-right: auto;
}

h1 {
  margin-bottom: 10px;
}

.course-container {
  position: relative;
  width: 900px;
  height: 400px;
  margin: 0 auto;
  background-size: cover;
  border: 2px solid black;
}

.voiture {
  width: 50px;
  height: 30px;
  position: absolute;
  bottom: 145px;
  left: -80px;
  transition: left 2s linear;
}

#voiture1 {
  position: absolute;
  bottom: 350px;
  left: 0px;
  width: 175px;
  height: 150px;
  z-index: 2;
}

#voiture2 {
  position: absolute;
  bottom: 250px;
  left: -15px;
  width: 195px;
  height: 150px;
  z-index: 2;
}

#imageCircuit {
  position: absolute;
  top: 350px;
  left: 0px;
  width: 100vw;
  height: 250px;
}

.timer {
  position: absolute;
  font-size: 18px;
  color: rgb(0, 0, 0);
  background-color: rgba(245, 40, 40);
  padding: 5px 10px;
  border: 2.5px solid black;
  border-radius: 5px;
  bottom: 200px;
  left: 40vw;
}

.timer:nth-child(2) {
  background-color: rgba(237, 237, 237);
  left: 50vw;
}

button {
  position: relative;
  margin: 1em 2em;
  padding: 1em 2em;
  border-radius: 1vw;
  border: none;
  color: #efcb24;
  background: rgb(12, 64, 138);
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
  transition: background-color 0.3s, transform 0.3s;
}

button:hover {
  background-color: #f90504;
  transform: scale(1.05);
}

#decompte {
  font-size: 35px;
  font-weight: bold;
}
