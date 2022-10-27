"# Hello_you.verhaallijn" 

print("Hi! ")
sleep(2.5)
print("in this simulation you will play a person who's just in the Netherlands. You just applied for asylum")
sleep(3.5)
print("before you can integrate. you have to follow integrate lessons. ")
sleep(2.5)
print("one day the teachers changed something on the schedule")
sleep(2.5)
print("They decided to give you and 8 other students a tour in a city named Rotterdam. just an excursion to experience what it's like to be in rotterdam and to learn something about our culture. ")
sleep(5)
print("before we begin choose you character. \n A. Adam \n B. Isabel")

#stuk01
def intro():
  choice = input()
  if choice in answer_a:
    print("you play Adam.")
    ChoiceT()
  elif choice in answer_b:
    print("you play Isabel.")
    ChoiceT()
  else:
   print(required)
   intro()

#stuk02
def ChoiceT(): 
  print("when you walked to the bus. are you deciding with who you will sit on the bus. who are you going to sit next to \nA. Michael \nB. Eugene \nC. James ")
  choice = input()
  if choice in answer_a:
   print("you sat down next to micheal and the whole trip was boring because he was just sleeping.")
   first()
  elif choice in answer_b:
   print("you sat down next to Eugene and you listened to music together the whole journey.")
   first()
  elif choice in answer_c:
   print("you sat down next to james that was a mistake because he got carsick and puked all over you.")
   first()
  else:
   print(required) 
   ChoiceT()
   
#stuk03
def first():
 print("your first stop is the euromast. \nyour at the top and you can see a beautiful view. you want to ask something.")
 sleep(2)
 print("A. when was the euromast built? \nB. are there more towers like this? ")
 choice = input()
 if choice in answer_a:
    print("the euromast is built in 1960. ")
    second()
 elif choice in answer_b:
    print("you have other towers like this, like the Bostoren or the uitkijktoren kootwijkerzand, but the euromast is the biggest tower in the Netherlands. ")
    second()
 else:
    print(required)
    first()

#stuk04
def second():
 print("for the next stop can you choose now. Between \nA. Kunsthal  \nB. fotomuseum ")
 choice = input()
 if choice in answer_a:
    kunsthal()
 elif choice in answer_b:
    fotomuseum()
 else:
    print(required)
    second()

#stuk05
def kunsthal():
 print("you have decided to go to the kunsthal \nyou and you fellow students are discussing. where do you want to go.")
 sleep(2.5)
 print("4 students want to go to ""illustrator"" and the other 4 wants to ""stap in de schoenen van tim walker"" \nwhere do you want to go? ")
 print("A. Illustrator \nB. Stap in de schoenen van tim walker ")
 choice = input()
 if choice in answer_a:
   Illustrator()
 elif choice in answer_b:
   tim_walker()
 else:
   print(required)
   kunsthal()

#stuk06
def Illustrator(): 
 print("you decided to go to the illustrator \nyou get the subject to make a painting. From something you like about Rotterdam \nwhat are you gonna paint? \n you thinking about what you all see when you was at the top of the euromast")
 print("what are you gonna paint \nA. euromast \nB. het park \nC. kleine parkhuis \nD. erasmusbrug ")
 choice = input()
 if choice in answer_a:
   print("nice painting! I like the way how you draw the euromast")
   endChoose()
 elif choice in answer_b:
   print("beautiful i see you like het park")
   endChoose()
 elif choice in answer_c:
   print("hmmm i see you paint het kleine huis")
   endChoose()
 elif choice in answer_d:
   print("interest choice")
   endChoose()
 else:
   print(required)
   Illustrator()

#stuk07
def tim_walker():
 print("you and your classmates choose for tim walker. tim walker is a exhibition from the most beautiful art.")
 print("you can choose between a: \nA. question \nB. remark ")
 choice = input()
 if choice in answer_a:
   print("you asks if you can know the artis who painted the Duckie Thot, Aubrey’s shadow. It was tim walker")
   TM()
 elif choice in answer_b:
   print("your remark was that you find some painting to white.")
   TM()  

