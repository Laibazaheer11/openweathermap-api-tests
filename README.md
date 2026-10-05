# OpenWeatherMap API - Automated Testing

Automated testing of OpenWeatherMap API using Postman and GitHub Actions CI/CD pipeline.

## 🚀 CI/CD Pipeline
[![Weather API Tests](https://github.com/Laibazaheer11/openweathermap-api-tests/actions/workflows/test.yml/badge.svg)](https://github.com/Laibazaheer11/openweathermap-api-tests/actions)

All tests are automatically executed on every push via GitHub Actions.

## 📋 Test Coverage
- Current Weather Data endpoint validation
- Status code assertion (200 OK)
- Response time validation (< 1000ms)
- JSON schema and data structure validation

## 🛠️ Tools Used
- Postman - API collection & test scripting
- Newman - CLI for running Postman collections
- GitHub Actions - Continuous Integration
- OpenWeatherMap API

## ▶️ Run Locally
```bash
npm install -g newman
newman run OpenWeather.json --env-var "api_key=YOUR_KEY" --env-var "base_url=https://api.openweathermap.org" --env-var "city=Ankara"
