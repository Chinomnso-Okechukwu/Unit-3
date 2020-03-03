### 1. Instantiating three new dogs, each with a different age. Then write a function called, get_biggest_number(), that takes any number of ages (*args) and returns the old one.

```.py
class Dogs:
    # Class Attribute
    species = 'mammal'
    # Instance Attributes
    def __init__(self, name, age):
        self.name = name
        self.age = age
        
    def get_biggest_number(self):
        if jimmy.age > mochi.age and jimmy.age > frank.age:
            print(f'The oldest dog is {jimmy.age})
        if jimmy.age < mochi.age and mochi.age > frank.age:
            print(f'The oldest dog is {mochi.age})
        if jimmy.age < framk.age and mochi.age < frank.age: 
            print(f'The oldest dog is {frank.age})
       
        
jimmy = Dogs("Jimmy", 8)
mochi = Dogs("Mochi", 3)
frank = Dogs("Frank", 6)

print(jimmy.get_biggest_number())
```

### 2. Create a Pets class that stores instances of dogs in a List; this claass is completely separate from the Dog class. In other words, the Dog class does not inherit from the Pets class. Then assign three dog instances to an instance of the Pets class. Start with the following code below.

```.py
class Dogs:

    species = 'mammal'
    
    def __init__(self, name, age):
        self.name = name
        self.age = age
        
    def description(self):
        return "{} is {} years old".format(self.name, sound)
        
class RussellTerrier(Dogs):
    def run(self, speed):
        return "{} runs {}".format(self.name, speed)

class Bulldog(Dogs):
    def run(self, speed):
        return "{} runs {}".format(self.name, speed)
        
class Pets:
    def __init__(self, listAnimnals):
        self.pets = listAnimals
        
myDogs = [
    Dogs('Tom', 6)
    RussellTerrier('Fletcher', 7)
    Bulldog('Larry', 9)
]

myPets = Pets(myDogs)
print('I have {} dogs'.format(len(myPets.pets)))
for dog in myPets.pets:
    print(dog.description())
print('And the are all {}, of course'.format(myPets.pets[0].species))
```

### 3. Using the Dogs class, add an instance attribute of is_hungry = True class. Then add a method called eat() which changes the value of is_hungry to False when called. Figure out the best way to feed each dog and then output "My dogs are hungry." if all are hungry or "My dogs are not hungry." if all are not hungry.
```.py
class Dogs:

    species = 'mammal'
    
    def __init__(self, name, age):
        self.name = name
        self.age = age
        self.is_hungry = True
        
    def description(self):
        return "{} is {} years old".format(self.name, sound)
    
    def eat(self):
        self.is_hungry = False
        
class RussellTerrier(Dogs):
    def run(self, speed):
        return "{} runs {}".format(self.name, speed)

class Bulldog(Dogs):
    def run(self, speed):
        return "{} runs {}".format(self.name, speed)
class Pets:
    def __init__(self, listAnimnals):
        self.pets = listAnimals
        
myDogs = [
    Dogs('Tom', 6)
    RussellTerrier('Fletcher', 7)
    Bulldog('Larry', 9)
]

myPets = Pets(myDogs)
print('I have {} dogs'.format(len(myPets.pets)))
for dog in myPets.pets:
    print(dog.description())
    dog.eat()
    
print('And the are all {}, of course'.format(myPets.pets[0].species))

hungry_pets = False
for dog in myPets.pets:
    if dog.is_hungry:
        hungry_pets = True
        break
        
if hungry_pets:
    print("My dogs are hungry")
else:
    print("My dogs are not hungry")
```

### 4. Next, add a walk() method to both the Pets and Dog classes so that when you call the methid on the Pets class, each dog instance assigned to the Pets class will walk.
```.py
```
