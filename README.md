# 🤖 Sistema de Automatización Documental con IA
### Caso Real · San Miguel de Tucumán, Argentina

![Status](https://img.shields.io/badge/Status-Production%20Ready-brightgreen)
![Stack](https://img.shields.io/badge/Stack-n8n%20%7C%20Groq%20%7C%20LLaMA%203.1-blue)
![Type](https://img.shields.io/badge/Type-Workflow%20Automation-orange)

---

## 📌 Contexto del Problema

En San Miguel de Tucumán, la mayoría de los estudios contables y pymes
procesan su documentación de forma **100% manual**: reciben comprobantes
por WhatsApp o email, los clasifican en carpetas, copian datos a Excel y
generan reportes a mano.

**Costo real del problema:**
- ⏱️ 3 horas diarias de trabajo manual repetitivo
- ❌ Errores frecuentes de transcripción
- 📉 Cero visibilidad en tiempo real del negocio
- 🔁 Sin escalabilidad ante crecimiento de clientes

---

## 💡 Solución Implementada

Pipeline de automatización **end-to-end** con IA generativa que transforma
el caos documental en inteligencia de negocio accionable, sin intervención
humana en el flujo operativo.

```
Cliente envía comprobante
         ↓
   Telegram Bot (24/7)
         ↓
   Groq API + LLaMA 3.1
   [Extracción inteligente de datos]
         ↓
   Google Sheets
   [Base de datos estructurada]
         ↓
   Confirmación automática al cliente
         +
   Reporte ejecutivo semanal
```

---

## 📊 Resultados Medibles

| Métrica | Antes | Después |
|---|---|---|
| Tiempo por documento | ~8 minutos | ~5 segundos |
| Errores de transcripción | Frecuentes | 0 |
| Disponibilidad del sistema | Horario laboral | 24/7 |
| Reporte semanal | 1 hora manual | Automático |
| Escalabilidad | Limitada | Ilimitada |

---

## 🛠️ Stack Tecnológico

| Herramienta | Rol en el sistema |
|---|---|
| **n8n** | Orquestador de flujos de trabajo |
| **Groq API** | Inferencia de LLM de alta velocidad |
| **LLaMA 3.1 8B** | Modelo de lenguaje para extracción de datos |
| **Telegram Bot API** | Canal de entrada y notificaciones |
| **Google Sheets API** | Base de datos y dashboard operativo |

---

## ⚙️ Arquitectura del Sistema

### Workflow 1 — Procesamiento en Tiempo Real
```
[Telegram Trigger]
       ↓
[HTTP Request → Groq API]
  prompt engineering para extracción estructurada
       ↓
[Google Sheets → Append Row]
  registro automático con metadata
       ↓
[Telegram → Confirmación al cliente]
  respuesta personalizada con datos procesados
```

### Workflow 2 — Inteligencia de Negocio Semanal
```
[Schedule Trigger → Lunes 8:00 AM]
       ↓
[Google Sheets → Get All Rows]
       ↓
[Code Node → Sanitización y preparación del contexto]
       ↓
[Groq API → Análisis ejecutivo con LLM]
  total documentos · monto acumulado · proveedores únicos
  observaciones clave y alertas
       ↓
[Telegram → Reporte ejecutivo al equipo]
```

---

## 🔐 Consideraciones de Seguridad

- Credenciales gestionadas via **environment variables** en n8n
- Ninguna API key expuesta en el repositorio
- Datos de clientes sanitizados (ficticios en este demo)
- Canal cifrado via HTTPS en todas las integraciones

---

## 🚀 Cómo usar este template

### Requisitos
- Cuenta n8n (cloud o self-hosted)
- API Key de [Groq](https://console.groq.com) *(gratuita)*
- Bot de Telegram via [@BotFather](https://t.me/BotFather)
- Google Account con Sheets habilitado

### Setup
```bash
# 1. Importar workflow_template.json en n8n
# 2. Configurar credenciales en n8n Settings
# 3. Activar los workflows
# 4. Enviar primer mensaje al bot de Telegram
```

> ⚠️ El archivo `workflow_template.json` incluye la estructura completa
> con placeholders para credenciales. Reemplazar `YOUR_API_KEY` por
> los valores reales antes de ejecutar.

---

## 💼 Sobre este proyecto

Este sistema fue diseñado como demostración práctica de competencias en:

- **Diseño de soluciones digitales** con enfoque en problemas reales locales
- **Integración de plataformas** via APIs REST y webhooks
- **AI-assisted workflows** con modelos de lenguaje de última generación
- **Prompt engineering** para extracción estructurada de datos no estructurados
- **Business Intelligence** automatizada a partir de datos operativos

> *Desarrollado como parte de un portfolio de Automatización & IA,
> enfocado en la transformación digital de pymes en el NOA argentino.*

---

## 📬 Contacto

¿Tienes un proceso manual que podría automatizarse?

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Conectar-blue)](https://linkedin.com/in/tu-perfil)
[![Email](https://img.shields.io/badge/Email-Contacto-red)](mailto:tu@email.com)

---

*Sistema 100% operativo · Stack gratuito · Listo para escalar*
