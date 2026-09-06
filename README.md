# Nabiha_23122053_Lab_01_AI_6A


#  Food Delivery Agent

A simple Python-based **Food Delivery Agent** that helps users choose food according to their available budget.

##  Project Description

The Food Delivery Agent takes the user's preferred food and available budget as input. It then checks whether the selected food is available and whether the user's budget is enough.

The agent currently supports:

- 🍚 Biryani
- 🍕 Pizza
- 🍔 Burger

For each available food option, the agent provides a recommended item and its price.

##  Objectives

The main objectives of this project are:

- To demonstrate a simple AI agent concept.
- To take user input.
- To use conditional statements in Python.
- To check food availability.
- To compare the user's budget with food prices.
- To provide suitable food recommendations.

## 🛠️ Technologies Used

- **Python 3**
- `input()`
- `if`
- `elif`
- `else`
- `int()`
- `print()`

## ⚙️ How It Works

The agent follows these steps:

1. The user enters the food they want to order.
2. The user enters their available budget in PKR.
3. The agent checks the selected food.
4. It compares the budget with the food price.
5. If the budget is sufficient, the agent recommends the food.
6. If the budget is insufficient, the agent displays a suitable message.
7. If the food is not available, the agent asks the user to choose from the available options.

## 🍽️ Available Food Options

| Food | Recommended Item | Price |
|------|------------------|-------|
| Biryani | Chicken Biryani | 500 PKR |
| Pizza | Chicken Pizza | 1200 PKR |
| Burger | Zinger Burger | 700 PKR |

## 💻 Python Code

```python
print("===== FOOD DELIVERY AGENT =====")

food = input("What food would you like to order? ")
budget = int(input("Enter your available budget in PKR: "))

if food.lower() == "biryani":
    if budget >= 500:
        print("You can order Biryani.")
        print("Recommended: Chicken Biryani")
        print("Price: 500 PKR")
    else:
        print("Your budget is not enough for Biryani.")

elif food.lower() == "pizza":
    if budget >= 1200:
        print("You can order Pizza.")
        print("Recommended: Chicken Pizza")
        print("Price: 1200 PKR")
    else:
        print("Your budget is low for Pizza.")

elif food.lower() == "burger":
    if budget >= 700:
        print("You can order Burger.")
        print("Recommended: Zinger Burger")
        print("Price: 700 PKR")

    else:
        print("Your budget is low for Burger.")

else:
    print("Sorry! This food is not available.")
    print("Please choose Biryani, Pizza, or Burger.")

print("Thank you for using Food Delivery Agent!")
