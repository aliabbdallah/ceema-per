 # Ceema

Ceema is a Flutter-based mobile application for film enthusiasts. It combines a personal movie diary, social networking, and a machine-learning powered recommendation engine into one seamless experience, backed by a cost-optimized Firebase backend.

---

## 🚀 Features

- **User Authentication**  
  • Email/password sign-up & login via Firebase Auth  
  • Profiles stored under `users/{uid}` in Firestore  

- **Feed System**  
  - **For You**: personalized ML-based recommendations  
  - **Trending**: posts from the last 14 days with high engagement  
  - **From Friends**: posts by users you follow  
  - Infinite scroll + pagination + local caching  

- **Posts & Journaling**  
  • Create diary-style posts with text, timestamp, likes, comments  

- **Recommendations**  
  • Hybrid rule-based + ML model (TensorFlow/PyTorch)  
  • Candidate generation → feature vector → inference → diversity filter  

- **Profile & Social**  
  • Follow/unfollow users  
  • View follower/following counts, avatar, stats  

- **Performance & Caching**  
  • Local caching of Firestore reads (`Hive`/`Drift` or `SharedPreferences`)  
  • Time-to-live + event-based invalidation  
  • In-memory LRU cache for movie metadata  

- **Future Enhancements**  
  • Push notifications (FCM)  
  • Offline write queue & background sync  
  • Post reactions & tagging  
  • Social sharing  

---

## 🛠 Tech Stack

| Layer              | Tool / Service           |
| ------------------ | ------------------------ |
| Frontend           | Flutter                  |
| State Management   | Provider                 |
| Auth               | Firebase Auth            |
| Database           | Firestore                |
| Storage            | Firebase Storage         |
| Local Cache        | Hive / Drift / SharedPreferences |
| Media Picker       | file_picker              |
| ML Model Training  | Python (TensorFlow/Keras)|
| Inference Server   | FastAPI / Cloud Run      |

---

## 📦 Getting Started

### Prerequisites

- Flutter SDK ≥ 3.x  
- Android Studio / Xcode (for simulators)  
- Firebase project with Auth, Firestore, Storage  

