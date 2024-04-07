# -
¿Me perdonas? :&lt;
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta http-equiv="X-UA-Compatible" content="IE=edge" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>¿Me perdonas?:< </title>
  <style>
    body {
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background-color: #f3f3f3;
      font-family: Arial, sans-serif;
    }
    #container {
      text-align: center;
    }
    h1 {
      font-size: 32px;
      color: #333;
    }
    #buttons {
      margin-top: 20px;
      display: flex;
      justify-content: center;
      align-items: center;
    }
    button {
      margin: 10px;
      padding: 10px 20px;
      font-size: 18px;
      color: #fff;
      background-color: #4CAF50;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.3s;
    }
    button:hover {
      background-color: #45a049;
    }
    #btnNo {
      background-color: #f44336;
    }
    #btnNo:hover {
      background-color: #d32f2f;
    }
    img {
      margin-top: 30px;
      max-width: 100%;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }
  </style>
  <script>
    function accionParaCuandoEllaDigaQueSi() {
      alert("Te amo demasiado mi niña hermosa❤️ );
    }
 
    function mueveElBoton() {
      const width = window.innerWidth;
      const height = window.innerHeight;

      const newWidth = Math.random() * width;
      const newHeight = Math.random() * height;

      const btnNo = document.getElementById("btnNo");
      btnNo.style.position = "absolute";
      btnNo.style.left = newWidth + "px";
      btnNo.style.top = newHeight + "px";
    }
  </script>
</head>
<body>
    <div id="container">
      <h1>¿Me perdonas?:<  </h1>
      <div id="buttons">
        <button onclick="accionParaCuandoEllaDigaQueSi()" id="btnSi">Sí</button>
        <button id="btnNo" onmouseover="mueveElBoton()">No</button>
      </div>
      <img src="img/2.jpeg" alt="" width="200">
    </div>

    <script>
      function accionParaCuandoEllaDigaQueSi() {
        const respuesta = confirm("TE AMO");
        if (respuesta) {
          // Redireccionar a la nueva página si responde "Sí"
          window.location.href = "opcionsi.html";
        } else {
          alert("Plisss 🥺");
        }
      }

      function mueveElBoton() {
        const width = window.innerWidth;
        const height = window.innerHeight;

        const newWidth = Math.random() * width;
        const newHeight = Math.random() * height;

        const btnNo = document.getElementById("btnNo");
        btnNo.style.position = "absolute";
        btnNo.style.left = newWidth + "px";
        btnNo.style.top = newHeight + "px";
      }
    </script>
  </body>
  </html>
  div {
    display: flex;
    flex-direction: column;
    align-items: center;
}


h1 {
    padding: 10px;
    color: #711DB0;
}



button {
    color: brown;
    width: 80px;
    height: 40px;
    border: 3px solid #711DB0;
    border-radius: 10px;
    background-color: transparent;
    font-size: xx-large;

}

#Si {
    grid-row:  5;
    grid-column: 5;
}

#No {
    grid-row: 5;
    grid-column: 6;

}

section {
    display: grid;
    grid-template-columns: 10% 10% 10% 10% 10% 10% 10% 10% 10% 10%;
    grid-template-rows: 10% 10% 10% 10% 10% 10% 10% 10% 10% 10%;
    width: 1200px;
    height: 600px;
    align-items: center;
    justify-items: center;
}

body {
    max-width: 1200px;
    max-height: 673px;
    margin: 0 auto;
    background-image: url(/pngtree-landscapes-wallpaper-images-picture-image_3021437.jpg);
    background-repeat: no-repeat; 
    background-position: center center; 
     background-size: cover;

}

p {
    font-size: xx-large;
    justify-content: center;
    color: pink;
}
 26 changes: 26 additions & 0 deletions26  
me_perdonas.js
@@ -0,0 +1,26 @@
let nob = document.getElementById("No")

nob.addEventListener("mousemove", function() {
    let alto = random(1,10)
    let ancho = random(1,10)
    console.log(alto, ancho)
    nob.style.gridRow = alto;
    nob.style.gridColumn = ancho;

    })


function random(min,max) {
    let numero = Math.floor(Math.random() * (max - min + 1) + min)
    return numero
}

let sib = document.getElementById("Si")

sib.addEventListener("click", function() {
    document.getElementById("p").removeAttribute("hidden")
    console.log("click")
    document.getElementById("1").style.color = "transparent";
    document.getElementById("Si").style.display = "none";
    document.getElementById("No").style.display = "none";
})

