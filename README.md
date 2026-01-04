<!doctype html>
<html lang="es" class="h-full">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Inmobiliaria Elegante</title>
  <script src="/_sdk/element_sdk.js"></script>
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    body {
      box-sizing: border-box;
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
    
    .fade-in-up {
      animation: fadeInUp 0.8s ease-out forwards;
    }
    
    .property-card {
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    
    .property-card:hover {
      transform: translateY(-8px);
      box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
    }
    
    .nav-link {
      transition: color 0.3s ease;
    }
  </style>
  <style>@view-transition { navigation: auto; }</style>
  <script src="/_sdk/data_sdk.js" type="text/javascript"></script>
 </head>
 <body class="h-full">
  <div id="app-wrapper" class="w-full h-full overflow-auto" style="background: #ffffff;"><!-- Navigation -->
   <nav class="w-full" style="background: #ffffff; border-bottom: 1px solid #e5e7eb; box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);">
    <div style="max-width: 1200px; margin: 0 auto; padding: 24px 32px;">
     <div style="display: flex; justify-content: space-between; align-items: center;">
      <div>
       <h1 id="company-name" style="font-size: 28px; font-weight: 700; margin: 0; color: #DDAE52;">Inmobiliaria Maison Heim</h1>
       <p id="tagline" style="font-size: 13px; margin: 4px 0 0 0; color: #6b7280;">Tu hogar ideal te espera</p>
      </div>
      <div style="display: flex; gap: 32px;"><a href="#propiedades" class="nav-link" style="text-decoration: none; font-weight: 500; font-size: 15px; color: #2c3e50;">Propiedades</a> <a href="#contacto" class="nav-link" style="text-decoration: none; font-weight: 500; font-size: 15px; color: #2c3e50;">Contacto</a>
      </div>
     </div>
    </div>
   </nav><!-- Hero Section -->
   <section style="padding: 100px 32px; text-align: center; background: linear-gradient(135deg, #f8f9fa 0%, #ffffff 100%);">
    <div style="max-width: 900px; margin: 0 auto;" class="fade-in-up">
     <h2 id="hero-title" style="font-size: 56px; font-weight: 800; margin: 0 0 24px 0; color: #2c3e50; line-height: 1.2;">Encuentra tu hogar perfecto</h2>
     <p id="hero-subtitle" style="font-size: 20px; margin: 0 0 40px 0; color: #6b7280;">Propiedades exclusivas en las mejores ubicaciones</p><a href="#propiedades" id="cta-button" style="display: inline-block; padding: 16px 48px; background: #DDAE52; color: #ffffff; text-decoration: none; border-radius: 8px; font-weight: 600; font-size: 16px; transition: background 0.3s ease, transform 0.3s ease; box-shadow: 0 4px 15px rgba(221, 174, 82, 0.3);">Ver Propiedades</a>
    </div>
   </section><!-- Properties Section -->
   <section id="propiedades" style="padding: 80px 32px; background: #ffffff;">
    <div style="max-width: 1200px; margin: 0 auto;">
     <h2 id="properties-title" style="font-size: 42px; font-weight: 700; margin: 0 0 60px 0; text-align: center; color: #2c3e50;">Propiedades Destacadas</h2>
     <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 32px;"><!-- Property 1 -->
      <div class="property-card" style="background: #f8f9fa; border-radius: 12px; overflow: hidden; box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08); border: 1px solid #e5e7eb;">
       <div style="width: 100%; height: 240px; background: linear-gradient(135deg, #DDAE52 0%, #c99a42 100%); display: flex; align-items: center; justify-content: center;">
        <svg width="80" height="80" viewbox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M3 9L12 2L21 9V20C21 20.5304 20.7893 21.0391 20.4142 21.4142C20.0391 21.7893 19.5304 22 19 22H5C4.46957 22 3.96086 21.7893 3.58579 21.4142C3.21071 21.0391 3 20.5304 3 20V9Z" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" /> <path d="M9 22V12H15V22" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
        </svg>
       </div>
       <div style="padding: 24px;">
        <h3 style="font-size: 22px; font-weight: 700; margin: 0 0 12px 0; color: #2c3e50;">Villa Moderna</h3>
        <p style="font-size: 14px; color: #6b7280; margin: 0 0 16px 0; line-height: 1.6;">Espectacular villa con diseño contemporáneo, 4 habitaciones, jardín y piscina privada.</p>
        <div style="display: flex; justify-content: space-between; align-items: center;"><span style="font-size: 28px; font-weight: 700; color: #DDAE52;">€850,000</span> <button onclick="showPropertyModal(0)" style="padding: 10px 24px; background: #2c3e50; color: #ffffff; border: none; border-radius: 6px; font-weight: 600; cursor: pointer; transition: background 0.3s ease;">Ver más</button>
        </div>
       </div>
      </div><!-- Property 2 -->
      <div class="property-card" style="background: #f8f9fa; border-radius: 12px; overflow: hidden; box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08); border: 1px solid #e5e7eb;">
       <div style="width: 100%; height: 240px; background: linear-gradient(135deg, #DDAE52 0%, #c99a42 100%); display: flex; align-items: center; justify-content: center;">
        <svg width="80" height="80" viewbox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M3 9L12 2L21 9V20C21 20.5304 20.7893 21.0391 20.4142 21.4142C20.0391 21.7893 19.5304 22 19 22H5C4.46957 22 3.96086 21.7893 3.58579 21.4142C3.21071 21.0391 3 20.5304 3 20V9Z" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" /> <path d="M9 22V12H15V22" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
        </svg>
       </div>
       <div style="padding: 24px;">
        <h3 style="font-size: 22px; font-weight: 700; margin: 0 0 12px 0; color: #2c3e50;">Ático Céntrico</h3>
        <p style="font-size: 14px; color: #6b7280; margin: 0 0 16px 0; line-height: 1.6;">Exclusivo ático en el centro de la ciudad con terraza panorámica y acabados de lujo.</p>
        <div style="display: flex; justify-content: space-between; align-items: center;"><span style="font-size: 28px; font-weight: 700; color: #DDAE52;">€620,000</span> <button onclick="showPropertyModal(1)" style="padding: 10px 24px; background: #2c3e50; color: #ffffff; border: none; border-radius: 6px; font-weight: 600; cursor: pointer; transition: background 0.3s ease;">Ver más</button>
        </div>
       </div>
      </div><!-- Property 3 -->
      <div class="property-card" style="background: #f8f9fa; border-radius: 12px; overflow: hidden; box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08); border: 1px solid #e5e7eb;">
       <div style="width: 100%; height: 240px; background: linear-gradient(135deg, #DDAE52 0%, #c99a42 100%); display: flex; align-items: center; justify-content: center;">
        <svg width="80" height="80" viewbox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M3 9L12 2L21 9V20C21 20.5304 20.7893 21.0391 20.4142 21.4142C20.0391 21.7893 19.5304 22 19 22H5C4.46957 22 3.96086 21.7893 3.58579 21.4142C3.21071 21.0391 3 20.5304 3 20V9Z" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" /> <path d="M9 22V12H15V22" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
        </svg>
       </div>
       <div style="padding: 24px;">
        <h3 style="font-size: 22px; font-weight: 700; margin: 0 0 12px 0; color: #2c3e50;">Casa Costera</h3>
        <p style="font-size: 14px; color: #6b7280; margin: 0 0 16px 0; line-height: 1.6;">Hermosa casa frente al mar con vistas impresionantes y acceso directo a la playa.</p>
        <div style="display: flex; justify-content: space-between; align-items: center;"><span style="font-size: 28px; font-weight: 700; color: #DDAE52;">€1,200,000</span> <button onclick="showPropertyModal(2)" style="padding: 10px 24px; background: #2c3e50; color: #ffffff; border: none; border-radius: 6px; font-weight: 600; cursor: pointer; transition: background 0.3s ease;">Ver más</button>
        </div>
       </div>
      </div>
     </div>
    </div>
   </section><!-- Property Modal -->
   <div id="property-modal" style="display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0, 0, 0, 0.7); z-index: 1000; align-items: center; justify-content: center; padding: 20px;">
    <div style="background: #ffffff; border-radius: 16px; max-width: 600px; width: 100%; max-height: 90%; overflow-y: auto; position: relative;"><button onclick="closePropertyModal()" style="position: absolute; top: 16px; right: 16px; background: #f8f9fa; border: none; width: 40px; height: 40px; border-radius: 50%; cursor: pointer; font-size: 24px; color: #2c3e50; display: flex; align-items: center; justify-content: center; transition: background 0.3s ease;">×</button>
     <div id="modal-content" style="padding: 40px;"><!-- Content will be filled by JavaScript -->
     </div>
    </div>
   </div><!-- Contact Section -->
   <section id="contacto" style="padding: 80px 32px; background: linear-gradient(135deg, #f8f9fa 0%, #ffffff 100%);">
    <div style="max-width: 800px; margin: 0 auto; text-align: center;">
     <h2 id="contact-title" style="font-size: 42px; font-weight: 700; margin: 0 0 16px 0; color: #2c3e50;">Contáctanos</h2>
     <p id="contact-subtitle" style="font-size: 18px; margin: 0 0 48px 0; color: #6b7280;">Estamos aquí para ayudarte a encontrar tu hogar ideal</p>
     <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 32px; margin-top: 48px; margin-bottom: 48px;">
      <div style="padding: 32px; background: #ffffff; border-radius: 12px; box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08); border: 1px solid #e5e7eb;">
       <svg style="margin: 0 auto 16px auto;" width="40" height="40" viewbox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M22 16.92V19.92C22 20.4696 21.7893 20.9968 21.4142 21.3869C21.0391 21.7771 20.5304 21.9999 20 22C16.7428 21.7248 13.6047 20.6127 10.85 18.76C8.30382 17.0775 6.18131 14.8338 4.66999 12.2C2.77999 9.38713 1.67317 6.17726 1.42999 2.85C1.42008 2.31467 1.62906 1.79743 2.00665 1.41051C2.38424 1.02359 2.89889 0.794662 3.42999 0.789999H6.42999C7.38006 0.780319 8.19732 1.42108 8.40999 2.33C8.60568 3.22925 8.89922 4.10437 9.27999 4.94C9.51289 5.51938 9.44373 6.17744 9.09999 6.69L7.78999 8.36C9.38541 11.069 11.7881 13.5981 14.41 15.27L16.08 13.93C16.5729 13.5682 17.2069 13.4945 17.77 13.73C18.5899 14.1181 19.4481 14.4189 20.33 14.62C21.2568 14.8367 21.9088 15.6801 21.91 16.65L22 16.92Z" stroke="#DDAE52" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
       </svg>
       <h3 id="phone-label" style="font-size: 16px; font-weight: 600; margin: 0 0 8px 0; color: #2c3e50;">Teléfono</h3>
       <p style="font-size: 14px; margin: 0; color: #6b7280;">+34 900 123 456</p>
      </div>
      <div style="padding: 32px; background: #ffffff; border-radius: 12px; box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08); border: 1px solid #e5e7eb;">
       <svg style="margin: 0 auto 16px auto;" width="40" height="40" viewbox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M4 4H20C21.1 4 22 4.9 22 6V18C22 19.1 21.1 20 20 20H4C2.9 20 2 19.1 2 18V6C2 4.9 2.9 4 4 4Z" stroke="#DDAE52" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" /> <path d="M22 6L12 13L2 6" stroke="#DDAE52" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
       </svg>
       <h3 id="email-label" style="font-size: 16px; font-weight: 600; margin: 0 0 8px 0; color: #2c3e50;">Email</h3>
       <p style="font-size: 14px; margin: 0; color: #6b7280;">info@inmobiliaria.com</p>
      </div>
      <div style="padding: 32px; background: #ffffff; border-radius: 12px; box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08); border: 1px solid #e5e7eb;">
       <svg style="margin: 0 auto 16px auto;" width="40" height="40" viewbox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M21 10C21 17 12 23 12 23C12 23 3 17 3 10C3 7.61305 3.94821 5.32387 5.63604 3.63604C7.32387 1.94821 9.61305 1 12 1C14.3869 1 16.6761 1.94821 18.364 3.63604C20.0518 5.32387 21 7.61305 21 10Z" stroke="#DDAE52" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" /> <path d="M12 13C13.6569 13 15 11.6569 15 10C15 8.34315 13.6569 7 12 7C10.3431 7 9 8.34315 9 10C9 11.6569 10.3431 13 12 13Z" stroke="#DDAE52" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
       </svg>
       <h3 id="address-label" style="font-size: 16px; font-weight: 600; margin: 0 0 8px 0; color: #2c3e50;">Dirección</h3>
       <p style="font-size: 14px; margin: 0; color: #6b7280;">Calle Principal 123, Madrid</p>
      </div>
     </div><!-- Contact Form -->
     <form id="contact-form" style="background: #ffffff; padding: 40px; border-radius: 12px; box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08); text-align: left; max-width: 600px; margin: 0 auto;">
      <h3 style="font-size: 24px; font-weight: 700; margin: 0 0 24px 0; color: #2c3e50; text-align: center;">Solicita Información</h3>
      <div style="margin-bottom: 20px;"><label for="name" style="display: block; font-size: 14px; font-weight: 600; margin-bottom: 8px; color: #2c3e50;">Nombre completo</label> <input type="text" id="name" name="name" required style="width: 100%; padding: 12px; border: 1px solid #e5e7eb; border-radius: 6px; font-size: 14px; box-sizing: border-box;">
      </div>
      <div style="margin-bottom: 20px;"><label for="email" style="display: block; font-size: 14px; font-weight: 600; margin-bottom: 8px; color: #2c3e50;">Email</label> <input type="email" id="email" name="email" required style="width: 100%; padding: 12px; border: 1px solid #e5e7eb; border-radius: 6px; font-size: 14px; box-sizing: border-box;">
      </div>
      <div style="margin-bottom: 20px;"><label for="phone" style="display: block; font-size: 14px; font-weight: 600; margin-bottom: 8px; color: #2c3e50;">Teléfono</label> <input type="tel" id="phone" name="phone" required style="width: 100%; padding: 12px; border: 1px solid #e5e7eb; border-radius: 6px; font-size: 14px; box-sizing: border-box;">
      </div>
      <div style="margin-bottom: 24px;"><label for="message" style="display: block; font-size: 14px; font-weight: 600; margin-bottom: 8px; color: #2c3e50;">Mensaje</label> <textarea id="message" name="message" rows="4" required style="width: 100%; padding: 12px; border: 1px solid #e5e7eb; border-radius: 6px; font-size: 14px; resize: vertical; box-sizing: border-box;"></textarea>
      </div><button type="submit" style="width: 100%; padding: 14px; background: #DDAE52; color: #ffffff; border: none; border-radius: 6px; font-weight: 600; font-size: 16px; cursor: pointer; transition: background 0.3s ease;">Enviar Mensaje</button>
      <div id="form-message" style="margin-top: 16px; padding: 12px; border-radius: 6px; display: none; text-align: center; font-size: 14px;"></div>
     </form>
    </div>
   </section><!-- Footer -->
   <footer style="padding: 32px; text-align: center; background: #f8f9fa; border-top: 1px solid #e5e7eb;">
    <p style="margin: 0; font-size: 14px; color: #6b7280;">© 2024 Inmobiliaria Maison Heim. Todos los derechos reservados.</p>
   </footer>
  </div>
  <script>
    const defaultConfig = {
      background_color: "#ffffff",
      surface_color: "#f8f9fa",
      text_color: "#2c3e50",
      primary_action_color: "#DDAE52",
      secondary_action_color: "#2c3e50",
      font_family: "system-ui, -apple-system, sans-serif",
      font_size: 16,
      company_name: "Inmobiliaria Maison Heim",
      tagline: "Tu hogar ideal te espera",
      hero_title: "Encuentra tu hogar perfecto",
      hero_subtitle: "Propiedades exclusivas en las mejores ubicaciones",
      cta_button: "Ver Propiedades",
      properties_title: "Propiedades Destacadas",
      contact_title: "Contáctanos",
      contact_subtitle: "Estamos aquí para ayudarte a encontrar tu hogar ideal",
      phone_label: "Teléfono",
      email_label: "Email",
      address_label: "Dirección"
    };

    // Property data
    const properties = [
      {
        title: "Villa Moderna",
        description: "Espectacular villa con diseño contemporáneo en una de las zonas más exclusivas de Madrid. Esta propiedad combina elegancia moderna con funcionalidad, ofreciendo amplios espacios luminosos y acabados de primera calidad.",
        price: "€850,000",
        details: {
          habitaciones: "4",
          banos: "3",
          superficie: "320 m²",
          ubicacion: "Pozuelo de Alarcón, Madrid",
          ano: "2020",
          tipo: "Villa independiente",
          estado: "Excelente",
          orientacion: "Sur"
        },
        features: [
          "Piscina privada climatizada de 40m²",
          "Jardín amplio de 500m² con sistema de riego automático",
          "Garaje para 2 coches con puerta automática",
          "Sistema de seguridad con cámaras y alarma",
          "Cocina equipada con electrodomésticos Bosch",
          "Suelo radiante en toda la vivienda",
          "Paneles solares para agua caliente",
          "Domótica integrada",
          "Trastero de 30m²",
          "Zona de BBQ cubierta"
        ],
        additionalInfo: "La villa está situada en una urbanización privada con seguridad 24h, zonas deportivas y parque infantil. Cerca de colegios internacionales, centros comerciales y con excelente acceso a la M-40 y M-50."
      },
      {
        title: "Ático Céntrico",
        description: "Exclusivo ático en el prestigioso barrio de Salamanca, completamente reformado con materiales de lujo. Disfruta de una terraza privada de 80m² con vistas panorámicas a toda la ciudad.",
        price: "€620,000",
        details: {
          habitaciones: "3",
          banos: "2",
          superficie: "180 m²",
          ubicacion: "Salamanca, Madrid",
          ano: "Edificio 1950, reformado 2022",
          tipo: "Ático con terraza",
          estado: "Reformado nuevo",
          orientacion: "Este-Oeste"
        },
        features: [
          "Terraza panorámica de 80m² con pérgola",
          "Vistas espectaculares 360°",
          "Ascensor privado directo al ático",
          "Cocina de diseño italiana Valcucine",
          "Aire acondicionado por conductos",
          "Suelos de roble natural",
          "Armarios empotrados a medida",
          "Baño principal con jacuzzi y ducha de lluvia",
          "Sistema de sonido integrado",
          "Portero con video y apertura remota"
        ],
        additionalInfo: "Ubicado en la Milla de Oro de Madrid, rodeado de boutiques de lujo, restaurantes con estrella Michelin y galerías de arte. A 5 minutos andando del Retiro y con todas las comodidades al alcance."
      },
      {
        title: "Casa Costera",
        description: "Hermosa villa mediterránea frente al mar en primera línea de playa en Marbella. Arquitectura andaluza tradicional con todas las comodidades modernas, perfecta para disfrutar del estilo de vida costero.",
        price: "€1,200,000",
        details: {
          habitaciones: "5",
          banos: "4",
          superficie: "450 m²",
          ubicacion: "Marbella, Málaga",
          ano: "2018",
          tipo: "Villa de lujo frente al mar",
          estado: "Impecable",
          orientacion: "Sur (vistas al mar)"
        },
        features: [
          "Acceso directo privado a la playa",
          "Vistas panorámicas al Mediterráneo",
          "Piscina infinity de 60m² con efecto espejo",
          "Zona de barbacoa profesional y comedor exterior",
          "Bodega climatizada para 200 botellas",
          "Gimnasio totalmente equipado",
          "Jacuzzi exterior con vistas al mar",
          "Suite principal de 80m² con vestidor",
          "Cocina profesional con isla central",
          "Garaje para 3 vehículos",
          "Sistema de domótica Lutron",
          "Jardines diseñados por paisajista"
        ],
        additionalInfo: "Propiedad única en una de las zonas más codiciadas de la Costa del Sol. A 10 minutos del Puerto Banús y del centro de Marbella. Incluye membresía opcional al club de playa exclusivo. Ideal como residencia permanente o inversión de lujo."
      }
    ];

    // Show property modal
    function showPropertyModal(index) {
      const property = properties[index];
      const modal = document.getElementById('property-modal');
      const modalContent = document.getElementById('modal-content');
      
      modalContent.innerHTML = `
        <h2 style="font-size: 32px; font-weight: 700; margin: 0 0 16px 0; color: #2c3e50;">${property.title}</h2>
        <p style="font-size: 36px; font-weight: 700; color: #DDAE52; margin: 0 0 24px 0;">${property.price}</p>
        
        <p style="font-size: 16px; color: #6b7280; margin: 0 0 32px 0; line-height: 1.7;">${property.description}</p>
        
        <h3 style="font-size: 20px; font-weight: 700; margin: 0 0 16px 0; color: #2c3e50;">Detalles de la Propiedad</h3>
        <div style="display: grid; grid-template-columns: repeat(2, 1fr); gap: 16px; margin-bottom: 32px;">
          <div style="padding: 16px; background: #f8f9fa; border-radius: 8px;">
            <div style="font-size: 12px; color: #6b7280; margin-bottom: 4px; text-transform: uppercase; letter-spacing: 0.5px;">Habitaciones</div>
            <div style="font-size: 18px; font-weight: 600; color: #2c3e50;">${property.details.habitaciones}</div>
          </div>
          <div style="padding: 16px; background: #f8f9fa; border-radius: 8px;">
            <div style="font-size: 12px; color: #6b7280; margin-bottom: 4px; text-transform: uppercase; letter-spacing: 0.5px;">Baños</div>
            <div style="font-size: 18px; font-weight: 600; color: #2c3e50;">${property.details.banos}</div>
          </div>
          <div style="padding: 16px; background: #f8f9fa; border-radius: 8px;">
            <div style="font-size: 12px; color: #6b7280; margin-bottom: 4px; text-transform: uppercase; letter-spacing: 0.5px;">Superficie</div>
            <div style="font-size: 18px; font-weight: 600; color: #2c3e50;">${property.details.superficie}</div>
          </div>
          <div style="padding: 16px; background: #f8f9fa; border-radius: 8px;">
            <div style="font-size: 12px; color: #6b7280; margin-bottom: 4px; text-transform: uppercase; letter-spacing: 0.5px;">Año</div>
            <div style="font-size: 18px; font-weight: 600; color: #2c3e50;">${property.details.ano}</div>
          </div>
          <div style="padding: 16px; background: #f8f9fa; border-radius: 8px;">
            <div style="font-size: 12px; color: #6b7280; margin-bottom: 4px; text-transform: uppercase; letter-spacing: 0.5px;">Tipo</div>
            <div style="font-size: 18px; font-weight: 600; color: #2c3e50;">${property.details.tipo}</div>
          </div>
          <div style="padding: 16px; background: #f8f9fa; border-radius: 8px;">
            <div style="font-size: 12px; color: #6b7280; margin-bottom: 4px; text-transform: uppercase; letter-spacing: 0.5px;">Estado</div>
            <div style="font-size: 18px; font-weight: 600; color: #2c3e50;">${property.details.estado}</div>
          </div>
          <div style="padding: 16px; background: #f8f9fa; border-radius: 8px; grid-column: 1 / -1;">
            <div style="font-size: 12px; color: #6b7280; margin-bottom: 4px; text-transform: uppercase; letter-spacing: 0.5px;">Orientación</div>
            <div style="font-size: 18px; font-weight: 600; color: #2c3e50;">${property.details.orientacion}</div>
          </div>
          <div style="padding: 16px; background: #f8f9fa; border-radius: 8px; grid-column: 1 / -1;">
            <div style="font-size: 12px; color: #6b7280; margin-bottom: 4px; text-transform: uppercase; letter-spacing: 0.5px;">📍 Ubicación</div>
            <div style="font-size: 18px; font-weight: 600; color: #2c3e50;">${property.details.ubicacion}</div>
          </div>
        </div>
        
        <h3 style="font-size: 20px; font-weight: 700; margin: 0 0 16px 0; color: #2c3e50;">✨ Características Principales</h3>
        <ul style="margin: 0 0 32px 0; padding-left: 20px; color: #4a5568; line-height: 2.2; font-size: 15px;">
          ${property.features.map(feature => `<li style="margin-bottom: 8px;">${feature}</li>`).join('')}
        </ul>
        
        <div style="background: #f0f7ff; border-left: 4px solid #DDAE52; padding: 20px; border-radius: 8px; margin-bottom: 32px;">
          <h3 style="font-size: 18px; font-weight: 700; margin: 0 0 12px 0; color: #2c3e50;">ℹ️ Información Adicional</h3>
          <p style="font-size: 15px; color: #4a5568; margin: 0; line-height: 1.7;">${property.additionalInfo}</p>
        </div>
        
        <button onclick="showInterestForm('${property.title}')" style="width: 100%; padding: 16px; background: #DDAE52; color: #ffffff; border: none; border-radius: 8px; font-weight: 600; font-size: 17px; cursor: pointer; transition: all 0.3s ease; box-shadow: 0 4px 12px rgba(221, 174, 82, 0.3);">🏠 Estoy Interesado - Solicitar Más Información</button>
      `;
      
      modal.style.display = 'flex';
      document.body.style.overflow = 'hidden';
    }

    // Close property modal
    function closePropertyModal() {
      const modal = document.getElementById('property-modal');
      modal.style.display = 'none';
      document.body.style.overflow = 'auto';
    }

    // Show interest form (scroll to contact)
    function showInterestForm(propertyName) {
      closePropertyModal();
      const contactSection = document.getElementById('contacto');
      contactSection.scrollIntoView({ behavior: 'smooth' });
      
      setTimeout(() => {
        const messageField = document.getElementById('message');
        messageField.value = `Estoy interesado en la propiedad: ${propertyName}`;
        messageField.focus();
      }, 800);
    }

    // Contact form submission
    document.getElementById('contact-form').addEventListener('submit', function(e) {
      e.preventDefault();
      
      const formMessage = document.getElementById('form-message');
      const submitButton = this.querySelector('button[type="submit"]');
      
      // Disable button and show loading state
      submitButton.disabled = true;
      submitButton.textContent = 'Enviando...';
      submitButton.style.opacity = '0.7';
      
      // Simulate form submission
      setTimeout(() => {
        formMessage.style.display = 'block';
        formMessage.style.background = '#d4edda';
        formMessage.style.color = '#155724';
        formMessage.style.border = '1px solid #c3e6cb';
        formMessage.textContent = '¡Mensaje enviado con éxito! Nos pondremos en contacto contigo pronto.';
        
        // Reset form
        this.reset();
        
        // Re-enable button
        submitButton.disabled = false;
        submitButton.textContent = 'Enviar Mensaje';
        submitButton.style.opacity = '1';
        
        // Hide message after 5 seconds
        setTimeout(() => {
          formMessage.style.display = 'none';
        }, 5000);
      }, 1500);
    });

    // Close modal on backdrop click
    document.getElementById('property-modal').addEventListener('click', function(e) {
      if (e.target === this) {
        closePropertyModal();
      }
    });

    async function onConfigChange(config) {
      const backgroundColor = config.background_color || defaultConfig.background_color;
      const surfaceColor = config.surface_color || defaultConfig.surface_color;
      const textColor = config.text_color || defaultConfig.text_color;
      const primaryActionColor = config.primary_action_color || defaultConfig.primary_action_color;
      const secondaryActionColor = config.secondary_action_color || defaultConfig.secondary_action_color;
      const customFont = config.font_family || defaultConfig.font_family;
      const baseSize = config.font_size || defaultConfig.font_size;
      const baseFontStack = 'system-ui, -apple-system, sans-serif';

      // Update colors
      document.getElementById('app-wrapper').style.background = backgroundColor;
      document.querySelector('nav').style.background = backgroundColor;
      document.getElementById('company-name').style.color = primaryActionColor;
      
      const navLinks = document.querySelectorAll('.nav-link');
      navLinks.forEach(link => {
        link.style.color = textColor;
      });

      const propertyCards = document.querySelectorAll('.property-card');
      propertyCards.forEach(card => {
        card.style.background = surfaceColor;
      });

      const propertyTitles = document.querySelectorAll('.property-card h3');
      propertyTitles.forEach(title => {
        title.style.color = textColor;
      });

      const priceElements = document.querySelectorAll('.property-card span');
      priceElements.forEach(price => {
        price.style.color = primaryActionColor;
      });

      const viewMoreButtons = document.querySelectorAll('.property-card button');
      viewMoreButtons.forEach(button => {
        button.style.background = secondaryActionColor;
      });

      document.getElementById('cta-button').style.background = primaryActionColor;
      document.getElementById('properties-title').style.color = textColor;
      document.getElementById('contact-title').style.color = textColor;
      document.getElementById('contact-subtitle').style.color = textColor;

      const contactLabels = document.querySelectorAll('#contacto h3');
      contactLabels.forEach(label => {
        label.style.color = textColor;
      });

      const contactIcons = document.querySelectorAll('#contacto svg path');
      contactIcons.forEach(icon => {
        icon.setAttribute('stroke', primaryActionColor);
      });

      const contactSection = document.querySelector('#contacto');
      contactSection.style.background = `linear-gradient(135deg, ${surfaceColor} 0%, ${backgroundColor} 100%)`;

      // Update fonts
      document.getElementById('company-name').style.fontFamily = `${customFont}, ${baseFontStack}`;
      document.getElementById('company-name').style.fontSize = `${baseSize * 1.75}px`;
      
      document.getElementById('tagline').style.fontFamily = `${customFont}, ${baseFontStack}`;
      document.getElementById('tagline').style.fontSize = `${baseSize * 0.8125}px`;
      
      document.getElementById('hero-title').style.fontFamily = `${customFont}, ${baseFontStack}`;
      document.getElementById('hero-title').style.fontSize = `${baseSize * 3.5}px`;
      
      document.getElementById('hero-subtitle').style.fontFamily = `${customFont}, ${baseFontStack}`;
      document.getElementById('hero-subtitle').style.fontSize = `${baseSize * 1.25}px`;
      
      document.getElementById('cta-button').style.fontFamily = `${customFont}, ${baseFontStack}`;
      document.getElementById('cta-button').style.fontSize = `${baseSize}px`;
      
      document.getElementById('properties-title').style.fontFamily = `${customFont}, ${baseFontStack}`;
      document.getElementById('properties-title').style.fontSize = `${baseSize * 2.625}px`;
      
      const propertyTitles = document.querySelectorAll('.property-card h3');
      propertyTitles.forEach(title => {
        title.style.fontFamily = `${customFont}, ${baseFontStack}`;
        title.style.fontSize = `${baseSize * 1.375}px`;
      });

      document.getElementById('contact-title').style.fontFamily = `${customFont}, ${baseFontStack}`;
      document.getElementById('contact-title').style.fontSize = `${baseSize * 2.625}px`;
      
      document.getElementById('contact-subtitle').style.fontFamily = `${customFont}, ${baseFontStack}`;
      document.getElementById('contact-subtitle').style.fontSize = `${baseSize * 1.125}px`;

      // Update text content
      document.getElementById('company-name').textContent = config.company_name || defaultConfig.company_name;
      document.getElementById('tagline').textContent = config.tagline || defaultConfig.tagline;
      document.getElementById('hero-title').textContent = config.hero_title || defaultConfig.hero_title;
      document.getElementById('hero-subtitle').textContent = config.hero_subtitle || defaultConfig.hero_subtitle;
      document.getElementById('cta-button').textContent = config.cta_button || defaultConfig.cta_button;
      document.getElementById('properties-title').textContent = config.properties_title || defaultConfig.properties_title;
      document.getElementById('contact-title').textContent = config.contact_title || defaultConfig.contact_title;
      document.getElementById('contact-subtitle').textContent = config.contact_subtitle || defaultConfig.contact_subtitle;
      document.getElementById('phone-label').textContent = config.phone_label || defaultConfig.phone_label;
      document.getElementById('email-label').textContent = config.email_label || defaultConfig.email_label;
      document.getElementById('address-label').textContent = config.address_label || defaultConfig.address_label;
    }

    function mapToCapabilities(config) {
      return {
        recolorables: [
          {
            get: () => config.background_color || defaultConfig.background_color,
            set: (value) => {
              config.background_color = value;
              window.elementSdk.setConfig({ background_color: value });
            }
          },
          {
            get: () => config.surface_color || defaultConfig.surface_color,
            set: (value) => {
              config.surface_color = value;
              window.elementSdk.setConfig({ surface_color: value });
            }
          },
          {
            get: () => config.text_color || defaultConfig.text_color,
            set: (value) => {
              config.text_color = value;
              window.elementSdk.setConfig({ text_color: value });
            }
          },
          {
            get: () => config.primary_action_color || defaultConfig.primary_action_color,
            set: (value) => {
              config.primary_action_color = value;
              window.elementSdk.setConfig({ primary_action_color: value });
            }
          },
          {
            get: () => config.secondary_action_color || defaultConfig.secondary_action_color,
            set: (value) => {
              config.secondary_action_color = value;
              window.elementSdk.setConfig({ secondary_action_color: value });
            }
          }
        ],
        borderables: [],
        fontEditable: {
          get: () => config.font_family || defaultConfig.font_family,
          set: (value) => {
            config.font_family = value;
            window.elementSdk.setConfig({ font_family: value });
          }
        },
        fontSizeable: {
          get: () => config.font_size || defaultConfig.font_size,
          set: (value) => {
            config.font_size = value;
            window.elementSdk.setConfig({ font_size: value });
          }
        }
      };
    }

    function mapToEditPanelValues(config) {
      return new Map([
        ["company_name", config.company_name || defaultConfig.company_name],
        ["tagline", config.tagline || defaultConfig.tagline],
        ["hero_title", config.hero_title || defaultConfig.hero_title],
        ["hero_subtitle", config.hero_subtitle || defaultConfig.hero_subtitle],
        ["cta_button", config.cta_button || defaultConfig.cta_button],
        ["properties_title", config.properties_title || defaultConfig.properties_title],
        ["contact_title", config.contact_title || defaultConfig.contact_title],
        ["contact_subtitle", config.contact_subtitle || defaultConfig.contact_subtitle],
        ["phone_label", config.phone_label || defaultConfig.phone_label],
        ["email_label", config.email_label || defaultConfig.email_label],
        ["address_label", config.address_label || defaultConfig.address_label]
      ]);
    }

    if (window.elementSdk) {
      window.elementSdk.init({
        defaultConfig,
        onConfigChange,
        mapToCapabilities,
        mapToEditPanelValues
      });
    }

    // Smooth scroll for navigation
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
          target.scrollIntoView({ behavior: 'smooth', block: 'start' });
        }
      });
    });

    // Button hover effects
    document.querySelectorAll('button').forEach(button => {
      button.addEventListener('mouseenter', function() {
        this.style.transform = 'scale(1.05)';
      });
      button.addEventListener('mouseleave', function() {
        this.style.transform = 'scale(1)';
      });
    });

    // CTA button hover effect
    const ctaButton = document.getElementById('cta-button');
    ctaButton.addEventListener('mouseenter', function() {
      this.style.transform = 'translateY(-2px)';
      this.style.boxShadow = '0 6px 20px rgba(221, 174, 82, 0.4)';
    });
    ctaButton.addEventListener('mouseleave', function() {
      this.style.transform = 'translateY(0)';
      this.style.boxShadow = '0 4px 15px rgba(221, 174, 82, 0.3)';
    });
  </script>
 <script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9b8c2b971719cc40',t:'MTc2NzU0NDc0OC4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
