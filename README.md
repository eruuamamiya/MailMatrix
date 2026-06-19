# 📧 Mail Matrix
Advanced and high-performance Android email generator tool. Mail Matrix allows users to instantly generate thousands of valid email variations using Plus Addressing and Dot Matrix algorithms, all routing back to a single primary inbox. 
Perfect for managing multiple accounts for gaming (PUBG, MLBB), social media, or software testing.
## ✨ Key Features
* **➕ Plus Addressing Engine:** Instantly append custom tags to your email (e.g., `user+tag@gmail.com`). Includes one-click quick categories for popular platforms.
* **🔴 Dot Trick Engine:** Generates all possible dot variations of an email prefix (e.g., `u.ser@gmail.com`, `u.s.e.r@gmail.com`) using a highly optimized recursive bitmasking algorithm `2^(n-1)`.
* **⚡ Real-Time Live Preview:** Dynamic UI that instantly formats and validates your email configuration as you type.
* **🛡️ Anti-Crash Protection:** Built-in safeguards that limit the Dot Trick engine to 15-character usernames (max 16,384 combinations) to prevent memory leaks and `OutOfMemory` (OOM) Force Closes on Android devices.
* **📋 1-Click Copy:** Seamlessly copy generated emails or live previews straight to your clipboard.
* **🎨 Smart UI Auto-Detect:** Category buttons dynamically react to manual keyboard inputs and touch events for a flawless user experience.
## 🛠️ Tech Stack
* **Language:** Java
* **Platform:** Android
* **UI/UX:** Native Android XML with dynamic `GradientDrawable` manipulation.
## 💡 How it Works
### 1. Plus Addressing (`+` symbol)
Many email providers (like Gmail) ignore everything from the `+` sign to the `@` sign. 
* Input: `johndoe@gmail.com`
* Tag: `pubg`
* Result: `johndoe+pubg1@gmail.com` (Emails sent here will arrive in `johndoe@gmail.com`).
### 2. The Dot Matrix (`.` symbol)
Gmail ignores dots in the username. The app calculates all possible combinations of dots between characters.
* Input: `abc@gmail.com`
* Results: 
  1. `a.bc@gmail.com`
  2. `ab.c@gmail.com`
  3. `a.b.c@gmail.com`
## 📸 Screenshots
*(Add your screenshots here by dragging and dropping images into GitHub)*

| Splash Screen | Home | Plus Engine | Dot Engine |
| :--- | :--- | :--- | :--- |
| ![Splash](link-gambar-lu) | ![Home](link-gambar-lu) | ![Plus](link-gambar-lu) | ![Dot](link-gambar-lu) |

## ⚠️ Disclaimer
This tool is intended for personal email management, software testing, and legitimate multi-account management. The developer is not responsible for any misuse of this application for spamming or violating third-party Terms of Service.
---
*Built with logic, coffee, and pure Java.*
