# line.py
"""
Importing pandas which is used to create dataframes
"""
import pandas as pd
"""
Made input variable Item, which asks to enter the item
"""
Item = input("Please enter the item: ")
"""
Same as pervious input statement except the response to the Item variable is include
as a string. Also used integer since numbers are being entered.
"""
Price = int(input("What is the price of one "+str(Item)+":"  ))
"""
Same as previous variable without string
"""
Qty = int(input("How many of this item: "))
"""
The Subtotal variable multiply the Price and Qty to get subtotal
"""
Subtotal = Price * Qty
"""
Create a dictionary to store the data, to work with pandas dataframe
"""
data = {
'Item':[Item],
'Price':[Price],
'Qty':[Qty],
'Subtotal':[Subtotal] }

"""
Sent data to pandas Dataframe/ variable purchase
"""
purchase = pd.DataFrame(data)
"""
print data
"""
print(purchase)
