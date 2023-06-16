# Assign-petDog
 class Pet:
        def __init__(self, name, age):
            self.name = name
            self.age = age

        def print_info(self):
            print('Pet Information:')
            print('   Name:', self.name)
            print('   Age:', self.age)

    class Dog(Pet):
        def __init__(self, name, age, breed):
            super().__init__(name, age) 
            self.breed = breed
        def print_info(self):
            super().print_info()
            print ('   Breed:', self.breed)

    pet_name = input()
    pet_age = int(input())
    dog_name = input()
    dog_age = int(input())
    dog_breed = input()

    pet = Pet(pet_name, pet_age)
    pet.print_info()
    dog = Dog(dog_name, dog_age, dog_breed)
    dog.print_info()
