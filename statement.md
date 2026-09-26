# Project Statement

## Problem Statement

Students often manage tight, irregular budgets funded by allowances, part-time income, or scholarships, but rarely track where their money actually goes. Without a simple way to log daily spending, categorize it, and compare it against a set budget, it becomes easy to overspend on non-essentials and run short on funds for essentials like food, transport, or education-related costs before the month ends. Most students either use no tracking method at all or rely on scattered notes that don't provide any real insight into their spending patterns.

**SmartSpend** addresses this gap with a lightweight, terminal-based expense and budget tracker that lets students log expenses, categorize spending, set a monthly budget, and instantly see whether they are on track or over budget.

## Scope of the Project

SmartSpend is a **single-user, command-line application** built in Python. Its scope covers:

- Recording, viewing, searching, editing, and deleting individual expense entries
- Organizing expenses into a fixed set of common student spending categories
- Setting and updating a monthly budget
- Comparing total spending against the budget to show remaining balance or overspending
- Generating summary statistics (total, average, highest, lowest expense) and category-wise breakdowns
- Producing a consolidated monthly report combining budget status and category analysis

**Out of scope** (for this version): multi-user accounts, cloud sync, mobile/web interfaces, multi-currency support, and recurring/auto-scheduled expenses. The current implementation also runs with in-memory data by default, with persistent file-based storage (JSON/CSV) planned as an enhancement.

## Target Users

- **College and university students** managing a personal monthly budget (allowance, stipend, or part-time earnings)
- **Hostel/PG residents** who need to track category-specific costs such as food, hostel fees, and transport separately
- **Budget-conscious beginners** who want a simple, no-frills tool without the complexity of full personal-finance apps
- Anyone comfortable using a command-line interface who wants a fast, distraction-free way to log expenses

## High-Level Features

- **Add Expense** – log a new expense with date, category, description, and amount
- **View All Expenses** – list every recorded expense in a readable format
- **Search Expense** – find expenses by category or description keyword
- **Edit Expense** – update the details of an existing expense using its unique ID
- **Delete Expense** – remove an expense by its ID
- **Set Monthly Budget** – define a spending limit for the month
- **View Budget Status** – see total spent, remaining balance, and over/under-budget status
- **Expense Analysis** – view total, average, highest, and lowest expenses, plus category-wise spending totals
- **Generate Report** – produce a complete monthly summary combining budget status, analysis, and transaction count
- **Input Validation** – guards against invalid amounts, malformed dates, empty descriptions, and out-of-range category choices throughout
