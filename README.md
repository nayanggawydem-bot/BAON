print("==========================================")
print("              BAON BUDDY                 ")
print("==========================================")

print("FOOD MENU")
print("[A] Burger        - P50")
print("[B] Sandwich      - P40")
print("[C] Fries         - P35")
print("[D] Rice Meal     - P75")
print("[E] Juice         - P25")
print("==========================================")

code = input("Enter food code: ").upper()

if code == "A":
    product = "Burger"
    price = 50
elif code == "B":
    product = "Sandwich"
    price = 40
elif code == "C":
    product = "Fries"
    price = 35
elif code == "D":
    product = "Rice Meal"
    price = 75
elif code == "E":
    product = "Juice"
    price = 25
else:
    print("Invalid code")
    exit()

qty = int(input("Enter quantity: "))

if qty <= 0:
    print("Invalid quantity")
    exit()

subtotal = price * qty

print("==========================================")
print("               BAON RECEIPT              ")
print("==========================================")
print(f"Food          : {product}")
print(f"Price         : P{price:.2f}")
print(f"Quantity      : {qty}")
print("==========================================")
print(f"Total         : P{subtotal:.2f}")
print("==========================================")

budget = float(input("Enter your baon: P"))

if budget >= subtotal:
    remaining = budget - subtotal
    print(f"Your baon     : P{budget:.2f}")
    print(f"Money left    : P{remaining:.2f}")
    print("Within budget! Good job!")
elif budget < subtotal:
    needed = subtotal - budget
    print(f"Your baon     : P{budget:.2f}")
    print(f"Additional needed: P{needed:.2f}")
    print("This is over your budget.")
