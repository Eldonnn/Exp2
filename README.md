def income_tax(annual_income):
    if annual_income <= 250000:
    tax = 0
  elif annual_income <= 400000:
    tax = 15/100 * (annual_income - 250000)
  elif annual_income <= 800000:
    tax = 22500 + 20/100 * (annual_income - 400000)
  elif annual_income <= 2000000:
    tax = 102500 + 25/100 * (annual_income - 800000)
  elif annual_income <= 8000000:
    tax = 402000 + 30/100 * (annual_income - 2000000)
  else:
    tax = 2202500 + 35/100 * (annual_income - 8000000)

monthly_tax = tax / 12
return tax, monthly tax

annual income = float(input("Enter you annual income:   "))
tax, montlhy_tax = income_tax(annual_income)

print("Annual Tax:", tax)
print("Monthtly tax:", monthly_tax)
print("\nThank you for using this Program!\n")