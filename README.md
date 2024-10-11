<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Midnightsnacks</title>
    <style>
        /* Esquema de colores */
        :root {
            --azul-claro: #add8e6;
            --azul-normal: #0000ff;
            --azul-oscuro: #00008b;
            --blanco: #ffffff;
            --gris-claro: #f2f2f2;
            --gris: #cccccc;
        }

        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: var(--gris-claro);
            color: var(--azul-oscuro);
        }

        /* Navegación */
        header {
            background-color: var(--azul-normal);
            padding: 20px;
            text-align: center;
            color: var(--blanco);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav a {
            margin: 0 15px;
            color: var(--blanco);
            text-decoration: none;
            font-weight: bold;
        }

        nav a:hover {
            text-decoration: underline;
        }

        /* Sección Principal */
        #principal {
            padding: 40px 20px;
            text-align: center;
        }

        #principal h2 {
            color: var(--azul-oscuro);
        }

        .productos {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
                margin-top: 30px;
        }

        .producto {
            background-color: var(--blanco);
            border: 1px solid var(--gris);
            border-radius: 8px;
            width: 250px;
            padding: 15px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            transition: transform 0.2s;
        }

        .producto:hover {
            transform: scale(1.05);
        }

        .producto img {
            width: 100%;
            height: 150px;
            object-fit: cover;
            border-radius: 4px;
        }

        .producto h3 {
            margin: 15px 0 10px;
            color: var(--azul-normal);
        }

        .producto p {
            color: var(--gris);
        }

        .producto .precio {
            font-size: 1.2em;
            color: var(--azul-oscuro);
            margin: 10px 0;
        }

        .producto button {
            background-color: var(--azul-normal);
            color: var(--blanco);
            border: none;
            padding: 10px 20px;
            border-radius: 4px;
            cursor: pointer;
            font-size: 1em;
        }

        .producto button:hover {
            background-color: var(--azul-oscuro);
        }

        /* Sección Contacto */
        #contacto {
            background-color: var(--azul-claro);
            padding: 40px 20px;
            color: var(--azul-oscuro);
        }

        #contacto h2 {
            text-align: center;
            margin-bottom: 30px;
        }

        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background-color: var(--blanco);
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .contact-form label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }

        .contact-form input, 
        .contact-form textarea {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid var(--gris);
            border-radius: 4px;
            resize: vertical;
        }

        .contact-form button {
            background-color: var(--azul-normal);
            color: var(--blanco);
            border: none;
            padding: 10px 20px;
            border-radius: 4px;
            cursor: pointer;
            font-size: 1em;
        }

        .contact-form button:hover {
            background-color: var(--azul-oscuro);
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 20px;
            background-color: var(--azul-normal);
            color: var(--blanco);
            position: fixed;
            width: 100%;
            bottom: 0;
        }

        /* Responsividad */
        @media (max-width: 600px) {
            .productos {
                flex-direction: column;
                align-items: center;
            }

            footer {
                position: static;
            }
        }
    </style>
</head>
<body>

    <!-- Encabezado y Navegación -->
    <header>
        <h1>Midnightsnacks</h1>
        <nav>
            <a href="#principal">Principal</a>
            <a href="#contacto">Contacto</a>
        </nav>
    </header>

    <!-- Sección Principal -->
    <section id="principal">
        <h2>Productos Destacados</h2>
        <div class="productos">
            <!-- Producto 1: Ring Pops -->
            <div class="producto">
                <img src="https://via.placeholder.com/250x150?text=Ring+Pops" alt="Ring Pops">
                <h3>Ring Pops</h3>
                <p>Deliciosos y coloridos Ring Pops para endulzar tu día.</p>
                <div class="precio">$0.75</div>
                <button>Comprar</button>
            </div>
            <!-- Producto 2: Chicles -->
            <div class="producto">
                <img src="https://via.placeholder.com/250x150?text=Chicles" alt="Chicles">
                <h3>Chicles</h3>
                <p>Chicles de sabores variados para disfrutar en cualquier momento.</p>
                <div class="precio">$0.50</div>
                <button>Comprar</button>
            </div>
            <!-- Puedes agregar más productos siguiendo el mismo formato -->
        </div>
    </section>

    <!-- Sección Contacto -->
    <section id="contacto">
        <h2>Contacto</h2>
        <div class="contact-form">
            <form action="#" method="post">
                <label for="nombre">Nombre:</label>
                <input type="text" id="nombre" name="nombre" required>

                <label for="email">Correo Electrónico:</label>
                <input type="email" id="email" name="email" required>

                <label for="mensaje">Mensaje:</label>
                <textarea id="mensaje" name="mensaje" rows="5" required></textarea>

                <button type="submit">Enviar</button>
            </form>
        </div>
    </section>

    <!-- Pie de Página -->
    <footer>
        &copy; 2024 Midnightsnacks. Todos los derechos reservados.
    </footer>

</body>
</html>