#stuk08
def endChoose():
 print("after 2 hours of hard work your master piece is done and the time is up. the teacher says that we have two options \nA. we can all go home now \nB. we can diner at the goudenwolk.")
 choice = input()
 if choice in answer_a:
   travelb1()
 elif choice in answer_b:
   dinner()
 else:
   print(required)
   endChoose()

#stuk09
def dinner():
 print("the waiter ask what you want. You can choose between \nA. spaghetti \nB. pizza \nC. chilli con carne ")
 choice = input()
 if choice in answer_a:
   print("you liked the spaghetti")
   print("you had a good day, have a nice painting and a and well dined")
   travelb2()
 elif choice in answer_b:  
   print("the pizza was delicious you said")
   print("you had a good day, have a nice painting and a and well dined")
   travelb2()
 elif choice in answer_c:  
   print("its not bad you said")
   print("you had a good day, have a nice painting and a and well dined")
   travelb2()
 else:
   print(required)
   dinner()

#stuk10
def TM():
  print("after more than 3 hours looking at art the end is in sight")
  print("you had a great day and learn so much about tim walker's art")
  dinner()

#stuk11
def fotomuseum():
 print("you and your classmates have desided to go to the fotomuseum \nyou are at the entrance and wait for your guide ")
 print("9 minutes later you see your guide \nyour first stop is the work of johan van der keuken")
 print("you want to asks something what are you gonna ask? \nA. why is everything grey \nB. is this sirious art? ")
 choice = input()
 if choice in answer_a:
  print("the guide said: \nthat grey is he's style. Art doesn't have to be colorful to be beautiful")
  next_stop()
 elif choice in answer_b:
  print("the guide said: \nthat yes this is art because there is depth in it and emotion")
  next_stop
 else:
   print(required)
   fotomuseum()
 
#stuk12
def next_stop():
 print("the next stop is the Typische Nederlander \nyou see so many pictures and you want to tell something what are you gonna say?")
 print("A. they made a picture but they didn't made art \nB. why do i see so many tractors? ")
 choice = input 
 if choice in answer_a:
  print("the guide said: you can say its more a picture then art i agree with you")
  trail()
 elif choice in answer_b:
  print("the guide said: the Dutch people is a farm country its normal if there are so many picture of a tractor")
  trail()
 else:
   print(required)
   next_stop()

#stuk13
def trail():
  print("the last stop is a trail you and a fellow student can now make your own pictures you try to make beautiful pictures around you or of yourself")
  print("choose first your buddy: \nA. gio \nB. Brian \nC. leyla ")
  choice = input()
  if choice in answer_a:
    gio()
  elif choice in answer_b:
    Brian()
  elif choice in answer_c:
    leyla()
  else:
   print(required)
   trail()

#stuk14
def gio():
  print("you and gio can choose between: \nA. selfies \nB. statue pictures")
  choice = input()
  if choice in answer_a:
    print("the guide understand why you choose selfies but hes says also its not creative enough ")
    endCHoose2()
  elif choice in answer_b:
    print("the guide finds that you and gio made great pictures")
    endCHoose2()
  else:
   print(required)
   gio()

#stuk15
def Brian():
  print("you and Brian can choose between: \nA. selfies \nB. statue pictures")
  choice = input()
  if choice in answer_a:
   print("the guide understand why you choose selfies but hes says also its not creative enough ")
   endCHoose2()
  elif choice in answer_b:
    print("the guide finds that you and Brian made great pictures")
    endCHoose2()
  else:
   print(required)
   Brian()

#stuk16
def leyla():
  print("you and leyla can choose between: \nA. selfies \nB. statue pictures")
  choice = input()
  if choice in answer_a:
   print("the guide understand why you choose selfies but hes says also its not creative enough ")
   endCHoose2()
  elif choice in answer_b:
    print("the guide finds that you and leyla made great pictures")
    endCHoose2()
  else:
   print(required)
   leyla()

#stuk17
def endCHoose2():
  print("at the end of the day you all go home but when you walk to the exit you see a giftshop are you gonna ask to get al a soevenir or not?")
  choice = input()
  if choice in yes:
    souvenir()
  elif choice in no:
    print ("you had a great day and you al are gonna go home now ")
    travelb3()
  else:
    print(required)
    endCHoose2()

