<html lang="es"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>Manuel Álvarez - Portfolio</title>
<script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined" rel="stylesheet"/>
<style type="text/tailwindcss">
        :root {
      --bg-color: #0A0A0A;
      --text-color: #EAEAEA;
      --card-bg: #1A1A1A;
      --primary-color: #6A44E8;
      --secondary-color: #B8A6F9;
      --border-color: #2A2A2A;
    }
    body {
      font-family: 'Inter', sans-serif;
      background-color: var(--bg-color);
      color: var(--text-color);
    }
    .material-symbols-outlined {
      font-variation-settings:
      'FILL' 0,
      'wght' 300,
      'GRAD' 0,
      'opsz' 24
    }
    .section-glow {
        position: relative;
    }
    .section-glow::before {
        content: '';
        position: absolute;
        top: 50%;
        left: 50%;
        width: 60%;
        height: 60%;
        border-radius: 9999px;
        background-image: radial-gradient(circle, rgba(106, 68, 232, 0.2) 0%, rgba(106, 68, 232, 0) 60%);
        transform: translate(-50%, -50%);
        z-index: -1;
        pointer-events: none;

    }

    /* Certificaciones flip 3D */
    .cert-grid{display:grid;grid-template-columns:1fr 1fr;gap:16px}
    @media(max-width:1000px){.cert-grid{grid-template-columns:1fr}}
    .flip{perspective:1200px}
    .flip-inner{position:relative;height:220px;border-radius:16px;border:1px solid var(--border);background:rgba(255,255,255,.04);transform-style:preserve-3d;transition:transform .6s cubic-bezier(.2,.8,.2,1)}
    .flip-face{position:absolute;inset:0;display:flex;flex-direction:column;align-items:center;justify-content:center;padding:14px;backface-visibility:hidden}
    .flip-back{text-align:center;transform:rotateY(180deg)}
    .flip:hover .flip-inner, .flip.flipped .flip-inner{transform:rotateY(180deg)}
    .flip-front img{max-height:120px;width:auto;display:block;filter:drop-shadow(0 0 18px rgba(127,19,236,.25))}
    .lead{color:var(--muted)}


    </style>
</head>
<body class="antialiased">
<div class="container mx-auto px-4 sm:px-6 lg:px-8">
<header class="py-16 sm:py-24">
<div class="max-w-4xl mx-auto text-center">
<img alt="Manuel Álvarez" class="w-24 h-24 rounded-full mx-auto mb-6 border-2 border-[var(--primary-color)]" src="https://media.licdn.com/dms/image/v2/D4D03AQHh5_w3l5YC6w/profile-displayphoto-shrink_800_800/B4DZb8cCsKHsAg-/0/1747991932217?e=1761782400&v=beta&t=7JqHcHFyELjpSJKoqmNnkw2RwDzQIgJrprZfsbkJFW0"/>
<h1 class="text-4xl sm:text-5xl font-bold tracking-tight text-white">Manuel Álvarez</h1>
<p class="mt-4 text-lg sm:text-xl text-gray-400">Junior IT | Técnico de Sistemas y Redes</p>
<p class="mt-4 text-lg sm:text-xl text-gray-400">Diseñador y desarrollador UX/UI</p>
<p class="mt-6 max-w-2xl mx-auto text-gray-400">
                    Apasionado por crear experiencias digitales intuitivas y elegantes. Combinando diseño y tecnología para construir productos que la gente ame usar.
                </p>
<div class="mt-8 flex justify-center gap-4">
<a class="inline-flex items-center justify-center px-6 py-3 border border-transparent text-base font-medium rounded-md text-white bg-[var(--primary-color)] hover:bg-opacity-90 transition-colors" href="#proyectos">
                        Ver proyectos
                    </a>
<a class="inline-flex items-center justify-center px-6 py-3 border border-transparent text-base font-medium rounded-md text-white bg-[var(--primary-color)] hover:bg-opacity-90 transition-colors" href="#contacto">
                        Contacto
                    </a>
