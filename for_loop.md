the_count = [1, 2, 3, 4, 5]
fruits = ["apples", "oranges", "pears", "apricots"]
change = [1, "pennies", 2, "dimes", 3, "quarters"]

# This first kind of for-loop goes through a list
for number in the_count:
    print(f"This is count {number}")

# Same as above
for fruit in fruits: 
    print(f"A fruit of type: {fruit}")

# Also we can go through mixed lists too
for i in change:
    print(f"I got {i}")

# We can also build lists, first start with an empty one
elements = []

# Then use the range function to do 0 to 5 counts
for i in range(0, 6):
    print(f"Adding {i} to the list.")
    # Append is a function that lists understand
    elements.append(i)

# Now we can print them out too
for i in elements: 
    print(f"Element was: {i}")
    
# Man kann statt: for zutat in zutaten. Kann man for i in zutaten schreiben.

# 1, 2, 3, 4 Trivial:
print(1)
print(2)
print(3)
print(4)

print("-" * 10)

# Etwas besser:
for zahl in [1, 2, 3, 4]:
    print(zahl)
    
print("-" * 10)

# Optimale Variante:
for i in range(1, 5):
    print(i)
    
print("-" * 10)

# Zählen wie ein Computer: Drei Mal etwas tun.
for i in range(3):
    print(i)

print("-" * 10)

for i in range(1, 4):
    print(i)
print("Los!")

print("-" * 10)

# Durchnummerierte Zutaten
zutaten = ["Nüsse", "Eier", "Mehl"]

for i , zutat in enumerate(zutaten, 1):
    print(f"{i}. {zutat}")
    
# Etwas am Ende der Liste anhängen
zutaten.append("Zucker")

# Etwas vom Ende der Liste entfernen
zutaten.pop()

# Ein bestimmtes Element aus der Liste entfernen
zutaten.remove("Mehl")

# Fragen ob ein bestimmtes Element in der Liste vorkommt:
print("Nüsse" in zutaten)
print("Pizza" in zutaten)