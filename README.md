# Actividad-4<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
  
    <script>
        function contarFilas() {
            var filas = document.querySelectorAll("tbody tr").length;
            document.getElementById("total-personas").innerText = "Total de personas: " + filas;
        }
        window.onload = contarFilas;
    </script>
    <title>Actividad 4</title>
</head>
<body>
    <div class="cuadro">
        <table border="2">
            <thead>
                <tr>
                    <th><strong>Nombre:</strong></th>
                    <th><strong>Curso:</strong></th>
                    <th><strong>Maestro:</strong></th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Eriberto</td>
                    <td>Programación Web</td>
                    <td>Angel Soriano</td>
                </tr>
                <tr>
                    <td>Juan</td>
                    <td>Cibersecurity</td>
                    <td>Angel Soriano</td>
                </tr>
                <tr>
                    <td>Pedro</td>
                    <td>Big Data</td>
                    <td>Angel Soriano</td>
                </tr>
                <tr>
                    <td>Pablo</td>
                    <td>Diseño grafico</td>
                    <td>Angel Soriano</td>
                </tr>
                <h1  style="font-family: Verdana, Geneva, Tahoma, sans-serif ; color: blueviolet;" ><strong>Tabla realizada por Eriberto</strong></h1>
            </tbody>
            <tfoot>
                <tr>
                    <td colspan="3" id="total-personas"></td>
                </tr>
            </tfoot>
        </table>
    </div>
   
    <style>
        .formulario label {
            display: inline-block;
            width: 80px; 
        }
        .formulario input, .formulario select {
            margin-bottom: 10px;
        }
        .formulario .boton {
            background-color: blue;
            color: rgb(255, 255, 255);
            margin-left: 40px;
        }
    </style>
</head>
<body>
    <section>
        <h1>Formulario de Registro</h1>
        <form action="Formulario" class="formulario">
            <label for="Nombre">Nombre:</label>
            <input type="text" id="Nombre" name="Nombre"><br>

            <label for="Correo">Correo:</label>
            <input type="email" id="email" name="email"><br>

            <label for="Edad">Edad:</label>
            <input type="number" id="Edad" name="Edad"><br>

            <label for="Sexo">Sexo:</label>
            <select name="Sexo" id="Sexo">
                <option value="Hombre">Hombre</option>
                <option value="Mujer">Mujer</option>
                <option value="Ind">Prefiero no decirlo</option>
            </select><br>

            <label for="temas"><strong>Temas de la clase:</strong></label><br>
            <input type="checkbox" name="tema" value="TI">Tecnología<br>
            <input type="checkbox" name="tema" value="IA">Inteligencia Artificial<br><br>

            <button class="boton">Enviar</button>
        </form>
    

    <style>
        body {
            background-color: rgb(239, 195, 106);
        }
    </style>
</body>
</html>
