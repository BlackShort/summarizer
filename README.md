# Intelligent Document Summarizer

[Live Demo](https://app-yt-manager.vercel.app/) | [GitHub Repository](https://github.com/BlackShort/yt-manager)

## Overview

The Intelligent Document Summarizer is a powerful tool designed to automatically generate concise summaries from lengthy documents. Built with advanced transformer-based models from Hugging Face, it significantly reduces the manual effort and time required to review documents, improving efficiency by up to 60%.

## Key Features

- **High-accuracy Summarization**: Achieves high accuracy in understanding and summarizing key content, powered by state-of-the-art LLMs (Large Language Models).
- **Real-time Processing**: Deployed with AWS services (Lambda, S3) and FastAPI, enabling scalable, real-time document processing for seamless performance.

## Tech Stack

- **Backend**: Python, FastAPI
- **Machine Learning**: Hugging Face Transformers
- **Cloud Deployment**: AWS (Lambda, S3)

## Project Structure

```plaintext
├── app                # FastAPI application
│   ├── main.py        # Main entry point for API
│   └── routers        # API route definitions
├── models             # Machine learning models and utilities
│   ├── summarizer.py  # Transformer model for summarization
├── aws                # AWS Lambda configuration and deployment files
└── README.md          # Project documentation
```

## Setup and Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/BlackShort/document-summarizer.git
   cd document-summarizer
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up AWS credentials**:
   Ensure that your AWS credentials are properly configured for Lambda and S3 access.

4. **Run the application locally**:
   ```bash
   uvicorn app.main:app --reload
   ```

## Deployment

The application is deployed on AWS using Lambda for serverless execution and S3 for file storage. The FastAPI backend interacts with Lambda functions to perform document summarization in real time.

## Usage

1. Upload a document through the web interface or API endpoint.
2. The tool will generate a summarized version of the document, available for download or viewing in real time.

## Future Enhancements

- Adding support for multi-lingual document summarization.
- Incorporating fine-tuning capabilities for specific industries.
- Extending the web interface with batch document summarization.

## License

This project is licensed under the MIT License.

---

For any issues or contributions, please refer to the [GitHub Issues](https://github.com/BlackShort/yt-manager/issues) section.
