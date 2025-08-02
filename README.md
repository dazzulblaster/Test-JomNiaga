# **JomNiaga**

#### *"Simplifying business for all in one platform, one journey, and endless growth."* 🚀

---

## 📝 Overview

**JomNiaga** is a digital business onboarding platform designed to simplify the journey for Malaysian MSMEs to enter the digital economy. The app provides an **all-in-one solution** for new and informal businesses to easily:

- Register and formalize their business  
- Manage compliance and licensing  
- Integrate with digital payment systems  
- Access financial services such as loans, grants, and government programs  

By streamlining onboarding into a **single, reusable flow**, JomNiaga reduces paperwork, minimizes dropout rates, and unlocks continuous access to financial tools. The platform nudges MSMEs toward better financial practices while supporting **sustainability** and **inclusivity** as part of Malaysia's evolving digital payment ecosystem.

---

## Get Started with JomNiaga  
This guide will walk you through setting up the JomNiaga app on your machine using Expo Go.  
1. Download Expo Go app from App store or Google Playstore.
2. Scan the QR below using your device's camera
![Solution Architecture](./expoqr.jpg) 
---

## 🚧 Challenges

1. **Complex MSME Onboarding**  
   MSMEs face fragmented and repetitive registration processes across multiple platforms, slowing down digital adoption.

2. **Limited Access to Financial Services**  
   Small businesses struggle to qualify for loans, grants, and support programs due to lack of formalization and real-time eligibility checks.

3. **High Dropout Rates During Formalization**  
   Cumbersome forms and unclear steps lead to up to **50% of MSMEs** abandoning digital onboarding before completion.

---

## ✨ Key Features

- **One-Stop Business Onboarding 🗂️**  
  Simplifies MSME registration, licensing, and compliance into a single, automated process using document scanning and auto-fill features.

- **Digital Payment Integration 💳**  
  Enables MSMEs to easily accept payments through **DuitNow QR**, e-invoicing, and digital payment gateways.

- **Financial Access Enablement 💰**  
  Provides MSMEs with access to loans, grants, and government programs through continuous financial assessment and eligibility checks.

- **Real-Time Notifications 🔔**  
  Sends timely alerts for license renewals, compliance deadlines, and available funding opportunities.

- **Simplified User Experience 🧭**  
  Offers a user-friendly interface designed to be accessible for MSMEs of all sizes and digital literacy levels.

- **Continuous Support & Growth 📈**  
  Delivers ongoing financial health assessments and business insights to help MSMEs grow and improve their operations.

- **NiagaChat: Your MSME Assistant 🤖**  
  Guides users through business-related tasks by suggesting financial aids, services, and educational content through an interactive chatbot.

- **NiagaCommunity: Educational Content 📚**  
  Provides MSMEs with educational content, success stories, and interactive resources to empower them in their business journey.

- **NiagaCentre: Service Marketplace 🛠️**  
  Allows MSMEs to offer and receive services that help each other grow, such as consulting, design, and marketing.

---

## 🏗️ Solution Architecture

![Solution Architecture](./solution.png)  

---

## 🛠️ **Technology Stack**

### **Frontend:**
- **React Native** – For building cross-platform mobile applications for both iOS and Android.

### **Backend:**
- **FastAPI** – A modern, fast web framework for building APIs with Python, used for financial calculations and backend services.
- **Node.js** – For handling non-blocking, event-driven server-side applications (if applicable for other backend services).

### **Database:**
- **Firebase Realtime Database** – A cloud-hosted NoSQL database that allows data to be synced in real-time across all clients.
- **Firebase Cloud Storage** – For storing and serving user files such as documents, images, etc.

### **Authentication:**
- **Firebase Authentication** – Provides backend services to help authenticate users, including simple pass-through authentication using passwords, social media logins (Google, Facebook), and phone numbers.

### **Machine Learning & Automation:**
- **n8n** – For workflow automation and integrating third-party services to automate tasks like loan eligibility checks, financial data assessment, etc.
- **Pinecone** – Used for vector embeddings, powering smarter recommendations in the app (e.g., content and business suggestions).

### **External Integrations:**
- **SSM API** – For accessing business registration data to verify business details.
- **LHDN (Peppol Network)** – For integrating e-invoicing and tax compliance features.
- **MDEC API** – For integration with government programs, like grants and microcredit services.

### **Hosting & Deployment:**
- **Expo** – For React Native app development and deployment.
- **Render** – For backend hosting, serverless functions, and managing API endpoints.

---

This **technology stack** gives an overview of the key tools, services, and frameworks used in building **JomNiaga**, helping developers understand the architecture and dependencies of the app.

---

# 🚀 Loan Eligibility Risk Classifier

This project is an *end-to-end machine learning pipeline* to classify *business loan applications* into risk categories:

- ✅ *Safe*
- ⚠️ *Moderate*
- ❌ *High Risk*

The model is deployed via **FastAPI** and hosted on **Render.com**.

---

## 🌐 Live API

**Base URL:**  
https://loan-eligibility-ml.onrender.com/

**API Documentation (Swagger UI):**  
https://loan-eligibility-ml.onrender.com/docs

---

# 📊 Features & Financial Calculations

The model uses *24 months of financial transaction data* per business to compute the following metrics:

### 💵 Average Monthly Sales


### 💸 Average Monthly Expenses


### 📈 Volatility of Sales

*Measures the business stability:*

### 🔄 Net Operating Cash Flow (NOCF)



### 🧮 Debt Service Ratio (DSR)

*Measures the ability to service debt:*

---

# 🧠 Risk Classification Logic

| Condition | Risk Category |
|------------|---------------|
| DSR > 1.8 and Volatility < 0.15 | ✅ *Safe* |
| DSR < 0.8 or Volatility > 0.5 | ❌ *High Risk* |
| Else | ⚠️ *Moderate* |


---

## 📄 Project Info

**Project Title:** JomNiaga  
**Team Name:** Paytriots  
**Team Members:** Izzul, Zaid, Afifah, Adli, Fahmi  
**Institution:** Universiti Tenaga Nasional (UNITEN)  
**Event:** PayHack 2025
