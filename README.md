# Radix Sort and Hash Functions – Separate Chaining

## 📌 Mini Project

This mini project demonstrates two important **Data Structures and Algorithms** concepts through simple C programs:

1. **Radix Sort**
2. **Hash Functions using Separate Chaining**

The project is developed as part of the **Data Structures and Algorithms Laboratory** at **Kamaraj College of Engineering and Technology**.

---

## 👨‍💻 Team Members

| Name                | Roll Number |
| ------------------- | ----------- |
| D.R. Rohith         | 25UAD003    |
| M. Dharshan         | 25UAD041    |
| R. Raghava Krishnan | 25UAD018    |

**Class:** II ADS B
**Department:** Artificial Intelligence and Data Science
**College:** Kamaraj College of Engineering and Technology
**Batch:** 2024–2029

---

## 🎯 Objectives

* To implement **Radix Sort** for sorting non-negative integers.
* To demonstrate a **Hash Function** using the modulo operation.
* To implement **Separate Chaining** for handling hash collisions.
* To perform **insertion, searching, and deletion** operations in a hash table.
* To understand the working of these Data Structures and Algorithms through practical implementation.

---

## 🔹 Project 1: Radix Sort

Radix Sort is a non-comparison-based sorting algorithm that processes numbers digit by digit.

This project uses the **LSD (Least Significant Digit)** approach.

### How it works

For every digit position:

1. Start with the units digit.
2. Apply Counting Sort based on that digit.
3. Move to the tens digit.
4. Continue with hundreds, thousands, and so on.
5. Stop when all digits have been processed.

### Example

Input:

```text
170 45 75 90 802 24 2 66
```

Output:

```text
2 24 45 66 75 90 170 802
```

### Algorithm Used

```text
Radix Sort
    ↓
Find maximum element
    ↓
Process units digit
    ↓
Process tens digit
    ↓
Process hundreds digit
    ↓
Continue until all digits are processed
    ↓
Sorted Array
```

---

## 🔹 Project 2: Hash Function – Separate Chaining

The second part of the project demonstrates hashing using a modulo-based hash function.

### Hash Function

The hash index is calculated using:

```text
index = key % table_size
```

For example, if the table size is `5`:

```text
10 % 5 = 0
15 % 5 = 0
20 % 5 = 0
7 % 5 = 2
```

Here, `10`, `15`, and `20` produce the same index. This is called a **collision**.

### Collision Handling

The project uses **Separate Chaining** to handle collisions.

Example:

```text
[0] → 20 → 15 → 10 → NULL
[1] → NULL
[2] → 7 → NULL
[3] → NULL
[4] → NULL
```

Multiple keys having the same hash index are stored in a linked list.

---

## ⚙️ Operations Supported

The Hash Table program supports:

### 1. Insert

Adds a new key to the hash table.

```text
Key → Hash Function → Index → Linked List
```

### 2. Search

Searches for a given key in the appropriate chain.

### 3. Delete

Removes a specified key from the hash table.

### 4. Display

Displays all hash-table indices and their corresponding chains.

---

## 🛠️ Technologies Used

* **Programming Language:** C
* **Compiler:** GCC / MinGW
* **IDE:** Visual Studio Code
* **Concepts:** Data Structures and Algorithms
* **Data Structures:** Arrays, Linked Lists, Hash Tables

---

## 💻 Requirements

### Hardware

* Computer or Laptop
* Basic RAM and storage
* Modern processor

### Software

* Visual Studio Code
* C/C++ compiler such as GCC or MinGW
* Operating System: Windows/Linux/macOS

---

## 🚀 How to Run

### Step 1: Clone the Repository

```bash
git clone <your-github-repository-link>
```

### Step 2: Open the Project

Open the project folder in **Visual Studio Code**.

### Step 3: Compile Radix Sort

```bash
gcc radix_sort.c -o radix_sort
```

Run:

```bash
./radix_sort
```

On Windows:

```bash
radix_sort.exe
```

### Step 4: Compile Hash Table

```bash
gcc hash_separate_chaining.c -o hash_table
```

Run:

```bash
./hash_table
```

On Windows:

```bash
hash_table.exe
```

---

## 📂 Project Structure

```text
Radix-Sort-Hash-Functions/
│
├── radix_sort.c
├── hash_separate_chaining.c
├── README.md
│
└── screenshots/
    ├── radix-sort.png
    └── hash-table.png
```

---

## 📊 Sample Radix Sort Output

```text
Enter number of elements: 8

Enter 8 elements:
170 45 75 90 802 24 2 66

Original array:
170 45 75 90 802 24 2 66

Sorted array:
2 24 45 66 75 90 170 802
```

---

## 📊 Sample Hash Table Output

```text
Enter hash table size: 5

10 inserted at index 0
15 inserted at index 0
20 inserted at index 0
7 inserted at index 2

Hash Table:

[0] -> 20 -> 15 -> 10 -> NULL
[1] -> NULL
[2] -> 7 -> NULL
[3] -> NULL
[4] -> NULL
```

---

## 📚 Concepts Demonstrated

### Radix Sort

* LSD Radix Sort
* Counting Sort
* Digit extraction
* Array manipulation

### Hashing

* Hash Function
* Modulo operation
* Hash Table
* Collision
* Separate Chaining
* Linked List
* Insertion
* Searching
* Deletion

---

## 🔮 Future Scope

The project can be extended by:

* Adding a graphical visualization of Radix Sort.
* Showing every digit-processing step.
* Visualizing hash-table collisions.
* Adding other collision-resolution techniques such as Linear Probing and Quadratic Probing.
* Comparing the performance of different sorting and hashing techniques.
* Adding automated test cases.
* Developing a web-based version of the algorithms.

---

## ✅ Conclusion

This mini project provides a practical demonstration of **Radix Sort and Hash Functions using Separate Chaining**. Radix Sort efficiently sorts non-negative integers by processing individual digits, while the hashing module demonstrates how keys are mapped to table positions and how collisions are handled using linked lists.

The project helps students understand the practical implementation of important Data Structures and Algorithms concepts.

---

## 📖 References

1. Data Structures and Algorithms Laboratory – Kamaraj College of Engineering and Technology.
2. Project-provided mini project materials on Radix Sort and Hash Functions – Separate Chaining.
3. C Programming language concepts for arrays, structures, pointers and linked lists.

---

## 👥 Contributors

**D.R. Rohith** – 25UAD003
**M. Dharshan** – 25UAD041
**R. Raghava Krishnan** – 25UAD018

**Kamaraj College of Engineering and Technology**
**Department of Artificial Intelligence and Data Science**
**II ADS B**
