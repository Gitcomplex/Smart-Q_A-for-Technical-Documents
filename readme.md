# Retrieval Augmented Generation - Demo

This project demonstrates how to create a ChatGPT-like application with your custom data using Azure OpenAI and Azure AI Search, following the Retrieval Augmented Generation (RAG) pattern. It enables multi-turn chat and Q&A functionality tailored for specific data needs.

## Key Features

- **Chat Interface:** Offers both multi-turn chat and Q&A modes.
- **Data Retrieval:** Uses Azure AI Search for indexing and retrieving documents in various formats.
- **Configurable Interface:** Allows users to adjust settings to tweak model behavior.
- **Optional Integrations:** Vision-based document analysis, speech input/output, and secure Microsoft Entra login.

## Getting Started

### Prerequisites

- **Azure Account:** Sign up if you don't have one, with permissions for Azure OpenAI Service.
- **Tools Required:** Install the [Azure Developer CLI](https://aka.ms/azure-dev-cli).

### Installation

1. **Clone the Repository:**

   ```bash
   git clone [your-repo-url]

   ```

2. **Set Up Environment: Initialize the environment with:**

   ```bash
   azd init -t azure-search-openai-demo

   ```

3. **Deploy Resources: Provision Azure and deploy the app:**
   ```bash
   azd up
   ```

### Running the App

1. **In Azure: Access the deployed WebApp via the URL shown after deployment.**

2. **Locally: Start the app with the following:**

   ```bash
   ./start.sh  # for Unix
   ./start.ps1 # for PowerShell

   ```

3. **Navigate to http://127.0.0.1:50505 to use the app.**

### Monitoring & Troubleshooting

1. **Performance Monitoring: View logs and traces in Application Insights for diagnostics.**

2. **Common Issues: For troubleshooting tips, refer to docs/troubleshooting.md.**

### Cleanup

1. **To delete the Azure resources created by this project, run:**
   ```bash
   azd down
   ```
