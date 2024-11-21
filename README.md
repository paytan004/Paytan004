# Tienda de Maquillaje Asiático K-GLOW

**FACULTAD DE INGENIERÍA**  
Carrera de Ingeniería de Sistemas y Software  

**DESARROLLO DE APP WEB PARA TIENDA DE MAQUILLAJE ASIÁTICO K-GLOW**  

**Curso Integrador I: Sistemas Software**  
Ing. Villalta Flores, Claudia Yolanda  

## Integrantes
- Castro Sánchez, Arghel Giannulli  
- Cossío Vega, Antony Piero  
- Escudero Rodríguez, Crhist Leonor  
- Paytan Díaz, Ana Claudia  
- Rodríguez Chacaliaza, Airton Clides  

Lima, Perú  
30 de septiembre 2024  

---

## Resumen
El presente proyecto describe el desarrollo de una aplicación web destinada a K-Glow, una empresa especializada en la comercialización de productos cosméticos asiáticos. Su objetivo principal es mejorar la formalidad y eficiencia de las operaciones comerciales. Este proyecto considera aspectos como la gestión de procesos de negocio, los requerimientos funcionales y no funcionales del sistema, y un análisis del estado del arte en el ámbito del desarrollo de software.  

La implementación utiliza enfoques arquitectónicos como Modelo-Vista-Controlador (MVC), Desarrollo Guiado por Pruebas (TDD) y Acceso a Datos (DAO). Actualmente, el avance del código se encuentra en un 30%, permitiendo evaluaciones continuas y ajustes pertinentes.

---

## Capítulo 1 – Aspectos Generales

### 1.1 Definición del Problema

#### 1.1.1 Descripción del Problema
K-Glow enfrenta diversas problemáticas:  
- La informalidad en la venta de productos genera desconfianza entre los consumidores, disminuyendo las ventas.  
- La dependencia de redes sociales para ventas ha causado saturación en la atención al cliente, comprometiendo la calidad y eficiencia del servicio.  

La creación de una aplicación web ayudará a formalizar las operaciones comerciales, reducir la dependencia de redes sociales y mejorar la experiencia de compra de los clientes.  

#### 1.1.2 Diagrama Actual de Procesos de Negocio
> **Figura 1**: Diagrama de Procesos de Negocio (Elaborado por: Los Milanesos)  
![Diagrama de Procesos de Negocio Inicial]("https://web.whatsapp.com/21623aaa-7160-43de-aa12-a921b2c3c10b")

### 1.2 Planteamiento de Alternativas de Solución
Se han considerado tres soluciones para el diseño de la interfaz de la aplicación:  

1. **Estilo Tierno/Adorable**  
   - Incluye una paleta de colores pastel y elementos visuales amigables.  
   - Ejemplo: **Figura 2**: Inicio de Sesión, **Figura 3**: Catálogo de Productos, etc.  
   ![s1_1]("https://web.whatsapp.com/91e5fdc1-9be3-4e5d-a635-0160aa1acba6")
   ![s1_2]("https://web.whatsapp.com/0b288532-a9ab-4afd-8f4a-006279f0bdee")
   ![s1_3]("https://web.whatsapp.com/b39e9f8a-da72-4de1-b9e9-5aba9da987c1")
   ![s1_4]("https://web.whatsapp.com/3161c077-6dab-4a2b-81ec-c518437c0f37")
   ![s1_5]("https://web.whatsapp.com/db62c76a-17ab-4ee3-985b-3a1718c9be00")
   ![s1_6]("https://web.whatsapp.com/03926021-eb51-4bf2-b6b2-be3500ecab6d")
2. **Estilo Juvenil/Moderno**  
   - Diseño basado en tendencias minimalistas, con colores vivos y navegación intuitiva.  
   - Ejemplo: **Figura 8**: Página principal, **Figura 9**: Inicio de Sesión, etc.  
   ![s2_1]("https://web.whatsapp.com/95fe6256-3385-482a-b790-0a4ec232ecfb")
   ![s2_2]("blob:https://web.whatsapp.com/139bc226-da94-4f7c-94c4-41dd867bd112")
   ![s2_3]("blob:https://web.whatsapp.com/4cc2310c-33fe-44d5-b358-878e544032aa")
   ![s2_4]("blob:https://web.whatsapp.com/efaaeb91-807a-41f5-9c67-2e2a5e490abe")
   ![s2_5]("blob:https://web.whatsapp.com/2f7e1ee8-59f6-4ada-a59c-62d6d56c375b")
   ![s2_6]("blob:https://web.whatsapp.com/e6c30247-58fb-466a-a8e3-f806e9bd42d8")
   ![s2_7]("blob:https://web.whatsapp.com/e6c35483-dba9-4c9b-932f-64fb28e41372")
   ![s2_8]("blob:https://web.whatsapp.com/40ec2275-9a85-49da-8db5-12ede693e548")

