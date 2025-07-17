# 📊 Lab 12 - HTML Data Tables

This workspace demonstrates how to create and format data tables using HTML. It contains two example files, each showcasing different aspects of HTML table creation.

## Overview

HTML tables are used to organize data into rows and columns. They are created using the `<table>` element, with rows defined by `<tr>`, headers by `<th>`, and data cells by `<td>`. Captions can be added using the `<caption>` tag to describe the table's content.

## 📁  Files

### [📝 Lab 12a.html](Lab%2012a.html)

- **Description:**  
  This file contains a data table with 4 rows and 5 columns. The first row uses `<th>` elements to define headers: "Roll No", "Name", "Address", "DOB", and "Gender". The following rows contain sample student data.
- **Table Features:**
  - Red border (`border="3"` and `bordercolor="red"`)
  - Cell padding and spacing for better readability (`cellpadding="5"`, `cellspacing="5"`)
  - A caption ("Data Table") aligned at the bottom of the table
  - Demonstrates the use of table headers and data cells

### [📝 Lab 12b.html](Lab%2012b.html)

- **Description:**  
  This file contains a similar table structure (4 rows, 5 columns) but without any headers or data. All cells are empty, serving as a template or for practice.
- **Table Features:**
  - Red border (`border="3"` and `bordercolor="red"`)
  - Larger cell padding and spacing (`cellpadding="10"`, `cellspacing="10"`)
  - A caption ("Data Table") aligned at the bottom of the table
  - Useful for understanding the basic structure of an HTML table

## ✨ Key HTML Elements Used
- Both tables use a **red border**, cell padding, and cell spacing for improved readability.
- Demonstrates the use of:
- `<table>`: Defines the table.
- `<tr>`: Table row.
- `<th>`: Table header cell (bold and centered by default).
- `<td>`: Table data cell.
- `<caption>`: Table caption (description/title for the table).

## 🔍 How the Tables Work

- **Borders and Colors:**  
  The `border` and `bordercolor` attributes add a visible border to the table and set its color to red.
- **Cell Padding and Spacing:**  
  `cellpadding` controls the space inside each cell, while `cellspacing` controls the space between cells.
- **Captions:**  
  The `<caption>` tag provides a title for the table. The `align="bottom"` attribute places the caption below the table.

## 🚀 How to Use

1. Open either [Lab 12a.html](Lab%2012a.html) or [Lab 12b.html](Lab%2012b.html) in your web browser.
2. Observe the structure and formatting of the tables.
3. Use these examples as a reference for creating your own HTML tables.

## 📚 Learning Outcomes

- Understand the structure of HTML tables.
- Learn how to add headers, data, and captions to tables.
- Practice using table attributes for styling and layout.

## 🧩 FFurther Exploration

- Try adding more rows or columns to the tables.
- Experiment with different border colors, cell padding, and spacing values.
- Add more data or headers to customize the tables for different purposes.

---
For more information on HTML tables, see the [MDN Web Docs: Tables](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/table).
