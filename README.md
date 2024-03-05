# pag-web
!DOCTYPE html>
<html>
<head>
<title>ESTETICA ANIMAL</title>
<link rel="stylesheet" href="estilo.css"> 
<style>
    #dialog {
        display: none;
        position: fixed;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%) ;
        background-color: #ffffff;
        padding: 20px;
        border: 1px solid #ffffff;
        border-radius: 8px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        z-index: 1000;
}
    #overlay {
        display: none;
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, 0.5);
        z-index: 999;
    }
    </style>
</head>
<body>

<h1>BIENVENIDO A LA ESTETICA ANIMAL DEL EQUIPO 5</h1>
<h2>Ingrese el nombre de su mascota para mostrarla!!</h2>
<button onclick="showDialog()">Ingresar nombre de mascota</button>
<div id="dialog">
    <h3>Ingresa el nombre de tu mascota</h4>
    <input type="text" id="variableInput">
    <button onclick="addVariable()">Agregar</button>
    <button onclick="hideDialog()">Cancelar</button>
</div>
<div id="mascotas"></div>
<script>
