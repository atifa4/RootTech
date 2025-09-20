# RootTech
Digital Krishi Officer is a multilingual AI-powered farmer advisory system designed to provide location-aware insights on pests, weather, subsidies, and market trends. Farmers can interact with the system through text, voice, or images, making it inclusive for all literacy levels. A custom knowledge engine integrates data from APIs, government databases, and agricultural datasets to deliver personalized and reliable advice. The system contextualizes queries using local weather, soil, and crop data to ensure accuracy. Responses are provided in farmer-friendly formats such as text, voice, and visuals. For complex or unclear queries, the system includes an escalation mechanism to Agro Officers. Continuous feedback loops improve the knowledge engine, making the solution scalable, sustainable, and farmer-first.

Digital Krishi Officer – Detailed Project Explanation

1. Input Process
-Farmer Profile & Authentication: Farmers log in with their profile (name, location, language preference). Authentication ensures security and privacy of their data.
-Input Modes: Farmers can ask queries through text (NLP), voice (STT – Speech to Text), or image (RCN – image recognition for crop/pest detection).
-Location & Data Fetching: The system automatically fetches GPS location, weather, and soil data to contextualize the query.

2. Brain & Processing
-Central AI Brain: This module processes the farmer’s query using Natural Language Processing (NLP) and context awareness.

-Knowledge Sources:
APIs & Data.gov.in for government-approved schemes and weather data.
User Database for farmer history and previous queries.
Web Scraping / Web Surfing for additional crop and market information.

-Advanced AI Models:
Hugging Face Models for language understanding and multilingual query handling.
Retrieval Augmented Generation (RAG) to combine stored knowledge with live data.
Vector Database (RAG DB) for efficient query-answer retrieval.

-Fallback Mechanism: If the system cannot fetch from DB, it performs live search and processes the data.

4. Output Processing
-The system decides the output format based on farmer preference:
Text Response (for literate farmers).
Voice Response (for low-literacy farmers).
Image Output (for charts, pest identification, crop visuals).

-This ensures inclusivity across farmer literacy levels.

4. Escalation System

-First-Level Queries: Simple, structured queries (like weather, subsidy info) are handled fully by AI.

-Complex Queries: If the system cannot confidently generate an answer, the query is forwarded to an Agro Officer.

-Expert Feedback: Officer responses are stored in the system and used to improve the AI model through continuous learning.

5. Feedback & Continuous Learning
Farmers provide feedback on responses.
Feedback is validated by experts and stored in the database.
The system continuously retrains using this real-world feedback, ensuring it becomes more accurate and localized over time.

6. Frontend
-Farmers interact via a mobile/web dashboard built with React + Tailwind.
Dashboard features:
Weather updates
Subsidy alerts
Query history
Pest/crop advisories
-Works in multilingual mode (Malayalam, Tamil, English) and supports both text and voice chat.

