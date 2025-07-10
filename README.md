# Reneuw: An AI-Powered Brain Stroke Rehabilitation Application


## 📌 Introduction

Reneuw – Rewiring Minds, Restoring Lives – is a cross-platform mobile health (mHealth) application developed using Flutter, designed to empower stroke survivors with comprehensive cognitive, physical, emotional, and lifestyle rehabilitation tools. Available for both Android and iOS, Reneuw integrates advanced AI technologies, including a voice-enabled chatbot, MRI-based stroke prediction, and gamified cognitive exercises, to provide personalized, home-based care. 
Key Features:

Health Monitoring: Tracks daily water intake, meal nutrients (calories, carbs, proteins, fats, sugars, cholesterol), and body measurements (BMI, BMR, caloric needs).
Cognitive Training: Includes games like Chess, Snakes and Ladders, and Memory Match to enhance mental agility.
Emotional Wellness: Offers depression risk self-assessment and guided meditation/yoga routines.
AI-Powered Chatbot: Supports text and voice queries using LangChain and Gemini 1.5 for speech-to-text, aiding users with speech impairments.
Stroke Prediction: Utilizes a fine-tuned VGG-19 model to classify ischemic and hemorrhagic strokes from MRI scans with 94% accuracy.
News Feed: Fetches daily health articles via a News API to promote cognitive engagement.

Reneuw leverages a FastAPI backend and MongoDB Atlas for scalable data management, ensuring secure, real-time health tracking and a seamless user experience.


## 🛠 Tech Stack

| *Layer*        | *Tools/Frameworks*              |
|------------------|-----------------------------------|
| Frontend         | Flutter                           |
| Backend          | FastAPI                           |
| Database         | MongoDB Atlas                     |
| Authentication   | Firebase                          |
| ML Model         | VGG-19 (Keras)                    |
| Chatbot/NLP      | LangChain + LLM (Gemini/GPT)      |
| Voice Input      | Gemini 1.5 Speech-to-Text         |
| Articles         | News API                          |





## 🏛️ Overall work flow

