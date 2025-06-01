<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Clock App</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      scroll-behavior: smooth;
    }

    section {
      height: 100vh;
      padding: 60px 20px;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
    }

    .navbar {
      position: fixed;
      bottom: 0;
      width: 100%;
      background-color: #333;
      display: flex;
      justify-content: space-around;
      padding: 5px 0px;
    
      z-index: 1000;
    }

    .navbar a {
      color: white;
      text-decoration: none;
      font-size: 40px;
      padding: 40px 20px;
    }

    .navbar a:hover {
      background-color: #444;
      border-radius: 10px;
    }

    h1, p {
      color: white;
      text-align: center;
    }
    p{
      font-size: 70px;
      background-color: black;
      padding:5px;
      text-align: center;
      border-radius:25px;
      width:420px;
      font-family: ;
      box-shadow:0px 0px 30px white;
      text-shadow:4px 4px 8px white;
    }

    #digital { background: linear-gradient(45deg,violet,blue);}
    #analog {  background: linear-gradient(45deg,violet,blue); }
    #alarm {background: linear-gradient(45deg,violet,blue); }
    #stopwatch {background: linear-gradient(45deg,violet,blue); }

  .clock {
      width: 300px;
      height: 300px;
      border: 4px solid white;
      border-radius: 50%;
      position: relative;
      background: black;
      box-shadow: 0 0 30px white;
      margin:50px;
    }

    .hand {
      position: absolute;
      bottom: 50%;
      left: 50%;
      transform-origin: bottom center;
      transform: translateX(-50%) rotate(0deg);
    }

    .hour {
      width: 6px;
      height: 80px;
      background: white;
      box-shadow:0 0 20px white;
      border-radius:5px;
    }

    .minute {
      width: 4px;
      height: 100px;
      background: gray;
      box-shadow:0 0 20px white;
      border-radius:5px;
    }

    .second {
      width: 2px;
      height: 120px;
      background: red;
    }

    .center {
      width: 12px;
      height: 12px;
      background: lightgray;
      box-shadow:0 0 30px white;
      border-radius: 50%;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }


    #alarmTime {
      padding: 10px;
      font-size: 30px;
      margin-bottom:40px;
    }

    button {
      padding: 10px 20px;
      margin: 29px;
      font-size: 20px;
      background: linear-gradient(45deg,green,yellow); 
      color:white;
      border-radius:10px;
      box-shadow:4px 4px 5px gray;
      cursor: pointer;
    }

    #stopwatchDisplay {
      font-size: 4rem;
      font-family: monospace;
      margin: 30px;
      color:white;
      background-color: black;
      border-radius:20px;
      box-shadow:4px 4px 30px white; 
      text-shadow:4px 4px 5px white;
      padding:10px;
    }
  </style>
</head>
<body>

  <!-- Digital Clock -->
  <section id="digital">
    <h1>Digital Clock</h1>
    <p id="digitalTime">Loading...</p>
  </section>

  <!-- Analog Clock -->
  <section id="analog">
    <h1>Analog Clock</h1>
      <div class="clock">
    <div class="hand hour" id="hourHand"></div>
    <div class="hand minute" id="minuteHand"></div>
    <div class="hand second" id="secondHand"></div>
    <div class="center"></div>
  </div>
  </section>

  <!-- Alarm -->
  <section id="alarm">
    <h1>Set Alarm</h1>
    <input type="time" id="alarmTime">
    <button onclick="setAlarm()">Set Alarm</button>
    <p id="alarmStatus">No alarm set</p>
  </section>

  <!-- Stopwatch with Milliseconds -->
  <section id="stopwatch">
    <h1>Stopwatch</h1>
    <div id="stopwatchDisplay">00:00:00:000</div>
    <button onclick="startStopwatch()">Start</button>
    <button onclick="stopStopwatch()">Stop</button>
    <button onclick="resetStopwatch()">Reset</button>
  </section>

  <!-- Bottom Navigation -->
  <div class="navbar">
    <a href="#digital">Digital</a>
    <a href="#analog">Analog</a>
    <a href="#alarm">Alarm</a>
    <a href="#stopwatch">Stopwatch</a>
  </div>

  <!-- Scripts -->
  <script>
    // Digital Clock
    setInterval(() => {
      const now = new Date();
      document.getElementById("digitalTime").innerHTML =
        now.toLocaleTimeString();
    }, 50);

    // Analog Clock
    function updateAnalogClock() {
      const now = new Date();
      const sec = now.getSeconds() * 6;
      const min = now.getMinutes() * 6 + sec / 60;
      const hr = (now.getHours() % 12) * 30 + min / 12;

      document.getElementById("secondHand").style.transform = `rotate(${sec}deg)`;
      document.getElementById("minuteHand").style.transform = `rotate(${min}deg)`;
      document.getElementById("hourHand").style.transform = `rotate(${hr}deg)`;
    }
    setInterval(updateAnalogClock, 1000);

    // Alarm
    let alarmTime = null;
    let alarmTriggered = false;

    function setAlarm() {
      alarmTime = document.getElementById("alarmTime").value;
      document.getElementById("alarmStatus").innerHTML = "Alarm set for " + alarmTime;
      alarmTriggered = false;
    }

    setInterval(() => {
      if (!alarmTime || alarmTriggered) return;
      const now = new Date();
      const currentTime = now.toTimeString().slice(0, 5);
      if (currentTime === alarmTime) {
        alert("⏰ Alarm Ringing!");
        document.getElementById("alarmStatus").innerHTML = "Alarm Triggered!";
        alarmTriggered = true;
      }
    }, 1000);

    // Stopwatch with milliseconds
    let startTime = 0;
    let elapsedTime = 0;
    let stopwatchInterval;

    function updateStopwatchDisplay() {
      const time = elapsedTime;
      const hrs = Math.floor(time / 3600000);
      const mins = Math.floor((time % 3600000) / 60000);
      const secs = Math.floor((time % 60000) / 1000);
      const ms = time % 100;

      document.getElementById("stopwatchDisplay").innerHTML =
        `${hrs.toString().padStart(2, '0')}:` +
        `${mins.toString().padStart(2, '0')}:` +
        `${secs.toString().padStart(2, '0')}:` +
        `${ms.toString().padStart(2, '0')}`;
    }

    function startStopwatch() {
      if (stopwatchInterval) return;

      startTime = Date.now() - elapsedTime;
      stopwatchInterval = setInterval(() => {
        elapsedTime = Date.now() - startTime;
        updateStopwatchDisplay();
      }, 1); // update every 1ms
    }

    function stopStopwatch() {
      clearInterval(stopwatchInterval);
      stopwatchInterval = null;
    }

    function resetStopwatch() {
      stopStopwatch();
      elapsedTime = 0;
      updateStopwatchDisplay();
    }

    updateStopwatchDisplay(); // initialize
  </script>

</body>
</html>
