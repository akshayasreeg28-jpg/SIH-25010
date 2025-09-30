# Smart India Hackathon Workshop
# Date:30/09/25
## Register Number:25018408
## Name:AKSHAYA SREE G
## Problem Title
SIH 25010: Smart Crop Advisory System for Small and Marginal Farmers
## Problem Description
A majority of small and marginal farmers in India rely on traditional knowledge, local shopkeepers, or guesswork for crop selection, pest control, and fertilizer use. They lack access to personalized, real-time advisory services that account for soil type, weather conditions, and crop history. This often leads to poor yield, excessive input costs, and environmental degradation due to overuse of chemicals. Language barriers, low digital literacy, and absence of localized tools further limit their access to modern agri-tech resources.

Impact / Why this problem needs to be solved

Helping small farmers make informed decisions can significantly increase productivity, reduce costs, and improve livelihoods. It also contributes to sustainable farming practices, food security, and environmental conservation. A smart advisory solution can empower farmers with scientific insights in their native language and reduce dependency on unreliable third-party advice.

Expected Outcomes

• A multilingual, AI-based mobile app or chatbot that provides real-time, location-specific crop advisory.
• Soil health recommendations and fertilizer guidance.
• Weather-based alerts and predictive insights.
• Pest/disease detection via image uploads.
• Market price tracking.
• Voice support for low-literate users.
• Feedback and usage data collection for continuous improvement.

Relevant Stakeholders / Beneficiaries

• Small and marginal farmers
• Agricultural extension officers
• Government agriculture departments
• NGOs and cooperatives
• Agri-tech startups

Supporting Data

• 86% of Indian farmers are small or marginal (NABARD Report, 2022).
• Studies show ICT-based advisories can increase crop yield by 20–30%.

## Problem Creater's Organization
Government of Punjab

## Theme
Agriculture, FoodTech & Rural Development

## Proposed Solution
1. Multi-Channel Access for Farmers
To ensure inclusivity and adoption, the platform will be accessible through:
 Mobile App (Android)
 WhatsApp/Telegram Chatbot
 SMS and IVRS (for non-smartphone users)
 Web Dashboard (for officers/administrators)
Features like local language support and voice assistance will make it easy to use.

 2. Personalized Crop Recommendations
The system suggests the best crops based on:
Soil data (pH, type, moisture)
Season & geography
Weather forecast
Water availability
Past yield trends
Uses ML models like Decision Trees, Random Forest, or KNN.

3. Weather-Based Advisory & Alerts
Real-time and predictive guidance through:
Rainfall & drought alerts
Sowing/harvesting recommendations
Irrigation planning
Heatwave and frost warnings
Uses IMD/OpenWeather APIs and forecasting models.

4. AI-Based Pest & Disease Detection
Farmers can upload an image of affected crops.
CNN & image processing models detect pests/disease
Immediate advisory on treatment (chemical/organic)
Alert other farmers in the region automatically
Tools: TensorFlow / PyTorch / OpenCV

5. Fertilizer & Soil Health Advisory
NPK and micronutrient guidance
Fertigation schedule suggestions
Soil Health Card data integration
Organic alternative recommendations
This reduces cost and improves soil sustainability.

6. Market & Price Advisory
Shows mandi/bazaar rates from Agmarknet/eNAM
Suggests the right time & place to sell
Helps reduce exploitation by intermediaries

7. Offline & Low-Internet Functionality
Data caching in local storage
SMS-based inputs and alerts
Syncs automatically when connected
IVRS for voice-based help

8. Admin & Analytics Dashboard
Authorities and NGOs can:
Monitor crop trends
View region-wise soil/pest patterns
Predict risk zones
Offer localized interventions

9. Scalable & Modular Architecture
The system is built with:
Microservices architecture
API integration for easy scaling
Cloud deployment (AWS/GCP/Azure)
AI models upgradable over time

10. Future Integration Readiness
The solution is designed to integrate with: IoT sensors (soil moisture, weather, irrigation) ,Drones for crop health imaging , Satellite-based prediction systems , Blockchain for supply chain and subsidy tracking

 Summary 
