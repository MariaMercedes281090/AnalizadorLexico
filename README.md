# AnalizadorLexico
Analizador lexio en javascrip y html

<!DOCTYPE html>
<html>
<head>
       <h2> <label for="forumlario">Formulario</label> </h2>
</head>    
<body>

<span>Ingresar datos</span></br>
<div class "alert sucess>
<strong>
<div class="panel panel-primary">
<div>
<h4><label for="ubi">Ubicacion:</label></h4>
<blockquote>
<input id="ubicacion" type="text" class "ubi"/></br>
</blockquote>
</div>

<div>
<h4><label for="blo">Bloque:</label></h4>
<blockquote>
<input id="bloque" type="text" class "blo"/></br>
</blockquote>
</div>

<div>
<h4><label for="po">Posicion:</label></h4>
<blockquote>
<input id="posicion" type="text" class "po"/></br>
</blockquote>
</div>

<div>
<h4><label for="res">Referencia:</label></h4>
<blockquote>
<input id="referencia" type="text" class "res"/></br>
</blockquote>
</div>

<div>
<h4><label for="fe">Fecha:</label></h4>
<blockquote>
<input id="fecha" type="text" class "fe"/></br>
</blockquote>
</div>

<h4><input onclick="ValidarCadenaExpReg()" type="button" value="Aceptar" class "btn btn-primary btn-lg" /></h4>
</strong>
</div>

                   
    
</body>
</html>
<script>
    function ValidarCadenaExpReg() {
        // Expresion regular que representa un Email válido
        cadena = "^[0-9]{3}$"; 
		cadena1= "^[A-Z]{1}$";
		cadena2="^[0-9]{1}$";
		cadena4="^[A-Z]{3}[^A-Za-z0-9]{1}[-]{1}[0-9]{3}[-]{1}[0-9]{1}$";
		cadena5="^[0-9]{2}[/]{1}[0-9]{2}[/]{1}[0-9]{4}$";
		re = new RegExp(cadena);
		se = new RegExp(cadena1);
		de = new RegExp(cadena2);
		ge = new RegExp(cadena4);
		he = new RegExp(cadena5);
        if (document.getElementById("ubicacion").value.match(re))
            alert("ingreso ubicacion correctamente");  
        else 
            alert("no ingresado la ubicacion correctamente"); 

		
        if (document.getElementById("bloque").value.match(se))
            alert("ingreso bloque correctamente");
        else
            alert("no ingresado el bloque correctamente");

			
		if (document.getElementById("posicion").value.match(de))
            alert("ingreso posicion correctamente");
        else
            alert("no ingresado la posicion correctamente");


		if (document.getElementById("referencia").value.match(ge))
            alert("ingreso referencia correctamente ");
        else
            alert("no ingresado la referencia correctamente");

			
		if (document.getElementById("fecha").value.match(he))
            alert("ingreso fecha correctamente ");
        else
            alert("no ingresado la fecha correctamente");	

			
    }
</script>

