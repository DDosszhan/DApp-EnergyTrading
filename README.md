# Clone the repository and navigate to the project directory
git clone https://github.com/your-username/energy-trading-platform.git
cd energy-trading-platform

# Install backend dependencies
echo "Installing backend dependencies..."
npm install

# Compile smart contracts
echo "Compiling smart contracts..."
npx hardhat compile

# Deploy smart contracts to specified network (e.g., localhost, ropsten, rinkeby)
echo "Deploying smart contracts..."
npx hardhat run scripts/deploy.js --network localhost

# Navigate to the client directory and install frontend dependencies
cd client
echo "Installing frontend dependencies..."
npm install

# Start the frontend development server
echo "Starting the frontend server..."
npm start
