# 🏥 Organ Donation App (Blood & Buddies)

A full-stack Android application that connects **organ donors** with **recipients** in real-time.
This app helps users find compatible donors/recipients based on blood group and organ requirements.

---

## 🚀 Features

* 🔐 **User Authentication**

  * Signup / Login using Firebase Authentication
  * Forgot Password support

* 👤 **User Roles**

  * Donor Registration
  * Recipient Registration

* 📊 **Dashboard**

  * View available donors/recipients
  * Real-time data from Firebase

* 🔍 **Filter System**

  * Search by blood group
  * Matching logic (Donor ↔ Recipient)

* 🧾 **User Profile**

  * View & update personal details

* 🔔 **Notifications**

  * Alerts when matches are found

* 📧 **Email Integration**

  * Contact users via email (JavaMail API)

---

## 🛠️ Tech Stack

| Technology                 | Purpose                  |
| -------------------------- | ------------------------ |
| Java                       | Core Android development |
| Android SDK                | App framework            |
| Firebase Authentication    | User login/signup        |
| Firebase Realtime Database | Store user data          |
| Firebase Storage           | Profile images           |
| Firebase Analytics         | Usage tracking           |
| Glide                      | Image loading            |
| Material Design            | UI components            |

---

## 📱 How the App Works

1. User signs up as **Donor** or **Recipient**
2. Data is stored in Firebase
3. App fetches matching users:

   * Donor → sees Recipients
   * Recipient → sees Donors
4. Users can contact each other via email

---

## 📦 Installation (Run Locally)

### 🔧 Prerequisites

* Android Studio
* Android device or emulator
* Firebase account

---

### 🪜 Steps

1. Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/organ-donation-app.git
```

2. Open project in Android Studio

3. Add Firebase configuration:

   * Go to Firebase Console
   * Create project
   * Add Android app:

     ```
     com.ali.organdonation
     ```
   * Download `google-services.json`
   * Place it inside:

     ```
     app/google-services.json
     ```

4. Enable Firebase services:

   * Authentication → Email/Password
   * Realtime Database

5. Sync Gradle & Run ▶

---

## 📂 Project Structure

```
app/
 ├── java/com/ali/organdonation/
 │   ├── activities/
 │   ├── adapters/
 │   ├── models/
 │   └── utils/
 ├── res/
 │   ├── layout/
 │   ├── drawable/
 │   └── values/
```

---

## ⚠️ Important Notes

* `google-services.json` is NOT included for security reasons
* You must add your own Firebase configuration
* Email feature may require Gmail App Password

---

## 🔐 Firebase Rules (for testing only)

```json
{
  "rules": {
    ".read": true,
    ".write": true
  }
}
```

⚠️ Do NOT use these rules in production

---

## 🎯 Future Improvements

* Push Notifications (FCM)
* Better UI/UX design
* Secure database rules
* Admin panel
* Location-based matching

---

## 👨‍💻 Author

Mohd Abdul Raheem

---

## 📌 Conclusion

This project demonstrates:

* Android development using Java
* Firebase backend integration
* Real-time data handling
* User-based matching system

---

⭐ If you like this project, consider giving it a star!

  