![Screenshot 2025-04-23 111736](https://github.com/user-attachments/assets/ab32fe50-27b9-4da7-9249-7dcdd539746a)

## 🤖 Chabot Architecture 

We offer two types of chatbots:

## 🤖💬 Text-to-Text Chatbot for text-based conversations.

![image](https://github.com/user-attachments/assets/217c9225-8e5c-4c38-81ac-e7d6835f256c)

## 🎙️📝 Voice-to-Text Chatbot for voice input converted to text.

![image](https://github.com/user-attachments/assets/e2dbac1f-6b28-4af7-a92f-a61716f741da)



## 📦 APIs Used

Gemini 1.5 API: Speech-to-text conversion for the chatbot.
News API: Daily health and rehabilitation articles.
Pre-trained VGG-19 Model: Fine-tuned for MRI-based stroke classification.

## 🏃‍♂️ Getting Started
These instructions will help you set up and run Reneuw on your local machine for development and testing.
------------------------------
📋 Prerequisites

- Flutter SDK with a recent version.
- Android Studio or Xcode for Android/iOS emulation.
- Git for repository cloning.
= Python for the FastAPI backend.
- MongoDB Atlas and Firebase accounts for database and authentication.

🧱 Setting Up Your Development Environment



- Download and install Git.


- Fork the Repository:

- Fork the Reneuw project on GitHub.


- Clone the Repository: git clone https://github.com/YOUR-USERNAME/Reneuw.git



- Open the Project:

Open your preferred IDE (VS Code, Android Studio, etc.).
Select "Open an Existing Project" and navigate to the cloned Reneuw directory.


- Set Up Firebase:

Create a Firebase project at console.firebase.google.com.
Add an Android/iOS app and download google-services.json (Android) or GoogleService-Info.plist (iOS).
Place these files in android/app/ (Android) or ios/Runner/ (iOS).
Enable Email/Password and Google Sign-In in Firebase Authentication.


- Configure the Backend:

Navigate to the backend directory (e.g., backend/).
Install Python dependencies:pip install -r requirements.txt


Create a .env file in the backend directory:MONGODB_URI=your_mongodb_atlas_connection_string
GEMINI_API_KEY=your_gemini_api_key
NEWS_API_KEY=your_news_api_key


Start the FastAPI server:uvicorn main:app --reload




- Install Flutter Dependencies:

In the project root, run:flutter pub get




- Run the Application:

Connect an Android/iOS emulator or physical device.
Click the Run  button in your IDE or use:flutter run





## 👀 Application Preview

![login](https://github.com/user-attachments/assets/944839c2-2a81-45a2-8cc4-ef22229d065e)
![2](https://github.com/user-attachments/assets/ea3a235d-a61c-44fa-8751-a24eeb4f993a)
![Screenshot 2025-04-23 111333](https://github.com/user-attachments/assets/4ab08ae8-c85a-4590-9237-0bb9a56451a1)
![3](https://github.com/user-attachments/assets/df6cf845-07ed-413c-860b-df28e550922d)
![image](https://github.com/user-attachments/assets/b92c65ed-44f0-47ff-9bec-47f5a06013e9)





## 📝 Why This Project?

Stroke is a leading cause of long-term disability globally, affecting millions each year. Survivors often require extensive rehabilitation to regain cognitive, physical, and emotional function, but traditional clinical care is frequently inaccessible due to logistical, financial, or geographical constraints. Existing mobile health solutions lack the comprehensive, integrated approach needed for effective post-stroke recovery, particularly for users with speech or motor impairments.
Reneuw addresses these gaps by offering an all-in-one platform that empowers stroke survivors to manage their rehabilitation from home. By combining health tracking, cognitive exercises, mental wellness tools, and AI-driven diagnostics, it provides a holistic, user-centric solution. The app’s accessibility features, like voice-enabled interaction, cater to diverse needs, while its scalable architecture supports future enhancements like teleconsultation and wearable integration.

## 🏃‍♂️ How We Came to Solve This Problem?

Recognizing the challenges of post-stroke recovery, we developed Reneuw to deliver personalized, inclusive, and technology-driven rehabilitation:

Comprehensive Care: Tracks hydration, nutrition, and body metrics to manage stroke risk factors, while cognitive games and news articles stimulate mental engagement.
Inclusivity: The AI chatbot’s voice-to-text functionality supports users with speech impairments, and the intuitive Flutter UI is designed for elderly or motor-impaired users.
Early Detection: The VGG-19 model’s 94% accurate stroke classification from MRI scans enables timely interventions, especially in underserved areas.
Emotional Support: Depression risk assessments and guided meditation/yoga promote mental wellness, addressing isolation and stress.
Scalable Infrastructure: FastAPI and MongoDB ensure secure, real-time data management, enabling longitudinal health tracking and personalized recommendations.

Reneuw integrates these features into a single, seamless app, reducing the need for multiple tools and fostering consistent engagement in the recovery process.


## 🎓 Resources

New to Flutter or backend development? Start here:

Lab: [Write Your First Flutter App](https://docs.flutter.dev/get-started/codelab)

Cookbook: [Useful Flutter Samples](https://flutter.github.io/samples/#)

Flutter Documentation: [Tutorials, samples, and API references](https://docs.flutter.dev/)

FastAPI Documentation:https://fastapi.tiangolo.com/

MongoDB Atlas Getting Started:https://learn.mongodb.com/?utm_source=google&utm_campaign=search_gs_pl_evergreen_atlas_general_retarget-brand_gic-null_apac-in_ps-all_desktop_eng_lead&utm_term=mongodb%20atlas%20database&utm_medium=cpc_paid_search&utm_ad=p&utm_ad_campaign_id=22194044286&adgroup=174717488619&cq_cmp=22194044286&gad_source=1&gbraid=0AAAAADQ14006-fCp8P5uoG9KaxT5GPP0g&gclid=Cj0KCQjw_JzABhC2ARIsAPe3ynpvK3Nj37VTAdG0fghpMHHi3T8oHgq1H4Ty-Hf5chRIw5mpbvTI4vwaAu1rEALw_wcB

## ✨ Team Reneuw

Thanks to these wonderful contributors :


    Alajangi Venkata Satya 
    K N Lakshmi
    K Hemavardhan Reddy
    K V Vamshidhar Reddy
    DR. Keerthika T
  


## 🙌 Contributing

We welcome contributions! Please read our Contributing Guidelines and submit pull requests to enhance Reneuw’s features or fix issues.

Built with 💙 by Team Reneuw at Amrita School of Artificial Intelligence, Amrita Vishwa Vidyapeetham.


## 🧠 Remember :
The project, totaling 4.4GB, cannot be fully uploaded due to size limitations. Even with Git LFS, discrepancies persist, so the model and TFLite files are excluded from the repository. All remaining code files are stored in the `lib` and `pages` folders, including MongoDB and Voice API backend code located in the `pages` folder.

