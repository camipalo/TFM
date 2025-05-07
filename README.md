# Detección Automática de Relaciones entre Argumentos de los ODS

Este repositorio contiene el código, los prompts, los resultados y el documento en LaTeX del informe titulado **"Detección Automática de Relaciones entre Argumentos de los Objetivos de Desarrollo Sostenible (ODS)"**, presentado en el marco del curso **Herramientas y Aplicaciones de la Inteligencia Artificial (MIARFID)** de la Universitat Politècnica de València.

Se emplean distintos modelos como:

- **Generación de palabras clave por ODS**: GPT-4.5, Claude 3.7, Deepseek-v3, Gemini 2.5
- **Extracción y clasificación de argumentos**: LLAMA 3.2 (vía Ollama) y PoliGPT (API compatible con OpenAI)
- **Detección de relaciones**: modelo RoBERTa especializado en minería de argumentos

## Estructura del Repositorio

- Extract/ : contiene los Notebooks y archivos `JSON` correspondientes a la exracción de argumentos.
- ExtractClassify/ : contiene los Notebooks y archivos `JSON` correspondientes a la exracción de argumentos y detección de relaciones.
- Classify/ : contiene los Notebooks y archivos `.csv` correspondientes a la detección de relaciones.


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

## Autoras

- Ana Valentina López Chacón.
- Camila Palomeque Tato.
