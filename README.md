<!DOCTYPE html>
<html lang="es">

<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Sistema Control de Salidas QR</title>


<style>

*{
    box-sizing:border-box;
    font-family:'Segoe UI', Arial, sans-serif;
}


body{

    margin:0;

    background:#08783f;

    min-height:100vh;

    padding-top:100px;

}



/* =====================
   ENCABEZADO
===================== */


.header{

    position:fixed;

    top:0;

    left:0;

    width:100%;

    height:95px;

    background:#056331;

    color:white;

    display:flex;

    align-items:center;

    justify-content:space-between;

    padding:10px 35px;

    box-shadow:0 4px 12px rgba(0,0,0,.3);

    z-index:1000;

}



.logo img{

    width:75px;

    height:75px;

    object-fit:contain;

    border-radius:10px;

}



.titulo{

    text-align:center;

    flex:1;

}



.titulo h2{

    margin:0;

    font-size:25px;

}



.titulo p{

    margin:5px;

    font-size:15px;

}



.usuario{

    text-align:right;

    font-size:14px;

}



/* =====================
   CONTENEDOR
===================== */


.contenedor{

    display:flex;

    justify-content:center;

    align-items:center;

    padding:30px;

}



/* =====================
   TARJETA
===================== */


.card{

    width:450px;

    background:white;

    border-radius:20px;

    box-shadow:0 10px 30px rgba(0,0,0,.35);

    overflow:hidden;

}



/* CABECERA TARJETA */


.card-header{

    background:#08783f;

    color:white;

    text-align:center;

    padding:20px;

}


.card-header h3{

    margin:0;

}



/* CUERPO */


.card-body{

    padding:25px;

}



.estado{

    text-align:center;

    font-size:45px;

    color:#08783f;

}



.mensaje{

    text-align:center;

    font-weight:bold;

    color:#08783f;

    margin-bottom:20px;

}



/* DATOS */


.dato{

    background:#f1f5f2;

    padding:12px;

    border-radius:10px;

    margin-bottom:10px;

}



/* OTP */


.otp{

    margin-top:20px;

    padding:15px;

    background:#e8f5e9;

    border-left:5px solid #08783f;

    border-radius:10px;

}



input{

    width:100%;

    padding:12px;

    margin-top:10px;

    border-radius:8px;

    border:1px solid #ccc;

    text-align:center;

    font-size:20px;

    letter-spacing:8px;

}



/* BOTONES */


button{

    width:100%;

    padding:14px;

    margin-top:15px;

    border:none;

    border-radius:10px;

    background:#08783f;

    color:white;

    font-size:16px;

    cursor:pointer;

}



button:hover{

    background:#056331;

}



.secundario{

    background:white;

    color:#08783f;

    border:2px solid #08783f;

}



/* =====================
 RESPONSIVE
===================== */


@media(max-width:600px){


.header{

    height:auto;

    flex-direction:column;

    position:relative;

}


body{

    padding-top:0;

}


.usuario{

    text-align:center;

}



.card{

    width:100%;

}



}


</style>


</head>



<body>
<!-- =====================
     ENCABEZADO
===================== --><header class="header">
<div class="logo"><img src="https://i.ibb.co/ymbvfZSb/tulcan.jpg" alt="Cooperativa Tulc&aacute;n" /></div>
<div class="titulo">
<h2>COOPERATIVA TULC&Aacute;N</h2>
<p>Sistema de Control de Salidas mediante C&oacute;digo QR</p>
</div>
<div class="usuario">Usuario: <br />Funcionario Institucional <br />29/07/2026</div>
</header><!-- =====================
     FORMULARIO
===================== -->
<div class="contenedor">
<div class="card">
<div class="card-header">
<h3>Validaci&oacute;n de Salida QR</h3>
</div>
<div class="card-body">
<div class="estado">✔</div>
<div class="mensaje">QR VALIDADO CORRECTAMENTE</div>
<div class="dato"><b>C&eacute;dula:</b> 0401752183</div>
<div class="dato"><b>Funcionario:</b> Galo David Jativa Bravo</div>
<div class="dato"><b>Cargo:</b> Supervisor de Seguridades de la Informaci&oacute;n</div>
<div class="dato"><b>Agencia:</b> Matriz Tulc&aacute;n</div>
<div class="dato"><b>Fecha salida:</b> 29/07/2026 15:30:25</div>
<hr />
<h3 style="text-align: center;">🔐 Validaci&oacute;n OTP</h3>
<div class="otp">Se envi&oacute; un c&oacute;digo de seguridad al celular registrado: <br /><br /><b> Celular: 099*****25 </b></div>
<input type="text" maxlength="6" placeholder="000000" /> <button> Validar C&oacute;digo OTP </button> <button class="secundario"> Reenviar OTP </button><hr /><button> ✔ Confirmar Registro de Salida </button></div>
</div>
</div>
</body>

</html>
