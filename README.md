OVERVIEW

The Car class is a simple C++ implementation that models a car's attributes and behaviors. It allows users to create car objects with specific year models and makes, and provides methods to manipulate and retrieve the car's speed.

Features
Attributes:

yearModel: The model year of the car.
make: The manufacturer of the car.
speed: The current speed of the car.

Methods:

  Constructors:
  Car(int year, std::string carMake): Initializes a car with a specified year and make.
  Car(): Default constructor that initializes the car to the year 2022 and an empty make.

  Setters:
  setYearModel(int year): Sets the car's model year.
  setMake(std::string carMake): Sets the car's make.
  setSpeed(int carSpeed): Sets the car's speed.
  
  Getters:
  getYearModel(): Returns the car's model year.
  getMake(): Returns the car's make.
  getSpeed(): Returns the car's current speed.
  
  Behavior Methods:
  accelerate(): Increases the car's speed by 5.
  brake(): Decreases the car's speed by 5.

Installation
  
  Compile the Program:
  
  Use a C++ compiler to compile the program. 
  
  For example, 
              
          using g++: g++ -o car car.cpp

  Usage
  
  Creating a Car Object: 
    
          Car myCar(2021, "Toyota"); 
  
  Using Setters: 
            
          myCar.setSpeed(50);

Using Getters: 
          
          int currentSpeed = myCar.getSpeed();

Accelerating and Braking: 
          
          myCar.accelerate(); // Increases speed by 5 
          
          myCar.brake();      // Decreases speed by 5

Example: 

    #include <iostream>

    #include "Car.h"

    int main() {
    
    Car myCar(2021, "Toyota");
    
    myCar.accelerate();
    
    std::cout << "Current speed: " << myCar.getSpeed() << " km/h" << std::endl;
    
    return 0;
    
    }
