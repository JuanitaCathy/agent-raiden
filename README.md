# Agent Raiden

Agent Raiden is an AI-powered gaming assistant designed to enhance your gaming experience by providing real-time insights, video stream summaries, and strategic gameplay tips. It integrates seamlessly with Telegram to offer personalized recommendations and data-driven guidance.

## Features

### 🎮 **Gaming Assistance**
- **Game Stream Summarization** – Extracts key moments, strategies, and highlights from YouTube game streams.
- **Gameplay Tips & Tricks** – AI-generated suggestions based on your playstyle and game history.
- **Boss Fight Strategies** – In-depth analysis of boss mechanics and tactics for easy victories.

### 📩 **Productivity Tools for Gamers**
- **Gaming Newsletter Management** – Send and receive gaming-related emails.
- **Unread Email Summarization** – Quickly get insights from unread emails.
- **Google Calendar Integration** – Schedule game sessions with teammates.
- **Excel Sheet Creation** – Track game stats and performance metrics.

### 🔍 **Smart Query & Search**
- **Web Search Integration** – Uses SERP API and Wikipedia for knowledge retrieval.
- **Memory & Context Awareness** – Stores chat history using PostgreSQL for refined responses.

## Workflow Overview

Agent Raiden is powered by **n8n**, ensuring a structured data flow for optimal performance. The workflow follows these key steps:

### 1️⃣ **Trigger Nodes**
- **Telegram Trigger** – Detects user messages from Telegram.
- **Webhook Trigger** – Captures external requests from Agent Zero or other sources.

### 2️⃣ **Processing Nodes**
- **Input Preparation** – Formats data fields like query, user ID, request ID, and session ID.
- **AI Agent Processing** – Handles user input and generates AI-driven responses.

### 3️⃣ **Conditional Routing**
- **If Node** – Determines the response destination (Telegram or Webhook) based on the input source.

### 4️⃣ **Output Nodes**
- **Telegram Output** – Sends responses back to the Telegram user.
- **Webhook Response** – Delivers responses to external applications or Agent Zero.

## Use the file!

You can import the json file into your n8n workspace and replace/fill with appropriate credentials!

