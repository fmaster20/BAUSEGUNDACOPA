<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>2da Copa del Under - Freestyle Dominicano</title>
    <style>
        :root {
            --primary: #121212;
            --secondary: #1E1E1E;
            --accent: #FF5A5F;
            --accent-dark: #E53E3E;
            --light: #FFFFFF;
            --urban-graffiti: #06D6A0;
            --urban-dark: #2B2D42;
        }
        
        body {
            font-family: 'Urbanist', sans-serif;
            margin: 0;
            padding: 0;
            background-color: var(--primary);
            color: var(--light);
            line-height: 1.6;
        }
        
        header {
            background: linear-gradient(to right, var(--urban-dark), var(--primary));
            padding: 20px 0;
            text-align: center;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.5);
            border-bottom: 3px solid var(--urban-graffiti);
        }
        
        .logo {
            max-width: 250px;
            height: auto;
            margin: 0 auto;
            transition: transform 0.5s ease;
        }
        
        .logo:hover {
            transform: rotate(360deg);
        }
        
        .hero {
            background: url('cover.jpg') no-repeat center center/cover;
            height: 70vh;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
        }
        
        .hero::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
        }
        
        .hero-content {
            z-index: 1;
            text-align: center;
            padding: 20px;
        }
        
        .hero h1 {
            font-size: 4rem;
            margin-bottom: 10px;
            color: var(--urban-graffiti);
            text-transform: uppercase;
            text-shadow: 3px 3px 0 var(--primary);
            letter-spacing: 2px;
        }
        
        .hero p {
            font-size: 1.8rem;
            margin-bottom: 20px;
            font-weight: bold;
        }
        
        .date {
            font-size: 2.2rem;
            font-weight: bold;
            color: var(--accent);
            margin: 20px 0;
            background: rgba(0, 0, 0, 0.7);
            display: inline-block;
            padding: 10px 25px;
            border-radius: 50px;
            border: 2px solid var(--urban-graffiti);
        }
        
        .cta-button {
            display: inline-block;
            background-color: var(--accent);
            color: var(--light);
            padding: 15px 35px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 2px;
            transition: all 0.3s ease;
            margin: 15px;
            font-size: 1.1rem;
            border: none;
            box-shadow: 0 4px 0 var(--accent-dark);
        }
        
        .cta-button:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(255, 90, 95, 0.4);
            background-color: var(--accent-dark);
        }
        
        .info-section {
            padding: 80px 20px;
            text-align: center;
            background-color: var(--secondary);
            background-image: linear-gradient(
                to bottom,
                var(--secondary),
                var(--primary)
            );
        }
        
        .info-section h2 {
            font-size: 3rem;
            margin-bottom: 40px;
            color: var(--urban-graffiti);
            text-transform: uppercase;
            letter-spacing: 3px;
        }
        
        .details {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 30px;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .detail-card {
            flex: 1;
            min-width: 250px;
            background: rgba(255, 255, 255, 0.05);
            padding: 30px;
            border-radius: 10px;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s ease;
        }
        
        .detail-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.3);
            border-color: var(--urban-graffiti);
        }
        
        .detail-card h3 {
            color: var(--accent);
            margin-top: 0;
            font-size: 1.5rem;
            border-bottom: 2px solid var(--urban-graffiti);
            display: inline-block;
            padding-bottom: 5px;
        }
        
        .detail-card p {
            font-size: 1.1rem;
        }
        
        footer {
            background-color: var(--primary);
            padding: 30px;
            text-align: center;
            font-size: 1rem;
            border-top: 1px solid var(--urban-graffiti);
        }
        
        footer p {
            margin: 5px 0;
        }
        
        .design-credit {
            color: var(--urban-graffiti);
            font-weight: bold;
        }
        
        @media (max-width: 768px) {
            .hero {
                height: 60vh;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .hero p {
                font-size: 1.3rem;
            }
            
            .date {
                font-size: 1.5rem;
            }
            
            .info-section h2 {
                font-size: 2rem;
            }
            
            .cta-button {
                padding: 12px 25px;
                font-size: 1rem;
                margin: 10px;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Urbanist:wght@400;700;900&display=swap" rel="stylesheet">
</head>
<body>
    <header>
        <img src="BAU.jpg" alt="Copa del Under Logo" class="logo">
    </header>
    
    <section class="hero">
        <div class="hero-content">
            <h1>COPA DEL UNDER</h1>
            <p>2DA EDICIÓN</p>
            <div class="date">SÁBADO 27 DE SEPTIEMBRE</div>
            <a href="https://wa.me/18092186244?text=Hola,%20¿cómo%20obtengo%20mi%20boleta%20para%20la%20Copa%20del%20Under?" class="cta-button">COMPRAR BOLETAS</a>
            <a href="#info" class="cta-button">MÁS INFORMACIÓN</a>
        </div>
    </section>
    
    <section class="info-section" id="info">
        <h2>INFORMACIÓN DEL EVENTO</h2>
        <div class="details">
            <div class="detail-card">
                <h3>FECHA Y HORA</h3>
                <p>Sábado 27 de Septiembre</p>
                <p>4:00 PM</p>
            </div>
            <div class="detail-card">
                <h3>UBICACIÓN</h3>
                <p>Mercedez 313</p>
                <p>Zona Colonial</p>
            </div>
            <div class="detail-card">
                <h3>PRECIOS</h3>
                <p>Cover: $350 P/P</p>
                <p>Premios en efectivo</p>
            </div>
            <div class="detail-card">
                <h3>VIAJE ESPECIAL</h3>
                <p>Viaje al Salvador incluido</p>
                <p>Para los ganadores</p>
            </div>
        </div>
    </section>
    
    <footer>
        <p>© 2023 Copa del Under - Todos los derechos reservados</p>
        <p>Organizado por BAU | <span class="design-credit">Diseñado por La Oposición</span></p>
    </footer>
</body>
</html>
