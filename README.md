# week-3-python-
assignment
QUESTION 1
def calculate_discount(price, discount_percent):
    # Apply discount only if it's 20% or more
    if discount_percent >= 20:
        discount_amount = (discount_percent / 100) * price
        final_price = price - discount_amount
        return final_price
    else:
        return price
        
QUESTION 2
# Prompt the user for input
try:
    original_price = float(input("Enter the original price of the item: "))
    discount = float(input("Enter the discount percentage: "))

    final_price = calculate_discount(original_price, discount)

    if discount >= 20:
        print(f"Discount applied. Final price: ${final_price:.2f}")
    else:
        print(f"No discount applied. Price remains: ${final_price:.2f}")

except ValueError:
    print("Please enter valid numerical values for price and discount.")

