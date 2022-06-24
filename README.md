# word-navigation-game
# word navigation game for beginner using python language!!

print("welcome to my first game! ")
name = input("what is your name? ")
age  = int(input("what is your age? "))

health = 10

if age >= 18:
  print("you are old enough to play the game! ")

  
  wants_to_play = input("do you want to play? ").lower()
  if wants_to_play == "yes":
    print("hello", name, "you are", age, "years old.")
    print("let's play! ")

    left_or_right =  input("first choice... left or right (left/right)? ")
    if left_or_right == "left":
      ans = input("nice, you follow the path and reach a lake... Do you swim across or       go around (across/around)? ")
      if ans == "around":
        print("you went around and reached the other side of the lake. ")
      elif ans == "across": 
        print("you managed to swim across, but were bit by a fish and lost 5 health. ")
        health -= 5
        

      ans = input("you notice a house and a river. which do you go to (river/house)? ")  
      if ans == "house":
        print("you go to the house an are greted by the owner... He dosen't like you and you lose 5 health. ")
        health -= 5

        if health <=  0:
          print("you have 0 health and you lose the game...")
        else: 
          print("you have survived...you win")
      else:
        print("you fell in the river and lost....")
              
  else:
    print("cya...")

    
elif age >= 14:
  print("you can play the game with a supervision! ")
else:
  print("age restriction you're not allowed to play the game! ")
  
