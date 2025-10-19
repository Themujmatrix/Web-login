# Web-login
print("\n\t<<Website Login>>\n")
users = {"adam":"85672346",
       "eric":"12348567",
       "william":"15346391",
       "jessica":"18567345",
       "matt":"23856756"}
loged_in = False
while loged_in == False:
    answer = input("Are you a registered user? (Yes/No):").strip().lower()
    if answer == 'no':
        while True:
            new_user = input("Enter a username:").strip().lower()
            if new_user not in users.keys():
                while True:
                    users[new_user] = input("Enter a password:")
                    if len(users[new_user]) < 8:
                        print("Password must be at least 8 characters long.")
                    else:
                        print("Password created successfully.")
                        break
                print(f"Finished signing up your account {new_user.title()}.")
                break
            else:   
                print("Username already taken, choose another.")
    print("\n\tLogin Here\n")
    login_user = input("Enter your username:").strip().lower()
    if login_user in users.keys():
        while True:
            login_password = input("Enter your password:")
            if login_password == users[login_user]:
                print("Login successful.")
                loged_in = True
                break
            else:
                print("Incorrect password.")
    else:
        print("You are not a registered user.")
        print("Sign up first.")