</div>
</div>
</header>
<main>
<section class="py-16 sm:py-24 section-glow" id="proyectos">
<div class="max-w-6xl mx-auto">
<h2 class="text-3xl sm:text-4xl font-bold tracking-tight text-center text-white">Proyectos Destacados</h2>
<p class="mt-4 text-lg text-center text-gray-400 max-w-2xl mx-auto">Una selección de mis trabajos recientes en diseño y desarrollo.</p>
<div class="mt-12 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
<div class="group relative flex flex-col bg-[var(--card-bg)] border border-[var(--border-color)] rounded-xl overflow-hidden hover:border-[var(--primary-color)] hover:shadow-[0_0_5000px_rgba(106,68,232,0.5)] transition-all duration-300">
<div class="p-6 flex-grow">
<h3 class="text-xl font-semibold text-white">APP Móvil/Escritorio — Expo Go — Google Play</h3>
<p class="mt-2 text-gray-400">React Native (JS/TS). Inicio como Developer en Google</p>
<p class="mt-4 text-sm text-gray-300">
                                <strong>· Uso:</strong> utilidades y contenido propio (calendario temático).<br/>
                                <strong>· Finalidad:</strong> publicar y mantener una app en producción (Play Store) con actualizaciones OTA.<br/>
                                <strong>· Herramientas:</strong> React Native, Expo, JS/TS, OTA, GitHub.<br/>
                                <strong>· Motivación:</strong> consolidar skills móviles y ciclo de despliegue real.
                            </p>
</div>
<div class="p-6 bg-black/20">
<div class="flex flex-wrap gap-2 mb-4">
<span class="bg-white/10 text-[var(--secondary-color)] text-xs font-medium px-2.5 py-1 rounded-full">Expo</span>
<span class="bg-white/10 text-[var(--secondary-color)] text-xs font-medium px-2.5 py-1 rounded-full">Navegación</span>
<span class="bg-white/10 text-[var(--secondary-color)] text-xs font-medium px-2.5 py-1 rounded-full">OTA</span>
</div>
<div class="flex gap-4">
<a class="flex items-center justify-center w-full text-sm font-medium rounded-md text-white bg-white/10 hover:bg-white/20 transition-colors py-2 px-4" href="https://github.com/manu-alvarez/CalendarioMaya-ManoElectricaAzul">
<span class="material-symbols-outlined mr-2 text-base">code</span> GitHub
                                    </a>
<a class="flex items-center justify-center w-full text-sm font-medium rounded-md text-white bg-white/10 hover:bg-white/20 transition-colors py-2 px-4" href="https://play.google.com/store/apps/details?id=com.manoelectricaazul.app">
<span class="material-symbols-outlined mr-2 text-base">play_circle</span> Play Store
                                    </a>
</div>
</div>
</div>
<div class="group relative flex flex-col bg-[var(--card-bg)] border border-[var(--border-color)] rounded-xl overflow-hidden hover:border-[var(--primary-color)] hover:shadow-[0_0_5000px_rgba(106,68,232,0.5)] transition-all duration-300">
<div class="p-6 flex-grow">
<h3 class="text-xl font-semibold text-white">VPS Ubuntu 24.04 — Sistema Multiagéntico</h3>
<p class="mt-2 text-gray-400">Dockerizado (n8n, Nextcloud, Flowise, Hetzner) | Base para futuros proyectos</p>
<p class="mt-4 text-sm text-gray-300">
                                <strong>· Uso:</strong> hosting de servicios, agentes y automatizaciones.<br/>
                                <strong>· Finalidad:</strong> plataforma estable y escalable con reverse-proxy y SSL.<br/>
                                <strong>· Herramientas:</strong> Ubuntu 24.04, Docker Compose, Nginx Proxy Manager, Coolify, MySQL/Postgres.<br/>
                                <strong>· Motivación:</strong> centralizar desarrollo y facilitar despliegues.
                            </p>
</div>
<div class="p-6 bg-black/20">
<div class="flex flex-wrap gap-2 mb-4">
<span class="bg-white/10 text-[var(--secondary-color)] text-xs font-medium px-2.5 py-1 rounded-full">Reverse‑Proxy</span>
<span class="bg-white/10 text-[var(--secondary-color)] text-xs font-medium px-2.5 py-1 rounded-full">SSL</span>
<span class="bg-white/10 text-[var(--secondary-color)] text-xs font-medium px-2.5 py-1 rounded-full">Backups</span>
</div>
<a class="flex items-center justify-center w-full text-sm font-medium rounded-md text-white bg-white/10 hover:bg-white/20 transition-colors py-2 px-4" href="https://alvarezconsult.com/">
<span class="material-symbols-outlined mr-2 text-base">dns</span> Visitar servidor
                                </a>
