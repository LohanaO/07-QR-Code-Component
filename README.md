## RETO N° 7 100 DAYS OF PROYECTS 

### 07-QR Code Component

<img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1714241420017/7162f83f-950c-4fd1-b2e5-5aa06b467200.jpeg?auto=compress,format&format=webp" alt="Texto alternativo" width="800"/>

### Tecnologias
[![HTML](https://img.shields.io/badge/HTML5-orange?style=flat&logo=html5)](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5)
[![CSS](https://img.shields.io/badge/CSS3-blue?style=flat&logo=css3)](https://developer.mozilla.org/en-US/docs/Web/CSS)

### Ver demo

[Demo](https://lohanao.github.io/07-QR-Code-Component/)

## Desafio
Nuestra misión será crear una tarjeta de código QR, usando HTML y CSS, y lograr que se parezca lo más posible al diseño.
### Los usuarios deberían poder:
Ver un diseño óptimo en pantallas grandes(1200px), medianas(768px) y pequeñas(375px).
### Importante:

Agrega un icono favicon al proyecto.

Agrega una URL fácil de recordar (ej. 07-qr-code-component).

Agrega un título al proyecto (ej. QR Code Component - Frontend Club).

Bonus: Agrega un archivo readme.md al proyecto.

## Solución
### Resolución con HTML y CSS
En este proyecto, utilicé HTML y CSS para crear una tarjeta de codigo QR que muestra una imagen con un código Qr, un titulo y una descripción.

### Estructura HTML
El contenido de la tarjeta de código QR se estructuró utilizando elementos HTML semánticos para mejorar la accesibilidad y el SEO del sitio web. A continuación se muestra una vista general de la estructura HTML utilizada:

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="css/style.css" />
    <link rel="shortcut icon" href="images/favicon-32x32.png" type="image/.png">
    <title>QR Code Component.Frontend Club</title>
  </head>
  <body>
    <main class="container">
      <article class="card">
        <img src="images/image-qr-code.png" alt="QR Code" />
        <h3>Improve your front-end skills by building projects</h3>
        <p>
          Scan the QR code to visit Frontend Mentor and take your coding skills
          to the next level
        </p>
      </article>
    </main>
  </body>
</html>

```


Para lograr el diseño deseado de la tarjeta de producto, sigue estos pasos:

### Definir estilos básicos para el contenedor y la tarjeta:
#### El contenedor debe tener un estilo para centrar su contenido verticalmente y horizontalmente. Puedes lograr esto use display: flex, justify-content: center y align-items: center.
#### La tarjeta debe tener un fondo blanco y algún relleno para separar su contenido del borde. Aplique background-color: white y padding.
#### Use los siguientes estilos CSS le di un ancho maximo a la tarjeta para evitar usar medias queries y una pequeña animación que hace que la card aparezca al cargar la pagina.
```
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@100..900&display=swap');
:root{
--White: hsl(0, 0%, 100%);
--Light-gray: hsl(212, 45%, 89%);
--Grayish-blue: hsl(220, 15%, 55%);
--Dark-blue: hsl(218, 44%, 22%);



}

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body{
    font-family: 'Outfit', sans-serif;
    background-color: var(--Light-gray);
}

.container{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

.card{
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: var(--White);
    max-width: 320px;
    padding: 20px;
    border-radius: 20px;
    text-align: center;
    box-shadow: 0 0 20px 0 rgba(0,0,0,0.2);
    animation: fadeIn 2s ease-in-out;
}

.card img{
    width: 100%;
    border-radius: 10px;
}

.card h3{
    font-size: 22px;
    font-weight: 700;
    margin: 20px 0;
    width: 90%;
    color: var(--Dark-blue);
}

.card p{
    font-size: 15px;
    font-weight: 400;
    color: var(--Grayish-blue);
    width: 80%;
    margin-bottom: 20px;
}

@keyframes fadeIn {
    0% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  }

 ```

## Conclusiones
En conclusión, la creación de esta tarjeta  fue un ejercicio interesante para practicar mis habilidades en HTML y CSS. Espero que este README te haya proporcionado una buena comprensión del proyecto y de mi proceso de desarrollo.

¡Gracias por revisar mi proyecto!

Para cualquier pregunta o comentario, no dudes en contactarme a través de mi correo electrónico: lohaorellano13@gmail.com
