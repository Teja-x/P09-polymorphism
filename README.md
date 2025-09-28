# Animal Inheritance Demo 🐾

This project demonstrates **Java OOP concepts** such as **inheritance, polymorphism, and method overriding** using a simple hierarchy of animals.

---

## 📂 Package Structure

org
└── studyeasy
    ├── Main.java
    └── animal
        ├── Animal.java
        ├── fish
        │   └── Eel.java
        ├── bird
        │   ├── Bird.java
        │   └── Eagle.java
        └── reptile
            ├── Reptile.java
            └── Crocodile.java

---

## ✨ Features

- **Base Class:**  
  - `Animal` → defines the base behavior of all animals.  

- **Derived Classes:**  
  - `Bird` and `Eagle` (extends `Animal`)  
  - `Reptile` and `Crocodile` (extends `Animal`)  
  - `Eel` (extends `Animal`)  

- **Polymorphism in Action:**  
  - All animals are stored in a `List<Animal>` and processed uniformly.  
  - The overridden `showInfo()` method ensures each animal type prints its own info.

---

## 🛠️ How It Works

The `Main` class:

1. Creates different animal objects (`Animal`, `Reptile`, `Crocodile`, `Eel`, `Eagle`).
2. Stores them inside a single `List<Animal>`.
3. Calls `listAnimals()`, which loops through the list and prints each animal’s info.

```java
private static void listAnimals(List<Animal> animals) {
    for(Animal animal: animals){
        System.out.println(animal.showInfo());
    }
}
