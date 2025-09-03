# Análisis de Políticas de Sostenibilidad mediante técnicas de Argumentacion Computacional

Este repositorio contiene el código, los prompts, los resultados y el documento en LaTeX del TFM titulado **"Análisis de Políticas de Sostenibilidad mediante técnicas de Argumentacion Computacional"**, presentado como Trabajo Final del **Master en Inteligencia Artificial Reconocimiento de Formas e Imagen Digital (MIARFID)** de la Universitat Politècnica de València.

Se emplean distintos modelos como:

- **Generación de palabras clave por ODS**: GPT-4.5, Claude 3.7, Deepseek-v3, Gemini 2.5
- **Extracción y clasificación de argumentos**: Gemma3-27b, Llama3.3-70b, Deepseek-r1-70b (via poliGPT API compatible con Ollama) y modelos más pequeños en Ollama local Gemma3-4b, Qwen2.5-3b
- **Detección de relaciones**: modelo RoBERTa especializado en minería de argumentos (raruidol/ArgumentMining-EN-ARI-AIF-RoBERTa_L), modelo generativo pre-
entrenado de DeBERTa-v3-base (MoritzLaurer/DeBERTa-v3-base-mnli-fever-anli), google/flan-t5-base, facebook/bart-large-mnli

## Estructura del Repositorio
0. PDF RawTextExtraction notebook: realiza el pasaje de los documentos PDF de interés a texto plano por página y por capítulo. Se guardan en Data/Processed Files...
1. Extract: contiene los Notebooks correspondientes a la exracción de argumentos, que se guardan en Data/Extracted Arguments...
2. Clean & Process: contiene los Notebooks correspondientes a la depuración manual de los  argumentos extraidos, que se guardan en Data/Processed Arguments...
3. Clean & Process: contiene los Notebooks correspondientes a la clasificación de los argumentos procesados, que se guardan en Data/Relationships...
4. Analyse: contiene los Notebooks utilizados para generar todos los cuadros y figuras presentados en el informe (métricas de evaluación de extracción entre modelos, análisis de polaridad, métricas de clasificación y análisis relacional entre e intra ODS).
- Data: Es el directorio que contiene todos los datos generados, pero también contiene el corpus de argumentos anotados por documento (ground truth para extracción) en /Annotations y las relaciones anotadas dentro de /Relationship Keywords/Annotated


## Requisitos

- Python 3.8 o superior
- [Ollama](https://ollama.com/) (para servir modelos como LLAMA localmente)
- Dependencias principales:
  - `PyMuPDF (fitz)`
  - `pydantic`
  - `langchain`
  - `transformers`
  - `scikit-learn`
  - `matplotlib`

## Autora

- Camila Palomeque Tato.
