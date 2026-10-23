# EventFlow — Event Management & Budget Analysis System

A responsive event management and budget dashboard built as a single HTML file. The project demonstrates array-based priority queue and binary search concepts using JavaScript.

## Download / files

- `index.html` — the complete website, including its HTML, CSS, and JavaScript.
- `README.md` — this documentation file.

## Features

- Dashboard cards for total events, pending tasks, allocated budget, and expenses.
- Create, view, edit, and delete events with dates, venues, descriptions, and budgets.
- Add tasks with High, Medium, or Low priority. Tasks are sorted using an array-based priority queue.
- Set the allocated budget and record expenses under categories such as Venue, Food, Decoration, Transportation, Equipment, and Other.
- View total expenses, remaining balance, and a category chart.
- Search expense records by ID using binary search on a sorted list.
- Save changes in the current browser with `localStorage`.
- Responsive layout for desktop and mobile screens.

## Run locally

1. Download `index.html`.
2. Open the file in a modern browser such as Chrome, Edge, or Firefox.
3. No installation, package manager, or server is required.

For a local server, open a terminal in the folder containing `index.html` and run:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.

## Demonstrating the data structures

### Array-based priority queue

1. Find the **Priority tasks** section.
2. Add a task and choose High, Medium, or Low.
3. Observe that High priority tasks appear before Medium and Low priority tasks.

Priority values are represented as numbers: `1 = High`, `2 = Medium`, and `3 = Low`. The JavaScript sorts the task array after updates. This is an educational array-based priority queue demonstration, not a heap implementation.

### Binary search

1. Find **Expense records**.
2. Search for expense ID `1003` to locate the sample “Stage backdrop” expense.
3. Search for `9999` to see a not-found result.

The program sorts expense records by numeric ID, then checks the middle element and halves the search range each iteration. Binary search takes `O(log n)` time on a sorted list.

## Sample data

The initial dashboard contains four events, five tasks, and six expenses with IDs `1001` through `1006`. The sample allocated budget is ₹2,50,000.

## Notes

- This is a front-end academic demo; it does not include a Java backend.
- The working website logic is JavaScript. If the course requires actual Java data-structure implementations, provide separate Java classes as well.
- Data is stored in the current browser only. Clearing browser storage removes saved changes.
- Use the reset button in the dashboard header to restore the original sample data.
- The budget chart is drawn with the HTML Canvas API and does not require a chart library.

## Project explanation

“EventFlow is an event management and budget analysis dashboard. It enables users to manage event details, prioritize tasks, and track expenses against an allocated budget. An array-based priority queue organizes tasks according to importance, while binary search locates expense records efficiently from a sorted list of IDs. The interface is implemented in HTML and CSS, with JavaScript handling interactions, calculations, and browser-side data storage.”
