# BusSwap — Web Prototype v1

BusSwap is an early-stage concept for helping passengers who can no longer travel explore an operator-approved way to release or rebook a bus seat, while helping another passenger find an available seat.

## Current status

This repository contains a **front-end demonstration only**. It does not connect to bus operators, ticketing platforms, payment gateways, or live inventory. All sample journeys and requests are demo data stored in the browser.

**Important policy and legal constraint:** A bus ticket is not automatically transferable. Some operators and booking platforms prohibit ticket transfers or resale. BusSwap must never facilitate a transfer unless the relevant operator and booking platform explicitly permit the exact process. The current prototype therefore treats a submitted listing as a request for manual/operator review. It does not confirm a transfer, issue a ticket, collect money, or guarantee a refund.

## Prototype features

- Passenger dashboard with sample upcoming trips
- Search and filter sample bus journeys
- Create a seat-release / rebooking request
- Validation for required details, departure deadline, and requested price
- Requested price cannot exceed 90% of the entered original ticket price (prototype concept rule)
- Operator-approval status before any transfer can be considered
- Local browser storage for demo requests
- Responsive layout for desktop and mobile

## Run locally

No build tools or dependencies are required.

1. Download or clone this repository.
2. Open `index.html` in a browser, or use the VS Code **Live Server** extension.
3. Use the sample data to explore the dashboard and submit a demo request.

## Project structure

```
Bus_swap_prototype/
├── index.html
├── styles.css
├── app.js
└── README.md
```

## Product rules represented in this demo

1. The operator's written policy takes priority over BusSwap's proposed rules.
2. A request remains pending until an operator explicitly confirms an allowed process.
3. The requested resale amount is capped at 90% of the original fare as a concept rule; this does not override operator policy or applicable law.
4. Requests must be submitted before the configured departure cut-off.
5. No payment, ticket transfer, cancellation, or booking is performed by this demo.

## Not included yet

- Authentication and user accounts
- Backend API and database
- Operator dashboard or verified operator integrations
- Real-time bus inventory
- Payment/refund processing
- Identity, booking, and fraud verification
- Production security, privacy, and compliance review

## Next development milestone

Validate the operating model with bus operators and booking platforms first. Only after written permission and a compliant transfer/rebooking process are established should the backend, operator approval workflow, and payment integrations be developed.

## License

No license has been granted yet. All rights reserved by the repository owner unless a license is added.
