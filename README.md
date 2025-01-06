# WidgetBonus
A program that assigns a $200 bonus to every employee that sells 3000 widgets. Employees that do not make the 3000 widget mark do not earn a bonus.
def calculate_bonus(widgets_sold):
  """
  Calculates the bonus for an employee based on widget sales.

  Args:
    widgets_sold: The number of widgets sold by the employee.

  Returns:
    The bonus amount in dollars.
  """
  num_bonus = widgets_sold // 3000  # Calculate the number of bonuses earned
  return num_bonus * 200

# Employee sales data
employee_sales = {
    "Jason": 4500,
    "Casey": 1200,
    "Michal": 8000,
    "Eleanor": 6000
}

# Calculate and print bonuses for each employee
for employee, sales in employee_sales.items():
  bonus = calculate_bonus(sales)
  print(f"{employee} earned a bonus of ${bonus:.2f}")