#stuk18
def souvenir():
  print("you can choose between a \nA. plussy \nB. a T-shirt \nC. keychain ")
  choice = input()
  if choice in answer_a:
   print("you bought a nice plussy ")
   travelb4()
  elif choice in answer_b:
   print("you bought a nice T-shirt")
   travelb4()
  elif choice in answer_c:
   print("you bought a nice keychain")
   travelb4()
  else:
    print(required)
    souvenir()

#stuk19
def travelb1():
 print("when you tried to get your paintings on the bus it was too tight the kunsthal would like to keep your paintings but then you have to pick up the painting within a week")
 print("do you agree?")
 if choice in yes:
   print("you agreed but unfortunately you forgot")
   end1()
 elif choice in no:
   print("you took the risk but unfortunately they were damaged")
   end1()
 else:
   print(required)
   travelb1()

#stuk20
def end1():
  print("after the trip you are all tired but it was a fun and educational day")
  print("Do you think you also want to go to the Kunsthal in Rotterdam")
  choice = input()
  if choice in yes:
    print("ok i hope your day will be as nice as in this story")
  elif choice in no:
   print("well maybe you like to go somewhere else in another city like in Haarlem or Amsterdam or Leiden. there are also many museums to visit")
  else:
   print(required)
   end1()

#stuk21
def travelb2():
  print("after dinner you will take the bus back home who will you sit next to on the return journey? \nA. Micheal \nB. Eugene \nC. James ")
  choice = input()
  if choice in answer_a:
   print("you sat down next to micheal and the whole trip was boring because he was only sleeping.")
   end2()
  elif choice in answer_b:
   print("you sat down next to Eugene and you listened to music together the whole journey.")
   end2()
  elif choice in answer_c:
   print("you sat down next to james that was a mistake because he got carsick and puked all over you.")
   end2()
  else:
   print(required)
   travelb2()

#stuk22
def end2():
  print("after this day you had a fantastic day and you are full of food")
  print("Do you think you also want to go to the Kunsthal in Rotterdam?")
  choice = input()
  if choice in yes:
   print("ok i hope your day will be as nice as in this story")
  elif choice in no:
   print("well maybe you like to go somewhere else in another city like in Haarlem or Amsterdam or Leiden. there are also many museums to visit")
  else:
   print(required)
   end2()

#stuk23
def travelb3():
  print("when you walked to the bus you asked if you could sit in the front because you are a bit nauseous")
  print("they asked if you wanted a bucket just to be sure \n Y/N")
  choice = input()
  if choice in yes:
   print("you couldn't hold it in anymore and you threw up luckily you had that bucket")
   end3()
  elif choice in no:
   print("you couldn't hold it anymore and you threw up")
   end3()
  else:
   print(required)
   travelb3()

#stuk24
def end3():
  print("when you got home you had a bad aftertaste but also a fun and educational day. would you go to it too the foto museum? ")
  choice = input()
  if choice in yes:
   print("good choice because it is very interesting and educational to go to such a place")
  elif choice in no:
   print("there are always other options to go to")
  else:
   print(required)
   end3()

#stuk25
def travelb4():
  print("when you walked to the bus with your beautiful souvenir are you going to exchange souvenirs with someone who are you going to do that with?")
  print("A. Eugene \nB. gio \nC. leyla")
  choice = input()
  if choice in answer_a:
   print("you are not happy with the exchange")
   end4()
  elif choice in answer_b:
   print("you are happy with the exchange")
   end4()
  elif choice in answer_c:
   print("you are very satisfied with the exchange")
   end4()
  else:
   print(required)
   travelb4()

#stuk26
def end4():
  print("after the trip you learned a lot and took a souvenir home")
  print("would you go to it foto museum? \n Y/N")
  choice = input()
  if choice in yes:
   print("good choice, maybe you can also take such a nice souvenir with you")
  elif choice in no:
   print("then maybe you'll find the kunsthal more fun")
  else:
   print(required)
   end4

intro() 
