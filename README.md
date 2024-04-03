# airdrop
class Wallet:
    def __init__(self, address, balance):
        self.address = address
        self.balance = balance

def perform_airdrop(wallets, amount_per_wallet):
    for wallet in wallets:
        wallet.balance += amount_per_wallet

# Example usage
if __name__ == "__main__":
    # Creating wallet objects
    wallet1 = Wallet(address="0x123abc", balance=0)
    wallet2 = Wallet(address="0x456def", balance=0)
    wallet3 = Wallet(address="0x789ghi", balance=0)

    # List of wallets
    wallets = [wallet1, wallet2, wallet3]

    # Performing airdrop
    perform_airdrop(wallets, amount_per_wallet=100)  # Each wallet receives 100 tokens

    # Displaying updated wallet balances
    for wallet in wallets:
        print(f"Wallet Address: {wallet.address}, Balance: {wallet.balance}")
