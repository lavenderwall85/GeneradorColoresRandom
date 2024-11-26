<script>
    let color = '#FFFFFF';
    let color_default = '#2aa8ca';
    function generarColor() {
      let r = Math.floor(Math.random() * 256);
      let g = Math.floor(Math.random() * 256);
      let b = Math.floor(Math.random() * 256);
  
      color = `#${r.toString(16).padStart(2, '0')}${g.toString(16).padStart(2, '0')}${b.toString(16).padStart(2, '0')}`;
    }
  </script>
  
  <main>
    <h1>Generador de Colores Aleatorios</h1>
  
    <button on:click={generarColor} style="background-color: {color_default};">Generar Color</button>
  
    <div class="color-display" style="background-color: {color};">
      <p>{color}</p>
    </div>
  </main>
  
  <style>
    main {
      text-align: center;
      margin-top: 50px;
      font-family: Arial, sans-serif;
    }
  
    button {
      padding: 10px 20px;
      font-size: 16px;
      cursor: pointer;
      background-color: #4CAF50;
      color: white;
      border: none;
      border-radius: 5px;
    }
  
    button:hover {
      background-color: #45a049;
    }
  
    .color-display {
      width: 200px;
      height: 200px;
      margin-top: 20px;
      display: inline-block;
      text-align: center;
    }
  
    p {
      color: white;
      font-weight: bold;
    }
  </style>
  