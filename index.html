<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Modelo Anatómico - 6 Capas con Reset</title>
    <style>
        /* --- ESTILOS GENERALES --- */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #1a252f;
            color: #ecf0f1;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 20px;
            margin: 0;
            min-height: 100vh;
        }

        h1 { 
            color: #2ecc71; 
            margin-bottom: 5px; 
            text-align: center;
        }
        
        p.instrucciones { 
            color: #bdc3c7; 
            margin-bottom: 15px; 
            text-align: center; 
            max-width: 600px;
            line-height: 1.5;
        }

        /* --- ESTILO DEL BOTÓN DE RESET --- */
        #btn-reset {
            background-color: #e74c3c;
            color: white;
            border: none;
            padding: 10px 25px;
            font-size: 16px;
            font-weight: bold;
            border-radius: 5px;
            cursor: pointer;
            margin-bottom: 20px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.3);
            transition: background-color 0.3s, transform 0.1s;
        }

        #btn-reset:hover {
            background-color: #c0392b;
        }

        #btn-reset:active {
            transform: scale(0.95); /* Se hunde un poquito al hacer clic */
        }

        /* --- CONTENEDOR PRINCIPAL (FONDO FINAL / HUESOS) --- */
        #modelo-interactivo {
            width: 400px; 
            height: 600px; 
            background-image: url('oseo.jpg'); /* CAPA 6: HUESOS */
            background-size: 400px 600px; 
            background-position: top left;
            border: 5px solid #2c3e50;
            border-radius: 8px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.8);
            display: flex;
            flex-wrap: wrap; 
            cursor: crosshair;
            overflow: hidden; 
        }

        /* --- CAPA 1: PIEL (ESTADO INICIAL) --- */
        .pedacito {
            box-sizing: border-box;
            background-image: url('cuerpo.jpg'); 
            background-size: 400px 600px; 
            border-radius: 3px; 
            transition: transform 0.1s, opacity 0.2s;
        }

        /* --- CAPAS INTERMEDIAS Y FINALES --- */
        .pedacito.musculo { background-image: url('musculo.jpg'); }
        .pedacito.circulatorio { background-image: url('circulatorio.jpg'); }
        .pedacito.nervioso { background-image: url('nervioso.jpg'); }
        .pedacito.organo { background-image: url('organo.jpg'); }
        .pedacito.hueso {
            background-image: none;
            background-color: transparent;
        }

        /* Efecto al pasar el mouse por los pedacitos */
        .pedacito:hover {
            transform: scale(0.85);
            z-index: 10;
        }
    </style>
</head>
<body>

    <h1>Exploración Anatómica Profunda</h1>
    <p class="instrucciones">
        <strong>Instrucciones:</strong> Haz clic sostenido y arrastra el ratón sobre la silueta. <br>
        Capas: <strong>Piel ➔ Músculo ➔ Circulatorio ➔ Nervioso ➔ Órganos ➔ Huesos</strong>.
    </p>

    <button id="btn-reset" onclick="restaurarCapas()">🔄 Restaurar Piel</button>

    <div id="modelo-interactivo"></div>

    <script>
        const contenedor = document.getElementById('modelo-interactivo');
        
        const anchoContenedor = 400; 
        const altoContenedor = 600;
        const tamañoPedacito = 25; 

        const columnas = anchoContenedor / tamañoPedacito;
        const filas = altoContenedor / tamañoPedacito;

        contenedor.addEventListener('dragstart', (e) => e.preventDefault());

        // CREACIÓN DE LA CUADRÍCULA
        for (let y = 0; y < filas; y++) {
            for (let x = 0; x < columnas; x++) {
                let pedacito = document.createElement('div');
                pedacito.classList.add('pedacito');
                pedacito.style.width = `${tamañoPedacito}px`;
                pedacito.style.height = `${tamañoPedacito}px`;

                let posX = -(x * tamañoPedacito);
                let posY = -(y * tamañoPedacito);
                pedacito.style.backgroundPosition = `${posX}px ${posY}px`;

                pedacito.dataset.capa = 0;

                pedacito.addEventListener('mousedown', function() { desgarrar(this); });
                pedacito.addEventListener('mouseenter', function(e) {
                    if (e.buttons === 1) { desgarrar(this); }
                });

                contenedor.appendChild(pedacito);
            }
        }

        // LÓGICA DE LAS 6 CAPAS
        function desgarrar(elemento) {
            let capaActual = parseInt(elemento.dataset.capa);

            switch(capaActual) {
                case 0: 
                    elemento.classList.add('musculo');
                    elemento.dataset.capa = 1;
                    break;
                case 1: 
                    elemento.classList.remove('musculo');
                    elemento.classList.add('circulatorio');
                    elemento.dataset.capa = 2;
                    break;
                case 2: 
                    elemento.classList.remove('circulatorio');
                    elemento.classList.add('nervioso');
                    elemento.dataset.capa = 3;
                    break;
                case 3: 
                    elemento.classList.remove('nervioso');
                    elemento.classList.add('organo');
                    elemento.dataset.capa = 4;
                    break;
                case 4: 
                    elemento.classList.remove('organo');
                    elemento.classList.add('hueso');
                    elemento.dataset.capa = 5;
                    break;
            }
        }

        // --- NUEVA FUNCIÓN PARA EL BOTÓN DE RESET ---
        function restaurarCapas() {
            // Selecciona todos los pedacitos generados
            let todosLosPedacitos = document.querySelectorAll('.pedacito');
            
            // Recorre cada uno y le quita todas las clases extrañas, devolviéndolo a 0
            todosLosPedacitos.forEach(function(pedacito) {
                pedacito.classList.remove('musculo', 'circulatorio', 'nervioso', 'organo', 'hueso');
                pedacito.dataset.capa = 0; // Vuelve a ser Piel
            });
        }
    </script>

</body>
</html>