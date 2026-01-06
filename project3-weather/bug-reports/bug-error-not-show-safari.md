# 🐞 Weather Page Bug Report — Error not shown

**Bug ID:** BUG-WEATHER-001  
**Severity:** S2 — Major  
**Priority:** P1  
**Status:** Open  
**Environment:** Safari / macOS Sequoia
**Build:** Weather App (https://openweathermap.org/find)

## Description
When click search without input or when searching with invalid city name, no error shown.

## Steps to Reproduce
1. Navigate to [https://openweathermap.org/find](https://openweathermap.org/find)  
2. click search without input
3. Click **Search**  
4. No error show
5. Type random "dskcndc"
6. Click **Search**
7. No error show

## Expected Result
Detailed error should show so user knows what to do next

## Actual Result
Page just flash with no error shown

## Impact
- Users do not know what happening

## Suggested Fix
- Add error indicator and error message
