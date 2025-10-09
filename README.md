<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Manuel Álvarez - CV</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

```
    body {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        background: linear-gradient(135deg, #0a0e27 0%, #1a0b2e 50%, #16001e 100%);
        color: #e0e0e0;
        line-height: 1.6;
        min-height: 100vh;
    }

    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 20px;
    }

    header {
        background: linear-gradient(135deg, rgba(219, 39, 119, 0.15), rgba(59, 130, 246, 0.15));
        border: 2px solid rgba(0, 247, 255, 0.3);
        border-radius: 15px;
        padding: 40px;
        margin-bottom: 30px;
        box-shadow: 0 0 30px rgba(219, 39, 119, 0.3), 0 0 60px rgba(59, 130, 246, 0.2);
        position: relative;
        overflow: hidden;
    }

    header::before {
        content: '';
        position: absolute;
        top: -50%;
        left: -50%;
        width: 200%;
        height: 200%;
        background: radial-gradient(circle, rgba(219, 39, 119, 0.1) 0%, transparent 70%);
        animation: pulse 4s ease-in-out infinite;
    }

    @keyframes pulse {
        0%, 100% { transform: scale(1); opacity: 0.5; }
        50% { transform: scale(1.1); opacity: 0.8; }
    }

    h1 {
        font-size: 3em;
        color: #00f7ff;
        text-shadow: 0 0 20px rgba(0, 247, 255, 0.8), 0 0 40px rgba(219, 39, 119, 0.5);
        margin-bottom: 10px;
        position: relative;
        z-index: 1;
    }

    .subtitle {
        font-size: 1.2em;
        color: #db2777;
        text-shadow: 0 0 10px rgba(219, 39, 119, 0.8);
        margin-bottom: 20px;
        position: relative;
        z-index: 1;
    }

    .contact-info {
        display: flex;
        flex-wrap: wrap;
        gap: 20px;
        font-size: 0.95em;
        position: relative;
        z-index: 1;
    }

    .contact-info span {
        color: #a78bfa;
        padding: 5px 15px;
        background: rgba(167, 139, 250, 0.1);
        border-radius: 20px;
        border: 1px solid rgba(167, 139, 250, 0.3);
    }

    .contact-info a {
        color: #00f7ff;
        text-decoration: none;
        transition: all 0.3s;
    }

    .contact-info a:hover {
        text-shadow: 0 0 10px rgba(0, 247, 255, 1);
    }

    .section {
        background: linear-gradient(135deg, rgba(26, 11, 46, 0.6), rgba(22, 0, 30, 0.6));
        border: 2px solid rgba(219, 39, 119, 0.3);
        border-radius: 15px;
        padding: 30px;
        margin-bottom: 25px;
        box-shadow: 0 5px 20px rgba(0, 0, 0, 0.5), inset 0 0 20px rgba(59, 130, 246, 0.05);
        transition: all 0.3s;
    }

    .section:hover {
        border-color: rgba(0, 247, 255, 0.5);
        box-shadow: 0 5px 30px rgba(219, 39, 119, 0.4), inset 0 0 30px rgba(59, 130, 246, 0.1);
    }

    h2 {
        color: #db2777;
        font-size: 1.8em;
        margin-bottom: 20px;
        text-shadow: 0 0 15px rgba(219, 39, 119, 0.6);
        border-bottom: 2px solid rgba(0, 247, 255, 0.3);
        padding-bottom: 10px;
    }

    h3 {
        color: #00f7ff;
        font-size: 1.3em;
        margin-top: 15px;
        margin-bottom: 10px;
        text-shadow: 0 0 10px rgba(0, 247, 255, 0.5);
    }

    .skills-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        gap: 15px;
        margin-top: 15px;
    }

    .skill-item {
        background: rgba(59, 130, 246, 0.1);
        border: 1px solid rgba(0, 247, 255, 0.3);
        border-radius: 10px;
        padding: 15px;
        transition: all 0.3s;
    }

    .skill-item:hover {
        background: rgba(219, 39, 119, 0.15);
        border-color: rgba(219, 39, 119, 0.5);
        transform: translateY(-3px);
        box-shadow: 0 5px 15px rgba(219, 39, 119, 0.3);
    }

    .skill-item strong {
        color: #a78bfa;
        display: block;
        margin-bottom: 5px;
    }

    .project-card, .experience-card {
        background: linear-gradient(135deg, rgba(59, 130, 246, 0.08), rgba(219, 39, 119, 0.08));
        border: 1px solid rgba(167, 139, 250, 0.3);
        border-radius: 10px;
        padding: 20px;
        margin-bottom: 15px;
        transition: all 0.3s;
    }

    .project-card:hover, .experience-card:hover {
        border-color: rgba(0, 247, 255, 0.5);
        box-shadow: 0 0 20px rgba(0, 247, 255, 0.2);
        transform: translateX(5px);
    }

    .project-card h3, .experience-card h3 {
        font-size: 1.2em;
        margin-top: 0;
    }

    ul {
        list-style: none;
        padding-left: 0;
    }

    ul li {
        padding: 8px 0;
        padding-left: 25px;
        position: relative;
        color: #d1d5db;
    }

    ul li::before {
        content: '▹';
        position: absolute;
        left: 0;
        color: #db2777;
        font-size: 1.3em;
    }

    .cert-badge {
        display: inline-block;
        background: linear-gradient(135deg, rgba(219, 39, 119, 0.2), rgba(167, 139, 250, 0.2));
        border: 1px solid rgba(0, 247, 255, 0.4);
        color: #00f7ff;
        padding: 10px 20px;
        border-radius: 25px;
        margin: 5px;
        font-size: 0.95em;
        transition: all 0.3s;
    }

    .cert-badge:hover {
        background: linear-gradient(135deg, rgba(219, 39, 119, 0.3), rgba(167, 139, 250, 0.3));
        box-shadow: 0 0 15px rgba(0, 247, 255, 0.4);
        transform: scale(1.05);
    }

    .availability {
        background: linear-gradient(135deg, rgba(0, 247, 255, 0.1), rgba(219, 39, 119, 0.1));
        border: 2px solid rgba(0, 247, 255, 0.4);
        border-radius: 10px;
        padding: 20px;
        text-align: center;
        font-size: 1.1em;
        color: #00f7ff;
        text-shadow: 0 0 10px rgba(0, 247, 255, 0.5);
    }

    @media (max-width: 768px) {
        h1 {
            font-size: 2em;
        }
        
        .contact-info {
            flex-direction: column;
        }
        
        .skills-grid {
            grid-template-columns: 1fr;
        }
    }
</style>
```

