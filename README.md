# Money Management Software

---

## 1. Cover Page

**Project Title:** Money Management Software  
**Developed by:** SANKIL SUDRIK  
**Course:** CSE-AIML  
**Institution:** VIT BHOPAL
**Date:** 25 November 2025

---

## 2. Introduction

Managing personal finances efficiently is a challenge for many individuals. This software aims to help users track expenses and incomes, set budgets, and receive alerts to avoid overspending, promoting financial discipline.

---

## 3. Problem Statement

Many people struggle to effectively monitor their spending and savings, leading to financial stress and unplanned overspending. The project solves this by providing an easy-to-use budget management tool.

---

## 4. Functional Requirements

- Add, view, and delete expenses and incomes with detailed notes and dates.  
- Set monthly budget limits.  
- Display alerts when expenses exceed the budget.  
- Show summaries of all transactions, including net balance.  
- Validate all user inputs to prevent errors.

---

## 5. Non-functional Requirements

- User-friendly GUI with responsive interaction.  
- Real-time updates and notifications.  
- Input validation and error handling for data integrity.  
- Maintainable modular code design.  
- Secure confirmation prompts for critical operations.  
- Portable across systems supporting Python 3 and Tkinter.

---

## 6. System Architecture

The system uses a client-side architecture with Tkinter as the GUI toolkit. Data is stored in memory during sessions, and operations are handled through modular Python classes following an MVC-like pattern.

---

## 7. Design Diagrams

- **Use Case Diagram:** Illustrates user interactions such as adding expenses/incomes and setting budgets.  
Use Case Flow
User
→ Adds Expense
→ Adds Income
→ Sets Budget
→ Views Transactions
→ Deletes Entry
→ Checks Budget Status

- **Workflow Diagram:** Shows the sequence of user actions and system responses.  
Workflow Flowchart
text
[Start] 
   ↓
[Open App] 
   ↓
[Add Expense or Income] 
   ↓
[Save Entry] 
   ↓
[Set or Update Budget?] ———> [Yes] ———> [Enter Budget]  
   |                                  ↓ 
   No                                  
   ↓                                  
[Check Expenses vs Budget] 
   ↓                        
[Show Alert if Overspent?] ———> [Yes] ———> [Display Alert]  
   |                                  ↓ 
   No                                  
   ↓                                  
[View Transactions] 
   ↓
[Delete Last Entry?] ———> [Yes] ———> [Delete Entry]  
   |                                  ↓ 
   No                                  
   ↓                                  
[Exit] 
   ↓ 
[End]

- **Sequence Diagram:** Details the interactions between GUI components and backend logic during key operations.  
Sequence of Adding Expense
User clicks "Add Expense" button.

Input form opens.

User enters amount, date, and note.

User submits data.

Expense is saved in memory.

Confirmation message is shown.

- **Class/Component Diagram:** Depicts class structures and relationships. 
Class Description 
BudgetManager

Attributes: budget, expenses list, incomes list

Methods: add_expense(), add_income(), set_budget(), delete_entry(), show_transactions(), check_expenses()

EntryDialog

Responsible for getting input details and validating them

Methods: submit(), cancel()
 
- **ER Diagram:** Not applicable as persistent storage is not implemented.

These simple flow and text diagrams can be drawn manually or recreated with tools like draw.io to match your project documentation style with clarity and ease.
---

## 8. Design Decisions & Rationale

- **Tkinter GUI** was chosen for simplicity and ease of cross-platform development.  
- **In-memory data storage** allows quick prototyping without dependencies.  
- Modular class design improves maintainability and scalability.  
- Input validation ensures data quality and user confidence.

---

## 9. Implementation Details

The application is implemented in Python using Tkinter. The main class `BudgetManager` handles UI and core functionalities. A secondary dialog class manages user inputs. Exception handling is implemented for invalid data.

---

## 10. Screenshots / Results

#main
https://github.com/Monster-3-2/Vit-Project/blob/4f41bba417ae22a907971b5bc2d0feb50d7298ae/main%20ui.png
#add expense
https://github.com/Monster-3-2/Vit-Project/blob/ece8700a28b2c547ae8d8ee87d0bb0ef3b52e670/add%20expense.png
#add income
https://github.com/Monster-3-2/Vit-Project/blob/046500f4588b3fb3fc7eca19fe83409a7834b81f/add%20income.png
#show expenses
https://github.com/Monster-3-2/Vit-Project/blob/acf75bc79fd87300f8c86c0d9ef5d51b5746cf8b/show%20expenses.png
#show income
https://github.com/Monster-3-2/Vit-Project/blob/d0a7d64c35d4c93b8c074c47ff530667e5e1d760/show%20income.png
#set budget
https://github.com/Monster-3-2/Vit-Project/blob/f348844b1f9447eae8a4141f6f35a18d83f9cfb0/set%20budget.png
#check expenses
https://github.com/Monster-3-2/Vit-Project/blob/cb697579aeae0afa9e27309f462c5a9a3debb60a/budget%20check.png
#transactions
https://github.com/Monster-3-2/Vit-Project/blob/e2bf55547de831f1864d60cc5f3f364206fa46d0/transactions.png
#exit
https://github.com/Monster-3-2/Vit-Project/blob/fea0df17e054c8400f8170fb273fad85b6936bbe/exit.png

---

## 11. Testing Approach

Manual testing was performed by entering various valid and invalid data sets to verify input validation, error handling, and budget alert mechanisms. Test cases included edge dates, empty notes, and large values.

---

## 12. Challenges Faced

- Handling date validation to prevent invalid entries.  
- Designing a responsive and user-friendly GUI layout.  
- Providing meaningful alerts without overwhelming users.

---

## 13. Learnings & Key Takeaways

- Importance of input validation and error handling in user-facing apps.  
- Practical application of OOP concepts in GUI programming.  
- Balancing functionality and simplicity for user experience.

---

## 14. Future Enhancements

- Implement persistent storage (database or file system).  
- Add automatic importing of bank statements.  
- Introduce graphical trend analysis and dashboards.  
- Provide mobile application version.  
- Add authentication and multi-user support.

---

## 15. References

- Python Official Documentation - https://docs.python.org/3  
- Tkinter GUI Tutorial - https://docs.python.org/3/library/tkinter.html  
- Personal finance management concepts - various online resources  
- VIT project guidelines and templates.

---

*End of README*