“An AI-driven, multilingual, multi-channel advisory system that delivers personalized crop, pest, weather, and market guidance to small and marginal farmers, with offline access, image-based diagnosis, and data-driven insights
<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/00e3378c-f1a9-4cb4-94a4-b1866986225d" />

# Technical Approach
1. System Architecture Overview
A hybrid architecture combining:
   Mobile App / Web Portal / Chatbot / IVRS as front-end interfaces
   Backend server for data processing
   AI/ML models for insights
   APIs & databases for real-time updates
   Cloud deployment for scalability

 2. Core Components of the Technical Approach
  Front-End Layer
 User Interfaces based on literacy and device access:
 Android Mobile App (with offline mode)
 WhatsApp/Telegram Chatbot (for quick advisory)
 IVRS/SMS (for non-smartphone users)
 Web Dashboard (for officers & admins)
 
 Features:
Crop suggestions
Alerts & notifications
Voice support in local languages
Image upload for pest diagnosis

Tech Stack:
Flutter / React Native / Kotlin
Twilio / Gupshup (for SMS & IVRS)
HTML/CSS/React (web interface)

Backend & APIs
Handles authentication, advisory logic, and integration.
REST API / GraphQL to manage:
User profiles (farmers, officers)
Soil & crop request handling
Weather & pest advisory
AI model communication

Tech Stack:
Node.js / Django / FastAPI
Express / Flask
Firebase / Supabase (optional)

 Database & Storage Layer
Stores farmer data, crop patterns, and historical analytics.
Relational DBs:
PostgreSQL / MySQL
NoSQL (for fast access or offline sync):
MongoDB / Firebase Firestore

File storage:
AWS S3 / Firebase Storage for images
Data Stored:
Farmer profile
Soil data
Location and crop history
Weather + yield stats
Pest/disease logs
Advisory outputs

AI/ML Intelligence Layer
1. Crop Recommendation System
Inputs:
Soil type, pH, moisture
Weather and season
Geography
Historical yield patterns

Algorithm:
Decision Trees / Random Forest / Ensemble ML
Reinforcement Learning (optional)

2. Pest & Disease Detection
Farmer uploads image of crop
CNN-based image classification using:
TensorFlow
PyTorch
OpenCV

3. Weather Prediction & Advisory
Real-time data from IMD/OpenWeather API
ML model for predictive insights

4. Fertilizer Optimization
Rule-based engine + AI model
NPK (Nitrogen, Phosphorus, Potassium) suggestions
Quantity and timing alerts

 Data Sources & Integration
Weather APIs:
OpenWeatherMap / AccuWeather / IMD
Soil Data APIs & Offline Input:
ICAR / Soil Health Card / user entry
Market Price Feeds:
Government mandi databases (Agmarknet API)
Pest Advisory APIs:
FAO PlantVillage, local agri databases

 Deployment & Scalability
Hosting Options:
AWS / GCP / Azure
Railway.app / Render / Firebase (budget-friendly)
Containerized Deployment:
Docker + Kubernetes (if scaling is needed)
Microservices-based approach = easier updates

 Security & Authentication
JWT-based login
SSL/TLS for all communication
Role-based access (farmer, officer, admin)

Offline/Low Internet Support
Local caching (SQLite, Room DB, MMKV)
SMS gateway fallback
Periodic sync once online

 Technical Workflow (Example)
1️⃣ Farmer registers with name, land size, and location
2️⃣ Soil type/weather auto-fetched via API or manual input
3️⃣ System processes data and recommends suitable crops
4️⃣ Farmers get alerts:

Pest risks
Weather-based actions
Fertilizer schedules
Market prices:
5️⃣ Uploaded pest image → ML detection → remedy suggestion
6️⃣ Data stored for future predictions & analytics

Future Enhancements
Blockchain for supply chain transparency
Smart sensors/IoT integration
Voice-enabled virtual farm assistant
Drone monitoring addons
GIS mapping for precision farming

