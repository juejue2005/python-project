#practice
total_amount=0
print('Enter l for login to account ')
position=input('Enter :') #ask user to login (that is first reqriment that every user have to do)
position=position.lower()# covert input to lowercase
if position =='l':
        name=input('Enter your name: ')
        allow_passwords = [111111, 222222, 333333, 444444, 555555]  # Allowed passwords
        while True:
            password = input("Enter your password (must be 6 digits): ")

            if password.isdigit():  # Make sure it's a number
                if len(password) == 6:  # Check for exact 6 digits
                    if int(password) in allow_passwords:  # Check if password is valid
                        print(" You are accepted!\nWelcome to PureSkinMart store.")
                        break  # Exit loop once accepted
                    else:
                        print(" Invalid password. Please try again.")
                else:
                    print(" Your password must be exactly 6 digits.")
            else:
                print(" Please enter only numbers.")
#main loop
while True:
    #show main menu
    print("Enter b for personal bank\n")
    print('Enter s for go to store\n')
    print('Enter p for go to my  personal\'s profile\n')
    print('Enter q for quit\n')
    position=input('Enter your perfence :')
    position=position.lower()

    if position=='b':
        user_name=input('Enter your name\n')
        valid_passwords = [111111, 222222, 333333, 444444, 555555]  # Valid passwords
        
        try:
                password = int(input('Enter your account password:\n'))  # Try converting input to integer
                if password in valid_passwords:  # Check if password is valid(try except)
                    print('Welcome to PureSkinMart personal bank')
                else:
                    print('Incorrect password. Please try again.')
        except ValueError:#catch non-numeric input
                print('Invalid input! Password must contain only numbers. \n your actual password from login account.') 
            

        while True:#bank loop
                print('Enter d for deposit\n')
                print('Enter w for withdraw\n')
                print('Enter c for check total amount\n')
                print('Enter q for quit\n')
                            
                user_option=input('Enter your option :')
                if user_option=='d':
                    deposit=int(input('Enter deposit amount:'))
                    if deposit<=0:
                          print('Invalid amount')
                    else:
                        total_amount += deposit
                        print('Your deposit amount is ', deposit, '\nYour total amount is ', total_amount)
                elif user_option=='w':
                        withdraw=int(input('Enter your withdraw amount :'))
                        if withdraw<=0:
                            print('Invalid amount.')
                        elif withdraw>total_amount:
                            print('Insufficient amount')
                        elif withdraw>0 and withdraw<=total_amount:
                            total_amount-=withdraw
                            print('You withdrawed',withdraw,'your remaining amount is ',total_amount)
                        else:
                            print('Invalid Option')

                elif user_option=='c':
                        print('User name :',user_name,'\nUser passwordb :',password,'\nTotal amount:',total_amount)
                        print('if you woul love to set up to use your bank card trougth payment with our personal bank\n please content with bank for more information ')
                elif user_option=='q':
                        print('Thanks for choosing our Bank')
                        break
                else:
                    print('Invalid')
        break            
        
              
    elif position=='s':
        while True:
            print('enter p for prouct list')# go for as a list in both proucts
            
            user_preference=input('enter p for to see the avaliable and restock product list:')
            if user_preference=='p':
                product_list=['innisfree','\nlaneige','\nsome by mi','\nnature repunic','\nmissha','\ncorsrx']
                print('available products:')
                for product in product_list:
                    print(product)
            else:user_preference=='r'
            print('restock product list are:')
            restock_list= [ #list 
                {"name": 'Benton', "category": 'skin care'},
                {"name": 'lancome' , "category" : 'lip care'},
                {"name" : 'dior' , "category" : 'lip oil'},
                {"name" : 'skin 1004' , "category" : 'serum & sun cream'}

            ]
            for product1 in restock_list:
                print(f"- {product1['name'].title()} ({product1['category']})")
            break
    elif position=='p':
        while True:#premium loop
            print('enter u for upgrade to premium\n')
            print('enter c for check account\n')
            print('enter r for reward code\n')
            print('enter q for quit\n')
            decision=input('enter your preference:\n')
            if decision=='u':# bank payment for upgrade premium
                print("(Note \n Upgrade to Premium and enjoy 5% off every purchase, unlock exclusive discounts, \n earn a personal reward CODE to share — get 2% every time someone uses your CODE! " )
                preference=input('Enter yes or no :')
                if preference=='yes':
                        print(" Welcome to the Premium Upgrade Portal")

                        user_name = input("Enter your full name: ")
                        email = input("Enter your email address: ")

                        print("\nChoose a payment method:")
                        print("1.personal Bank Transfer")
                        print("2. Credit/Debit Card")
                        print("3. Mobile Payment (e.g., Wave, KBZPay)")
                        method = input("Enter the number of your payment method: ")

                        if method == "1":
                            bank_number = input("Enter your bank account number: ")
                            bank_name = input("Enter your bank name: ")
                            print(f"\nThank you, {user_name}. We'll process your upgrade via {bank_name} account {bank_number}.")

                        elif method == "2":
                            card_number = input("Enter your card number (xxxx-xxxx-xxxx-xxxx): ")
                            expiry = input("Enter card expiry date (MM/YY): ")
                            cvv = input("Enter CVV (3 digits): ")
                            print(f"\nThank you, {user_name}. Your card ending in {card_number[-4:]} will be used for the upgrade.")

                        elif method == "3":
                            mobile_id = input("Enter your mobile payment ID or phone number: ")
                            app_name = input("Enter the app name (e.g., WavePay, KBZPay): ")
                            print(f"\nThanks, {user_name}. We’ll send a request via {app_name} to {mobile_id}.")

                        else:
                            print(" Invalid payment method selected.")

                        print("\n Premium upgrade request received. We’ll verify your payment shortly!")

                else: decision=='no'
                print('thank you for taking time')
            elif decision=='c':#check the account
                 print('User name :',user_name,'\nUser passwordb :',password,'\nTotal amount:',total_amount)
            elif decision=='r':#reward code 
                print('Enter your name to get a reward code:')
                user_name = input()

                import random#to generate number for reward code
                user_name = input("Enter your name to get a reward code: ")
                generate_code = lambda name: f"{name.upper()}{random.randint(1000, 9999)}"
            
                reward_code = generate_code(user_name)
                                

                print("Your reward code is:", reward_code)
                break
            else:decision=='q'
            print('thank you for choosing us')
    else:position=='q'
    print('thank you for shoping with us')
    break