3. **Estilo Encantador/Etéreo**  
   - Enfatiza la estética elegante con fondos suaves y detalles delicados.  
   - Ejemplo: **Figura 16**: Inicio con Ofertas y Redes, **Figura 17**: Inicio de Sesión, etc.  
   ![s3_1]("blob:https://web.whatsapp.com/098a6110-06b8-4e09-a412-b31b79a586f0")
   ![s3_2]("blob:https://web.whatsapp.com/d5aa2f09-f1f9-43a2-a182-4f91cdeb2024")
   ![s3_3]("blob:https://web.whatsapp.com/aabd8e75-4857-4283-a139-0642cfda7845")
   ![s3_4]("blob:https://web.whatsapp.com/75a8f5b1-daea-4996-8726-78662bc1f3b5")
   ![s3_5]("blob:https://web.whatsapp.com/a0e1e45a-afd0-47b1-9fd0-a81748cc578f")

### 1.3 Definición de Objetivos

#### 1.3.1 Objetivo General
Desarrollar una aplicación web que automatice y optimice el proceso de ventas de la tienda de maquillaje asiático K-Glow, mejorando la experiencia del cliente y aumentando la eficiencia operativa.  

#### 1.3.2 Objetivos Específicos
- Diseñar una interfaz visualmente atractiva que destaque los productos y refleje la identidad de la marca.  
- Implementar galerías de imágenes y descripciones breves para facilitar las compras.  
- Desarrollar una navegación intuitiva para encontrar productos fácilmente.  
- Simplificar el proceso de compra para mejorar la conversión de ventas.  

### 1.4 Alcances y Limitaciones
La aplicación web formalizará las operaciones comerciales de K-Glow, mejorará la experiencia del cliente y permitirá una gestión más eficiente de ventas e inventarios, reduciendo la dependencia de redes sociales.  

### 1.5 Justificación
La implementación de la aplicación responde a la necesidad de digitalización en un mercado competitivo. Esto permitirá:  
- Ampliar el alcance de la marca.  
- Optimizar la experiencia de compra de los clientes.  
- Consolidar la posición de K-Glow en el mercado de cosmética coreana en Perú.  

---

## Capítulo 2 – Marco Teórico

### 2.1 Análisis del Estado del Arte

#### 2.1.1 Buenas Prácticas en la Programación
El modelo tradicional de cascada ha sido clave para el desarrollo del proyecto. Permite capturar requisitos al inicio y realizar revisiones y pruebas en cada etapa, reduciendo errores y retrasos.  

#### 2.1.2 Preguntas de la Clase

**Semana 10**  
- **Medidas con Apache POI para evitar archivos maliciosos**:  
  1. Deshabilitar macros.  
  2. Validar la estructura del archivo.  
  3. Usar sandbox para procesar archivos.  
  4. Escanear contenido por código malicioso.  
  5. Control de acceso y permisos.  

- **Validación y sanitización de archivos Excel**:  
  - Escaneo antivirus, revisión de estructura, eliminación de información oculta y contenido sospechoso.  

- **Importancia de mantener Apache POI actualizado**:  
  - Las actualizaciones corrigen errores de seguridad, mejoran compatibilidad y reducen riesgos de ataque.  

**Semana 11**  
- **Diferencia entre `git init` y `git clone`**:  
  - `git init`: Crea un repositorio local desde cero.  
  - `git clone`: Descarga un repositorio remoto con todo su historial.  

- **Propósito de `git add` y `git commit`**:  
  - `git add`: Agrega archivos al área de preparación.  
  - `git commit`: Confirma los cambios con un mensaje.  

- **Uso de `git push`**:  
  - Sube los cambios locales a un repositorio remoto.  

- **Manejo de conflictos en Git**:  
  - Identificar el conflicto, editar archivos en conflicto, marcarlos como resueltos (`git add`), y completar la fusión (`git commit`).  

### 2.2 Fundamento Teórico

#### 2.2.1 Business Process Management (BPM)
Es una metodología para analizar, modelar y mejorar flujos de trabajo dentro de una organización, reduciendo costos y tiempos, mientras se mejora la eficiencia.  

#### 2.2.2 Aplicativo Web
Aplicaciones accesibles desde el navegador que permiten realizar tareas en línea sin necesidad de instalar software adicional.  

#### 2.2.3 Arquitectura de Software
Es el diseño estructural de un sistema que organiza sus componentes y asegura funcionalidad, seguridad y escalabilidad.  

#### 2.2.4 Mockups
Representaciones visuales detalladas de interfaces que incluyen elementos gráficos como colores y tipografías, esenciales para una experiencia visual coherente antes del desarrollo.  

#### 2.2.5 Lenguaje de Programación
Java es ideal para gestionar el backend, mientras que HTML, CSS y JavaScript se utilizan para el frontend.  

#### 2.2.6 Java
Lenguaje robusto, multiplataforma, ideal para aplicaciones web empresariales. Frameworks como Spring facilitan su uso en el desarrollo de software seguro y escalable.  

#### 2.2.7 Base de Datos
Gestión estructurada de datos como inventarios, usuarios y transacciones mediante sistemas DBMS como MySQL, PostgreSQL o MongoDB.  

#### 2.2.8 MySQL
Sistema de gestión de bases de datos relacional que permite consultas rápidas y manejo eficiente de grandes volúmenes de información, esencial para la experiencia de usuario en tiendas en línea.  