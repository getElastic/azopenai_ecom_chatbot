# azopenai_ecom_chatbot

This eCommerce chatbot offers essential services, such as order status inquiries, return policy details, and user contact collection for human follow-up. Built with Flask and integrated with Azure OpenAI's GPT-4, it ensures efficient customer support.

## Prerequisites

- Docker

## Setup

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/azopenai_ecom_chatbot.git
   cd azopenai_ecom_chatbot
   ```
   
2. **Add your OpenAI API key**:

   Update the docker-compose.yml file with your OpenAI API key:
   ```bash
   AZURE_OPENAI_API_KEY: your_azure_openai_api_key_here
   AZURE_OPENAI_ENDPOINT: your_azure_openai_endpoint_here
   ```

## How to Run
Build and run the Docker container:

In the root directory of the project, run the following command to build and start the Docker container:

   ```bash
   docker-compose up --build
   ```

This command will build the Docker image and start the Flask application inside a Docker container.


## Access the application:

Once the container is running, you can access the application in your web browser at http://localhost:5000.

##  Usage
- **Order Status:** The chatbot can provide the status of an order. Simply ask for the status and provide the order ID when prompted.
- **Request Live Agent:** To speak with a human agent, provide your contact information including full name, email, and phone number.
- **Return Policies:** The chatbot can provide information on return policies, including conditions for returning items, non-returnable items, and the refund process.


## Files Description
- **app.py:** The main Flask application file.
- **templates/index.html:** The HTML template for the chatbot UI
- **order_status.csv:** A CSV file containing order statuses.
- **contact_info.csv:** A CSV file for storing contact information.