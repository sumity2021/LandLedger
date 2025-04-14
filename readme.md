

# LandLedger - Decentralized Land Registry

LandLedger is a decentralized land registry system built using **Solidity** (for smart contracts), **Truffle** (for smart contract management), and **React** (for the front-end). This system allows users to register, view, and manage land ownership records on the blockchain.

## Features

- **Smart Contracts**: Manages land registration and ownership using Ethereum blockchain.
- **User Interface**: A React-based frontend to interact with the blockchain, view land details, and register land.
- **Admin Interface**: Admin functionalities to manage users and land records.
- **Smart Contract Tests**: Automated tests to ensure the integrity of smart contracts.

## Project Structure

```
LandLedger/
│
├── contracts/                 # Solidity smart contracts
│   └── Migrations.sol         # Migration contract
│   └── Registry.sol           # Main contract for land registry
│
├── front-end/                 # React frontend
│   ├── public/                # Public assets
│   │   └── favicon.ico        # Favicon file
│   │   └── index.html         # Main HTML file
│   │   └── manifest.json      # Web app manifest
│   │   └── robots.txt         # Robots file
│   │
│   ├── src/                   # React source code
│   │   ├── components/        # React components
│   │   │   ├── Admin.jsx
│   │   │   ├── DisplayExploreResult.jsx
│   │   │   ├── DisplayLandDetails.jsx
│   │   │   ├── DisplayRequested.jsx
│   │   │   ├── DisplayRequests.jsx
│   │   │   ├── Explore.jsx
│   │   │   ├── Navbar.jsx
│   │   │   ├── Profile.jsx
│   │   │   ├── Property.jsx
│   │   │   ├── RegisterLand.jsx
│   │   │   ├── Requested.jsx
│   │   │   ├── Requests.jsx
│   │   │   ├── SuperAdmin.jsx
│   │   │   ├── UserProfile.jsx
│   │   ├── css/               # CSS files for styling
│   │   │   ├── Explore.css
│   │   │   ├── Navbar.css
│   │   │   ├── Profile.css
│   │   │   ├── RegisterLand.css
│   │   │   ├── SuperAdmin.css
│   │   ├── images/            # Image assets
│   │   │   └── emblem.svg
│   │   ├── index.css          # Global CSS
│   │   ├── index.js           # React entry point
│   │   ├── App.css            # Main app CSS
│   │   ├── App.js             # Main React component
│   │   ├── App.test.js        # Tests for React app
│   │   ├── reportWebVitals.js # Web vitals tracking
│   │   ├── setupTests.js      # Jest setup for tests
│   │   ├── utils/             # Utility functions
│   │   │   └── loadContract.js
│   ├── package.json           # Frontend dependencies
│
├── migrations/                # Truffle deployment scripts
│   ├── 1_initial_migration.js
│   ├── 2_registry.js
│
├── package.json               # Backend dependencies
├── readme.md                  # Project documentation
└── truffle-config.js          # Truffle configuration file
```

## Installation

### 1. Clone the Repository

Clone the repository to your local machine:

```bash
git clone https://github.com/sumity2021/LandLedger.git
cd LandLedger
```

### 2. Install Backend (Solidity Contracts)

Navigate to the backend folder and install the dependencies:

```bash
npm install
```

### 3. Install Frontend (React)

Navigate to the frontend folder and install the dependencies:

```bash
cd front-end
npm install
```

### 4. Configure the `.env` File

Create a `.env` file in the `front-end` directory and add your environment variables (e.g., contract address, network ID, etc.):

```bash
REACT_APP_CONTRACT_ADDRESS=0xYourContractAddressHere
REACT_APP_NETWORK_ID=5777
```

> Make sure to **never commit** this file to version control. It should be in `.gitignore`.

## Running the Application

### 1. Start the Smart Contracts

In the root directory, run:

```bash
truffle migrate --network development
```

This will deploy the smart contracts to the local Ethereum blockchain (make sure you have **Ganache** running).

### 2. Run the React Frontend

Navigate to the `front-end` directory and run:

```bash
npm start
```

This will start the React development server and open the app in your browser.

## Testing

### 1. Smart Contract Tests

Run the smart contract tests using:

```bash
truffle test
```

### 2. Frontend Tests

To test the React components, run:

```bash
npm test
```

## Contributing

Feel free to fork the repository and submit pull requests. Ensure to follow the code style and write tests for any new features.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

---

This **README.md** includes sections on installation, running the app, testing, contributing, and license, along with the structure you provided. Let me know if you'd like to customize or add any more details!
