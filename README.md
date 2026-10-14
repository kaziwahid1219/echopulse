
# EchoPulse 

An offline-resilient, voice-first emergency response network designed to orchestrate community help during natural disasters when cellular networks fail. Built for the Amazon Developer Hackathon.

## Core Features
- **Voice-First Ingestion:** Victims simply speak to an Alexa-enabled smart hub to report emergencies without complex user interfaces.
- **AI Triage Brain:** Uses **Amazon Bedrock (Claude 3.5 Sonnet)** to parse unstructured voice data, extract key entities (victim count, injuries, required supplies), and dynamically calculate priority scores.
- **Resilient Routing:** Powered by **Amazon Location Service** to map danger areas and safely route first responders around dynamic hazards.

##  Architecture & Tech Stack
- **Frontend / Voice UI:** Alexa Skills Kit (ASK) & Alexa Connect Kit
- **AI Engine:** Amazon Bedrock (Claude 3.5 Sonnet)
- **Compute Layer:** AWS Lambda (Serverless Python/Node.js)
- **Database:** Amazon DynamoDB (Ultra-low latency key-value store)
- **Location Services:** Amazon Location Service

##  Setup & Installation
1. **Clone the repository:**
   ```bash
  git clone https://github.com
   cd echopulse
   ```
2. Configure your AWS credentials:
   ```bash
   aws configure
   ```
3. Deploy the stack using AWS SAM:
   ```bash
   sam deploy --guided
   ```

##  License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
