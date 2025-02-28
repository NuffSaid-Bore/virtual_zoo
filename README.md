## Zoo Animal Simulation



# Introduction

This is a simple Java-based zoo animal simulation application. The application models several animals (Tiger, Dolphin, and Penguin) using Object-Oriented Programming concepts such as inheritance, interfaces, and polymorphism. It allows users to interact with the animals by setting properties, displaying properties, simulating movements, and simulating feeding actions.

# Features
1. Animal Classes and Interfaces:
   - Animal Class: The base class for all animals, containing common properties such as name, weight, height, and age.
   - Eat Interface: Provides methods for feeding actions (eating food and completing eating).
   - Walk Interface: Provides methods for walking actions.
   - Swim Interface: Provides methods for swimming actions.
   - Tiger, Dolphin, and Penguin: These classes extend Animal and implement relevant interfaces (e.g., Swim, Walk) to define animal-specific behaviors.
2. Interactive Menu:
   - The user can choose between three animals: Tiger, Dolphin, or Penguin.
   - Once an animal is selected, the user can perform various actions, such as setting properties (e.g., speed, color), viewing properties, or simulating the movement and eating actions of the animal.
3. Movement Simulation:
   - The Tiger can simulate walking.
   - The Dolphin can simulate swimming.
   - The Penguin can either swim or walk, depending on its current state.

# Project Structure
  - Animal Class: A base class for all animals.
  - Eat Interface: Defines eating behavior.
  - Swim Interface: Defines swimming behavior.
  - Walk Interface: Defines walking behavior.
  - Tiger Class: Represents a tiger, capable of walking.
  - Dolphin Class: Represents a dolphin, capable of swimming and eating.
  - Penguin Class: Represents a penguin, capable of walking and swimming.
  - App Class: The main class with the interactive menu to simulate the zoo animal actions.

# Classes and Interfaces
  Animal Class
The Animal class is an abstract class that implements the Eat interface. It has the following properties and methods:
  - Properties:
      - nameOfAnimal: The name of the animal.
      - weight: The weight of the animal.
      - height: The height of the animal.
      - age: The age of the animal.
  - Methods:
      - Getters and setters for all properties.
      - An implementation of the eatingFood() method from the Eat interface.
  - Eat Interface
    The Eat interface defines two methods:
      - eatingFood(): Simulates the animal eating.
      - eatingCompleted(): Marks the completion of the animal's eating.
  - Swim Interface
    The Swim interface defines the swimming() method for animals that are capable of swimming.
  - Walk Interface
    The Walk interface defines the walking() method for animals that are capable of walking.
  - Tiger Class
    The Tiger class extends the Animal class and implements the Walk interface. It has the following properties:
      - speed: The speed of the tiger.
      - numberOfStripes: The number of stripes on the tiger's body.
      - soundLevelOfRoar: The sound level of the tiger's roar.
    It overrides the walking() method to simulate the tiger's movement.

  - Dolphin Class
    The Dolphin class extends the Animal class and implements the Swim interface. It has the following properties:
      - color: The color of the dolphin.
      - swimmingSpeed: The speed at which the dolphin swims.
    It overrides the swimming() method to simulate the dolphin swimming and the eatingFood() method to simulate the dolphin eating.
  - Penguin Class
    The Penguin class extends the Animal class and implements both the Swim and Walk interfaces. It has the following properties:
      - isSwimming: A boolean to determine if the penguin is swimming.
      - walkSpeed: The speed at which the penguin walks.
      - swimSpeed: The speed at which the penguin swims.
    It overrides the swimming() and walking() methods, with behavior depending on whether the penguin is swimming or walking.
  - App Class
    The App class contains the main interactive console menu, allowing the user to choose an animal and perform actions like:
      1. Setting animal properties (e.g., speed, color).
      2. Displaying animal properties.
      3. Simulating movement (walking/swimming).

  # Example Interaction

  ******* ZOO ANIMAL choice menu ******
1. Tiger
2. Dolphin
3. Penguin
Enter choice of animal (1-3): 1

The animal which is chosen is : Tiger
******* ANIMAL details menu for: Tiger ******
1. Set properties
2. Display properties
3. Display movement
4. Display eating
Enter choice (1-4): 2

Age: 5

Height: 3

Weight: 200

Speed: 50

Number of stripes: 20

Sound level of roar: 10


# Contributing
Feel free to fork this repository and make contributions. You can:
  - Add more animal classes.
  - Add more animal behaviors (e.g., sleeping, playing).
  - Improve the user interface or add more interactive options.

# License
This project is open-source and free to use.
  
