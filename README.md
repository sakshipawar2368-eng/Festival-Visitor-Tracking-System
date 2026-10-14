#math_Activity
# Festival Visitor Tracking System

## 📌 Project Overview

The **Festival Visitor Tracking System** is a C++ console-based application designed to analyze visitor attendance across different festival events.

The festival consists of three main events:

- 🎵 Music Shows
- 💃 Dance Performances
- 🎭 Drama Events

Since some visitors may attend more than one event, simply adding the number of visitors for all events can result in duplicate counting. This project uses the **Principle of Inclusion-Exclusion** from Set Theory to calculate the actual number of unique visitors.

---

## 🎯 Objectives

The main objectives of this project are:

- To record visitors attending Music, Dance, and Drama events.
- To calculate the total number of unique visitors.
- To identify visitors attending only one event.
- To identify visitors attending exactly two events.
- To calculate visitors attending all three events.
- To avoid duplicate counting using the Inclusion-Exclusion Principle.
- To provide useful information for festival planning and crowd management.

---

## 🧮 Mathematical Concept Used

The project is based on the **Principle of Inclusion-Exclusion**.

For three sets:

- `M` = Visitors attending Music Shows
- `D` = Visitors attending Dance Performances
- `R` = Visitors attending Drama Events

The total number of unique visitors is calculated using:

```text
|M ∪ D ∪ R| = |M| + |D| + |R|
              - |M ∩ D|
              - |M ∩ R|
              - |D ∩ R|
              + |M ∩ D ∩ R|
```

In the C++ program:

```cpp
uniqueVisitors = M + D + R - MD - MR - DR + MDR;
```

---

## ✨ Features

The program provides a menu-driven interface with the following options:

1. **Display Event-wise Visitors**  
   Shows the number of visitors registered for Music, Dance, and Drama events.

2. **Display Total Unique Visitors**  
   Calculates the actual number of different visitors using the Inclusion-Exclusion Principle.

3. **Display Single Event Visitors**  
   Displays visitors who attended only Music, only Dance, or only Drama.

4. **Display Multiple Event Visitors**  
   Displays visitors who attended exactly two events and all three events.

5. **Display Complete Analysis**  
   Provides a complete summary of registrations, unique visitors, duplicate registrations, and attendance categories.

6. **Display Planning Suggestions**  
   Provides basic suggestions for crowd management, seating, refreshments, and movement between venues.

7. **Exit**  
   Terminates the program.

---

## 💻 Technologies Used

- **Programming Language:** C++
- **Concepts:** Set Theory and Principle of Inclusion-Exclusion
- **Programming Concepts:**
  - Variables
  - User Input/Output
  - Arithmetic Operations
  - `do-while` Loop
  - `switch-case`
  - Menu-Driven Programming

---

## 📥 Input

The user enters:

```text
Number of Music visitors
Number of Dance visitors
Number of Drama visitors
Visitors attending Music and Dance
Visitors attending Music and Drama
Visitors attending Dance and Drama
Visitors attending all three events
```

---

## 📤 Output

The program can display:

- Event-wise visitor count
- Total unique visitors
- Only Music visitors
- Only Dance visitors
- Only Drama visitors
- Music & Dance only visitors
- Music & Drama only visitors
- Dance & Drama only visitors
- Visitors attending all three events
- Exactly one-event visitors
- Exactly two-event visitors
- Exactly three-event visitors
- Duplicate registration count
- Festival planning suggestions

---

## 🧪 Example

Suppose the input is:

```text
Music Visitors = 100
Dance Visitors = 80
Drama Visitors = 70

Music & Dance = 30
Music & Drama = 20
Dance & Drama = 15

All Three = 10
```

The unique visitors are:

```text
Unique Visitors
= 100 + 80 + 70 - 30 - 20 - 15 + 10

= 195
```

Therefore:

```text
Total Unique Visitors = 195
```

---

## ⚙️ How to Run

### Step 1: Clone the Repository

```bash
git clone <your-repository-url>
```

### Step 2: Open the Project Folder

```bash
cd festival-visitor-tracking
```

### Step 3: Compile the Program

Using a C++ compiler such as G++:

```bash
g++ main.cpp -o festival
```

### Step 4: Run the Program

On Windows:

```bash
festival.exe
```

On Linux/macOS:

```bash
./festival
```

---

## 📂 Project Structure

```text
Festival-Visitor-Tracking/
│
├── main.cpp
├── README.md
└── screenshots/
    └── output.png
```

---

## 🌍 Real-World Applications

This project demonstrates how mathematical Set Theory can be applied to real-world problems such as:

- Festival visitor management
- Event registration analysis
- Crowd management
- Resource allocation
- Seating arrangements
- Refreshment planning
- Venue management
- Avoiding duplicate visitor counting

---

## 📊 Conclusion

The **Festival Visitor Tracking System** demonstrates the practical application of the **Principle of Inclusion-Exclusion** using C++.

The program efficiently calculates unique visitors even when people attend multiple events. It also provides detailed attendance analysis that can help organizers make better decisions regarding crowd management, seating, refreshments, and event planning.

This project shows how mathematical concepts such as **sets, intersections, unions, and Inclusion-Exclusion** can be implemented through computer programming to solve practical problems.
