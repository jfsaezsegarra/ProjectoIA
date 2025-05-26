# ProjectoIA
# Asistente conversacional con Flask, Supabase y Gemini 🚀🤖

## ✅ Descripción general
Este proyecto es un asistente conversacional que conecta Telegram, Flask, Supabase y el modelo Gemini. El flujo consiste en:
1. El usuario envía una pregunta desde Telegram.
2. Flask recibe el mensaje y genera un vector de la pregunta.
3. Supabase devuelve los textos más relevantes.
4. Se compone un *prompt* con el contexto y se envía a Gemini.
5. Gemini genera una respuesta que se envía de vuelta al usuario por Telegram.

Repositorio en GitHub: [https://github.com/jfsaezsegarra/ProjectoIA.git](https://github.com/jfsaezsegarra/ProjectoIA.git)

## ✅ Instrucciones de instalación y uso
### Requisitos previos
- Python 3.10 o superior
- Cuenta de Supabase y Gemini
- Token de Telegram Bot

### Instalación
Clona el repositorio y accede al directorio:
```bash
git clone https://github.com/jfsaezsegarra/ProjectoIA.git
cd ProjectoIA
