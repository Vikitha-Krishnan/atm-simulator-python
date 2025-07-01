username = input("Enter username:")
password = input("Enter your ATM password: ")

if username == "admin" and password == "1234":
  print("Access granted. Welcome to the Python Bank.")
elif username == "admin":
  print("Incorrect password. Access denied.")
  exit()
elif password == "1234":
  print("User name not found Access denied.")
  exit()
else:
  print("Incorrect username and password. Access denied.")
  exit()

balance = 1000
while True:
  print("welcome to python bank")
  print("your current balance :₹ 1000")
  print("1.check balance")
  print("2.deposite money")
  print("3.withdraw money")
  print("4.Exit")
  choice = int(input("enter your choise :"))
  if choice == 1:
    print("your current balance :₹", balance)
    print("Thankyou for visiting python bank")
  elif choice == 2:
    amount = int(input("enter anount to deposite :"))
    balance = balance + amount
    print("your current balance:", balance)
    print("thanl you for visiting python bank")
  elif choice == 3:
    amount = int(input("enter withdraw amount :"))
    if amount > 1000:
      print("insufficient balance")
      print("Thank you for visiting python bank")
    else:
      balance -= amount
      print("withdraw successfull")
      print("your current balance:", balance)
      print("Thankyou for visiting python bank:")
  elif choice == 4:
    print("Exit")
    print("Thank you for visiting python bank")
  else:
    print("your choise is invalid please enter 1-4")

