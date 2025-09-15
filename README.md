# Community Safety Program Console
# by Your Community

def show_menu():
    print("\n=== COMMUNITY SAFETY PROGRAM ===")
    print("1. View Safety Tips")
    print("2. Report an Incident")
    print("3. Contact Emergency Numbers")
    print("4. Exit")
    choice = input("Please select an option (1-4): ")
    return choice

def safety_tips():
    print("\n--- SAFETY TIPS ---")
    print("1. Always wear safety gear when needed.")
    print("2. Keep emergency numbers handy.")
    print("3. Report unsafe conditions immediately.")
    print("4. Look out for your neighbors and community.")
    print("5. Stay calm and act quickly in emergencies.\n")

def report_incident():
    print("\n--- REPORT AN INCIDENT ---")
    incident = input("Please describe the incident: ")
    print("Thank you! Your report has been recorded:\n")
    print(f"-> {incident}\n")

def emergency_numbers():
    print("\n--- EMERGENCY NUMBERS ---")
    print("Police: 117")
    print("Fire Department: 160")
    print("Ambulance: 911")
    print("Community Hotline: 123-4567\n")

# Main Program Loop
while True:
    user_choice = show_menu()
    
    if user_choice == "1":
        safety_tips()
    elif user_choice == "2":
        report_incident()
    elif user_choice == "3":
        emergency_numbers()
    elif user_choice == "4":
        print("\nThank you for using the Community Safety Program. Stay safe!")
        break
    else:
        print("Invalid option, please try again.\n")
