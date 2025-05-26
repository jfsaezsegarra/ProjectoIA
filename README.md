
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

### Instalación
Clona el repositorio y accede al directorio:
\`\`\`bash
git clone https://github.com/jfsaezsegarra/ProjectoIA.git
cd ProjectoIA
\`\`\`

Instala las dependencias:
\`\`\`bash
pip install -r requirements.txt
\`\`\`

### Variables de entorno y configuración
Configura estas variables antes de iniciar:
\`\`\`bash
export TELEGRAM_BOT_TOKEN="tu_token"
export SUPABASE_URL="https://tu-proyecto.supabase.co"
export SUPABASE_KEY="tu_api_key"
export GEMINI_API_KEY="tu_api_key"
\`\`\`

### Uso
Ejecuta el servidor Flask:
\`\`\`bash
python app.py
\`\`\`

Envía un mensaje al bot de Telegram para probarlo.

## ✅ Estructura del proyecto
\`\`\`
/ProjectoIA
├── app.py
├── requirements.txt
├── README.md
└── ...
\`\`\`

## ✅ Ejemplos y código
Aquí un ejemplo de cómo se define el endpoint en Flask:
\`\`\`python
from flask import Flask, request
app = Flask(__name__)

@app.route('/webhook', methods=['POST'])
def webhook():
    data = request.get_json()
    pregunta = data['message']['text']
    # Generar embedding, consultar Supabase y componer prompt...
    return {"respuesta": "¡Hola! Soy el asistente conversacional."}
\`\`\`

## ✅ Preguntas frecuentes (FAQ)
**¿Cómo cambio el bot de Telegram?**  
Edita la variable \`TELEGRAM_BOT_TOKEN\` en tu entorno.

**¿Puedo usar otro modelo en lugar de Gemini?**  
Sí, simplemente adapta el endpoint en el archivo \`app.py\`.

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
MIT License. Puedes usarlo, modificarlo y compartirlo bajo los términos de esta licencia.


