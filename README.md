# Python-Week-3-Assignment-submission

def calculate_discount(price, discount_percent):
    
    Calculate the final price after applying a discount (if discount is 20% or higher).
    Args:
        price (float): Original price of the item.
        discount_percent (float): Discount percentage (e.g., 20 for 20%).
    Returns:
        float: Final price after discount (or original price if discount < 20%).
    
    if discount_percent >= 20:
        discounted_price = price * (1 - discount_percent / 100)
        return discounted_price
    else:
        return price

# Prompt user for input
original_price = float(input("Enter the original price of the item: "))
discount = float(input("Enter the discount percentage (e.g., 20 for 20%): "))

# Calculate and print the final price
final_price = calculate_discount(original_price, discount)
print(f"Final price after discount: ${final_price:.2f}")
