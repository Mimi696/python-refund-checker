# main.py

# Ask the user for purchase details
purchase_days_ago = int(input('How many days ago have you purchased the item? '))
is_used = input('Have you used the item at all [y/n]? ')
is_broken = input('Has the item broken down on its own [y/n]? ')

# Apply refund policy rules
if(is_broken == 'y' or  (purchase_days_ago < 10 and is_used == 'n')):
    print('You can get a refund.')
else:
    print('You cannot get a refund.')

# Refund Policy Helper

## 📌 Overview
This is a simple Python program that helps an online store determine whether a customer is eligible for a refund based on the store's refund policy.

## 🛒 Refund Policy
A customer can get a refund if:
1. They purchased the item **within 10 days** and **haven't used it**, **OR**
2. The item **broke down on its own** (no matter when it was bought).

📋 Example Run

Input:

How many days ago have you purchased the item? 8
Have you used the item at all [y/n]? n
Has the item broken down on its own [y/n]? n


Output:

You can get a refund.

🛠 Requirements

Python 3.x
