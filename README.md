# 💳 Credit Card Validator - C & Python Implementation

[![C](https://img.shields.io/badge/C-A8B9CC?logo=c&logoColor=white)](https://en.wikipedia.org/wiki/C_(programming_language))
[![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Algorithm](https://img.shields.io/badge/Algorithm-Luhn-brightgreen)](https://en.wikipedia.org/wiki/Luhn_algorithm)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Robust credit card validation system implementing Luhn's Algorithm with card type detection in both C and Python, demonstrating cross-language programming proficiency.

## 🎯 Features

- 🔐 **Luhn Algorithm Validation** - Industry-standard checksum verification
- 💳 **Card Type Detection** - Identifies Visa, MasterCard, and American Express
- 🛡️ **Input Validation** - Handles invalid data with error recovery
- 🚀 **Performance Optimized** - O(n) time complexity with O(1) space usage
- 🔄 **Cross-Language** - Identical logic implemented in C and Python
- ⚡ **Efficient Processing** - Mathematical operations without string manipulation

## 🛠️ Tech Stack

**Languages:** C (systems programming), Python (high-level scripting)  
**Algorithm:** Luhn's Algorithm for checksum validation  
**Concepts:** Pattern recognition, input sanitization, mathematical operations  
**Features:** Type safety, error handling, modular design

## 🚀 Quick Start

### C Implementation
```bash
# Clone and compile
git clone https://github.com/AjayMaan13/Credit-Card-Validator.git
cd Credit-Card-Validator

# Compile with GCC
gcc -o credit credit.c -std=c99

# Run the program
./credit
```

### Python Implementation
```bash
# Direct execution
python credit.py
```

## 📁 Structure

```
Credit-Card-Validator/
├── credit.c              # C implementation
├── credit.py             # Python implementation
├── test_cases.txt        # Validation test data
└── README.md            # Documentation
```

## 💻 Usage Examples

### Sample Execution
```bash
$ ./credit
Enter Card Number (0 to exit): 4003600000000014
VISA

Enter Card Number (0 to exit): 378282246310005
AMEX

Enter Card Number (0 to exit): 5555555555554444
MASTERCARD

Enter Card Number (0 to exit): 1234567890123456
INVALID
```

### Algorithm Implementation
```c
// Luhn Algorithm in C
int validate_luhn(long number) {
    int sum = 0, digit, alternate = 0;
    
    while (number > 0) {
        digit = number % 10;
        if (alternate) {
            digit *= 2;
            if (digit > 9) digit = digit / 10 + digit % 10;
        }
        sum += digit;
        alternate = !alternate;
        number /= 10;
    }
    return (sum % 10) == 0;
}
```

## 🏗️ Architecture

### Card Type Detection Logic
```
American Express: 15 digits, starts with 34 or 37
MasterCard: 16 digits, starts with 51-55
Visa: 13 or 16 digits, starts with 4
```

### Validation Process
1. **Input Sanitization** - Numeric validation and error handling
2. **Length Check** - Verify digit count matches card type
3. **Pattern Matching** - Check starting digits for card identification
4. **Luhn Validation** - Apply checksum algorithm for authenticity

## 🧪 Testing

### Valid Test Cases
```
4003600000000014 → VISA
5555555555554444 → MASTERCARD
378282246310005 → AMEX
```

### Performance Metrics
- **Time Complexity:** O(n) where n = number of digits
- **Space Complexity:** O(1) constant space
- **Validation Accuracy:** 100% Luhn compliance

## 📊 Stats

- **2 language implementations** (C and Python)
- **3 card types supported** (Visa, MasterCard, Amex)
- **Mathematical algorithm** with optimal efficiency
- **Cross-platform compatibility** (Windows, Linux, macOS)

## 👨‍💻 Author

**Ajaypartap Singh Maan**  
[GitHub](https://github.com/AjayMaan13) • [LinkedIn](https://linkedin.com/in/ajaypartap-singh-maan) • ajayapsmaanm13@gmail.com

---

⭐ **Star if helpful!**
