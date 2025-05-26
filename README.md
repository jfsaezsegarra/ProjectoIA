
# ProjectoIA 
# 🚀 Asistente conversacional con Flask, Supabase y Gemini 🤖

## ✅ Descripción general
Este proyecto es un asistente conversacional que conecta Telegram, Flask, Supabase y el modelo Gemini.  
El flujo consiste en:
1. El usuario envía una pregunta desde Telegram.
2. Flask recibe el mensaje y genera un vector de la pregunta.
3. Supabase devuelve los textos más relevantes.
4. Se compone un *prompt* con el contexto y se envía a Gemini.
5. Gemini genera una respuesta que se envía de vuelta al usuario por Telegram.

Repositorio en GitHub: [https://github.com/jfsaezsegarra/ProjectoIA.git](https://github.com/jfsaezsegarra/ProjectoIA.git)

## ✅ Requisitos previos
- Python 3.10 o superior
- Cuenta en Supabase y Gemini
- Token de Telegram Bot

## ✅ Instrucciones de instalación y uso

### Uso
Envía un mensaje al bot de Telegram para probarlo.

## ✅ Estructura del proyecto

/ProjectoIA
├── app.py
├── requirements.txt
├── README.md
└── ...



## ✅ Ejemplos y código
Aquí un ejemplo de cómo se define el endpoint en Flask:


## ✅ Preguntas frecuentes (FAQ)
**¿Cómo cambio el bot de Telegram?**  
**¿Puedo usar otro modelo en lugar de Gemini?**  


## ✅ Recursos útiles
- [Flask](https://flask.palletsprojects.com/)
- [Supabase](https://supabase.com/docs)
- [Gemini API](https://developers.google.com/)

## ✅ URL de trabajo: Pythonanywhere.com y Supabase
Este proyecto está desplegado en Pythonanywhere y usa Supabase como base de datos en la nube.

## ✅ Contacto o autoría
Creado por [Juan Francisco Sáez Segarra](https://github.com/jfsaezsegarra).  
Email: jf.saezsegarra@edu.gva.es

## ✅ Licencia


