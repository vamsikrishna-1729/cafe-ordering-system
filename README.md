# cafe-ordering-system
print("welcome to cafecorner")
menu = {
    'pizza' : 40,
    'coffee' : 20,
    'cakes' : 15,
    'burger' :60,
    'pasta' : 50,
}
print("pizza :Rs 40/-\ncoffee :Rs 20/-\ncakes :Rs 15/-\nburger :Rs 60/-\npasta :Rs 50/-")
order_total = 0
item_1=input("Enter the name of item you want to order = " )
if item_1 in menu:
    order_total += menu[item_1]
    print(f"your {item_1} has been added to your cart")
else:
    print(f"ordered {item_1} is not available yet!")
another_item=input('do you want add another item (yes/no)?')
if another_item =='yes':
    item_2=input("Enter the name of item you want to order = " )
    if item_2 in menu:
        order_total += menu[item_2]
        print(f"your {item_2} has been added to your cart")
    else:
        print(f"your {item_2} is not available yet ?")