## Impact and Benefits
1. Economic Benefits
Reduced Crop Losses
Accurate pest, disease, and weather alerts help prevent yield damage.
Cost-Effective Input Usage
Data-driven guidance on fertilizers, irrigation, and seeds reduces waste and lowers expenses.
Improved Crop Yields
Scientific recommendations increase productivity per acre.
Better Market Earnings
Price alerts and selling suggestions help farmers get higher returns.

2. Social Benefits
Empowerment of Small & Marginal Farmers
Provides access to expert advisory without the need for middlemen.
Local Language & Voice Support
Improves adoption among low-literacy and rural populations.
Inclusivity & Accessibility
IVRS and SMS modes help farmers without smartphones or internet.
Gender Inclusion
Women farmers can participate equally through mobile advisory platforms.

3. Environmental Benefits
Sustainable Farming
Encourages optimal use of fertilizers, pesticides, and water.
Reduced Soil Degradation
Prevents overuse of chemicals through precise NPK guidance.
Climate Resilience
Weather-based advisory helps farmers adapt to floods, droughts, and high temperatures.
Promotion of Crop Rotation & Soil Health
Improves long-term fertility and biodiversity.

 4. Technological Impact
 AI-Driven Decision Support
Bridges the knowledge gap using predictive analytics and image processing.
Real-Time Advisory
Live updates on climate, pests, and crop cycles enable timely action.
Digital Agriculture Adoption
Brings rural communities into the agri-tech ecosystem.
IoT/ML Integration Potential
Scalable for sensors, drones, and satellite-based monitoring.

 5. Government & Policy-Level Impact
 Supports Digital India & Agri Stack Initiatives
Aligns with national goals of smart farming.
 Boosts Farmer Welfare Schemes
Assists programs like PM-KISAN, Soil Health Card, and Crop Insurance.
Data for Policy Making
Analytics help government plan subsidies, crop planning, and disaster response.

 6. Long-Term Sustainable Impact
 Doubling Farmer Income Goal
Enhances financial stability of smallholders.
Reduced Rural Distress & Migration
Farmers can sustain livelihoods without relocating.
Food Security Improvement
Increased yield ensures better supply at national level.
Scalability Across States
Can be customized to region, weather, and local crops.

Benefit Area	Key Outcomes
Economic	Higher income, lower input cost, better crop planning
Social	Empowerment, inclusivity, accessibility
Environmental	Soil health, water conservation, sustainable practices
Technological	AI/ML adoption, real-time support, data integration
Policy Alignment	Govt collaboration, scheme support, analytics
Long-Term Impact	Food security, rural development, resilience


## Research and References
Key Studies & Insights
ICAR & NABARD reports highlight that >80% of Indian farmers lack timely advisory, leading to low yields.
FAO and World Bank studies show mobile-based advisory increases farmer productivity by 15–30%.
Soil Health Card research indicates tailored fertilizer guidance improves yield by 20–25%.
IITs & PlantVillage studies prove that AI image models can detect plant diseases with 90%+ accuracy.

Existing Platforms Referenced
mKisan SMS Advisory
Kisan Suvidha App
Plantix (pest detection)
Digital Green
eNAM & Agmarknet
ICAR + Krishi Vigyan Kendras

Limitations in current platforms include lack of: personalization, image-based diagnosis, offline access, and multilingual voice support—which this system addresses.
Data Sources & APIs Used
Weather: IMD, OpenWeatherMap
Soil: Soil Health Card Database, ICAR
Pests: PlantVillage / CABI datasets
Market Prices: eNAM, Agmarknet

Research Papers (Basis)
AI in Agriculture – Elsevier (2021)
ML for Crop Yield Prediction – IEEE (2020)
Mobile Advisory Systems – World Bank (2021)
Precision Farming Techniques – ICAR (2019)

Policy & SDG Alignment
Digital India Mission
AgriStack & PM-Kisan
UN SDGs: 2 (Zero Hunger), 9 (Innovation), 12 (Sustainable Production), 13 (Climate Action)



