<h1 align="center">Adrián Castrejón</h1>

<p align="center">
  <b>Desarrollador de aplicaciones</b> · Madrid, España<br>
  Doble CFGS en desarrollo (DAM + DAW) · Fundador de <a href="https://3daxstudio.com">3DAX Studio</a>
</p>

<p align="center">
  <a href="https://3daxstudio.com"><img src="https://img.shields.io/badge/Web-3daxstudio.com-0891b2?style=flat-square&logo=googlechrome&logoColor=white" alt="Web"></a>
  <a href="mailto:AdriCM427@gmail.com"><img src="https://img.shields.io/badge/Email-AdriCM427@gmail.com-7c3aed?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  <img src="https://img.shields.io/badge/Madrid-España-334155?style=flat-square&logo=googlemaps&logoColor=white" alt="Madrid">
</p>

---

Construyo aplicaciones de principio a fin: backend, interfaz y base de datos. Vengo de dos
ciclos superiores de desarrollo consecutivos y de un paso por QA donde aprendí a romper el
software antes de que lo rompa el usuario.

Desde 2024 llevo **3DAX Studio**, un estudio de diseño y fabricación 3D que monté yo y cuya
web mantengo en producción. En paralelo desarrollo sistemas de automatización de extremo a
extremo.

Me interesan la **automatización**, la **simulación** y la **ciberseguridad**.

## 🛠️ Con qué trabajo

| | |
|---|---|
| **Lenguajes** | Python · C# · JavaScript · Java · C++ |
| **Backend y APIs** | Spring Boot · APIs REST · Flask |
| **Frontend** | React · HTML5 · CSS3 · Bootstrap |
| **Bases de datos** | SQL · MySQL · PostgreSQL |
| **Automatización y QA** | Selenium · web scraping · Acunetix |
| **Infraestructura** | Cloudflare Pages · Raspberry Pi · Caddy |
| **3D y CAD** | Rhinoceros · Fusion 360 |

## 📌 Proyectos

### ⚙️ Generador de webs · *pipeline de automatización de extremo a extremo*

Sistema completo que **identifica negocios locales sin presencia web, les genera un sitio a
medida y gestiona todo el ciclo comercial** hasta la entrega. Diseñado para funcionar solo:
la única intervención humana es el contacto con el negocio, y es manual **a propósito**.

**Cómo funciona, de principio a fin:**

1. **Prospección** — barrido automatizado sobre datos públicos de fichas de negocios locales,
   con packs de ~100 gremios para recorrer una ciudad entera. El historial de búsquedas evita
   repetir trabajo: lo consultado hace menos de 14 días se salta solo.
2. **Puntuación** — cada negocio recibe un **score de 0 a 100** de potencial calculado a partir
   de reseñas, valoración, teléfono, fotografías y si la ficha está reclamada. El pipeline
   prioriza solo lo que merece la pena.
3. **Generación** — construye un prompt personalizado con los datos reales del negocio y genera
   una web *one-page* mediante LLM, con dirección de arte adaptada a cada gremio: una
   peluquería y un taller no salen con el mismo diseño.
4. **Despliegue** — publica una vista previa en Cloudflare Pages, con infraestructura alternativa
   sobre Raspberry Pi (Caddy + DNS dinámico). La versión definitiva se despliega en el dominio
   del cliente.
5. **Comercial** — genera presupuestos imprimibles en A4, **multi-idioma y multi-divisa**
   (adapta idioma, moneda y fórmula de precio al mercado del negocio), y prepara los mensajes
   de contacto personalizados.
6. **Seguimiento** — CRM propio con embudo de estados: `nuevo → web generada → contactado →
   interesado → vendido`.

**Decisiones técnicas de las que estoy orgulloso:**

- **Cero dependencias externas.** Los 12 módulos del pipeline funcionan solo con la librería
  estándar de Python. Nada que instalar, nada que se rompa al actualizarse.
- **Panel de control propio** servido en local: tabla de leads en vivo, lanzamiento del rastreo
  con progreso y log en tiempo real, inspección de prompts y generación de webs con límite de
  concurrencia.
- **Trabajo en equipo sin base de datos.** La sincronización va sobre Git: versiona únicamente
  los datos, integra con *rebase* automático y **fusiona el CRM campo a campo**; ante un
  conflicto gana el estado más avanzado del embudo, de modo que dos personas pueden trabajar
  sobre el mismo lead sin perder información.
- **Idempotencia por diseño.** Todo se fusiona por identificador: relanzar cualquier fase es
  seguro, nunca duplica ni pierde registros.
- **Cadena de suministro verificada.** La herramienta externa de rastreo se valida por hash
  SHA-256 contra el publicado por su autor antes de ejecutarse.

`Python` · `arquitectura de pipeline` · `web scraping` · `LLM` · `Cloudflare Pages` · `Raspberry Pi` · `Git como capa de sincronización`

> Repositorio privado por contener datos comerciales de terceros.

### 🌐 3DAX Studio · [3daxstudio.com](https://3daxstudio.com)

Tienda online de piezas diseñadas y fabricadas en 3D. **Programada a mano de principio a
fin**: backend, frontend y diseño de la base de datos relacional. En producción con clientes
reales desde 2024, con mantenimiento evolutivo continuo. Compagino en ella los tres papeles:
desarrollo, diseño de producto y atención al cliente.

`HTML5` · `CSS3` · `JavaScript` · `SQL`

> El código es privado por tratarse de un negocio en explotación. La web está viva y se puede visitar.

### 📊 Comparador de precios multi-tienda · *TFG del ciclo DAM*

Aplicación web que rastrea precios de productos en varias tiendas online, ejecuta búsquedas
sobre el catálogo completo y genera gráficos y estadísticas comparativas a partir de los datos
recogidos.

`Python` · `Flask` · `React` · `scraping web`

### 🔍 Automatización de QA · *Grupo Fractalia*

Validación de software entre entornos de desarrollo y producción, automatización de la
extracción de elementos web con Python y Selenium, y análisis de seguridad de aplicaciones
con Acunetix para detectar fallos antes de publicar.

`Python` · `Selenium` · `Acunetix`

## 🎓 Formación

**CFGS Desarrollo de Aplicaciones Web (DAW)** — IES Virgen de la Paloma · 2023–2024

**CFGS Desarrollo de Aplicaciones Multiplataforma (DAM)** — IES Tetuán de las Victorias · 2021–2023
<br><sub>Java con Spring Boot · APIs REST · Bootstrap</sub>

**CFGM Sistemas Microinformáticos y Redes** — La Salle Sagrado Corazón · 2019–2021

## 📫 Contacto

📧 **AdriCM427@gmail.com** · 🌐 **[3daxstudio.com](https://3daxstudio.com)** · 📍 **Madrid**

<sub>Abierto a oportunidades como desarrollador junior, QA automation y simulación.</sub>