</head>
<body>
    <div class="container">
        <header>
            <h1>Manuel Álvarez</h1>
            <div class="subtitle">Junior IT · Técnico de Sistemas y Redes · Developer</div>
            <div class="contact-info">
                <span>📍 Mequinenza (Zaragoza)</span>
                <span>📱 +34 651 352 065</span>
                <span>🔗 <a href="https://es.linkedin.com/in/manuel-alvarez-dianez-201664b7" target="_blank">LinkedIn</a></span>
            </div>
        </header>

```
    <div class="section">
        <h2>Perfil</h2>
        <p>Técnico de Sistemas y Redes (Junior IT) con experiencia en entornos Windows y Linux, redes y administración básica de servicios. Enfocado en mantener la infraestructura estable, resolver incidencias con rapidez y aportar soluciones prácticas. Como Developer, materializo ideas en proyectos funcionales y bien documentados. Busco aportar fiabilidad operativa y seguir creciendo en entornos profesionales.</p>
    </div>

    <div class="section">
        <h2>Habilidades técnicas</h2>
        <div class="skills-grid">
            <div class="skill-item">
                <strong>Sistemas</strong>
                Windows 10/11, Windows Server, Active Directory, Linux (Ubuntu)
            </div>
            <div class="skill-item">
                <strong>Redes</strong>
                TCP/IP, DHCP, DNS, Wi‑Fi, switching básico, cableado y diagnóstico L1–L3
            </div>
            <div class="skill-item">
                <strong>Herramientas/Plataforma</strong>
                Docker, Git/GitHub, Nginx
            </div>
            <div class="skill-item">
                <strong>Scripting</strong>
                PowerShell, Bash
            </div>
            <div class="skill-item">
                <strong>Desarrollo</strong>
                React Native, Node.js, HTML, CSS, JavaScript, TypeScript, Tailwind CSS
            </div>
        </div>
    </div>

    <div class="section">
        <h2>Proyectos destacados</h2>
        
        <div class="project-card">
            <h3>App móvil (React Native/Expo)</h3>
            <p>Aplicación demostrable que muestra dominio de RN/Expo, componentes, estado y consumo de APIs.</p>
        </div>

        <div class="project-card">
            <h3>VPS Ubuntu con servicios (Docker)</h3>
            <p>Despliegue y administración de servicios en contenedores (Nginx, bases de datos, utilidades), con prácticas de seguridad y copias.</p>
        </div>

        <div class="project-card">
            <h3>Automatización búsqueda de empleo</h3>
            <p>Scripts y flujos para simplificar búsquedas y registro de oportunidades con criterios definidos.</p>
        </div>
    </div>

    <div class="section">
        <h2>Experiencia</h2>
        
        <div class="experience-card">
            <h3>Codearts Solutions — Prácticas (Soporte/Systems)</h3>
            <p style="color: #a78bfa; margin-bottom: 10px;">2024</p>
            <ul>
                <li>Administración básica de entornos Linux y Windows</li>
                <li>Virtualización y contenedorización con Docker</li>
                <li>Mantenimiento preventivo y correctivo de equipos y servicios</li>
                <li>Documentación de procedimientos y buenas prácticas</li>
            </ul>
        </div>
    </div>

    <div class="section">
        <h2>Formación</h2>
        <p><strong style="color: #00f7ff;">Técnico en Sistemas Microinformáticos y Redes (SMR)</strong> — 2022–2024</p>
    </div>

    <div class="section">
        <h2>Certificaciones</h2>
        <div>
            <span class="cert-badge">Cisco Certified Support Technician (CCST) — Cybersecurity</span>
            <span class="cert-badge">Cisco Certified Support Technician (CCST) — Networking</span>
        </div>
    </div>

    <div class="section">
        <div class="availability">
            <strong>Disponibilidad:</strong> Presencial ≤100 km desde Mequinenza y remoto sin límite geográfico
        </div>
    </div>
</div>
```

</body>
</html>
