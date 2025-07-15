# Top Aus ETFs Dashboard

A React dashboard for visualising the top 10 performing Australian ETFs by time period, using real data from the ASX Investment Products monthly report.

## Features
- View top 10 ETFs by 1M, 1Y, or 5Y performance

## Project Structure
- **etf-dashboard-demo/**: React frontend (this project) - WORK IN PROGRESS
- **server/**: Node.js/Express backend for fetching and parsing ASX Excel data - WORK IN PROGRESS

## How It Works
- The backend downloads and parses the latest ASX ETF Excel file, normalizes the data, and exposes it via a REST API.
- The frontend fetches this data and displays the top 10 ETFs for the selected time period.

## Getting Started

### Prerequisites
- Node.js (v16+ recommended)
- npm

### 1. Start the Backend
```
cd ../server
npm install
npm run build
npm start
```
- The backend will run on [http://localhost:3001](http://localhost:3001) by default.

### 2. Start the Frontend
```
cd etf-dashboard-demo
npm install
npm start
```
- The frontend will run on [http://localhost:3000](http://localhost:3000)

## Customization
- To change the default time period, edit `selectedPeriod` in `src/App.tsx`.
- To update the data source or mapping, see `server/src/services/etfService.ts`.

## Source & Disclaimer
- **Source:** ASX Investment products monthly report
- **Disclaimer:** This dashboard is provided for informational purposes only and does not constitute financial, investment, tax, or other professional advice. Past performance is not indicative of future results. You should conduct your own research and/or consult a qualified professional before making any investment decisions.
