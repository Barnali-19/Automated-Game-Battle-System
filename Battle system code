import os
import time
import random

def six_sided_roll():
  roll = random.randint(1,6)
  return roll
  
def twelve_sided_roll():
  roll = random.randint(1,12)
  return roll
  
def eight_sided_roll():
  roll = random.randint(1,8)
  return roll
  
def health():
  health = ((six_sided_roll() * twelve_sided_roll()) / 2) + 10
  return health
  
def strength():
  str = ((six_sided_roll() * eight_sided_roll()) / 2) + 12
  return str

print("\033[31m⚔️ BATTLE TIME ⚔️\n\033[0m")
player1 = input("Name your Legend: ")
type1 = input("Character Type (Human, Elf, Wizard, Orc): ")
print("")
print(player1)
health1 = health()
print("HEALTH: ", health1)
print("STRENGTH: ", strength(),"\n")
print("Who are they battling?\n")
player2 = input("Name your Legend: ")
type2 = input("Character Type (Human, Elf, Wizard, Orc): ")
print("")
print(player2)
health2 = health()
print("HEALTH: ", health2)
print("STRENGTH: ", strength(),"\n")

time.sleep(4)
os.system("clear")

counter = 0
while True:
  print("\033[31m⚔️ BATTLE TIME ⚔️\n\033[0m")
  if counter == 0:
    print("The battle begins!\n")
  else:
    print("The battle continues!\n")
    
  first_blow = random.randint(1,2)
  counter += 1
  
  if first_blow == 1:
    print(player1, "wins the first blow")
    dmg = random.randint(1,10)
    print(player2, "takes a hit, with", dmg, "damage\n")
    health2 = health2 - dmg
    print(player1)
    print("HEALTH: ", health1)
    print(player2)
    print("HEALTH: ", health2)
    if health2 <= 0:
      print("Oh no", player2, "has died!")
      print(player1, "destroyed", player2, "in", counter, "rounds!")
      break
    else:
      print("And they're both standing for the next round!\n")
      time.sleep(4)
      os.system("clear")
      continue

  elif first_blow == 2:
    print(player2, "wins the first blow")
    dmg = random.randint(1,10)
    print(player1, "takes a hit, with", dmg, "damage\n")
    health1 = health1 - dmg
    print(player1)
    print("HEALTH: ", health1)
    print(player2)
    print("HEALTH: ", health2)
    if health1 <= 0:
      print("Oh no", player1, "has died!")
      print(player2, "destroyed", player1, "in", counter, "rounds!")
      break
    else:
      print("And they're both standing for the next round!\n")
      time.sleep(4)
      os.system("clear")
      continue
