# React Native with Maestro Testing

## Introduction

This repository contains a React Native mobile application with integrated Maestro end-to-end testing. The project demonstrates how to implement reliable UI testing workflows for cross-platform mobile apps using Maestro's declarative testing approach.

Key features:

- Production-ready React Native (v0.72+) base
- Pre-configured Maestro test suite
- Sample test flows for common mobile patterns

## Maestro with React Native

Maestro is the next-generation mobile UI testing framework that offers:

**Why Maestro for React Native?**
✔ Flakiness-resistant tests  
✔ No need for explicit test IDs (works with text visibility)  
✔ YAML-based test definitions  
✔ Cross-platform (Android & iOS) testing  
✔ Rapid test execution

**Key Integration Points:**

1. Works with React Native's rendering layer
2. Supports both JavaScript and native components
3. Handles React Navigation transitions
4. Compatible with state management solutions (Redux, MobX)

## Setup Guide

### 1. System Requirements

- Node.js v16+
- Java JDK 11 (for Android)
- Xcode 14+ (for iOS)
- Ruby 2.6+ (for Maestro)

### 2. Project Installation

```bash
# Clone repository
git clone https://github.com/your-org/react-native-maestro-demo.git
cd react-native-maestro-demo

# Install dependencies
npm install

# iOS specific setup
cd ios && pod install && cd ..
```

# Install Maestro CLI

curl -Ls "https://get.maestro.mobile.dev" | bash

# Verify installation

maestro --version

# Should output version 1.30+
