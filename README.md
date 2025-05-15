# 💳 Credit Card Validator - Implementation in C & Python

[![C](https://img.shields.io/badge/C-A8B9CC?logo=c&logoColor=white)](https://en.wikipedia.org/wiki/C_(programming_language))
[![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Algorithm](https://img.shields.io/badge/Algorithm-Luhn-brightgreen)](https://en.wikipedia.org/wiki/Luhn_algorithm)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> **Robust credit card validation system implementing Luhn's Algorithm with card type detection in both C and Python**

---

## 📋 Project Overview

This project demonstrates a comprehensive credit card validation system that verifies card numbers using **Luhn's Algorithm** and identifies card types based on industry-standard patterns. The implementation showcases programming proficiency in both **C** and **Python**, highlighting algorithm implementation, input validation, and cross-language development skills.

**👨‍💻 Developer:** Ajaypartap Singh Maan  
**📧 Contact:** ajayapsmaanm13@gmail.com  

---

## 🛠️ Technologies & Skills Demonstrated

### **Programming Languages**
- **C Programming** - Low-level systems programming with manual memory management
- **Python** - High-level scripting with object-oriented approach
- **Cross-Platform Compatibility** - Works on Windows, Linux, and macOS

### **Core Programming Concepts**
- **Algorithm Implementation** - Luhn's Algorithm for checksum validation
- **Input Validation** - Robust error handling for user input
- **Pattern Recognition** - Card type identification using digit patterns
- **Mathematical Operations** - Modular arithmetic and digit manipulation
- **Control Structures** - Loops, conditionals, and program flow control

### **Software Engineering Practices**
- **Code Organization** - Modular function design
- **Error Handling** - Graceful handling of invalid inputs
- **User Experience** - Continuous loop design with exit conditions
- **Documentation** - Clear code comments and README
- **Testing** - Comprehensive validation scenarios

### **Advanced Features**
- **Input Sanitization** - Handles strings, negative numbers, and invalid data
- **Future-Ready Design** - Placeholder functions for card masking and expiry validation
- **Cross-Language Implementation** - Demonstrates versatility in multiple paradigms

---

## 🔍 Algorithm Implementation

### **Luhn's Algorithm**
The Luhn algorithm (also known as the "modulus 10" algorithm) is a simple checksum formula used to validate various identification numbers:

1. Starting from the rightmost digit, double every second digit
2. If doubling results in a two-digit number, add the digits together
3. Sum all the digits (including undoubled ones)
4. If the total modulo 10 is 0, the number is valid

### **Card Type Detection**
```c
// American Express: 15 digits, starts with 34 or 37
// MasterCard: 16 digits, starts with 51-55
// Visa: 13 or 16 digits, starts with 4
```

---

## ✨ Key Features

### **🔐 Input Validation**
- **Type Safety** - Ensures only numeric input is processed
- **Range Validation** - Rejects negative numbers and invalid formats
- **Error Recovery** - Clears invalid input and continues execution
- **Exit Mechanism** - Clean program termination with '0' input

### **💳 Card Type Support**
- **American Express** - 15 digits starting with 34 or 37
- **MasterCard** - 16 digits starting with 51-55
- **Visa** - 13 or 16 digits starting with 4
- **Comprehensive Validation** - Both length and pattern matching

### **🚀 Performance Optimized**
- **Efficient Digit Extraction** - Mathematical operations instead of string manipulation
- **Minimal Memory Usage** - Direct calculation without storing intermediate values
- **Fast Execution** - Optimized loops and conditional statements

---

## 🧪 Example Usage

### **C Implementation**
```bash
$ gcc -o credit credit.c
$ ./credit
Enter Card Number (0 to exit): 4003600000000014
VISA
Enter Card Number (0 to exit): 378282246310005
AMEX
Enter Card Number (0 to exit): 5555555555554444
MASTERCARD
Enter Card Number (0 to exit): asf
Enter Card Number (0 to exit): 400000000
INVALID
Enter Card Number (0 to exit): 0
Exiting program.
```

### **Python Implementation**
```bash
$ python credit.py
Number: 4003600000000014
VISA
```

---

### **Performance Metrics**
- **Time Complexity:** O(n) where n is the number of digits
- **Space Complexity:** O(1) constant space usage
- **Input Range:** Supports up to 16-digit credit card numbers
- **Validation Accuracy:** 100% compliance with Luhn Algorithm

---

## 🎯 Learning Outcomes & Skills

### **Algorithm Development**
- **Mathematical Algorithm Implementation** - Luhn's checksum calculation
- **Pattern Recognition** - Card type identification logic
- **Edge Case Handling** - Invalid input scenarios
- **Optimization Techniques** - Efficient digit manipulation

### **Programming Proficiency**
- **C Programming** - Memory management, type safety, performance optimization
- **Python Programming** - Clean code design, readability, rapid prototyping
- **Cross-Language Development** - Implementing same logic in different paradigms
- **Input/Output Handling** - User interaction and data validation

### **Software Engineering**
- **Modular Design** - Separation of concerns with distinct functions
- **Error Handling** - Robust input validation and recovery
- **User Experience** - Intuitive interface with clear feedback
- **Code Documentation** - Comprehensive comments and explanations

---

## 🚀 Compilation & Execution

### **C Version**
```bash
# Compile with GCC
gcc -o credit credit.c -std=c99

# Run the program
./credit

# With debugging symbols
gcc -g -o credit credit.c -std=c99
```

### **Python Version**
```bash
# Direct execution
python credit.py

# Or make it executable
chmod +x credit.py
./credit.py
```

---

## ✅ Testing Scenarios

### **Valid Test Cases**
```
4003600000000014 → VISA (16 digits)
4111111111111111 → VISA (16 digits)
4012888888881881 → VISA (16 digits)
4222222222222220 → VISA (13 digits - truncated)
5555555555554444 → MASTERCARD
5105105105105100 → MASTERCARD
378282246310005 → AMEX
371449635398431 → AMEX
```

### **Invalid Test Cases**
```
1234567890123456 → INVALID (wrong pattern)
42424242424242 → INVALID (wrong length)
4000000000000002 → INVALID (checksum failure)
```

---

## 📞 Contact & Professional Links

**Ajaypartap Singh Maan**  
📧 **Email:** ajayapsmaanm13@gmail.com  
💼 **LinkedIn:** [Ajaypartap Singh Maan](https://linkedin.com/in/ajaypartap-singh-maan)  
🐙 **GitHub:** [@AjayMaan13](https://github.com/AjayMaan13)  

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🏷️ Tags

`C Programming` `Python` `Algorithms` `Luhn Algorithm` `Credit Card Validation` `Input Validation` `Financial Technology` `Cross-Language Development` `Mathematical Programming`

---