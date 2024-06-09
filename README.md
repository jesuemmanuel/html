//programa que consiste en ingresar un numero en el rango del 1 al 999, una vez ingresado se mostrara la tabla de multiplicar de el número ingresado


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CicloFor</title>
    <script>
      // Inicializacion de Variables
        var numero,res,tabla="";

      //Bienvenida e intrduccion de datos por parte del Usuario
        alert("-----Bienvenido a Tablas de Multiplicar del 1 al 999-----");
        numero=prompt("Introduzca el numero(Del 1 al 999):");

      //Validacion del Numero para saber si esta dentro del Rango
         if(numero <= 0 || numero > 999){
            alert("Numero no valido");
         }
         else{
            for(var i=1;i<=10;i++){
               res= numero * i; //Operacion de multiplicacion
                  //Unidades
                  if(res < 10){
                     if(i<10){
                        tabla=(tabla + "  " + numero + "  "+ "*" + "    " + i + "   " + " =" + "        " + res + "\n" );
                     }
                     else{
                        tabla=(tabla + "  " + numero + "  "+ "*" + "  " + i + "   " + " =" + "         " + res + "\n" );
                     }
                  }
                  else if(res >= 10 && res < 100){
                  //Decenas
                     if(i<10){
                        tabla=(tabla + "  " + numero + "  "+ "*" + "    " + i + "   " + " =" + "      " + res + "\n");
                     }
                     else{
                        tabla=(tabla + "  " + numero + "  "+ "*" + "  " + i + "   " + " =" + "      " + res + "\n");
                     }
                  }
                  else if(res>=100 && res<1000){
                  //Centenas
                     if(i<10){
                        tabla=(tabla + "  " + numero + "  "+ "*" + "    " + i + "   " + " =" + "    " + res + "\n");
                     }
                     else{
                        tabla=(tabla + "  " + numero + "  "+ "*" + "  " + i + "   " + " =" + "    " + res + "\n");
                     }
                  }
                  else{
                  //Miles
                     if(i<10){
                        tabla=(tabla + "  " + numero + "  "+ "*" + "    " + i + "   " + " =" + "  " + res + "\n");
                     }
                     else{
                        tabla=(tabla + "  " + numero + "  "+ "*" + "  " + i + "   " + " =" + "  " + res + "\n");
                  }
               }

               }
         
               alert(tabla);
            }
        
    </script>

</head>
<body>
    
</body>
</html>
