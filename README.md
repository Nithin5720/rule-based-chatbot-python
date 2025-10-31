# 💬 Rule-Based Chatbot using Python

## 🎯 Objective
To create a **simple rule-based chatbot** that interacts with users using `if-elif-else` conditions in Python.

---

## 🧰 Tools & Technologies
- **Language:** Python  
- **IDE:** VS Code / IDLE / Jupyter Notebook  

---

## 🧠 Concept
A rule-based chatbot replies based on fixed patterns or keywords using simple logic — no machine learning or NLP library is used.  
It helps beginners understand how chatbots handle user input and produce output responses.

---

## 🪄 Features
- Responds to greetings and questions.  
- Uses **if-elif-else** logic to simulate conversation.  
- Keeps chatting until the user types **"bye"** or **"exit"**.  
- Displays current time when asked.  

---

## 📜 Code

```python
# Task 8: Rule-based Chatbot using if-else
# Objective: Understand basic NLP structure

print("🤖 Hello! I am ChatBot.")
print("Type 'bye' to end the chat.\n")

while True:
    user_input = input("You: ").lower()

    if "hello" in user_input or "hi" in user_input:
        print("ChatBot: Hello there! How can I help you today?")
    
    elif "how are you" in user_input:
        print("ChatBot: I'm just a program, but I'm doing great! How about you?")
    
    elif "your name" in user_input:
        print("ChatBot: I'm ChatBot, your virtual assistant.")
    
    elif "college" in user_input:
        print("ChatBot: I'm developed by Nithin from Dayananda Sagar Academy of Technology and Management.")
    
    elif "time" in user_input:
        from datetime import datetime
        current_time = datetime.now().strftime("%H:%M:%S")
        print(f"ChatBot: The current time is {current_time}.")
    
    elif "weather" in user_input:
        print("ChatBot: I can’t check the weather yet, but you can try asking Google!")
    
    elif "bye" in user_input or "exit" in user_input:
        print("ChatBot: Goodbye! Have a great day! 👋")
        break
    
    else:
        print("ChatBot: Sorry, I didn’t understand that. Can you rephrase?")
