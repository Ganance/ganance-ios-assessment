# Ganance iOS Developer Assessment

**Estimated Time:** 1 hour  
**Tech Requirements:** Swift, SwiftUI, Combine or async/await  
**Submission Format:** GitHub repo link or zipped Xcode project

---

## Overview

This assessment simulates a lightweight version of the work you would do at Ganance. Our product involves connecting a mobile app to a hardware device over Bluetooth/BLE, so we want to understand how you structure async workflows, handle device-like interactions, and manage app state.

This challenge **does not** require real Bluetooth functionality. Instead, you will simulate a device connection and data sync using delays and mock data.

The focus is on clarity, architecture, and your ability to build a realistic but simple flow.

---

## Your Task

Build a small SwiftUI app that does the following:

### 1. Connect to a Simulated Device

Create a service that simulates connecting to a wearable device.

**Requirements:**

- The “connection” should take about 2–3 seconds using `Task.sleep` or any async method.
- **20% of the time, the connection should fail** with a simulated error.
- Expose this using async/await or a Combine publisher.

---

### 2. Fetch Mock Health Data

Once "connected," fetch a mock payload like:

```json
{
  "steps": 7342,
  "heartRate": 72,
  "sleepHours": 7.3
}
```

### 3. Display the Results in SwiftUI

Create a simple UI with:

- A **Connect** button  
- A **loading** state  
- A **success** state showing the health data  
- An **error** state with a retry option  

UI design does not need to be perfect — clarity is more important than polish.

---

### 4. Architecture Requirements

- Use **MVVM** or another clean architectural pattern  
- Split logic into **service layer** + **view model**  
- Use **Combine** or **async/await** for async workflows  

---

### 5. Bonus (Optional)

Only attempt these if you have extra time:

- Cache the last successful sync in **UserDefaults**
- Show a **timestamp** for last sync
- Add **very lightweight unit tests** for your service or view model

These are optional but helpful.

---

## What We're Looking For

We will evaluate:

- Clear, maintainable architecture  
- Readable, well-structured code  
- Thoughtful handling of async workflows  
- Clean state management (loading, error, success)  
- Ability to simulate real-world device connectivity challenges  
- Optional notes explaining decisions (if included)

We are **not** evaluating:

- Pixel-perfect UI design  
- Real BLE functionality  
- Large or complex boilerplate  
- Over-engineered solutions  

---

## How to Submit

Choose one of the options below.

### Option 1 — GitHub

- Push your project to GitHub  
- Send us the repo link  
- If private, grant access to:  
  **[INSERT GITHUB USERNAME HERE]**

### Option 2 — ZIP File

- Zip the Xcode project folder  
- Email it to: **careers@ganance.com**

---

## Optional: Notes for Review

You may include a short section or comments explaining:

- Architectural choices  
- Anything you would improve with more time  
- How you might adapt this for real BLE communication  

This is optional.

---

## Thank You

We appreciate your time and interest in working with Ganance.  
We look forward to reviewing your work!

