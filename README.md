# Chatbot Universitario

Este proyecto es un chatbot diseñado para proporcionar información académica sobre la carrera de Ingeniería en Sistemas en la Universidad ORT. Utiliza un LLM para generar respuestas naturales y relevantes basadas en datos extraídos de la pagina oficial de la ORT.

## Características

- **Procesamiento de Lenguaje Natural (NLP):** Generación de respuestas utilizando `mistralai/Mistral-7B-Instruct-v0.1`.
- **Búsqueda Vectorial:** Implementación de FAISS y Elasticsearch para la recuperación eficiente de información.
- **Extracción de Datos:** Web scraping con BeautifulSoup para obtener información actualizada.
- **Generación de Embeddings:** Uso del modelo `sentence-transformers/all-MiniLM-L6-v2` para mejorar la precisión en la búsqueda de información.
- **RAG (Retrieval-Augmented Generation):** Combinación de recuperación y generación de respuestas para mejorar la coherencia y relevancia.

## Uso

Para ejecutar el archivo CHATBOT.ipynb en Google Colab y utilizar los modelos de Hugging Face, necesitarás un Hugging Face API Token. Este token permite acceder a los modelos y servicios necesarios para el chatbot.


