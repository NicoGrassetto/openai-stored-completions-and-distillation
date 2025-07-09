# Azure OpenAI Stored Completions Demo

This project demonstrates Azure OpenAI Stored Completions and Distillation features.

## 🚀 Quick Start

### 1. Clone or Download
```bash
# If using git
git clone <repository-url>
cd openai-stored-completions-and-distillation

# Or download and extract the project files
```

### 2. Set up Virtual Environment
```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
.\venv\Scripts\Activate.ps1
# On macOS/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

### 3. Install Jupyter Kernel
```bash
python -m ipykernel install --user --name=azure-openai-stored-completions --display-name="Azure OpenAI Stored Completions"
```

### 4. Configure Azure OpenAI
Update the notebook with your Azure OpenAI settings:
- `AZURE_OPENAI_ENDPOINT`: Your Azure OpenAI resource URL
- `MODEL_DEPLOYMENT_NAME`: Your model deployment name

### 5. Run the Notebook
```bash
jupyter notebook azure_openai_stored_completions_demo.ipynb
```

## 📋 Requirements

- Python 3.8+
- Azure OpenAI resource with API version `2025-02-01-preview` or later
- Appropriate Azure permissions (Cognitive Services OpenAI Contributor role)

## 🔒 Authentication

This demo uses **Azure Managed Identity** for secure authentication. Ensure you're logged in to Azure:

```bash
az login
```

## 📚 Features Demonstrated

- ✅ Creating stored completions with metadata
- ✅ Listing and filtering stored completions
- ✅ Retrieving specific completion details
- ✅ Updating completion metadata
- ✅ Analyzing data for distillation readiness
- ✅ Preparing evaluation datasets
- ✅ Managing and cleaning up completions

## 🛡️ Security Best Practices

- Uses Managed Identity (no hardcoded credentials)
- Proper error handling and resource management
- Rate limiting to avoid API throttling
- Structured metadata for organization

## 📖 Documentation

- [Azure OpenAI Stored Completions](https://learn.microsoft.com/en-us/azure/ai-foundry/openai/how-to/stored-completions)
- [Fine-tuning Guide](https://learn.microsoft.com/en-us/azure/ai-foundry/openai/how-to/fine-tuning)
- [Azure AI Foundry Portal](https://ai.azure.com)
