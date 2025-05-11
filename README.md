
![Write your topic or idea](https://github.com/user-attachments/assets/3bf861d4-13be-4d88-a5dd-0b1da0c38e41)

# 📱 React Native with Maestro Testing

## 🚀 Introduction

This repository contains a React Native mobile application with integrated Maestro end-to-end testing. The project demonstrates how to implement reliable UI testing workflows for cross-platform mobile apps using Maestro's declarative testing approach.

✨ **Key Features:**

- ⚛️ Production-ready React Native (v0.72+) base
- 🧪 Pre-configured Maestro test suite
- 📲 Sample test flows for common mobile patterns

---
🎥 Demo Video


https://github.com/user-attachments/assets/5f9cce96-9a38-4a4b-92a5-b2d33ad946e6


```bash
# Example Login Page
appId: com.awesomeproject # Your application's package name
---
# Launch the application and wait for initial load
- launchApp
- waitForAnimationToEnd # Ensure all startup animations complete

# LOGIN SECTION
# ------------------------------
# Enter username in the Username field
- tapOn:
    id: 'Username' # Targets element with ID 'Username'
- inputText: 'your_username' # Inputs test username

# Enter password in the Password field
- tapOn:
    id: 'Password' # Targets element with ID 'Password'
- inputText: 'your_password_here' # Inputs test password

# LOGIN ACTION
# ------------------------------
- tapOn:
    id: 'Login'


```

## 🧭 Maestro with React Native

Maestro is the next-generation mobile UI testing framework that offers:

### ✅ Why Maestro for React Native?

- 🧱 Flakiness-resistant tests
- 👁️ No need for explicit test IDs (works with text visibility)
- 📄 YAML-based test definitions
- 📱 Cross-platform (Android & iOS) testing
- ⚡ Rapid test execution

### 🔗 Key Integration Points:

1. 🖼️ Works with React Native's rendering layer
2. 🔌 Supports both JavaScript and native components
3. 🔄 Handles React Navigation transitions
4. 💾 Compatible with state management solutions (Redux, MobX)

---

## 🛠️ Setup Guide

### 1. 📋 System Requirements

- 🟢 Node.js v16+
- ☕ Java JDK 11 (for Android)
- 🍎 Xcode 14+ (for iOS)
- 💎 Ruby 2.6+ (for Maestro)

### 2. 📦 Project Installation

```bash
# Clone repository
git clone https://github.com/your-org/react-native-maestro-demo.git
cd react-native-maestro-demo

# Install dependencies
npm install

# iOS specific setup
cd ios && pod install && cd ..
```

# 📥 Install Maestro CLI

curl -Ls "https://get.maestro.mobile.dev" | bash

# ✅ Verify Installation

maestro --version

## Should output version 1.30+

## 📁 Project Structure

```bash

├── android/                  # Android native code
├── ios/                      # iOS native code
├── e2e/                      # Maestro test suites
│   └── artifacts/            # Test outputs
├── src/                      # React Native source
```

## ▶️ Running Tests

### 🧪 Basic Commands

```bash
# Run all test suites
maestro test e2e/

# Run a specific test file
maestro test e2e/login-flow.yaml

# Run tests on specific device
maestro test --device=iPhone_15 e2e/
```

### 🛠️ Advanced Options

```bash
# Run with verbose output
maestro --verbose test e2e/

# Run tests with tags
maestro test --tags=critical e2e/

# Generate JUnit report
maestro test --format=junit e2e/ > e2e/artifacts/report.xml
```

## 🤔 How to contribute

Have an idea? Found a bug? Please raise to [ISSUES](https://github.com/avisek123/helper-box/issues).
Contributions are welcome and are greatly appreciated! Every little bit helps, and credit will always be given.

## 👨‍💻 About Me

![WhatsApp Image 2024-09-19 at 7 49 24 PM](https://github.com/user-attachments/assets/a6204283-d754-44c8-a1c7-2cb0dffcd316)
