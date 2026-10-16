<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ilumitech | Soluciones Eléctricas Profesionales</title>
    <style>
        :root {
            --azul-fondo: #001a33;
            --azul-card: #002b55;
            --amarillo-ilumitech: #ffcc00;
            --blanco: #ffffff;
            --texto-gris: #e0e0e0;
        }

        body {
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: var(--azul-fondo);
            color: var(--blanco);
            scroll-behavior: smooth;
        }

        /* HEADER - CON TU BANNER LARGO */
        header {
            height: 80vh;
            background-color: #000;
            background-image: linear-gradient(rgba(0, 26, 51, 0.5), rgba(0, 26, 51, 0.7)), url('banner2.jpg'); 
            background-size: cover;
            background-position: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
        }

        header h1 { font-size: 4rem; color: var(--amarillo-ilumitech); margin: 0; text-shadow: 3px 3px 15px #000; }
        header p { font-size: 1.5rem; text-shadow: 2px 2px 10px #000; }

        /* SECCIONES */
        section { padding: 60px 10%; }
        h2.section-title {
            text-align: center;
            color: var(--amarillo-ilumitech);
            font-size: 2.5rem;
            margin-bottom: 50px;
            text-transform: uppercase;
        }

        /* SPOTLIGHT - TU BANNER VERTICAL */
        .promo-spotlight {
            display: flex;
            align-items: center;
            gap: 50px;
            background: var(--blanco);
            color: var(--azul-fondo);
            padding: 60px 10%;
            flex-wrap: wrap;
        }

        .promo-img { flex: 1; min-width: 300px; text-align: center; }
        .promo-img img { max-width: 100%; border-radius: 20px; box-shadow: 0 15px 40px rgba(0,0,0,0.3); }

        .promo-text { flex: 1; min-width: 300px; }
        .promo-text h2 { color: var(--azul-fondo); border-bottom: 4px solid var(--amarillo-ilumitech); width: fit-content; padding-bottom: 10px; }

        /* SOBRE NOSOTROS */
        .about-container { display: flex; align-items: center; gap: 50px; flex-wrap: wrap; }
        .about-img img { width: 300px; border-radius: 50%; border: 5px solid var(--amarillo-ilumitech); filter: drop-shadow(0 0 15px rgba(255,204,0,0.5)); }
        .about-text p { font-size: 1.2rem; color: var(--texto-gris); line-height: 1.8; }

        /* SERVICIOS */
        .services-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 25px; }
        .service-card { background: var(--azul-card); padding: 40px 20px; border-radius: 20px; text-align: center; transition: transform 0.3s; }
        .service-card:hover { transform: translateY(-10px); border-bottom: 5px solid var(--amarillo-ilumitech); }
        .service-card h3 { color: var(--amarillo-ilumitech); font-size: 1.4rem; }

        /* SECCIÓN DE VIDEOS (CON 3 VIDEOS) */
        .video-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 30px;
            margin-top: 40px;
        }
        .video-card {
            flex: 1;
            min-width: 300px;
            max-width: 400px;
            background: var(--azul-card);
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.4);
            border: 3px solid var(--amarillo-ilumitech);
            padding: 15px;
        }
        .video-card video {
            width: 100%;
            height: auto;
            border-radius: 10px;
            display: block;
        }
        .video-card h3 {
            color: var(--amarillo-ilumitech);
            text-align: center;
            margin-top: 15px;
            font-size: 1.2rem;
        }

        /* IMPORTANCIA */
        .highlight-box {
            background: linear-gradient(135deg, var(--azul-card), var(--azul-fondo));
            padding: 50px;
            border-radius: 30px;
            text-align: center;
            border: 1px solid rgba(255, 204, 0, 0.2);
            margin: 60px 0;
        }

        /* CONTACTO */
        .contact-container {
            display: flex;
            justify-content: space-around;
            align-items: center;
            flex-wrap: wrap;
            background: var(--blanco);
            color: var(--azul-fondo);
            padding: 50px;
            border-radius: 30px;
        }

        .qr-box img { width: 200px; border: 5px solid var(--azul-fondo); border-radius: 10px; }
        .contact-info { max-width: 400px; }
        .btn-whatsapp {
            display: inline-block;
            background: #25d366;
            color: white;
            padding: 18px 35px;
            text-decoration: none;
            font-size: 1.2rem;
            font-weight: bold;
            border-radius: 50px;
            margin-top: 20px;
            box-shadow: 0 5px 15px rgba(37, 211, 102, 0.4);
        }

        footer { text-align: center; padding: 40px; background: #000; color: var(--texto-gris); }

        @media (max-width: 768px) {
            header h1 { font-size: 3rem; }
            .promo-spotlight, .about-container, .contact-container { flex-direction: column; text-align: center; }
            .promo-text h2 { text-align: center; margin: 0 auto 20px; }
        }
    </style>
</head>
<body>

    <!-- 1. HERO (Banner Largo) -->
    <header>
        <h1>ILUMITECH</h1>
        <p>Iluminamos tu mundo con efectividad</p>
    </header>

    <!-- 2. SPOTLIGHT (Banner Vertical/Flyer) -->
    <section class="promo-spotlight">
        <div class="promo-img">
            <img src="banner1.jpg" alt="Flyer Ilumitech">
        </div>
        <div class="promo-text">
            <h2>Soluciones Profesionales</h2>
            <p>Brindamos servicios eléctricos con altos estándares de calidad, seguridad y eficiencia. ¡Calidad garantizada en cada conexión!</p>
        </div>
    </section>

    <!-- 3. SOBRE NOSOTROS -->
    <section id="nosotros">
        <div class="about-container">
            <div class="about-img">
                <img src="logo.png" alt="Logo Ilumitech">
            </div>
            <div class="about-text">
                <h2 style="text-align: left; border-bottom: 4px solid var(--amarillo-ilumitech); width: fit-content;">¿Qué es Ilumitech?</h2>
                <p>Ilumitech es una empresa dedicada a ofrecer soluciones eléctricas y tecnología eficiente para hogares y negocios. Nuestro objetivo es brindar productos y servicios de calidad que ayuden a iluminar el futuro.</p>
            </div>
        </div>
    </section>

    <!-- 4. SERVICIOS -->
    <section id="servicios">
        <h2 class="section-title">Nuestros Servicios</h2>
        <div class="services-grid">
            <div class="service-card"><h3>Iluminación LED</h3><p>Ahorro y estilo para tu espacio.</p></div>
            <div class="service-card"><h3>Paneles Solares</h3><p>Energía limpia y renovable.</p></div>
            <div class="service-card"><h3>Instalaciones</h3><p>Seguridad en cada conexión.</p></div>
            <div class="service-card"><h3>Mantenimiento</h3><p>Optimización de sistemas eléctricos.</p></div>
        </div>
    </section>

    <!-- 5. VIDEOS (CON 3 VIDEOS) -->
    <section id="videos">
        <h2 class="section-title">Nuestra Tecnología en Acción</h2>
        <div class="video-container">
            
            <!-- Video 1 -->
            <div class="video-card">
                <video controls>
                    <source src="video1.mp4" type="video/mp4">
                    Tu navegador no reproduce el elemento de video.
                </video>
                <h3>Instalaciones de Paneles Solares</h3>
            </div>

            <!-- Video 2 -->
            <div class="video-card">
                <video controls>
                    <source src="video2.mp4" type="video/mp4">
                    Tu navegador no reproduce el elemento de video.
                </video>
                <h3>Mantenimiento de Redes Eléctricas</h3>
            </div>

            <!-- Video 3 -->
            <div class="video-card">
                <video controls>
                    <source src="video3.mp4" type="video/mp4">
                    Tu navegador no reproduce el elemento de video.
                </video>
                <h3>Proyecto de Iluminación LED</h3>
            </div>

        </div>
    </section>

    <!-- 6. IMPORTANCIA -->
    <section id="importancia">
        <div class="highlight-box">
            <h2 style="color: var(--amarillo-ilumitech); border:none;">La importancia de la electricidad</h2>
            <p>La electricidad es fundamental en la vida diaria porque permite iluminar los hogares, utilizar aparatos eléctricos y facilitar el trabajo. Su uso responsable ayuda a ahorrar energía y proteger el ambiente.</p>
        </div>
    </section>

    <!-- 7. CONTACTO -->
    <section id="contacto">
        <div class="contact-container">
            <div class="qr-box">
                <h3>Escanea para contactar</h3>
                <img src="qr.png" alt="QR Code Ilumitech">
            </div>
            <div class="contact-info">
                <h2>¿Listo para brillar?</h2>
                <p>Estamos en Guatemala, Chiquimula. Haz clic abajo y hablemos por WhatsApp de tu proyecto.</p>
                <a href="https://wa.me/50223439382?text=Hola%20Ilumitech,%20deseo%20más%20información" class="btn-whatsapp">
                    💬 Chatear con un experto
                </a>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2023 ILUMITECH - Calidad, Seguridad y Eficiencia Garantizada</p>
    </footer>

</body>
</html>
