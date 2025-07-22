
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>CV - Jaime Sánchez Navarro</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 0;
      background-color: #5a5a5a82;
      color: #333;
    }

    header {
      background-color: #7c7c7c;
      color: black;
      padding: 1rem;
      text-align: center;
    }

    nav {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      background-color: #555;
    }

    nav a {
      color: white;
      padding: 1rem;
      text-decoration: none;
      display: block;
    }

    nav a:hover {
      background-color: #444;
    }

    section {
      display: none;
      padding: 1.5rem;
      max-width: 800px;
      margin: auto;
      background: #94bcc9;
    }

    section.active {
      display: block;
    }

    h2 {
      color: #333;
      border-bottom: 2px solid #ddd;
      padding-bottom: 0.5rem;
      margin-top: 2rem;
    }

    ul {
      padding-left: 1.2rem;
    }

    @media (max-width: 600px) {
      nav a {
        flex: 1 1 100%;
        padding: 0.8rem;
        font-size: 0.95rem;
      }

      section {
        padding: 1rem;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>Jaime Sánchez Navarro</h1>
    <p>
      📍 <a href="https://www.google.com/maps/place/Hinojosa+del+Duque,+Córdoba,+España" target="_blank">Hinojosa del Duque</a> |
      📞 <a href="tel:+34640583528">+34 640 583 528</a> |
      ✉️ <a href="mailto:jaimesncv@gmail.com">jaimesncv@gmail.com</a>
    </p>
  </header>

  <nav>
    <a href="#" data-section="resumen">🎯 Resumen</a>
    <a href="#" data-section="habilidades-tecnicas">🛠️ Técnicas</a>
    <a href="#" data-section="habilidades-personales">🤝 Personales</a>
    <a href="#" data-section="experiencia">💼 Experiencia</a>
    <a href="#" data-section="formacion">🎓 Formación</a>
    <a href="#" data-section="idiomas">🌍 Idiomas</a>
    <a href="#" data-section="disponibilidad">💡 Intereses</a>
    <a href="#" data-section="trabajos">🗂️ Trabajos</a>
    <a href="#" data-section="certificados">📄 Certificados</a>
  </nav>

  <section id="resumen" class="active">
    <h2>🎯 Resumen Profesional</h2>
    <p>Técnico en Sistemas Microinformáticos y Redes con experiencia en soporte técnico,
    atención al cliente y mantenimiento de equipos. Me interesa aplicar mis conocimientos
    tanto en entornos TIC como en el sector retail.</p>
  </section>

  <section id="habilidades-tecnicas">
    <h2>🛠️ Habilidades Técnicas</h2>
    <ul>
      <li>Montaje y mantenimiento de equipos informáticos.</li>
      <li>Diagnóstico y reparación de averías hardware.</li>
      <li>Instalación de sistemas operativos (Windows, Linux).</li>
      <li>Configuración de redes LAN/WiFi, routers, switches.</li>
      <li>Ciberseguridad básica y antivirus.</li>
      <li>Soporte técnico remoto (TeamViewer, AnyDesk).</li>
      <li>Software ofimático (Office, Gimp, Sketchup...)</li>
    </ul>
  </section>

  <section id="habilidades-personales">
    <h2>🤝 Habilidades Personales</h2>
    <ul>
      <li>Resolución de problemas y atención al cliente.</li>
      <li>Trabajo en equipo y comunicación efectiva.</li>
      <li>Organización y puntualidad.</li>
      <li>Actitud proactiva y ganas de aprender.</li>
    </ul>
  </section>

  <section id="experiencia">
    <h2>💼 Experiencia Profesional</h2>
    <p><strong>Camarero de barra</strong> – Veranos 2022-2024 en Córdoba.</p>
    <p><strong>Soporte Informático</strong> – Ayuntamiento de Hinojosa del Duque (2024).</p>
    <p><strong>Técnico en tienda</strong> – InformaticaJPD – Getafe (2024).</p>
  </section>

  <section id="formacion">
    <h2>🎓 Formación Académica</h2>
    <p>Grado Medio en SMR – IES Jerez y Caballero – Córdoba (2022–2024)</p>
    <p>Grado Básico en Informática – IES Julio Verne – Madrid (2020–2021)</p>
    <p>ESO – IES Padre Juan Ruiz (2021–2022)</p>
  </section>

  <section id="idiomas">
    <h2>🌍 Idiomas</h2>
    <ul>
      <li>Español – Nativo</li>
      <li>Inglés – B1 (Estudiando)</li>
    </ul>
  </section>

  <section id="disponibilidad">
    <h2>💡 Disponibilidad e Intereses</h2>
    <ul>
      <li>Incorporación inmediata</li>
      <li>Flexibilidad horaria</li>
      <li>Interés en aplicar tecnología en entornos laborales</li>
    </ul>
  </section>

  <section id="trabajos">
    <h2>🗂️ Mis Trabajos</h2>
    <p>Esta página web :)</p>
  </section>

  <section id="certificados">
    <h2>📄 Certificados</h2>
    <p>En proceso de obtención.</p>
  </section>

  <script>
    const links = document.querySelectorAll("nav a");
    const sections = document.querySelectorAll("section");

    links.forEach(link => {
      link.addEventListener("click", e => {
        e.preventDefault();
        const id = link.getAttribute("data-section");

        sections.forEach(s => s.classList.remove("active"));
        document.getElementById(id).classList.add("active");
      });
    });
  </script>
</body>
</html>
