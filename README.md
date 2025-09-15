# Program Safety Rules Console
# CVN Hub Safety Program
# Version 1.0 - 15 Sept 2025

import sys

def show_menu():
    print("\n=== CVN PROGRAM SAFETY RULES ===")
    print("1. Code of Conduct")
    print("2. Security Rules")
    print("3. Contribution Guidelines")
    print("4. Reporting Procedure")
    print("5. Enforcement & Consequences")
    print("6. Incident Response")
    print("7. Exit")

def code_of_conduct():
    print("\n--- Code of Conduct ---")
    print("1. Show respect and professionalism.")
    print("2. No bullying or doxxing.")
    print("3. Avoid hate speech or offensive content.")
    print("4. Protect children and avoid harmful materials.")

def security_rules():
    print("\n--- Security Rules ---")
    print("1. Do not commit secrets or credentials.")
    print("2. Report vulnerabilities privately.")
    print("3. Regularly update dependencies.")
    print("4. Limit access permissions to trusted maintainers.")
    print("5. All pull requests must go through code review.")

def contribution_guidelines():
    print("\n--- Contribution Guidelines ---")
    print("1. Use issue and PR templates.")
    print("2. Protect the main branch.")
    print("3. Use clear commit messages (e.g., fix(auth): handle token expiry).")
    print("4. All PRs must include tests and CI checks.")

def reporting_procedure():
    print("\n--- Reporting Procedure ---")
    print("1. Non-security issues: open an issue using the template.")
    print("2. Security issues: report privately to security@cvnhub.link.")
    print("3. Abuse or harassment: report to repo admin or authorities.")

def enforcement():
    print("\n--- Enforcement & Consequences ---")
    print("1. Warning for minor violations.")
    print("2. Temporary restriction for repeated or serious violations.")
    print("3. Permanent ban and report to GitHub if necessary.")

def incident_response():
    print("\n--- Incident Response ---")
    print("1. Identification and logging.")
    print("2. Containment (disable keys, revoke tokens, rollback if needed).")
    print("3. Eradication & Recovery.")
    print("4. Post-mortem review and improvements.")

while True:
    show_menu()
    choice = input("\nChoose an option (1-7): ")
    if choice == "1":
        code_of_conduct()
    elif choice == "2":
        security_rules()
    elif choice == "3":
        contribution_guidelines()
    elif choice == "4":
        reporting_procedure()
    elif choice == "5":
        enforcement()
    elif choice == "6":
        incident_response()
    elif choice == "7":
        print("\nThank you for using the CVN Safety Program Console!")
        sys.exit()
    else:
        print("\nInvalid input. Please try again.")
