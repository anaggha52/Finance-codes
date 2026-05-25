
principal = float(input("Principal amount: "))
rate = float(input("Annual interest rate (%): "))
times = int(input("Times compounded per year: "))
years = float(input("Number of years: "))

amount = principal * (1 + rate / 100 / times) ** (times * years)
interest = amount - principal

print("Final Amount: $", round(amount, 2))
print("Interest Earned: $", round(interest, 2))