</div>
</div>
<div class="group relative flex flex-col bg-[var(--card-bg)] border border-[var(--border-color)] rounded-xl overflow-hidden hover:border-[var(--primary-color)] hover:shadow-[0_0_5000px_rgba(106,68,232,0.5)] transition-all duration-300">
<div class="p-6 flex-grow">
<h3 class="text-xl font-semibold text-white">Kit de Automatización — Búsqueda de Empleo</h3>
<p class="mt-2 text-gray-400">Trackers, Scripts, Bookmarklet y Workflow n8n (flujo guiado)</p>
<p class="mt-4 text-sm text-gray-300">
                                <strong>· Uso:</strong> captura de ofertas y correos (Gmail/Outlook) a un tracker centralizado.<br/>
                                <strong>· Finalidad:</strong> priorización, recordatorios y seguimiento con eventos en Calendar.<br/>
                                <strong>· Herramientas:</strong> Google Sheets/Apps Script, n8n, Telegram.<br/>
                                <strong>· Motivación:</strong> eliminar tareas repetitivas y asegurar follow-ups.
                            </p>
</div>
<div class="p-6 bg-black/20">
<div class="flex flex-wrap gap-2 mb-4">
<span class="bg-white/10 text-[var(--secondary-color)] text-xs font-medium px-2.5 py-1 rounded-full">Gmail/Outlook</span>
<span class="bg-white/10 text-[var(--secondary-color)] text-xs font-medium px-2.5 py-1 rounded-full">Calendar</span>
<span class="bg-white/10 text-[var(--secondary-color)] text-xs font-medium px-2.5 py-1 rounded-full">Telegram</span>
</div>
<a class="flex items-center justify-center w-full text-sm font-medium rounded-md text-white bg-white/10 hover:bg-white/20 transition-colors py-2 px-4" href="#contacto">
                                    Pedir demo
                                </a>
