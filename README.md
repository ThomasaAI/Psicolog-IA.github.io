<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Thomas AI - Plataforma de Salud Mental</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            background: #121212;
            color: #e0f2f1;
            overflow-x: hidden;
        }
        header, footer {
            background-color: #1a1a1a;
            color: white;
            text-align: center;
            padding: 2em 0;
            position: relative;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        header h1 {
            margin: 0;
            font-size: 4em;
            animation: slideInFromLeft 1s ease-in-out;
            color: #ff4081;
        }
        header p {
            font-size: 1.5em;
            margin: 0.5em 0;
            animation: slideInFromRight 1s ease-in-out;
            color: #ffd740;
        }
        nav {
            background-color: #333;
            overflow: hidden;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        nav a {
            float: left;
            display: block;
            color: white;
            text-align: center;
            padding: 14px 16px;
            text-decoration: none;
            transition: background-color 0.3s, transform 0.3s;
            animation: fadeIn 1s ease-in-out;
        }
        nav a:hover {
            background-color: #ff4081;
            transform: scale(1.1);
        }
        .container {
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
            animation: fadeIn 1.5s ease-in-out;
            background-color: #1a1a1a;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
        }
        .cta-buttons a {
            display: inline-block;
            padding: 12px 24px;
            margin: 10px;
            color: white;
            background-color: #00e676;
            text-decoration: none;
            border-radius: 25px;
            transition: background-color 0.3s, transform 0.3s;
        }
        .cta-buttons a:hover {
            background-color: #1de9b6;
            transform: scale(1.1);
        }
        .testimonial, .service, .blog-post {
            border: 1px solid #00e676;
            padding: 20px;
            margin: 20px 0;
            border-radius: 10px;
            background-color: #2c2c2c;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s;
        }
        .testimonial:hover, .service:hover, .blog-post:hover {
            transform: translateY(-10px);
        }
        footer a {
            color: white;
            text-decoration: none;
        }
        footer a:hover {
            text-decoration: underline;
        }
        .developer-info {
            background-color: #1a1a1a;
            color: white;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
        }
        .developer-info a {
            color: #80cbc4;
            text-decoration: none;
            transition: color 0.3s;
        }
        .developer-info a:hover {
            color: #4db6ac;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        @keyframes slideInFromLeft {
            from { opacity: 0; transform: translateX(-50px); }
            to { opacity: 1; transform: translateX(0); }
        }
        @keyframes slideInFromRight {
            from { opacity: 0; transform: translateX(50px); }
            to { opacity: 1; transform: translateX(0); }
        }
        @keyframes fadeInDown {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        form {
            display: flex;
            flex-direction: column;
        }
        form label {
            margin: 10px 0 5px;
        }
        form input, form textarea {
            padding: 10px;
            margin-bottom: 15px;
            border-radius: 5px;
            border: 1px solid #00e676;
            font-size: 1em;
            background-color: #2c2c2c;
            color: white;
        }
        form input[type="submit"] {
            background-color: #00e676;
            color: white;
            border: none;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.3s;
        }
        form input[type="submit"]:hover {
            background-color: #1de9b6;
            transform: scale(1.05);
        }
        .testimonial p:first-of-type {
            font-style: italic;
        }
        .testimonial p:last-of-type {
            text-align: right;
            font-weight: bold;
        }
        h2, h3 {
            color: #ff4081;
            animation: fadeInDown 1s ease-in-out;
            font-size: 2.5em;
        }
        p {
            line-height: 1.6;
        }
        @media (max-width: 768px) {
            nav a {
                float: none;
                display: block;
                text-align: left;
                padding: 14px;
            }
            .cta-buttons {
                text-align: center;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Thomas AI</h1>
        <p>Diagnósticos Tempranos y Apoyo Emocional a Través de IA</p>
    </header>
    <nav>
        <a href="#inicio">Inicio</a>
        <a href="#biografia">Biografía</a>
        <a href="#servicios">Servicios</a>
        <a href="#blog">Blog</a>
        <a href="#contacto">Contacto</a>
        <a href="#faqs">FAQs</a>
        <a href="#desarrolladores">Desarrolladores</a>
    </nav>
    <section id="inicio" class="container">
        <h2>Bienvenido a Thomas AI</h2>
        <p>Thomas AI es una plataforma digital avanzada desarrollada para proporcionar diagnósticos tempranos y precisos de trastornos mentales mediante inteligencia artificial. Nuestro objetivo es ayudar a las personas a comprender y gestionar mejor su salud mental, ofreciendo herramientas y recursos personalizados. Disponible en la Store de ChatGPT-4, Thomas AI es un GPT que proporciona apoyo emocional continuo y consultas en línea con profesionales de la salud mental.</p>
        <h3>Nuestros Servicios</h3>
        <div class="service">
            <h4>Diagnósticos Tempranos</h4>
            <p>Utilizamos algoritmos avanzados de inteligencia artificial para identificar trastornos mentales en sus primeras etapas, permitiendo intervenciones tempranas y efectivas. Nuestra tecnología analiza patrones de comportamiento y lenguaje para proporcionar diagnósticos precisos.</p>
        </div>
        <div class="service">
            <h4>Apoyo Emocional</h4>
            <p>Ofrecemos módulos interactivos y contenido educativo diseñado para proporcionar apoyo emocional personalizado. Nuestros recursos incluyen ejercicios de mindfulness, técnicas de manejo del estrés y herramientas de autoevaluación.</p>
        </div>
        <div class="service">
            <h4>Consultas en Línea</h4>
            <p>Accede a consultas con profesionales de la salud mental a través de nuestra plataforma segura y fácil de usar. Nuestros expertos están disponibles para ofrecer orientación y apoyo cuando más lo necesites.</p>
        </div>
        <h3>Testimonios</h3>
        <div class="testimonial">
            <p>"Thomas AI me ha ayudado a comprender mejor mis emociones y a buscar el apoyo que necesito. Altamente recomendado."</p>
            <p>- Usuario Satisfecho</p>
        </div>
    </section>
    <section id="biografia" class="container">
        <h2>Biografía</h2>
        <h3>Historia de Desarrollo</h3>
        <p>Thomas AI fue desarrollado por un equipo de expertos en inteligencia artificial y salud mental de E&M Soluciones con IA. El proyecto nació con la misión de mejorar el acceso a la atención emocional y el diagnóstico temprano de enfermedades mentales, especialmente en áreas remotas y desatendidas. Nuestra plataforma utiliza algoritmos avanzados de aprendizaje automático para ofrecer apoyo emocional y recursos útiles para aquellos que lo necesitan.</p>
        <h3>Visión y Misión</h3>
        <p><strong>Visión:</strong> Ser el asistente virtual líder en salud mental, proporcionando apoyo emocional y diagnóstico temprano a nivel global.</p>
        <p><strong>Misión:</strong> Mejorar la calidad de vida de las personas mediante el uso de tecnología avanzada para facilitar el acceso a servicios de salud mental y ofrecer apoyo continuo y efectivo.</p>
    </section>
    <section id="blog" class="container">
        <h2>Blog</h2>
        <div class="blog-post">
            <h3>El impacto del COVID-19 en la salud mental: Cómo afrontarlo</h3>
            <p>Exploramos los efectos del COVID-19 en la salud mental y ofrecemos estrategias para manejar el estrés y la ansiedad durante y después de la pandemia. <a href="https://www.unesco.org/es/articles/covid-19-problemas-sociales-y-psicologicos-en-la-pandemia" target="_blank">Artículo</a></p>
        </div>
        <div class="blog-post">
            <h3>Identificando los primeros signos de depresión y ansiedad</h3>
            <p>Una guía detallada para reconocer los síntomas iniciales de trastornos mentales comunes y cómo buscar ayuda. <a href="https://www.inegi.org.mx/contenidos/saladeprensa/boletines/2021/estsociodemo/enbiare_2021.pdf" target="_blank">Artículo</a></p>
        </div>
        <div class="blog-post">
            <h3>La importancia del autocuidado para la salud mental</h3>
            <p>Consejos prácticos sobre cómo implementar prácticas de autocuidado en tu vida diaria para mantener el bienestar mental. <a href="https://www.psicologia-online.com/autocuidado-en-salud-mental-3800.html" target="_blank">Artículo</a></p>
        </div>
        <div class="blog-post">
            <h3>Consejos y Recursos</h3>
            <p>La UNAM pone el servicio de la población un recurso para la salud mental de forma gratuita y anónima ante el panorama de la pandemia.</p>
            <p>En la página online de la Universidad Nacional Autónoma de México (UNAM) puede encontrar un recurso muy valioso que podría ayudarle a evaluar el nivel de riesgo que tiene actualmente en su salud mental ante el panorama de COVID 19, es gratuito y anónimo. <a href="https://coordinaciongenero.unam.mx/2021/10/unam-brinda-ayuda-online-gratuita-para-atender-salud-mental/" target="_blank">Artículo completo</a></p>
        </div>
        <div class="blog-post">
            <h3>Estrategias para mejorar el sueño</h3>
            <p>Consejos y trucos para mejorar la calidad del sueño, crucial para una buena salud mental. <a href="https://www.sleepfoundation.org/sleep-hygiene/healthy-sleep-tips" target="_blank">Artículo</a></p>
        </div>
        <div class="blog-post">
            <h3>Recursos de apoyo en línea para la salud mental</h3>
            <p>Una lista de recursos en línea, incluyendo aplicaciones, sitios web y líneas de ayuda que puedes utilizar para obtener apoyo emocional y psicológico. <a href="https://www.mentalhealth.gov/get-help/immediate-help" target="_blank">Artículo</a></p>
        </div>
        <div class="blog-post">
            <h3>Nuevos avances en la inteligencia artificial aplicada a la salud mental</h3>
            <p>Mantente al día con los últimos avances en la tecnología de IA que están revolucionando el campo de la salud mental.</p>
        </div>
        <div class="blog-post">
            <h3>La OMS publica el primer informe mundial sobre inteligencia artificial (IA) aplicada a la salud</h3>
            <p>La OMS publica el primer informe mundial sobre inteligencia artificial (IA) aplicada a la salud y seis principios rectores relativos a su concepción y utilización. <a href="https://www.who.int/es/news/item/28-06-2021-who-issues-first-global-report-on-ai-in-health-and-six-guiding-principles-for-its-design-and-use" target="_blank">Artículo</a></p>
        </div>
        <div class="blog-post">
            <h3>Eventos y seminarios sobre salud mental</h3>
            <p>Infórmate sobre los próximos eventos y seminarios que abordan temas cruciales sobre salud mental y bienestar. <a href="https://www.who.int/news-room/events" target="_blank">Artículo</a></p>
        </div>
    </section>
    <section id="contacto" class="container">
        <h2>Contacto</h2>
        <form action="#" method="post">
            <label for="name">Nombre:</label>
            <input type="text" id="name" name="name" required>
            <label for="email">Correo Electrónico:</label>
            <input type="email" id="email" name="email" required>
            <label for="message">Mensaje:</label>
            <textarea id="message" name="message" rows="4" required></textarea>
            <input type="submit" value="Enviar">
        </form>
        <p>Correo Electrónico: diego.enciso@ieee.org</p>
        <p>Correo Electrónico: alanmartinez@ieee.org</p>
        <p>Página de desarrolladores: <a href="https://www.facebook.com/profile.php?id=61556757911022&mibextid=ZbWKwL" target="_blank">Perfil de Facebook</a></p>
    </section>
    <section id="faqs" class="container">
        <h2>Preguntas Frecuentes</h2>
        <h3>Funcionamiento</h3>
        <p>¿Cómo funciona Thomas AI para el diagnóstico de enfermedades?</p>
        <p>Thomas AI utiliza algoritmos de aprendizaje automático para analizar patrones de comportamiento y respuestas a cuestionarios estructurados, identificando signos tempranos de trastornos mentales como la depresión y la ansiedad. Este diagnóstico es preliminar y se recomienda consultar a un profesional de salud mental para una evaluación completa.</p>
        <h3>Seguridad de Datos</h3>
        <p>¿Cómo asegura Thomas AI la privacidad y seguridad de mis datos?</p>
        <p>La privacidad y seguridad de tus datos son nuestras máximas prioridades. Utilizamos tecnologías de encriptación avanzada y seguimos estrictas políticas de privacidad para asegurar que tus datos personales y de salud estén completamente protegidos.</p>
        <h3>Acceso a Servicios</h3>
        <p>¿Cómo puedo acceder a los servicios de Thomas AI?</p>
        <p>Puedes acceder a nuestros servicios a través de nuestra plataforma en línea. Solo necesitas crear una cuenta y podrás comenzar a utilizar nuestros módulos interactivos y Test terapéuticos para recibir apoyo emocional y diagnóstico preliminar.</p>
    </section>
    <section id="desarrolladores" class="container developer-info">
        <h2>Desarrolladores</h2>
        <p>Desarrolladores: E&M Soluciones con IA</p>
        <p>Contacto: <a href="mailto:diego.enciso@ieee.org">diego.enciso@ieee.org</a> y <a href="mailto:alanmartinez@ieee.org">alanmartinez@ieee.org</a></p>
        <p>Página de desarrolladores: <a href="https://www.facebook.com/profile.php?id=61556757911022&mibextid=ZbWKwL" target="_blank">Perfil de Facebook</a></p>
    </section>
    <footer>
        <p>&copy; 2024 Thomas AI. Todos los derechos reservados.</p>
        <p><a href="#inicio">Volver al inicio</a></p>
    </footer>
    <script>
        const sections = document.querySelectorAll('.container');

        const observer = new IntersectionObserver(entries => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('show');
                }
            });
        }, {
            threshold: 0.1
        });

        sections.forEach(section => {
            observer.observe(section);
        });
    </script>
</body>
</html>
