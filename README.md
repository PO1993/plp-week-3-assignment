# plp-week-3-assignment

def calculate_discount(price, discount_percent):
    """
    Calculate the final price after applying a discount.
    If the discount percentage is 20% or higher, apply the discount.
    Otherwise, return the original price.
    """
    if discount_percent >= 20:
        final_price = price - (price * discount_percent / 100)
        return final_price
    else:
        return price

# Prompt the user for inputs
original_price = float(input("Enter the original price of the item: "))
discount_percent = float(input("Enter the discount percentage: "))

# Calculate the final price using the function
final_price = calculate_discount(original_price, discount_percent)

# Print the result
if discount_percent >= 20:
    print(f"The final price after a {discount_percent}% discount is: ${final_price:.2f}")
else:
    print(f"No discount applied. The original price is: ${original_price:.2f}")
