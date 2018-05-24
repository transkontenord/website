---
title: Contacto
layout: page
lang: es
permalink: /es/contacto
banner: /assets/uploads/images/originales/banner-contacto.jpg
---


<form enctype="multipart/form-data" action="https://paneles.gestiondecuenta.com/comprobar-formulario/" method="POST" id ="formGenGdc" onsubmit="return ValidarCaptcha();">

<label for="nombre">* Nombre</label>
<input type="text" name="nombre" class="todo"  />

<label for="email">* Cuenta de correo</label>
<input type="email" name="email" class="todo"  />

<label for="mensaje">Mensaje</label>
<textarea name="mensaje" class="todo" rows="8" cols="50"></textarea>

<label for="entradaVerificacion">Captcha</label>
<input type="hidden" value="" id="verificacionOculto" name="verificacionOculto"/>
<div id="muestraVerificacion"></div>
<input type="text" id="entradaVerificacion" name="entradaVerificacion" />


<input type="hidden" name="redirigir" class="" value="http://www.txorua.com/gracias.html" />
<input type="hidden" name="recipe" class="" value="txorua@txorua.com" />
<input type="hidden" name="asunto" class="" value="Envío formulario desde txorua.com" />
<input type="hidden" name="required" class="" value="nombre;email" />
<input type="hidden" name="dominio" class="" value="txorua.com" />
<input type="hidden" name="idioma" class="" value="es" />
<input type="submit" name="enviar" class="" value="Enviar" />

</form>

<script type="text/javascript">
  var a = Math.ceil(Math.random() * 10);
  var b = Math.ceil(Math.random() * 10);
  var c = a + b;
  function GenerarCaptcha(){
    var hidden = document.getElementById("verificacionOculto");
    var inputField = document.getElementById("entradaVerificacion");
    var muestra = document.getElementById("muestraVerificacion");
    muestra.innerHTML = a + " + " + b + " = ";
    hidden.value = c ;
  }
  function ValidarCaptcha(){
    var inputField = document.getElementById("entradaVerificacion");
    if (inputField.value == c) return true;
    else{inputField.style.color="red"; return false;}
  }
  GenerarCaptcha();
</script>


{% include google-map.html %}
