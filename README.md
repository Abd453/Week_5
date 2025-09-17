# 🏗️ Assignment 1: Design Your Own Class

## 📄 Description
This Python assignment demonstrates **object-oriented programming concepts** including **classes, objects, constructors, methods, inheritance, encapsulation, and polymorphism**. Students will create their own class with attributes and methods, explore inheritance, and implement polymorphism with multiple classes sharing the same method.

---

## 📁 Project Files
- **`superhero.py`** – Python script for creating a Superhero class with attributes, methods, and inheritance.  
- **`vehicles.py`** – Python script for practicing polymorphism with different vehicle classes.  
- **README.md** – This file.

---

## ⚡ Features
- Define your own class with attributes and methods.
- Initialize objects using constructors.
- Use inheritance to extend functionality.
- Demonstrate encapsulation with private attributes.
- Implement polymorphism with multiple classes.

---

## 🛠 How to Run
1. Make sure Python 3 is installed.
2. Navigate to the project folder.
3. Run the desired script:

```bash
python superhero.py
python vehicles.py


---

## 📝 Example Outputs

**Superhero Example:**

```
SkyMan uses Super Strength!
SkyMan flies at 300 km/h!
```

**Vehicles Example:**

```

```
Driving 🚗
Flying ✈️
Sailing ⛵
````

---

### 2️⃣ `superhero.py`

```python
# Superhero class with inheritance and encapsulation

class Superhero:
    def __init__(self, name, power):
        self.name = name
        self.__power = power  # Encapsulated attribute

    def use_power(self):
        print(f"{self.name} uses {self.__power}!")

class FlyingHero(Superhero):
    def __init__(self, name, power, flying_speed):
        super().__init__(name, power)
        self.flying_speed = flying_speed

    def fly(self):
        print(f"{self.name} flies at {self.flying_speed} km/h!")

# Demo
if __name__ == "__main__":
    hero = FlyingHero("SkyMan", "Super Strength", 300)
    hero.use_power()  # SkyMan uses Super Strength!
    hero.fly()        # SkyMan flies at 300 km/h!
````

---

### 3️⃣ `vehicles.py`

```python
# Polymorphism example with vehicles

class Car:
    def move(self):
        print("Driving 🚗")

class Plane:
    def move(self):
        print("Flying ✈️")

class Boat:
    def move(self):
        print("Sailing ⛵")

# Demo
if __name__ == "__main__":
    vehicles = [Car(), Plane(), Boat()]
    for v in vehicles:
        v.move()
```
---

## 📝 Example Outputs

**Superhero Example:**

```
SkyMan uses Super Strength!
SkyMan flies at 300 km/h!
```

**Vehicles Example:**

```
Driving 🚗
Flying ✈️
Sailing ⛵
```

---

## 🚀 Notes

* Modify `Superhero` to create your own characters and powers.
* Extend `Vehicles` to add more classes and test polymorphism.
* Attributes starting with `__` are private to demonstrate encapsulation.

```

---

This is now a **complete, professional README.md** specifically for your assignment.  

If you want, I can also make a **version with Markdown badges and formatting** to make it look extra polished for GitHub. Do you want me to do that?
```

## 📂 Project Folder Structure

```
Assignment_1_OOP/
│── README.md
│── superhero.py
│── vehicles.py
```

---
