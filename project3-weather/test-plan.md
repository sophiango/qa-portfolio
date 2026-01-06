# Spoonacular Recipe Finder — Formal Test Plan

## 1. Overview

**Application Under Test (AUT):** OpenWeather Dashboard (https://openweathermap.org/find) is app that displays live weather data based on user input.

### Purpose of Testing

Testing focuses on search input, validation, API results, UI display, and error handling.

## 2. Objectives
- Verify search by city returns correct weather data  
- Verify invalid or empty inputs are handled gracefully  
- Verify UI correctly displays dynamic data (temperature, humidity, description)  
- Identify reproducible bugs

## 3. In-Scope
- City search functionality  
- Input validation  
- API results display  
- Units toggle (metric/imperial)

## 4. Out-of-Scope
- User accounts  
- Mobile responsiveness beyond basic scaling  
- Full API testing / performance testing

## 5. Environment
- Safari, MacOS Sequoia
- Live internet connection

## 6. Test Strategy
- Functional testing  
- Exploratory testing  
- Edge-case testing (invalid city names, special characters, network interruptions)