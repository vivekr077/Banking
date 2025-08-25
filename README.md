# Horizon - Banking Application

A modern banking application built with Next.js that allows users to connect multiple bank accounts, view transactions, and transfer funds between users.

## Tech Stack

- **Frontend**: Next.js 14, TypeScript, Tailwind CSS
- **Backend**: Appwrite (Database & Authentication)
- **Banking Integration**: Plaid API
- **Payment Processing**: Dwolla
- **UI Components**: ShadCN/UI
- **Charts**: Chart.js

## Features

- 🔐 Secure authentication with Appwrite
- 🏦 Connect multiple bank accounts via Plaid
- 💰 Real-time transaction monitoring
- 📊 Financial analytics and spending insights
- 💸 Peer-to-peer money transfers
- 📱 Responsive design for all devices
- 🔄 Real-time data synchronization

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- Appwrite account
- Plaid account
- Dwolla account

### Installation

1. Clone the repository
```bash
git clone <your-repo-url>
cd horizon
```

2. Install dependencies
```bash
npm install
```

3. Set up environment variables
Create a `.env` file in the root directory with the following variables:

```env
# Next.js
NEXT_PUBLIC_SITE_URL=

# Appwrite
NEXT_PUBLIC_APPWRITE_ENDPOINT=https://cloud.appwrite.io/v1
NEXT_PUBLIC_APPWRITE_PROJECT=
APPWRITE_DATABASE_ID=
APPWRITE_USER_COLLECTION_ID=
APPWRITE_BANK_COLLECTION_ID=
APPWRITE_TRANSACTION_COLLECTION_ID=
APPWRITE_SECRET=

# Plaid
PLAID_CLIENT_ID=
PLAID_SECRET=
PLAID_ENV=sandbox
PLAID_PRODUCTS=auth,transactions,identity
PLAID_COUNTRY_CODES=US,CA

# Dwolla
DWOLLA_KEY=
DWOLLA_SECRET=
DWOLLA_BASE_URL=https://api-sandbox.dwolla.com
DWOLLA_ENV=sandbox
```

4. Run the development server
```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the application.

## Project Structure

```
horizon/
├── app/                 # Next.js app directory
├── components/          # Reusable UI components
├── lib/                 # Utility functions and configurations
├── types/              # TypeScript type definitions
└── public/             # Static assets
```

## API Setup

### Appwrite Configuration
- Create a new project in Appwrite
- Set up collections for users, banks, and transactions
- Configure authentication settings

### Plaid Integration
- Sign up for a Plaid account
- Get your API credentials
- Configure webhook endpoints

### Dwolla Setup
- Create a Dwolla developer account
- Set up webhook endpoints for transfer notifications
- Configure customer verification settings

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is licensed under the MIT License.
