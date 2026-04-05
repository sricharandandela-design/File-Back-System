<img width="14" height="6" alt="Screenshot 2025-11-26 153403" src="https://github.com/user-attachments/assets/5b80a7db-4bbb-49ba-ac62-5f08c331e5b2" /># File-Back-System
# 📁 File Backup System using Tree (C Program)

---

## 📌 Project Title

**File Backup System using Tree Data Structure in C**

---

## ❓ Problem Statement

In real-world systems, files are often modified multiple times, and it is important to maintain different versions of a file.
The problem is to design a system that can:

* Store multiple versions of a file
* Maintain relationships between versions
* Allow operations like add, delete, update, search, and display

---

## 🌍 Real-world Application

This system is similar to:

* Version control systems (like Git)
* Backup software
* Cloud storage version history (Google Drive, Dropbox)

It helps in:

* Tracking file changes
* Restoring previous versions
* Managing hierarchical file versions

---

## 🧠 Data Structure Used

**Tree (N-ary Tree)**

* Each node represents a **file version**
* Each node can have up to **5 child versions**
* Parent-child relationship represents version history

### Node contains:

* Version number
* File name
* Pointer to parent
* List of child nodes

---

## 🏗️ System Design

### Components:

1. **Node Structure**
2. **Tree Representation**
3. **Menu-driven Interface**

### Operations:

* Add Version
* Delete Version
* Update Version
* Search Version
* Display Tree

### Design Approach:

* Root node is the initial version
* New versions are added as children
* Traversal is done using **DFS (Depth First Search)**

---

## ⚙️ Algorithm

### 🔹 Add Version

1. Input parent version
2. Search parent node using DFS
3. If found and child limit not exceeded:

   * Create new node
   * Attach it as child

---

### 🔹 Search Version

1. Start from root
2. Compare version
3. Recursively search children (DFS)
4. Return node if found

---

### 🔹 Update Version

1. Input version number
2. Search node
3. Replace filename

---

### 🔹 Delete Version

1. Input version
2. Search node
3. Check:

   * Not root
   * Must be leaf node
4. Remove from parent
5. Free memory

---

### 🔹 Display Tree

1. Start from root
2. Print node with indentation
3. Recursively display children

---

## 💻 Implementation

* Language: **C**
* Concepts Used:

  * Structures
  * Pointers
  * Dynamic Memory Allocation (`malloc`, `free`)
  * Recursion (DFS traversal)

---


![WhatsApp Image 2026-04-05 at 2 44 42 PM](https://github.com/user-attachments/assets/2880dd7d-3de5-4293-b0a1-c636af56cbd0)
![WhatsApp Image 2026-04-05 at 2 45 22 PM](https://github.com/user-attachments/assets/01bcef10-16bb-4eac-af41-af22ad802105)
![WhatsApp Image 2026-04-05 at 2 45 35 PM](https://github.com/user-attachments/assets/db220ec4-7e61-42ea-b98e-fcf8092db7b1)
![WhatsApp Image 2026-04-05 at 2 45 43 PM](https://github.com/user-attachments/assets/8eeabd6f-f917-4c4b-aaa9-5098f0a51606)
![WhatsApp Image 2026-04-05 at 2 45 51 PM](https://github.com/user-attachments/assets/fe0407ea-5841-4001-ade3-3caf10f23f53)
![WhatsApp Image 2026-04-05 at 2 46 10 PM](https://github.com/user-attachments/assets/b5afdd9b-704f-4e53-ac3f-a26da32f806d)
<img width="198" height="189" alt="Screenshot 2026-04-05 165550" src="https://github.com/user-attachments/assets/2a6d2c90-b1df-4422-9143-59303e77ea38" />



## 🖥️ Demo Output

```



===== File Backup System =====
1. Add File Version
2. Delete Version
3. Update Version
4. Search Version
5. Display All Versions
6. Exit
Enter choice: 1

Enter parent version: 1
Enter new version number: 2
Enter file name: fileA
Version added successfully!

Enter choice: 5

File Versions Tree:
Version 1 (root_file)
  Version 2 (fileA)
```

---

## ✅ Conclusion

This project demonstrates how a **tree data structure** can be used to implement a simple file versioning system.

### Key Learnings:

* Efficient data organization using trees
* Recursive searching (DFS)
* Memory management in C
* Real-world application of data structures

### Limitations:

* Fixed number of children (max 5)
* Only leaf nodes can be deleted
* No permanent storage

---

## 🔮 Future Enhancements

* Dynamic child allocation
* File saving/loading (persistent storage)
* GUI interface
* Advanced version control features

---
