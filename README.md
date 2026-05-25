expenses = []

while True:
    print("Expense Tracker")
    print("1. Add Expense")
    print("2. View Expenses")
    print("3. Total Expenses")
    print("4. Exit")

    choice = input("Enter your choice: ")

    if choice == "1":
        name = input("Enter expense name: ")
        amount = float(input("Enter amount: "))

        expenses.append([name, amount])

        print("Expense added!")

    elif choice == "2":
        print("Your Expenses:")

        for expense in expenses:
            print(expense[0], "-", expense[1])

    elif choice == "3":
        total = 0

        for expense in expenses:
            total = total + expense[1]

        print("Total Expenses:", total)

    elif choice == "4":
        print("Goodbye!")
        break

    else:
        print("Invalid choice")
