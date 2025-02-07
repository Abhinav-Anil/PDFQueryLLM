## Description
PDFQuery-GPT is a full-stack AI-powered platform that enables users to upload PDF files and query the contents using a custom fine-tuned language model. The backend uses Django, PostgreSQL, and Transformer models for intelligent PDF analysis.

## Features
- **User Authentication:** Register and login functionality.
- **PDF Upload & Processing:** Extract and analyze text from PDF documents.
- **LLM Query Support:** Query uploaded PDF content using a custom-trained LLM model.
- **Training Pipeline:** Tools for fine-tuning models.

## Project Structure
```
project_root/
├── backend/
│   ├── manage.py
│   ├── backend/
│   ├── api/
│   └── models/
├── requirements.txt
├── training/
└── README.md
```

## Setup Instructions

### Prerequisites
- Python 3.8+
- PostgreSQL
- H100 GPU (optional but recommended)

### Installation
1. Clone the project:
   ```bash
   git clone https://github.com/your_username/PDFQuery-GPT.git
   cd PDFQueryLLM
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Configure PostgreSQL in `backend/settings.py`.
4. Apply migrations:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```
5. Run the development server:
   ```bash
   python manage.py runserver
   ```

## Usage
1. **Register/Login:** Create an account to upload PDF files.
2. **Upload a PDF:** Submit a PDF and query its contents.

## Training the Model
1. Place your custom data in `training/`.
2. Run the training script:
   ```bash
   python train_model.py
   ```
3. The model artifacts will be saved in `model_output/`.
