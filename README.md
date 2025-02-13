# gitbubpagtest
pagina web
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lechona JG La Original</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f4f4f9;
        }
        h1 {
            color: #333;
            margin-top: 20px;
        }
        .products {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 30px;
        }
        .product-card {
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
            width: 200px;
            padding: 15px;
        }
        .product-card img {
            width: 100%;
            border-radius: 10px;
        }
        .product-card h3 {
            font-size: 18px;
            color: #555;
        }
        .buy-button {
            display: inline-block;
            margin-top: 10px;
            padding: 10px 15px;
            background-color: #25D366;
            color: white;
            border: none;
            border-radius: 5px;
            text-decoration: none;
            cursor: pointer;
        }
        .buy-button:hover {
            background-color: #1ebe5a;
        }
    </style>
</head>
<body>
    <h1>Lechona JG La Original</h1>
    <section class="products">
        <div class="product-card">
            <img src="https://www.viveelmeta.com/wp-content/uploads/2024/01/premio-plato-de-lechona-5666.jpg" alt="Lechona Por Porciones">
            <h3>Lechona Por Porciones</h3>
            <button class="buy-button" onclick="comprar('Lechona Por Porciones')">Comprar ahora</button>
        </div>
        <div class="product-card">
            <img src="https://lechonaelgordo.com/wp-content/uploads/2021/08/Lechona.jpg" alt="Cojín de Lechona">
            <h3>Cojín de Lechona</h3>
            <button class="buy-button" onclick="comprar('Cojín de Lechona')">Comprar ahora</button>
        </div>
        <div class="product-card">
            <img src="https://lechonaelgordo.com/wp-content/uploads/2021/08/DSC_00841-scaled.jpg" alt="Lechona Entera">
            <h3>Lechona Entera</h3>
            <button class="buy-button" onclick="comprar('Lechona Entera')">Comprar ahora</button>
        </div>
        <div class="product-card">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR3QHZs__HtJZQsrYl7Za11lq5sovisXzzRfw&s" alt="Delicioso Chirizos">
            <h3>Delicioso Chirizos</h3>
            <button class="buy-button" onclick="comprar('Delicioso Chirizos')">Comprar ahora</button>
        </div>
        <div class="product-card">
            <img src="https://irp-cdn.multiscreensite.com/1595a6db/dms3rep/multi/092.jpg" alt="Empanadas de Lechona">
            <h3>Empanadas de Lechona</h3>
            <button class="buy-button" onclick="comprar('Empanadas de Lechona')">Comprar ahora</button>
        </div>
        
    </section>

    <script>
        function comprar(producto) {
            const numeroWhatsApp = "573107289414"; // Tu número de WhatsApp en formato internacional
            const mensaje = `👋 ¡Hola!, Me interesa el ${producto}. de Fashion Store. 😍 ¿Podrías darme más información? ¡Estoy emocionado por saber más y posiblemente hacer mi compra! 🛒🔥`;
            const url = `https://api.whatsapp.com/send?phone=${numeroWhatsApp}&text=${encodeURIComponent(mensaje)}`;
            window.location.href = url;
        }
    </script>
</body>
</html>
