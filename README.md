# ganance-ios-assessment
Short assessment for Ganance iOS Development Candidates
Ganance iOS Developer Assessment

Estimated Time: 1 hour
Tech Requirements: Swift, SwiftUI, Combine or async/await
Submission Format: GitHub repo link or zipped Xcode project

Overview

This assessment is designed to simulate a lightweight version of the work you would do at Ganance. Since our product involves connecting a mobile app to a hardware device over Bluetooth/BLE, we want to see how you structure code, handle async flows, and manage app state.

You will not need to implement real Bluetooth functionality. Instead, you will simulate a device connection and data sync process using delays and mock data.

The focus is on clarity, architecture, and your ability to build a simple but realistic mobile flow.

Your Task

Build a small SwiftUI app that does the following:

1. Connect to a Simulated Device

Create a service that simulates connecting to a wearable device. Requirements:

The “connection” should take 2–3 seconds using Task.sleep or any async method.

20% of the time, the connection should fail with an error.

Expose this as an async method or a Combine publisher.

2. Fetch Mock Health Data

Once "connected," fetch a mock payload that includes:

{
  "steps": 7342,
  "heartRate": 72,
  "sleepHours": 7.3
}


Use any model structure you’d like.

3. Display the Results in SwiftUI

Create a simple UI that shows:

A “Connect” button

A loading state while connecting

A success state with the returned data

An error state with a retry button

4. Architecture Requirements

Use MVVM or another pattern you’re comfortable with

Separate the logic into a service layer and a view model

Use either Combine or async/await

5. Bonus (Optional, Only if Time Permits)

These are not required but will help us understand your depth:

Cache the most recent successful data sync in UserDefaults

Add a timestamp to the UI showing when the data was last synced

Add very lightweight unit test coverage for the service or view model

What We’re Looking For

We are evaluating:

Clear, maintainable architecture

Clean, readable code

Thoughtful handling of async workflows

Proper management of loading, error, and success states

Ability to simulate real-world device connectivity challenges

How you communicate in code comments or a brief README section

We are not evaluating:

Pixel-perfect design

Real BLE integration

Edge-case perfection

Large amounts of boilerplate or over-engineering

How to Submit

Please provide one of the following:

Option 1 — GitHub

Push your project to GitHub (public or private)

Send us the link

If private, grant access to:
[INSERT GITHUB USERNAME HERE]

Option 2 — ZIP File

Zip the Xcode project folder

Email it to:
careers@ganance.com

Optional: Notes for Review

If you would like, include a short section explaining:

Architectural choices

Anything you would improve with more time

How you would adapt this code for real BLE communication

This is optional but appreciated.

Thank You

We appreciate the time you’re investing in this assessment.
We look forward to reviewing your work!
