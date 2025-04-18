
class Pet:
    def __init__(self, name, hunger=5, energy=5, happiness=5):
        self.name = name
        self.hunger = hunger
        self.energy = energy
        self.happiness = happiness

    def eat(self):
        self.hunger = max(0, self.hunger - 3)
        self.happiness = min(10, self.happiness + 1)
        print(f"{self.name} has eaten and feels happier!")
 

    def sleep(self):
        self.energy = min(10, self.energy + 5)
        print(f"{self.name} had a good rest and feels recharged!")
 

    def play(self):
        if self.energy >= 2: 
            self.energy -= 2
            self.happiness = min(10, self.happiness + 2)
            self.hunger = min(10, self.hunger + 1)
            print(f"{self.name} had fun playing!")
        else:
            print(f"{self.name} is too tired to play and needs to rest.")
 

    def get_status(self):
        print(f"Pet Status - Name: {self.name}, Hunger: {self.hunger}, Energy: {self.energy}, Happiness: {self.happiness}")
 

my_pet = Pet("Spothi")
Sphothi.get_status()
Sphothi.eat()
Sphothi.get_status()
Sphothi.play()
Sphothi.get_status()
Sphothi.sleep()
Sphothi.get_status()


### Bonus 🎯
- Add a method `train(trick)` that teaches your pet a new trick and stores it in a list.
- Add a method `show_tricks()` that prints all learned tricks.

class Pet:
    def __init__(self, name, hunger=5, energy=5, happiness=5):
        self.name = name
        self.hunger = hunger
        self.energy = energy
        self.happiness = happiness
        self.tricks = []  # List to store learned tricks

    def eat(self):
        self.hunger = max(0, self.hunger - 3)
        self.happiness = min(10, self.happiness + 1)
        print(f"{self.name} has eaten and feels happier!")
 

    def sleep(self):
        self.energy = min(10, self.energy + 5)
        print(f"{self.name} had a good rest and feels recharged!")
 

    def play(self):
        if self.energy >= 2
            self.energy -= 2
            self.happiness = min(10, self.happiness + 2)
            self.hunger = min(10, self.hunger + 1)
            print(f"{self.name} had a great time playing!")
        else:
            print(f"{self.name} is too tired to play and needs to rest.")
 

    def get_status(self):
        print(f"Pet Status - Name: {self.name}, Hunger: {self.hunger}, Energy: {self.energy}, Happiness: {self.happiness}")
 

    def train(self, trick):
        self.tricks.append(trick)
        self.happiness = min(10, self.happiness + 1)  
        print(f"{self.name} has learned a new trick: {trick}!")
 

    def show_tricks(self):
        if self.tricks:
            print(f"{self.name} knows the following tricks: {', '.join(self.tricks)}")
        else:
            print(f"{self.name} hasn't learned any tricks yet.")
 


my_pet = Pet("Sphothi")
Sphothi.get_status()
Sphothi.eat()
Sphothi.sleep()
Sphothi.play()
Sphothi.train("Roll Over")
Sphothi.train("Sit")
Sphothi.show_tricks()
Sphothi.get_status()


Bonus points for creativity (custom actions, emojis, pet types, etc.)

https://www.bing.com/images/search?q=dog%20emoji%20copy%20and%20paste&FORM=IQFRBA&id=233681728B304AF021E2D7F3E9F1FB3CD1CDDDA3
