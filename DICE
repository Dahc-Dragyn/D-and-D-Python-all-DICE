import random

def roll_die(num_sides):
  """Rolls a single die with the specified number of sides."""
  return random.randint(1, num_sides)

def roll_dice(num_dice, num_sides):
  """Rolls multiple dice with the specified number of sides."""
  rolls = []
  for _ in range(num_dice):
    rolls.append(roll_die(num_sides))
  return rolls

while True:
  print("\nChoose your die:")
  print("1. d4")
  print("2. d6")
  print("3. d8")
  print("4. d10")
  print("5. d12")
  print("6. d20")
  print("7. Custom die")
  print("8. Exit")

  choice = input("Enter your choice: ")

  if choice == '1':
    result = roll_die(4)
  elif choice == '2':
    result = roll_die(6)
  elif choice == '3':
    result = roll_die(8)
  elif choice == '4':
    result = roll_die(10)
  elif choice == '5':
    result = roll_die(12)
  elif choice == '6':
    result = roll_die(20)
  elif choice == '7':
    try:
      num_sides = int(input("Enter the number of sides: "))
      result = roll_die(num_sides)
    except ValueError:
      print("Invalid input. Please enter a number.")
      continue
  elif choice == '8':
    break
  else:
    print("Invalid choice.")
    continue

  print("You rolled:", result) 