</div>
</div>
</div>
</div>
</section>
<section class="py-16 sm:py-24" id="certificaciones">
<div class="max-w-4xl mx-auto">
<h2 class="text-3xl sm:text-4xl font-bold tracking-tight text-center text-white">Certificaciones</h2>
<div class="mt-12 grid grid-cols-1 md:grid-cols-2 gap-8">
<div class="bg-[var(--card-bg)] border border-[var(--border-color)] rounded-xl p-6 hover:border-[var(--primary-color)] transition-all duration-300">
<h3 class="text-xl font-semibold text-white mb-3">Cibersecurity</h3>
<div class="flip" tabindex="0" aria-label="Cisco CCST Cybersecurity">
<div class="flip-inner">
<div class="flip-face flip-front">
<img alt="Cisco CCST Cybersecurity" src="https://raw.githubusercontent.com/manu-alvarez/varios-external/refs/heads/main/ccst_cybersecurity_small.png">
</div>
<div class="flip-face flip-back">
<h3>CCST — Cybersecurity</h3>
<p class="lead">Amenazas, controles, redes seguras, endpoints y respuesta a incidentes.</p>
</div>
</div>
</div>
</div>
<div class="bg-[var(--card-bg)] border border-[var(--border-color)] rounded-xl p-6 hover:border-[var(--primary-color)] transition-all duration-300">
<h3 class="text-xl font-semibold text-white mb-3">Networking</h3>
<div class="flip" tabindex="0" aria-label="Cisco CCST Networking">
<div class="flip-inner">
<div class="flip-face flip-front">
<img alt="Cisco CCST Networking" src="https://raw.githubusercontent.com/manu-alvarez/varios-external/refs/heads/main/ccst_networking_small.png">
</div>
<div class="flip-face flip-back">
<h3>CCST — Networking</h3>
<p class="lead">IP · switching/routing · Wi‑Fi · troubleshooting L1–L3.</p>
</div>
</div>
</div>
</div>
</div>
</section>
<section class="py-16 sm:py-24" id="experiencia">
<div class="max-w-4xl mx-auto">
<h2 class="text-3xl sm:text-4xl font-bold tracking-tight text-center text-white">Experiencia y Formación</h2>
<div class="mt-12 space-y-8 relative before:absolute before:inset-0 before:ml-5 before:h-full before:w-0.5 before:bg-[var(--border-color)] before:origin-top">
<div class="relative flex items-start">
<div class="flex-shrink-0 w-10 h-10 rounded-full bg-[var(--primary-color)] flex items-center justify-center ring-8 ring-[var(--bg-color)]">
<span class="material-symbols-outlined text-white">business_center</span>
</div>
<div class="ml-6">
<h3 class="font-semibold text-white">Codearts Solutions — Internship</h3>
<p class="text-sm text-gray-400">2023</p>
<p class="mt-2 text-gray-300">Administración de sistemas Linux/Windows, despliegues Docker, instalación y configuración de servidores, virtualizaciones.</p>
</div>
</div>
<div class="relative flex items-start">
<div class="flex-shrink-0 w-10 h-10 rounded-full bg-[var(--primary-color)] flex items-center justify-center ring-8 ring-[var(--bg-color)]">
<span class="material-symbols-outlined text-white">school</span>
</div>
<div class="ml-6">
<h3 class="font-semibold text-white">Técnico de Sistemas Microinformáticos y Redes</h3>
<p class="text-sm text-gray-400">2022 - 2024</p>
<p class="mt-2 text-gray-300">Formación completa en hardware, software, redes y seguridad informática.</p>
</div>
</div>
<div class="relative flex items-start">
<div class="flex-shrink-0 w-10 h-10 rounded-full bg-[var(--primary-color)] flex items-center justify-center ring-8 ring-[var(--bg-color)]">
<span class="material-symbols-outlined text-white">lightbulb</span>
</div>
<div class="ml-6">
<h3 class="font-semibold text-white">Autoformación Continua</h3>
<p class="text-sm text-gray-400">Siempre aprendiendo</p>
<p class="mt-2 text-gray-300">Explorando IA (GPT, Claude, Gemini, Code Versions), funcionamiento de Asistentes, sistemas multiagentes, creación de flujos de trabajos (WorkFlows) y nuevas tecnologías de desarrollo.</p>
</div>
</div>
</div>
</div>
</section>
<section class="py-16 sm:py-24" id="habilidades">
<div class="max-w-4xl mx-auto">
<h2 class="text-3xl sm:text-4xl font-bold tracking-tight text-center text-white">Habilidades</h2>
<p class="mt-4 text-lg text-center text-gray-400">Mi caja de herramientas para construir productos increíbles.</p>
<div class="mt-12 grid grid-cols-1 md:grid-cols-2 gap-8">
<div class="bg-[var(--card-bg)] border border-[var(--border-color)] rounded-xl p-6 hover:border-[var(--primary-color)] transition-all duration-300">
<h3 class="text-xl font-semibold text-white mb-3">Desarrollo Backend & Automatización</h3>
<p class="text-gray-400">User Research, Design Systems, Accesibilidad, Docker, Ubuntu, Node.js, Scripts, n8n, Nginx Proxy Manager, MySQL/Postgres, Google Sheets/Apps Script, Webhooks</p>
</div>
<div class="bg-[var(--card-bg)] border border-[var(--border-color)] rounded-xl p-6 hover:border-[var(--primary-color)] transition-all duration-300">
<h3 class="text-xl font-semibold text-white mb-3">Desarrollo Frontend</h3>
<p class="text-gray-400">HTML5, React Native, JavaScript, TypeScript, React, Next.js, Tailwind CSS, Git/GitHub, Expo, APIs, Webhooks</p>
</div>
</div>
</div>
</div>
</section>
<section class="py-16 sm:py-24" id="contacto">
<div class="max-w-2xl mx-auto text-center">
<h2 class="text-3xl sm:text-4xl font-bold tracking-tight text-white">Contacto</h2>
<p class="mt-4 text-lg text-gray-400">¿Tienes un proyecto en mente o quieres conectar? Envíame un mensaje.</p>
<div class="mt-8">
<a class="inline-flex items-center justify-center px-8 py-4 border border-transparent text-base font-medium rounded-md text-white bg-[var(--primary-color)] hover:bg-opacity-90 transition-colors" href="mailto:manuelalvarezdianez@gmail.com">
<span class="material-symbols-outlined mr-2">email</span> manuelalvarezdianez@gmail.com
                         </a>
<br>
<br>
<a class="inline-flex items-center justify-center px-8 py-4 border border-transparent text-base font-medium rounded-md text-white bg-[var(--primary-color)] hover:bg-opacity-90 transition-colors" href="mailto:manuel@alvarezconsult.com">
<span class="material-symbols-outlined mr-2">email</span> manuel@alvarezconsult.com
                         </a>
</div>
</div>
</section>
</main>
<footer class="py-8">
<p class="mt-6 text-center text-sm text-gray-500">© 2025 Manuel Álvarez. Todos los derechos reservados.</p>
</footer>
</div>
</body></html>
