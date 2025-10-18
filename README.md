# 🧮 Calculator App (Java Swing)

A *GUI-based Calculator Application* built using *Java Swing* that performs basic arithmetic operations such as addition, subtraction, multiplication, and division.  
It features an intuitive design, error handling, and real-time calculations using Java’s event-driven programming.

---

## 🚀 Features
- ➕ Addition, ➖ Subtraction, ✖ Multiplication, ➗ Division  
- 💡 User-friendly graphical interface built with Swing  
- ⚡ Real-time results on button click  
- ❌ Error handling for invalid or undefined operations (like division by zero)  
- 🔄 Clear button to reset the calculator  

---

## 🧰 Tech Stack
| Component | Technology |
|------------|-------------|
| Language | Java |
| GUI Framework | Swing |
| IDE | IntelliJ IDEA / Eclipse / NetBeans |

---

## ⚙ How It Works
1. User inputs numbers using buttons or keyboard.  
2. Selects an operator (+, −, ×, ÷).  
3. The calculator computes the result and displays it on the screen.  
4. “C” button clears the current input.  

---

## 💻 Sample Code Snippet
```java
if (command.equals("=")) {
    num2 = Double.parseDouble(display.getText());
    switch (operator) {
        case '+': result = num1 + num2; break;
        case '-': result = num1 - num2; break;
        case '*': result = num1 * num2; break;
        case '/': 
            if (num2 == 0) {
                JOptionPane.showMessageDialog(this, "Cannot divide by zero!");
                return;
            }
            result = num1 / num2;
            break;
    }
    display.setText(String.valueOf(result));
}
