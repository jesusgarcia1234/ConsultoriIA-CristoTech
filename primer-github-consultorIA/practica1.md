
# ConsultorIA-CristoTech

**ConsultorIA-CristoTech** es una consultora tecnológica especializada en inteligencia artificial y automatización de procesos para pequeñas y medianas empresas (pymes).

Nuestro objetivo es ayudar a las empresas a ahorrar tiempo, reducir tareas repetitivas y mejorar su productividad mediante soluciones de IA adaptadas a sus necesidades. Queremos que negocios que no cuentan con grandes equipos informáticos también puedan aprovechar estas tecnologías.

Además, en el futuro queremos ampliar nuestros servicios con la instalación y administración de servidores para alojar aplicaciones, automatizaciones y agentes de inteligencia artificial.

**Integrantes:** Adrián y Jesús.

*Siempre conectados, siempre inteligentes. 24/7.*

---

## Índice

1. [Presentación de la consultora](#consultoria-cristotech)
2. [¿Qué hacemos?](#qué-hacemos)
3. [Clientes con los que trabajamos](#clientes-con-los-que-trabajamos)
4. [Elementos técnicos](#elementos-técnicos)
5. [Enlaces de interés](#enlaces-de-interés)
6. [Imagen o logotipo](#imagen-o-logotipo)

---

## ¿Qué hacemos?

En **ConsultorIA-CristoTech** ofrecemos soluciones de inteligencia artificial, automatización y servicios informáticos para mejorar el funcionamiento de las empresas.

Nuestros principales servicios son:

- **Agentes de inteligencia artificial:** instalación y configuración de asistentes inteligentes capaces de responder preguntas, consultar información de la empresa y ayudar a clientes o empleados.
- **Automatización de procesos:** creación de flujos de trabajo con herramientas como n8n para automatizar tareas repetitivas, como clasificar correos, generar informes o registrar pedidos.
- **Integración de APIs:** conexión entre diferentes aplicaciones, bases de datos y servicios para intercambiar información automáticamente.
- **Atención al cliente 24/7:** incorporación de chatbots en páginas web y canales como WhatsApp para responder consultas frecuentes y gestionar solicitudes.
- **Bases de conocimiento empresariales:** organización de documentos, manuales y datos internos para que los asistentes de IA puedan consultar información de la empresa.
- **Gestión de bases de datos:** configuración y mantenimiento de sistemas para almacenar clientes, productos, pedidos y otros datos necesarios.
- **Administración de servidores:** instalación, configuración y mantenimiento de servidores Linux y contenedores Docker para alojar nuestras aplicaciones.
- **Seguridad informática:** protección de los sistemas mediante control de accesos, actualizaciones, copias de seguridad y medidas de protección de datos.
- **Mantenimiento y soporte técnico:** supervisión de las automatizaciones, resolución de errores, actualizaciones y mejoras de los sistemas instalados.

Cada proyecto se adaptará a las necesidades de la empresa, teniendo en cuenta su presupuesto, las herramientas que ya utiliza y los procesos que quiere mejorar.

---

## Clientes con los que trabajamos

Nuestra consultora está orientada principalmente a pequeñas y medianas empresas de distintos sectores.

Estos son cinco ejemplos de posibles clientes y las soluciones tecnológicas que podríamos ofrecerles:

| Cliente | Sector | Necesidad tecnológica |
|---|---|---|
| TRIADA SPORT | Distribución deportiva | Automatizar la gestión de pedidos, actualizar el inventario y responder consultas sobre productos mediante IA. |
| HOTEL LEVANTE | Hostelería | Implantar un asistente de IA que responda dudas sobre habitaciones, horarios y disponibilidad, y ayude con las reservas. |
| EDUCA 21 | Educación | Crear un asistente que consulte documentos del centro y resuelva preguntas frecuentes de alumnos y profesores. |
| TECNOFÁBRICA | Industria | Automatizar informes de producción, conectar bases de datos y administrar servidores para sus aplicaciones. |
| COMERZIA | Comercio online | Integrar un chatbot en la tienda online, automatizar consultas sobre pedidos y conectar la web con el sistema de ventas. |

Estos clientes son ejemplos ficticios para el proyecto y representan posibles sectores en los que podría trabajar nuestra consultora.

---

## Elementos técnicos

Para desarrollar nuestras soluciones utilizaremos herramientas de automatización, archivos de configuración, programación y servidores.

A continuación, mostramos tres ejemplos técnicos relacionados con nuestra actividad.

### 1. Configuración de un agente de IA

Un agente de atención al cliente necesita conocer su función, el idioma en el que debe responder y la información que puede consultar.

El archivo `config-agente.json` podría almacenar una configuración básica como esta:

```json
{
  "nombre": "CristoTech-Asistente",
  "idioma": "es",
  "funcion": "atencion_al_cliente",
  "modelo": "modelo-ia",
  "base_conocimiento": "documentos_empresa",
  "activo": true
}
```

Este JSON es un ejemplo de cómo organizar los parámetros de un agente. No corresponde a una configuración oficial de una plataforma concreta.

### 2. Automatización de tareas con Python

Podemos utilizar Python para realizar tareas repetitivas de manera automática.

Por ejemplo, el siguiente código clasifica consultas de clientes según su contenido:

```python
consulta = "Quiero saber el precio de un producto"

if "precio" in consulta.lower():
    print("Enviar al departamento de ventas")
elif "problema" in consulta.lower():
    print("Enviar a soporte técnico")
else:
    print("Enviar a atención al cliente")
```

Este ejemplo utiliza condiciones para clasificar una consulta. En una solución más avanzada podríamos utilizar un modelo de IA para interpretar mensajes y conectarlo con otras aplicaciones mediante n8n.

### 3. Despliegue de aplicaciones con Docker

Docker permite ejecutar aplicaciones en contenedores, facilitando su instalación y administración en un servidor.

Por ejemplo, podemos preparar un volumen para guardar los datos de n8n:

```bash
docker volume create n8n_data
```

Después, podemos iniciar n8n en un contenedor para realizar pruebas locales:

```bash
docker run -it --rm --name n8n -p 5678:5678 -e TZ=Europe/Madrid -e GENERIC_TIMEZONE=Europe/Madrid -v n8n_data:/home/node/.n8n n8nio/n8n
```

Una vez iniciado, podemos acceder desde el navegador:

`http://localhost:5678`

Con n8n podríamos crear flujos de trabajo que conecten formularios, correos electrónicos, bases de datos y modelos de inteligencia artificial.

Este comando es un ejemplo para pruebas locales, no una configuración definitiva de producción.

---

## Enlaces de interés

Estas son algunas de las herramientas y plataformas que podemos utilizar para desarrollar automatizaciones y soluciones de inteligencia artificial para nuestros clientes:

- **n8n:** [Plataforma de automatización](https://n8n.io/) que permite conectar aplicaciones, crear flujos de trabajo e integrar agentes de IA.
- **OpenAI Platform:** [Plataforma de inteligencia artificial](https://platform.openai.com/) para integrar modelos de IA en aplicaciones y automatizaciones.
- **Claude:** [Plataforma de Anthropic](https://platform.claude.com/) para desarrollar soluciones de IA mediante sus modelos y API.
- **OpenRouter:** [Plataforma de acceso a modelos de IA](https://openrouter.ai/) que permite utilizar diferentes modelos mediante una API unificada.
- **Hermes Agent:** [Agente de IA de Nous Research](https://github.com/NousResearch/hermes-agent) capaz de utilizar herramientas, ejecutar tareas y desarrollar habilidades reutilizables.
- **Supabase:** [Plataforma de bases de datos](https://supabase.com/) para almacenar información y conectar aplicaciones con sistemas de IA.
- **Docker:** [Plataforma de contenedores](https://www.docker.com/) que permite desplegar y gestionar aplicaciones y servicios en servidores.

---

## Imagen o logotipo

Este es el logotipo de nuestra consultora, **ConsultorIA-CristoTech**:

![Logotipo de ConsultorIA-CristoTech](fotos/Logoh.png)
