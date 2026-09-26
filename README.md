# 💸 SmartSpend – Student Expense & Budget Tracker

SmartSpend is a simple command-line application that helps students track their daily expenses, manage a monthly budget, and analyze their spending habits — all from the terminal.

## Features

- **Add Expense** – Record a new expense with date, category, description, and amount.
- **View All Expenses** – List every recorded expense.
- **Search Expense** – Find expenses by category or description keyword.
- **Edit Expense** – Update the details of an existing expense by its ID.
- **Delete Expense** – Remove an expense by its ID.
- **Set Monthly Budget** – Define how much you plan to spend in a month.
- **View Budget Status** – See total spent, remaining budget, and whether you're within or over budget.
- **Expense Analysis** – View total, average, highest, and lowest expenses, plus a category-wise breakdown.
- **Generate Report** – Produce a full monthly summary combining budget status and category analysis.

## Requirements

- Python 3.7 or higher
- No external libraries required (uses only the built-in `datetime` module)

## Getting Started

1. Save the script as `smartspend.py`.
2. Open a terminal in the same folder as the file.
3. Run the program:

   ```bash
   python smartspend.py
   ```

4. Use the on-screen menu to navigate between options (enter a number from 1–10).

## Expense Categories

Each expense must be assigned to one of the following categories:

- Food
- Transport
- Education
- Shopping
- Entertainment
- Hostel
- Other

## Usage Notes

- **Date format:** Dates must be entered as `DD-MM-YYYY` (e.g., `26-09-2026`).
- **Amounts:** All amounts are in ₹ (INR) and must be positive numbers.
- **Expense IDs:** Each expense is automatically assigned a unique ID, used when editing or deleting.
- **Budget:** The monthly budget must be set (option 6) before checking budget status or seeing a status line in reports; if it isn't set, the report will note "Budget not set."
- **Data persistence:** Expenses and budget data are stored **in memory only** for the current session — nothing is saved to a file, so all data is lost when the program exits.

## Example Menu

```
==================================================
       < SMARTSPEND EXPENSE TRACKER >
==================================================
1 -> Add Expense
2 -> View All Expenses
3 -> Search Expense
4 -> Edit Expense
5 -> Delete Expense
6 -> Set Monthly Budget
7 -> View Budget Status
8 -> Expense Analysis
9 -> Generate Report
10 -> Exit
==================================================
```

## Project Structure

```
smartspend.py    # Main application file (menu, expense logic, budget logic, analysis, reports)
README.md        # Project documentation
```

## Possible Future Improvements

- Save/load expenses from a file (CSV or JSON) for persistence across sessions.
- Export reports to PDF or text files.
- Support multiple months/budget periods.
- Add data visualization (charts) for category-wise spending.

## License

This project is free to use and modify for personal or educational purposes.
