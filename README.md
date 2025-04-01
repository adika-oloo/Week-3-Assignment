# Python Week-3-Assignment
Create a function named calculate_discount(price, discount_percent) that calculates the final price after applying a discount. The function should take the original price (price) and the discount percentage (discount_percent) as parameters. If the discount is 20% or higher, apply the discount; otherwise, return the original price.
Using the calculate_discount function, prompt the user to enter the original price of an item and the discount percentage. Print the final price after applying the discount, or if no discount was applied, print the original price.



def calculate_discount(price, discount_percent):
    """Calculates the final price after applying a discount if it's 20% or higher."""
    if discount_percent >= 20:
        final_price = price - (price * discount_percent / 100)
        return final_price
    return price 
price = float(input("Enter the original price of the item: "))
discount_percent = float(input("Enter the discount percentage: "))
final_price = calculate_discount(price, discount_percent)
print(f"Final price after discount: ${final_price:.2f}")

Enter the original price of the item: 59
Enter the discount percentage: 478
Final price after discount: $-223.02
