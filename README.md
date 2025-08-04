# Chatbot Universitario

Este proyecto es un chatbot diseñado para proporcionar información académica sobre la carrera de Ingeniería en Sistemas en la Universidad ORT. Utiliza un LLM para generar respuestas naturales y relevantes basadas en datos extraídos de la pagina oficial de la ORT.

## Características

- **Procesamiento de Lenguaje Natural (NLP):** Generación de respuestas utilizando `mistralai/Mistral-7B-Instruct-v0.1`.
- **Búsqueda Vectorial:** Implementación de FAISS y Elasticsearch para la recuperación eficiente de información.
- **Extracción de Datos:** Web scraping con BeautifulSoup para obtener información actualizada.
- **Generación de Embeddings:** Uso del modelo `sentence-transformers/all-MiniLM-L6-v2` para mejorar la precisión en la búsqueda de información.
- **RAG (Retrieval-Augmented Generation):** Combinación de recuperación y generación de respuestas para mejorar la coherencia y relevancia.

## Uso

Para ejecutar el archivo `CHATBOT.ipynb` en Google Colab y utilizar correctamente el chatbot, se requieren **dos tokens de acceso**:

### 1. Hugging Face API Token

Necesario para acceder a los modelos de lenguaje utilizados por el chatbot.

#### ¿Cómo obtenerlo?

- Crear una cuenta en [https://huggingface.co](https://huggingface.co).
- Ir a **Settings > Access Tokens**.
- Generar un nuevo token con permisos de **lectura** (`read`).

#### ¿Cómo configurarlo en Colab?

- En el menú de Colab, ir a **Entorno de ejecución > Editar secretos**.
- Crear un nuevo secreto con:
  - **Nombre:** `HF_TOKEN`
  - **Valor:** tu Hugging Face API Token

### 2. Pinecone API Key

Necesaria para conectarse al vector store donde se almacenan los embeddings generados.

#### ¿Cómo obtenerla?

- Crear una cuenta en [https://www.pinecone.io/](https://www.pinecone.io/).
- Ir al panel de usuario y acceder a la sección **API Keys**.
- Crear o copiar una clave existente.
- Ingresar la clave cuando el notebook la solicite.

> ⚠️ **Nunca escribas las claves directamente en el código.** Utiliza secretos de Colab o inputs seguros para proteger la información.

