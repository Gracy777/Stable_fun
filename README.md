<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Stable.fun - Create Your Own Stablecoins</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.1/font/bootstrap-icons.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background: #f8fafc;
        }
        .gradient-bg {
            background: linear-gradient(135deg, #3b82f6 0%, #2563eb 100%);
        }
    </style>
</head>
<body>
    <nav class="gradient-bg text-white p-4">
        <div class="container mx-auto flex justify-between items-center">
            <h1 class="text-2xl font-bold">stable.fun</h1>
            <button id="connectWallet" class="bg-white text-blue-600 px-4 py-2 rounded-lg font-medium hover:bg-blue-50 transition-colors">
                Connect Wallet
            </button>
        </div>
    </nav>

    <main class="container mx-auto px-4 py-8">
        <!-- Create Stablecoin Section -->
        <div class="max-w-2xl mx-auto bg-white rounded-xl shadow-lg p-6 mb-8">
            <h2 class="text-2xl font-bold mb-6">Create Your Stablecoin</h2>
            <form id="createStablecoinForm" class="space-y-4">
                <div>
                    <label class="block text-sm font-medium mb-1">Token Name</label>
                    <input type="text" class="w-full p-2 border rounded-lg" placeholder="e.g., My Stable USD" required>
                </div>
                <div>
                    <label class="block text-sm font-medium mb-1">Token Symbol</label>
                    <input type="text" class="w-full p-2 border rounded-lg" placeholder="e.g., mUSD" required>
                </div>
                <div>
                    <label class="block text-sm font-medium mb-1">Target Fiat Currency</label>
                    <select class="w-full p-2 border rounded-lg" required>
                        <option value="USD">USD</option>
                        <option value="EUR">EUR</option>
                        <option value="GBP">GBP</option>
                        <option value="JPY">JPY</option>
                    </select>
                </div>
                <div>
                    <label class="block text-sm font-medium mb-1">Token Icon</label>
                    <input type="file" accept="image/*" class="w-full p-2 border rounded-lg" required>
                </div>
                <button type="submit" class="w-full gradient-bg text-white py-3 rounded-lg font-medium hover:opacity-90 transition-opacity">
                    Create Stablecoin
                </button>
            </form>
        </div>

        <!-- Existing Stablecoins Section -->
        <div class="max-w-4xl mx-auto">
            <h2 class="text-2xl font-bold mb-6">Your Stablecoins</h2>
            <div class="grid md:grid-cols-2 gap-4">
                <!-- Sample Stablecoin Card -->
                <div class="bg-white rounded-xl shadow-lg p-6">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 bg-blue-100 rounded-full flex items-center justify-center">
                            <i class="bi bi-coin text-2xl text-blue-600"></i>
                        </div>
                        <div class="ml-4">
                            <h3 class="font-bold">Demo Stable USD</h3>
                            <p class="text-sm text-gray-600">dUSD</p>
                        </div>
                    </div>
                    <div class="space-y-2">
                        <p class="text-sm"><span class="font-medium">Target:</span> USD</p>
                        <p class="text-sm"><span class="font-medium">Supply:</span> 1,000,000</p>
                        <div class="flex space-x-2">
                            <button class="flex-1 bg-blue-600 text-white py-2 rounded-lg hover:bg-blue-700 transition-colors">
                                Mint
                            </button>
                            <button class="flex-1 border border-blue-600 text-blue-600 py-2 rounded-lg hover:bg-blue-50 transition-colors">
                                Redeem
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>

    <script>
        // Simulate wallet connection
        document.getElementById('connectWallet').addEventListener('click', () => {
            alert('Wallet connection simulation. In production, this would connect to Phantom or other Solana wallets.');
        });

        // Form submission handler
        document.getElementById('createStablecoinForm').addEventListener('submit', (e) => {
            e.preventDefault();
            alert('Stablecoin creation simulation. In production, this would interact with the Solana blockchain.');
        });

        // Mint and Redeem functionality would be implemented here
        // These would interact with the Solana program using web3.js
    </script>
</body>
</html># Stable_fun
