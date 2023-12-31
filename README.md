# Rachel: Streamlined Voice Assistant for Enterprises

## Introduction

Meet Rachel, an agile voice assistant built for performance and user engagement. Combining Python and FastAPI, it delivers fast, concurrent API interactions with OpenAI-powered conversation capabilities. The frontend is sleek, powered by React, TypeScript, and styled with Tailwind CSS, with Yarn managing dependencies efficiently.

Tailored for businesses, Rachel automates customer support and streamlines operations. Its modular architecture allows for easy integration and secure deployment. Explore Rachel's capabilities on our GitHub repository.

<img src="/frontend/media/rachel.webp" alt="Rachel Image">

# Tech Stack

## Backend

- **Python**: A versatile programming language used here as the primary backend language.
- **FastAPI**: A modern web framework for building APIs with Python 3.6+ that offers high performance. It's designed to create APIs quickly and based on standard Python type hints.
- **OpenAI**: Provides AI functionalities, possibly for generating responses or understanding natural language.
- **python-decouple**: This library helps in keeping configuration and secrets separate from the codebase, which is essential for security and easy deployment across different environments.
- **python-multipart**: Allows the backend to handle file uploads by parsing multipart/form-data.
- **Uvicorn**: An ASGI server implementation that serves the FastAPI application, known for its speed and concurrency capabilities.

## Frontend

- **JavaScript**: The core scripting language used to create dynamic web pages on the client side.
- **React**: A library for building user interfaces, enabling the creation of a single-page application that can interact with the backend without needing to reload the page.
- **TypeScript**: A typed superset of JavaScript that adds static type definitions, leading to more robust code and error checking at compile time.
- **Tailwind CSS**: A utility-first CSS framework used to build custom designs without leaving the HTML.
- **Yarn**: A fast, reliable, and secure dependency management system.

# Usage and Enterprise Solutions

"Rachel" can be used in various contexts, including customer service, personal assistants, or in any domain requiring natural language processing and task automation. Enterprises can leverage this voice assistant to:

- **Improve Customer Service**: Automate responses to frequently asked questions, reducing the workload on human agents.
- **Enhance Productivity**: Integrate with enterprise systems to provide employees with quick access to information, such as schedules, reports, and analytics.
- **Accessibility**: Aid users with disabilities by enabling voice-driven interactions for various services.
- **Data Collection**: Gather insights into customer queries and interactions, which can be used to improve services and customer understanding.

# Problems Resolved

This voice assistant could potentially resolve several issues such as:

- Reducing the time taken to get responses for queries as it automates the interaction process.
- Handling multiple customer queries simultaneously, increasing efficiency.
- Providing a hands-free mode of interaction, which can be useful in situations where typing is not feasible.
- Personalizing user experience based on past interactions and preferences.

# Rachel

<img src="/frontend/media/Rachel2.PNG" alt="Rachel Image">

# Instructions

## Download

Download the package from GitHub

## Setup backend

Change directory into backend

```shell
cd chatbot/backend
```

### Setup virtual environment

Create a Virtual Environment

```shell
python3 -m venv venv
```

Activate Virtual Environment (MAC)

```shell
source venv/bin/activate
```

Activate Virtual Environment (Windows)

```shell
source venv/Scripts/activate
```

Upgrade PIP

```shell
pip3 install --upgrade pip
```

### Install Python packages

Install required Python packages

```shell
pip3 install openai python-decouple fastapi "uvicorn[standard]" python-multipart
```

Or use this alternative method (although this alternative method might not work if using Windows)

```shell
pip3 install -r requirements.txt
```

### Create Environment Variables

Create your .env file

```shell
touch .env
```

Update your .env file with the following. You can see your .env by typing sudo nano .env or just by clicking on the file if you are in VS Code.

```plain
OPEN_AI_ORG=enter-you-key-here
OPEN_AI_KEY=enter-you-key-here
ELEVEN_LABS_API_KEY=enter-you-key-here
```

### Start your backend server

Start your backend server

```shell
uvicorn main:app
```

Alternatively, you can ensure your server resets every time you make a change by typing:

```shell
uvicorn main:app -- reload
```

You can check your server is working by going to:

```plain
http://localhost:8000/health
```

## Setup frontend

Change directory into frontend

```shell
cd ..
  
```

Install packages

```shell
yarn --exact
```

Build application

```shell
yarn build
```

Start server in dev mode

```shell
yarn dev
```

You can check your dev server is working by going to:

```plain
http://localhost:5173/health
```

or alternatively in live mode:

```shell
yarn start
```

You can check your live server is working by going to:

```plain
http://localhost:4173/health
```
