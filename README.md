<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mensaje Especial</title>
  <style>
    .message {
      font-size: 24px;
      margin: 20px;
      font-weight: bold;
      text-align: center;
    }
    .buttons {
      margin-top: 20px;
      text-align: center;
    }
    .button {
      font-size: 18px;
      padding: 10px 20px;
      margin: 10px;
      color: white;
      background-color: #4CAF50;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      text-decoration: none;
    }
    .button.no {
      background-color: #f44336;
    }
    .hidden {
      display: none;
    }
  </style>
</head>
<body>
  <div style="text-align: center;">
    <h1>Un Mensaje para Ti MI FUTURA ESPOSITA💓</h1>
  </div>
  
  <img src="https://i.imgur.com/JHTocYe.gif" alt="Oso pidiendo perdón" style="display: block; margin: 0 auto;">
  
  <div class="message" id="initialMessage">¿ME PERDONAS MI AMORCITA HERMOSA??</div>
  
  <div class="buttons" id="initialButtons">
    <a href="#" id="yesButton" class="button">Sí</a>
    <a href="#" id="noButton" class="button no">No</a>
  </div>

  <div class="message hidden" id="thankYouMessage">
    Gracias mi amorcito, te amo y te amaré siempre 💖
  </div>
  
  <div class="buttons hidden" id="thankYouButtons">
    <img src="https://i.imgur.com/a5aJQvU.gif" alt="Te Amo GIF" style="width: 200px;">
    <br><p>Te amo muchísimo!</p>
  </div>
  
  <div class="message hidden" id="sureMessage">
    ¿Segura?
  </div>
  
  <div class="buttons hidden" id="sureButtons">
    <img src="https://i.imgur.com/wXq6hIn.gif" alt="Seguro GIF" style="width: 200px;">
    <br><a href="#" id="yesButton2" class="button">Sí</a>
    <a href="#" id="noButton2" class="button no">No</a>
  </div>

  <script>
    // Función para ocultar y mostrar elementos
    function toggleVisibility(elementsToHide, elementsToShow) {
      elementsToHide.forEach(function(element) {
        document.getElementById(element).classList.add('hidden');
      });
      elementsToShow.forEach(function(element) {
        document.getElementById(element).classList.remove('hidden');
      });
    }
