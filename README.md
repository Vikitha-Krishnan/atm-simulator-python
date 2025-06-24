# app.py
balance = 1000

print("Welcome to Python Bank")
print("Your current balance: ₹1000")
print("1. Check Balance")
print("2. Deposit Money")
print("3. Withdraw Money")
print("4. Exit")

choise = int(input("Enter your choice: "))

if choise == 1:
    print("Your current balance: ₹", balance)
    print("Thank you for visiting Python Bank")

elif choise == 2:
    amount = int(input("Enter amount to deposit: "))
    balance += amount
    print("Your new balance: ₹", balance)
    print("Thank you for visiting Python Bank")

elif choise == 3:
    amount = int(input("Enter amount to withdraw: "))
    if amount > balance:
        print("Insufficient balance ❌")
    else:
        balance -= amount
        print("Withdrawal successful!")
        print("Your current balance: ₹", balance)
    print("Thank you for visiting Python Bank")

else:
    print("Exiting...")
    print("Thank you for visiting Python Bank")

