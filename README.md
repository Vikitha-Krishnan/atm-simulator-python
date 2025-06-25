# app.py
balance = 1000

print ("welcome to python bank")
print ("your current balance :₹ 1000")
print ("1.check balance")
print ("2.deposite money")
print ("3.withdraw money")
print ("4.Exit")
choise = int(input("enter your choise :"))
if choise == 1:
  print("your current balance :₹", balance)
  print("Thankyou for visiting python bank")
elif choise == 2:
  amount = int(input("enter anount to deposite :"))
  balance = balance + amount
  print("your current balance:", balance)
  print("thanl you for visiting python bank")
elif choise == 3:
  amount =  int(input("enter withdraw amount :"))
  if amount>1000:  
    print("insufficient balance")
    print("thank you for visiting python bank")
  else:
    balance-=amount
    print("withdraw successfull")
    print("your current balance:", balance)
    print("thankyou for visiting python bank:")
elif choise==4:
  print("Exit")
  print("thank you for visiting python bank")
else:
  print("your choise is invalid please enter 1-4")
