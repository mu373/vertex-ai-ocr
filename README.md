# vertex-ai-ocr

A utility tool that uses Google Vertex AI's Gemini models to convert book images into structured Markdown format, with support for mathematical equations.

The default model is `gemini-3.8-flash`. Use the `global`, `us`, or `eu` endpoint;
the previous `us-central1` default is not supported by this model.

## Install

Use Python 3.12 and [uv](https://docs.astral.sh/uv/) to create a separate environment:

```sh
uv venv --python 3.12
uv pip install --python .venv/bin/python -r requirements.txt
.venv/bin/python -m ipykernel install --user --name vertex-ai-ocr --display-name "Vertex AI OCR"
```

Select **Vertex AI OCR** as the notebook kernel. Package versions, including the
Google Gen AI SDK, are pinned in `requirements.txt`.

## Usage
- Enable Vertex AI API in Google Cloud
- Create service account and download key
- Create a `.env` file
```env
GOOGLE_APPLICATION_CREDENTIALS=path/to/your/service-account-key.json
PROJECT_ID=your-google-cloud-project-id
LOCATION=global
```
- Run [notebook](book_to_markdown.ipynb) with the **Vertex AI OCR** kernel.
