# Cozcatl
Venta
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>COZCATL - Joyería de Plata</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            color: #333;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #333;
            color: #fff;
            padding: 20px;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #444;
        }
        nav a {
            color: #fff;
            padding: 15px 20px;
            text-decoration: none;
        }
        nav a:hover {
            background-color: #555;
        }
        section {
            padding: 20px;
        }
        .catalog-item {
            border: 1px solid #ddd;
            padding: 15px;
            margin: 10px 0;
            background-color: #fff;
        }
        .catalog-item img {
            max-width: 100%;
            height: auto;
        }
        .catalog-item button {
            background-color: #28a745;
            color: white;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
        }
        .catalog-item button.apartar {
            background-color: #ffc107;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
        footer a {
            font-size: 12px;
            color: #fff;
            text-decoration: none;
        }
    </style>
</head>
<body>
    <header>
        <h1>COZCATL - Joyería de Plata</h1>
    </header>
    <nav>
        <a href="#catalogo">Catálogo</a>
        <a href="#contacto">Contacto</a>
    </nav>
    <section id="catalogo">
        <h2>Catálogo</h2>

        <div class="catalog-item">
            <h3>Anillo de Plata</h3>
            <img src="ruta/a/tu-imagen-anillo.jpg" alt="Anillo de Plata">
            <p>Elegante anillo de plata 925. Precio: $500 MXN</p>
            <button onclick="comprar()">Comprar</button>
            <button class="apartar" onclick="apartar()">Apartar</button>
        </div>

        <div class="catalog-item">
            <h3>Collar de Plata</h3>
            <img src="ruta/a/tu-imagen-collar.jpg" alt="Collar de Plata">
            <p>Hermoso collar de plata con diseño moderno. Precio: $800 MXN</p>
            <button onclick="comprar()">Comprar</button>
            <button class="apartar" onclick="apartar()">Apartar</button>
        </div>

    </section>
    <section id="contacto">
        <h2>Contacto</h2>
        <p>Email: <input type="text" id="email" value="info@cozcatl.com"></p>
        <p>Teléfono: <input type="text" id="telefono" value="+52 123 456 7890"></p>
        <p>Dirección: <input type="text" id="direccion" value="Calle de la Plata, Ciudad de México, México"></p>
        <button onclick="guardarContacto()">Guardar Cambios</button>
    </section>
    <footer>
        &copy; 2024 COZCATL. Todos los derechos reservados.
        <br>
        <a href="https://www.cozcatl.com">Visita nuestra página oficial</a>
    </footer>

    <script>
        function comprar() {
            alert('Producto añadido al carrito de compras.');
        }
        function apartar() {
            alert('Producto apartado. Tienes 24 horas para finalizar la compra.');
        }
        function guardarContacto() {
            let email = document.getElementById('email').value;
            let telefono = document.getElementById('telefono').value;
            let direccion = document.getElementById('direccion').value;
            alert('Contacto actualizado: ' + email + ', ' + telefono + ', ' + direccion);
        }
    </script>
</body>
</html>