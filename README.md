# PortfolioPro — Stock Trading & Portfolio Management

A B.Tech 3rd-year full-stack project for the Banking & Finance domain.

## Stack
- Frontend: Angular 20 + TypeScript
- Backend: Java 21 + Spring Boot 3.5
- Database: MySQL 8.4
- Auth: Spring Security + JWT
- Trading: simulated/paper trading

## Features in this MVP
- Registration/login with JWT authentication
- ₹1,00,000 starting virtual cash per user
- Stock search and seeded Indian-market sample stocks
- Simulated BUY/SELL orders
- Holdings and average-cost calculation
- Portfolio value and P&L
- Transaction history
- Watchlist-ready database model
- Technical/fundamental analysis dashboard scaffold
- Responsive dark finance dashboard

## Run
### 1. Start MySQL
From the project root:
```bash
docker compose up -d
```

### 2. Start backend
Install Maven 3.9+ and run:
```bash
cd backend
mvn spring-boot:run
```
Backend: http://localhost:8080

### 3. Start frontend
```bash
cd frontend
npm install
npm start
```
Frontend: http://localhost:4200

## Notes
The current implementation intentionally uses seeded market quotes so the application works without an API key. For a production-style version, replace the seeded StockService data with an external market-data adapter and add historical price storage. The analysis page labels illustrative metrics where live fundamentals/indicators are not connected.

This is an academic paper-trading application and does not place real brokerage orders or provide guaranteed investment advice.
