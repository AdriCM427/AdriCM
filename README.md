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
ciclos superiores de desarrollo y de un paso por QA donde aprendí a romper el software antes
de que lo rompa el usuario. Ahora desarrollo sistemas de automatización y mantengo en
producción la web de mi propio estudio 3D.

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

### ⚙️ Generador de webs

**Pipeline que localiza negocios sin presencia web, les genera un sitio a medida y gestiona el
ciclo comercial completo.** Funciona solo de punta a punta: la única intervención humana es el
contacto con el negocio, y es manual a propósito.

12 módulos Python con **cero dependencias externas**, panel de control propio y sincronización
multiusuario resuelta sobre Git.

`Python` · `web scraping` · `LLM` · `Cloudflare Pages` · `Raspberry Pi`

<details>
<summary><b>Cómo funciona, paso a paso</b></summary>

<br>

| Fase | Qué hace |
|---|---|
| **Prospección** | Barrido automatizado sobre datos públicos de fichas de negocios, con packs de ~100 gremios para recorrer una ciudad entera. Lo consultado hace menos de 14 días se salta solo. |
| **Puntuación** | Score de 0 a 100 por potencial, calculado con reseñas, valoración, teléfono, fotografías y si la ficha está reclamada. |
| **Generación** | Prompt construido con los datos reales del negocio y web *one-page* generada mediante LLM, con dirección de arte adaptada a cada gremio. |
| **Despliegue** | Vista previa en Cloudflare Pages, con infraestructura alternativa sobre Raspberry Pi (Caddy + DNS dinámico). La definitiva va al dominio del cliente. |
| **Comercial** | Presupuestos A4 imprimibles multi-idioma y multi-divisa, adaptando precio y moneda al mercado del negocio. |
| **Seguimiento** | CRM propio con embudo: nuevo → web generada → contactado → interesado → vendido. |

</details>

<details>
<summary><b>Decisiones técnicas</b></summary>

<br>

- **Cero dependencias externas.** Todo el pipeline funciona con la librería estándar de Python.
  Nada que instalar, nada que se rompa al actualizarse.
- **Sincronización multiusuario sobre Git, sin base de datos.** Versiona solo los datos, integra
  con *rebase* automático y fusiona el CRM campo a campo; ante un conflicto gana el estado más
  avanzado del embudo, así que dos personas pueden trabajar sobre el mismo registro sin perder
  información.
- **Idempotencia por diseño.** Todo se fusiona por identificador: relanzar cualquier fase es
  seguro, nunca duplica ni pierde registros.
- **Cadena de suministro verificada.** Las herramientas externas se validan por hash SHA-256
  contra el publicado por su autor antes de ejecutarse.
- **Panel de control propio** servido en local: leads en vivo, lanzamiento del rastreo con
  progreso y log en tiempo real, y generación con límite de concurrencia.

</details>

> Repositorio privado por contener datos comerciales de terceros.

### 🌐 3DAX Studio · [3daxstudio.com](https://3daxstudio.com)

Tienda online de piezas diseñadas y fabricadas en 3D. **Programada a mano de principio a fin**:
backend, frontend y base de datos relacional. En producción con clientes reales desde 2024.

`HTML5` · `CSS3` · `JavaScript` · `SQL`

> Código privado por tratarse de un negocio en explotación. La web está viva y se puede visitar.

### 📊 Comparador de precios multi-tienda · *TFG del ciclo DAM*

Aplicación web que rastrea precios en varias tiendas online, busca sobre el catálogo completo y
genera gráficos y estadísticas comparativas.

`Python` · `Flask` · `React` · `scraping web`

### 🔍 Automatización de QA · *Grupo Fractalia*

Validación de software entre entornos, automatización de la extracción de elementos web con
Python y Selenium, y análisis de seguridad con Acunetix para detectar fallos antes de publicar.

`Python` · `Selenium` · `Acunetix`

## 🎓 Formación

**CFGS Desarrollo de Aplicaciones Web (DAW)** — IES Virgen de la Paloma · 2023–2024

**CFGS Desarrollo de Aplicaciones Multiplataforma (DAM)** — IES Tetuán de las Victorias · 2021–2023
<br><sub>Java con Spring Boot · APIs REST · Bootstrap</sub>

**CFGM Sistemas Microinformáticos y Redes** — La Salle Sagrado Corazón · 2019–2021

## 📫 Contacto

📧 **AdriCM427@gmail.com** · 🌐 **[3daxstudio.com](https://3daxstudio.com)** · 📍 **Madrid**

<sub>Abierto a oportunidades como desarrollador junior, QA automation y simulación.</sub>
