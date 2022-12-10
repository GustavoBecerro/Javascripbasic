# Javascripbasic
example


<script src="scripts/main.js"></script>


onst miTitulo = document.querySelector('h1');
miTitulo.textContent = '¡Hola mundo!';

let nombreDeLaVariable;

nombreDeLaVariable = 'Bob';

let nombreDeLaVariable = 'Bob';

nombreDeLaVariable;

let nombreDeLaVariable = 'Bob';
nombreDeLaVariable = 'Steve';

// Esto es un comentario

/*
Esto es un comentario
de varias líneas.
*/

//Condicionales
let helado = 'chocolate';
if (helado === 'chocolate') {
  alert('¡Sí, amo el helado de chocolate!');
} else {
  alert('Awwww, pero mi favorito es el de chocolate...');
}


//Funciones
let nombreDeLaVariable = document.querySelector('h1');
alert('¡Hola!');


function multiplica(num1,num2) {
  let resultado = num1 * num2;
  return resultado;
}


multiplica(4, 7);
multiplica(20, 20);
multiplica(0.5, 3);

//Evento+
document.querySelector('html').onclick = function() {
    alert('¡Ouch! ¡Deja de pincharme!');
}

document.querySelector('html').onclick = function(){};

let miHTML = document.querySelector('html');
miHTML.onclick = function(){};


//sobrecargar sitio web, cargar una img
let miImage = document.querySelector('img');
miImage.onclick = function () {
    let miSrc = miImage.getAttribute('src');
    if (miSrc === 'images/firefox-icon.png') {
      miImage.setAttribute('src','images/firefox2.png');
    } else {
      miImage.setAttribute('src', 'images/firefox-icon.png');
    }
}

//Msj bienvenida
<button>Cambiar de usuario</button>

let miBoton = document.querySelector('button');
let miTitulo = document.querySelector( 'h1');

function estableceNombreUsuario() {
    let miNombre = prompt('Por favor, ingresa tu nombre.');
    localStorage.setItem('nombre', miNombre);
    miTitulo.textContent = 'Mozilla es genial,' + miNombre;
}

if (!localStorage.getItem('nombre')) {
    estableceNombreUsuario();
}
else {
    let nombreAlmacenado = localStorage.getItem('nombre');
    miTitulo.textContent = 'Mozilla es genial,' + nombreAlmacenado;
}

miBoton.onclick = function() {
    estableceNombreUsuario();
}

//Nulo
function estableceNombreUsuario() {
  let miNombre = prompt('Introduzca su nombre.');
  if(!miNombre) {
    estableceNombreUsuario();
  } else {
    localStorage.setItem('nombre', miNombre);
    miTitulo.innerHTML = 'Mozilla is genial, ' + miNombre;
  }
}



