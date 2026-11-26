# Ingenieria Inversa - Booksy

## 1. Estructura
- **Hallazgo 1 (Catalogo y organizacion de vistas):**
 - Evidencia: ![Catalogo y estructura](<capturas/captura 6.jpg>)

  - Observaciones: Se muestran servicios agrupados con duración en minutos, precios y opciones para agendar o filtrar.

  - Impacto en Booksy: Estructurar el catálogo mostrando con claridad servicio, duración y precio para calcular franjas horarias y evitar choques de agenda.

- **Hallazgo 2 (Ficha de barberos, blog y pie de pagina):**
  - Evidencia:![Barberos, blog y footer](<capturas/captura 3.jpg>)

  - Observaciones: Se muestran servicios agrupados con duración en minutos, precios y opciones para agendar o filtrar.  

  - Impacto en Booksy: Organizar de forma clara la selección de profesional/disponibilidad y mantener un cierre limpio con información útil del negocio.

## 2. Sistema de Diseno
- **Hallazgo 3 (Tipografia y jerarquia visual):**
  - Evidencia: ![Tipografia y estilos](<capturas/captura 4.jpg>)
  - Observaciones: Hay una clara diferencia entre encabezados principales, subtítulos/fechas y textos de lectura o enlaces laterales.

  - Impacto en Booksy: Definir una escala tipográfica legible en vistas móviles y de escritorio para distinguir rápido nombres de servicios, duraciones y precios.

- **Hallazgo 4 (Colores, espaciado y componentes):**
  - Evidencia: ![Componentes y CSS](<capturas/captura 1.jpg>)
    
  - Observaciones: Se combinan fondos claros con acentos de color en botones y etiquetas, separando bloques con tarjetas y márgenes definidos.

  - Impacto en Booksy: Mantener componentes consistentes (tarjetas, botones de acción, estados activos y espaciados) para que la reserva se sienta coherente.

## 3. Red
- **Hallazgo 5 (Carga de recursos y peticiones):**
  - Evidencia: ![Pestana Red](<capturas/captura 2.jpg>)
    
  - Observaciones: La cabecera ofrece acceso directo a secciones clave y un botón principal visible desde el primer pantallazo.

  - Impacto en Booksy: Dar acceso rápido al catálogo y al flujo de reserva sin obligar al usuario a buscar entre menús confusos.

- **Hallazgo 6 (Dependencias y comportamiento en carga):**
  - Evidencia: ![Detalle de red](<capturas/captura 5.jpg>)
    
  - Observaciones: Reúne información contextual del local (ubicación, horario, valoración) junto con los profesionales disponibles.

  - Impacto en Booksy: Vincular claramente el servicio elegido con la disponibilidad del profesional o franja horaria correspondiente.

## 4. Estado
- **Hallazgo 7 (Interaccion y disponibilidad de turnos):**
  - Evidencia: ![Estado e interaccion](<capturas/captura 4.jpg>)
    
  - Observaciones: Separa el contenido editorial o guías de cuidado en un bloque independiente con listado lateral de entradas recientes.

  - Impacto en Booksy: Mantener enfocado el flujo principal de reserva sin saturarlo con contenido informativo secundario.

- **Hallazgo 8 (Colisiones, vacios y cola FIFO):**
  - Evidencia: ![Colisiones y cola](<capturas/captura 7.jpg>)
    
  - Observaciones: Se cargan imágenes, hojas de estilo y scripts en vista móvil, usando caché en ciertos recursos (slide.webp) y mostrando mensajes en consola.

  - Impacto en Booksy: Cargar solo lo necesario en clon/, evitar errores en consola y lograr que la interfaz responda rápido en pantallas pequeñas.

## 5. Lighthouse
- **Hallazgo 9 (Puntajes y metricas clave):**
  - Evidencia: 
  
  ![Estado e interaccion](<capturas/captura 9.jpg>)
    
  - Observaciones: Se evidencian cuellos de botella en carga inicial, fuentes, entrega de imágenes, caché y redistribuciones de diseño.

  - Impacto en Booksy: Evitar scripts/estilos bloqueantes innecesarios y mantener un diseño estable desde la primera carga.

- **Hallazgo 10 (Oportunidades y diagnosticos):**
  - Evidencia: 
  
  ![Lighthouse diagnosticos](<capturas/captura 10.jpg>)
  - Observaciones: El peso de JavaScript, las tareas largas en el hilo principal y la falta de dimensiones explícitas en imágenes afectan la fluidez.

  - Impacto en Booksy: Escribir JavaScript limpio y modular para clon/, evitando tareas pesadas al calcular horarios o actualizar el estado de la reserva.


