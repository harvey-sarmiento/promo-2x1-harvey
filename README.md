<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Acompañamiento Personalizado Harvey Sarmiento - Promo 2x1</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
            line-height: 1.5;
            color: #1a1a1a;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-font-smoothing: antialiased;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0;
        }

        .promo-banner {
            background: linear-gradient(45deg, #ff6b6b, #ee5a6f);
            color: white;
            text-align: center;
            padding: 12px 15px;
            font-weight: 700;
            font-size: 0.9em;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
            animation: pulse 2s infinite;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.01); }
        }

        .hero {
            background: white;
            border-radius: 0;
            padding: 30px 20px;
            margin: 0;
            text-align: center;
            box-shadow: 0 5px 20px rgba(0,0,0,0.15);
            animation: fadeInUp 0.8s ease-out;
        }

        .hero h1 {
            font-size: 1.8em;
            margin: 15px 0;
            color: #667eea;
            line-height: 1.2;
        }

        .promo-badge {
            background: linear-gradient(45deg, #f093fb 0%, #f5576c 100%);
            color: white;
            display: inline-block;
            padding: 15px 30px;
            border-radius: 50px;
            font-size: 1.5em;
            font-weight: 800;
            margin: 15px 0;
            box-shadow: 0 8px 20px rgba(245, 87, 108, 0.4);
            animation: bounce 2s infinite;
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-8px); }
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes slideInLeft {
            from {
                opacity: 0;
                transform: translateX(-50px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        @keyframes slideInRight {
            from {
                opacity: 0;
                transform: translateX(50px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        @keyframes scaleIn {
            from {
                opacity: 0;
                transform: scale(0.8);
            }
            to {
                opacity: 1;
                transform: scale(1);
            }
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
        }

        @keyframes glow {
            0%, 100% { box-shadow: 0 5px 20px rgba(102, 126, 234, 0.4); }
            50% { box-shadow: 0 5px 30px rgba(102, 126, 234, 0.8); }
        }

        .price-label {
            font-size: 1.1em;
            color: #333;
            margin: 15px 0;
            font-weight: 600;
        }

        .results-badge {
            background: linear-gradient(45deg, #11998e 0%, #38ef7d 100%);
            color: white;
            padding: 12px 25px;
            border-radius: 10px;
            display: inline-block;
            font-size: 1em;
            font-weight: 700;
            margin: 15px 0;
            box-shadow: 0 5px 15px rgba(17, 153, 142, 0.3);
            animation: float 3s ease-in-out infinite;
        }

        .section {
            background: white;
            padding: 30px 20px;
            margin: 15px 0;
            box-shadow: 0 5px 20px rgba(0,0,0,0.15);
            animation: fadeInUp 0.8s ease-out;
        }

        .section h2 {
            color: #667eea;
            font-size: 1.5em;
            margin-bottom: 20px;
            text-align: center;
            line-height: 1.3;
        }

        .objectives-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 12px;
            margin: 20px 0;
        }

        .objective-item {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 15px;
            border-radius: 12px;
            display: flex;
            align-items: center;
            font-size: 0.95em;
            transition: transform 0.3s;
            box-shadow: 0 3px 10px rgba(102, 126, 234, 0.3);
        }

        .objective-item:active {
            transform: scale(0.98);
        }

        .objective-item::before {
            content: "✓";
            font-size: 1.2em;
            margin-right: 12px;
            background: white;
            color: #667eea;
            min-width: 28px;
            height: 28px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-shrink: 0;
            font-weight: 700;
        }

        .step {
            background: #f8f9fa;
            padding: 18px;
            margin: 12px 0;
            border-radius: 12px;
            border-left: 4px solid #667eea;
            font-size: 0.95em;
        }

        .step-number {
            background: #667eea;
            color: white;
            width: 32px;
            height: 32px;
            border-radius: 50%;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            font-weight: 700;
            margin-right: 12px;
            font-size: 0.9em;
        }

        .plan-premium {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
            padding: 30px 20px;
            margin: 15px 0;
            box-shadow: 0 5px 20px rgba(0,0,0,0.2);
        }

        .plan-premium h2 {
            font-size: 1.8em;
            text-align: center;
            margin-bottom: 25px;
            color: white;
        }

        .plan-features {
            display: grid;
            grid-template-columns: 1fr;
            gap: 15px;
            margin: 20px 0;
        }

        .feature-card {
            background: rgba(255,255,255,0.95);
            padding: 20px;
            border-radius: 15px;
            border: 2px solid rgba(255,255,255,0.3);
            color: #333;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
        }

        .feature-card h3 {
            font-size: 1.1em;
            margin-bottom: 12px;
            color: #667eea;
        }

        .feature-card ul {
            list-style: none;
            padding-left: 0;
        }

        .feature-card li {
            padding: 6px 0 6px 25px;
            position: relative;
            font-size: 0.9em;
            line-height: 1.4;
        }

        .feature-card li::before {
            content: "✓";
            position: absolute;
            left: 0;
            font-weight: 700;
            color: #38ef7d;
        }

        .cta-button {
            background: linear-gradient(45deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 18px 35px;
            border: none;
            border-radius: 50px;
            font-size: 1.2em;
            font-weight: 700;
            cursor: pointer;
            text-decoration: none;
            display: block;
            margin: 20px auto;
            transition: transform 0.3s, box-shadow 0.3s;
            box-shadow: 0 5px 20px rgba(102, 126, 234, 0.4);
            text-align: center;
            width: 100%;
            max-width: 400px;
            animation: glow 2s ease-in-out infinite;
        }

        .cta-button:active {
            transform: scale(0.98);
        }

        .cta-button.large {
            font-size: 1.4em;
            padding: 22px 40px;
            margin: 25px auto;
        }

        .urgency {
            background: #fff3cd;
            border: 2px solid #ffc107;
            border-radius: 12px;
            padding: 18px 15px;
            margin: 15px 20px;
            text-align: center;
            font-weight: 700;
            color: #856404;
            font-size: 0.9em;
            line-height: 1.5;
        }

        .payment-info {
            margin: 25px 0;
            padding: 20px;
            background: #f8f9fa;
            border-radius: 15px;
        }

        .payment-info h3 {
            color: #667eea;
            font-size: 1.3em;
            margin-bottom: 15px;
        }

        .payment-info p {
            margin: 12px 0;
            font-size: 1em;
            line-height: 1.5;
        }

        .whatsapp-link {
            color: #25D366;
            font-weight: 700;
            text-decoration: none;
            font-size: 1.1em;
        }

        .footer {
            background: rgba(255,255,255,0.95);
            padding: 25px 20px;
            margin: 15px 0 0 0;
            text-align: center;
            box-shadow: 0 -5px 20px rgba(0,0,0,0.15);
        }

        .footer h3 {
            color: #667eea;
            font-size: 1.3em;
            margin-bottom: 15px;
            line-height: 1.3;
        }

        .footer p {
            margin: 10px 0;
            color: #666;
            font-size: 0.95em;
        }

        /* Testimonials Section */
        .testimonials {
            background: white;
            padding: 30px 20px;
            margin: 15px 0;
            box-shadow: 0 5px 20px rgba(0,0,0,0.15);
            overflow: hidden;
        }

        .testimonials h2 {
            color: #667eea;
            font-size: 1.5em;
            margin-bottom: 25px;
            text-align: center;
            line-height: 1.3;
        }

        .testimonials-slider {
            display: flex;
            gap: 20px;
            overflow-x: auto;
            scroll-snap-type: x mandatory;
            scroll-behavior: smooth;
            padding: 10px 0;
            -webkit-overflow-scrolling: touch;
            scrollbar-width: none;
        }

        .testimonials-slider::-webkit-scrollbar {
            display: none;
        }

        .testimonial-card {
            min-width: 280px;
            scroll-snap-align: center;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 5px 20px rgba(0,0,0,0.15);
            transition: transform 0.3s, box-shadow 0.3s;
            animation: scaleIn 0.6s ease-out;
        }

        .testimonial-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }

        .testimonial-card img {
            width: 100%;
            height: auto;
            display: block;
            object-fit: cover;
        }

        .slider-dots {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin-top: 20px;
        }

        .dot {
            width: 10px;
            height: 10px;
            border-radius: 50%;
            background: #d1d5db;
            transition: all 0.3s;
        }

        .dot.active {
            background: #667eea;
            width: 30px;
            border-radius: 5px;
        }

        /* Mejoras para tablets */
        @media (min-width: 600px) {
            .hero {
                border-radius: 20px;
                margin: 15px;
                padding: 40px 30px;
            }

            .section {
                border-radius: 20px;
                margin: 15px;
                padding: 40px 30px;
            }

            .testimonials {
                border-radius: 20px;
                margin: 15px;
                padding: 40px 30px;
            }

            .testimonial-card {
                min-width: 350px;
            }

            .plan-premium {
                border-radius: 20px;
                margin: 15px;
                padding: 40px 30px;
            }

            .footer {
                border-radius: 20px;
                margin: 15px;
            }

            .objectives-grid {
                grid-template-columns: repeat(2, 1fr);
                gap: 15px;
            }

            .plan-features {
                grid-template-columns: repeat(2, 1fr);
                gap: 20px;
            }
        }

        /* Mejoras para desktop */
        @media (min-width: 900px) {
            .hero h1 {
                font-size: 2.5em;
            }

            .promo-badge {
                font-size: 2em;
                padding: 20px 40px;
            }

            .section h2 {
                font-size: 2em;
            }

            .testimonials h2 {
                font-size: 2em;
            }

            .testimonial-card {
                min-width: 400px;
            }

            .plan-premium h2 {
                font-size: 2.5em;
            }

            .objectives-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .plan-features {
                grid-template-columns: repeat(3, 1fr);
            }

            .cta-button {
                max-width: 500px;
            }

            .cta-button:hover {
                transform: translateY(-3px);
                box-shadow: 0 8px 25px rgba(102, 126, 234, 0.6);
            }

            .objective-item:hover {
                transform: translateY(-3px);
            }
        }

        /* Optimizaciones para pantallas muy pequeñas */
        @media (max-width: 360px) {
            .hero h1 {
                font-size: 1.5em;
            }

            .promo-badge {
                font-size: 1.3em;
                padding: 12px 25px;
            }

            .cta-button {
                font-size: 1.1em;
                padding: 16px 30px;
            }

            .section h2 {
                font-size: 1.3em;
            }
        }
    </style>
</head>
<body>
    <div class="promo-banner">
        🚨 PROMO VÁLIDA HASTA 31 DE DICIEMBRE 2025 🚨
    </div>

    <div class="container">
        <div class="hero">
            <div class="promo-badge">🚨 PROMO 2x1 🚨</div>
            <h1>ACOMPAÑAMIENTO PERSONALIZADO<br>HARVEY SARMIENTO</h1>
            <p class="price-label">👉🏻 2 MESES DE ASESORÍA PREMIUM 🏅</p>
            <div class="results-badge">🔥 RESULTADOS DESDE TUS PRIMEROS 10 DÍAS 🔥</div>
            <p style="font-size: 1.1em; margin-top: 15px; font-weight: 600;">VÁLIDO PARA 1 PERSONA</p>
            
            <a href="https://checkout.bold.co/payment/LNK_GOKNWJSP76" class="cta-button large" target="_blank">
                🎯 ¡APROVECHA LA PROMO AHORA!
            </a>
        </div>

        <div class="section">
            <h2>🤓 LA ASESORÍA PERSONALIZADA SE AJUSTA A TUS OBJETIVOS</h2>
            <div class="objectives-grid">
                <div class="objective-item">Bajar tu % de grasa 🔥</div>
                <div class="objective-item">Reducir medidas abdominales y talla</div>
                <div class="objective-item">Marcar tu abdomen 🍫</div>
                <div class="objective-item">Eliminar la flacidez 💪🏽</div>
                <div class="objective-item">Reducir la celulitis y tonificar tu piel</div>
                <div class="objective-item">Aumentar y levantar tus glúteos 🍑</div>
                <div class="objective-item">Aumentar tu masa muscular 💪🏽</div>
                <div class="objective-item">Formar nuevos hábitos que te ayuden a mantener tus resultados 🧠</div>
            </div>
            <p style="text-align: center; font-size: 1.1em; margin-top: 20px; font-weight: 600;">
                Todo personalizado y ajustado a tus objetivos
            </p>
        </div>

        <div class="section">
            <h2>🤯 ¿CÓMO FUNCIONA?</h2>
            <p style="text-align: center; margin-bottom: 20px; font-size: 1em; color: #666;">
                Te enseñaré mediante módulos de video y información sencilla, específica y práctica a:
            </p>
            <div class="step">
                <span class="step-number">1</span>
                <strong>Comer saludable</strong> con un menú fácil que se ajuste a tu presupuesto, aprendiendo conceptos básicos de nutrición.
            </div>
            <div class="step">
                <span class="step-number">2</span>
                Aprenderás a controlar y calmar tu <strong>ansiedad</strong> con tips prácticos.
            </div>
            <div class="step">
                <span class="step-number">3</span>
                Aprenderás cómo <strong>mantener tus resultados</strong> cuando ya no estés en la asesoría.
            </div>
            <div class="step">
                <span class="step-number">4</span>
                Aprenderás a <strong>cambiar tus hábitos</strong> enfocándonos en trabajar en ti, en cómo te sientes y cómo te ves.
            </div>
        </div>

        <div class="plan-premium">
            <h2>💎 PLAN PREMIUM 💎</h2>
            <div class="plan-features">
                <div class="feature-card">
                    <h3>📚 MÓDULOS DE VIDEO</h3>
                    <ul>
                        <li>Nutrición aplicable</li>
                        <li>Cómo mantener tus resultados</li>
                        <li>Cómo evitar el efecto rebote</li>
                    </ul>
                </div>
                <div class="feature-card">
                    <h3>🏋️ ENTRENAMIENTO</h3>
                    <ul>
                        <li>Rutinas cortas y efectivas en video para la casa</li>
                        <li>Rutinas para el gym planificadas</li>
                        <li>Progresiones y biseries para acelerar resultados</li>
                    </ul>
                </div>
                <div class="feature-card">
                    <h3>🧠 TRABAJO DE ENFOQUE DIARIO</h3>
                    <ul>
                        <li>30 videos con pequeños desafíos</li>
                        <li>Te ayudarán a estar enfocada y motivada</li>
                        <li>Formar tu mentalidad y cambiar tus hábitos</li>
                    </ul>
                </div>
                <div class="feature-card">
                    <h3>🍽️ PLAN DE ALIMENTACIÓN</h3>
                    <ul>
                        <li>Acompañamiento de Harvey Sarmiento</li>
                        <li>Lista de compras</li>
                        <li>Alimentos y snacks</li>
                    </ul>
                </div>
                <div class="feature-card">
                    <h3>📋 GUÍAS Y RECURSOS</h3>
                    <ul>
                        <li>Guía de organización de comidas por semana</li>
                        <li>eBooks de recetas fáciles y económicas Vol. 1 y 2</li>
                    </ul>
                </div>
                <div class="feature-card">
                    <h3>📊 SEGUIMIENTO</h3>
                    <ul>
                        <li>Chequeo y valoración cada 10 días</li>
                        <li>Ajustes personalizados</li>
                    </ul>
                </div>
            </div>
        </div>

        <div class="urgency">
            ⚠️ CUPOS LIMITADOS ⚠️<br>
            INFO VÁLIDA HASTA 31 DE DICIEMBRE 2025<br>
            O AGOTAR CUPOS<br>
            (No se guardan cupos)
        </div>

        <div class="section">
            <h2>🌎 DESDE CUALQUIER PARTE DEL MUNDO</h2>
            <p style="text-align: center; font-size: 1.1em; margin: 15px 0; font-weight: 600;">
                ¡Transforma tu cuerpo y tu vida hoy!
            </p>
            
            <a href="https://checkout.bold.co/payment/LNK_GOKNWJSP76" class="cta-button large" target="_blank">
                💳 ¡REALIZAR PAGO AHORA!
            </a>
            
            <div class="payment-info">
                <h3>📋 DESPUÉS DE REALIZAR EL PAGO:</h3>
                <p>Automáticamente serás redirigido a WhatsApp para enviarnos tu comprobante de pago y recibir los pasos a seguir de tu asesoría.</p>
                <p style="margin-top: 15px;">
                    📞 WhatsApp: <a href="https://wa.me/573015619137" class="whatsapp-link">+57 301 561 9137</a>
                </p>
            </div>
        </div>

        <div class="footer">
            <h3>🫶🏼 GRACIAS POR ELEGIRTE Y CREAR UNA MEJOR VERSIÓN DE TI</h3>
            <p>Feliz día y muchas bendiciones 🙌🏻😁</p>
        </div>
    </div>
</body>
</html>
