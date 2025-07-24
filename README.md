# nudg - A Smart Diabetes Assistant

## Overview

**nudg** is a comprehensive iOS application designed for individuals with diabetes who use a Nightscout instance. It serves as a powerful client for Nightscout, providing a modern, user-friendly interface to view, log, and analyze diabetes-related data. The app is built with a focus on providing actionable insights and convenient tools to aid in daily management.

---

## Core Features

### Dashboard & Monitoring
* **Real-time Glucose Data**: Displays current blood glucose levels, trend arrows, and a detailed chart of recent readings fetched directly from your Nightscout site.
* **Customizable Dashboard**: Users can choose between a horizontally-sliding or a vertically-stacked layout. The dashboard consists of customizable cards displaying various statistics.
* **Active Insulin (IOB)**: Shows both rapid and long-acting insulin on board, with the ability to view expiry times.
* **Pending Dose Confirmation**: An optional safety feature that requires users to manually confirm an insulin injection before it's logged to Nightscout, preventing accidental logging.

### Data Logging
* **Comprehensive Entry Types**: Log bolus/basal insulin, carbohydrates, ketones, fluid intake, and weight.
* **Journaling**: Create detailed journal entries with categories (e.g., Food Note, Exercise, Feeling Sick) and moods (e.g., Happy, Tired, Sad) to add context to your data.
* **Health Records**: Keep track of important health events like eye screenings, blood tests, HbA1c results, and hospital appointments.
* **Tagging System**: Create and assign custom tags to meals to categorize them and enable advanced meal pattern analysis.

### Calculators & Tools
* **Correction Dose Calculator**: Suggests an insulin dose to correct for high blood glucose based on your Nightscout profile settings (ISF, Target Range) and current IOB.
* **Quick Bolus Calculator**: A streamlined tool for calculating a meal bolus based on carbohydrate intake and current glucose levels.
* **Nutrition Calculator**: Estimates carbohydrate counts for meals by querying the Nutritionix database.

### Analysis & Reporting
* **Advanced Analytics**: A dedicated view to analyze glucose data over various time ranges (1, 7, 14, 30 days), showing metrics like Estimated HbA1c, Time in Range, Standard Deviation, and Coefficient of Variation.
* **Post-Meal Analysis**: Tapping on a meal entry provides a detailed view of the post-prandial glucose response, including peak glucose, time to peak, and AI-generated insights.
* **PDF Report Generation**: Create professional, shareable PDF reports summarizing glucose data, treatments, and key statistics for a selected date range.

### Integrations
* **HealthKit Sync**: Securely syncs glucose, carbohydrate, and insulin data to and from Apple Health. It can also read workout, sleep, mindfulness, and menstrual data from HealthKit and log it to Nightscout.

---

## 💎 Premium Features

Upgrading to Premium unlocks the full potential of nudg:

* **AI Nutrition Calculator**: Utilizes the Gemini AI model to estimate carbohydrate counts from natural language descriptions of meals (a limited number of free uses are available via rewarded ads).
* **Extended Bolus Planner**: Helps plan split or extended boluses for slow-digesting meals, with custom plans generated from learned meal patterns.
* **Saved Meals Library**: Save frequently eaten meals with their carb counts and tags for quick access and logging.
* **Multiple Profiles**: Add and manage multiple Nightscout profiles, ideal for caregivers or individuals with multiple rigs.
* **Advanced Analytics & Reporting**: Full access to the advanced analytics suite and PDF report generation.
* **Enhanced Customization**: Unlock additional dashboard card slots and advanced color customization options.

---

## 🛠️ Configuration & Setup

* **Nightscout Connection**: The app requires a one-time setup to connect to the user's personal Nightscout instance. This involves providing the Nightscout URL and API Secret.
* **Profile Linking**: If the Nightscout site has multiple profiles, the user can link their in-app profile to a specific Nightscout profile.
* **Privacy First**: All health data is fetched directly from the user's own Nightscout site and is never sent to any third-party servers. The connection is direct between the user's device and their Nightscout instance.

---

## ⚙️ Technology Stack

* **UI Framework**: SwiftUI
* **Backend Connection**: Direct API calls to a user-provided Nightscout instance.
* **Authentication**: Firebase Anonymous Authentication for unique user identification.
* **In-App Purchases**: StoreKit 2 for managing premium subscriptions.
* **AI & Nutrition**:
    * Google's Gemini API for the AI Nutrition feature.
    * Nutritionix API for the standard nutrition calculator.
* **Health Data**: Apple's HealthKit for integration with the Health app.
* **Settings Sync**: iCloud Key-Value Store for syncing certain settings like learned meal patterns across devices.
* **Advertising**: Google AdMob for rewarded video ads.

---

## 📬 Support

* **Email**: [nudg@rhodzy.com](mailto:nudg@rhodzy.com)
* **Discord**: [Join our Discord server](https://discord.gg/gch8h5xr8b)
* **Facebook**: [Join our Facebook group](https://www.facebook.com/groups/1103988940963393)
