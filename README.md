# vertex-ai-ocr

A utility tool that uses Google Vertex AI's Gemini models to convert book images into structured Markdown format, with support for mathematical equations.

## Usage
- Enable Vertex AI API in Google Cloud
- Create service account and download key
- Create a `.env` file
```env
GOOGLE_APPLICATION_CREDENTIALS=path/to/your/service-account-key.json
PROJECT_ID=your-google-cloud-project-id
LOCATION=us-central1
```
- Run [notebook](book_to_markdown.ipynb)