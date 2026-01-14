# JSON for Sheets

**Robust, analyst-friendly JSON Functions for Google Sheets™.**

[Privacy Policy](privacy.html) | [Terms of Service](terms.html) | [Home](index.html)

---

## Overview

**JSON for Sheets** creates a bridge between complex data structures and your spreadsheets. Whether you are working with API responses, configuration files, or complex logs, this add-on brings the power of structural data parsing directly into your Google Sheets workflow.

Stop manually copying and pasting JSON or struggling with complex scripts. Use native-like formulas to parse, filter, and transform JSON data instantly.

## Key Features

### 🚀 Powerful Formulas

Unlock a suite of custom functions designed for data analysts and developers:

- **`=PARSE_JSON(json_string)`**
  Convert JSON strings into readable, flattened 2D tables or key-value maps instantly.

- **`=JSON_GET(json_string, path)`**
  Extract specific values using intuitive dot and bracket notation (e.g., `user.address.city` or `items[0].id`).

- **`=JSON_TO_TABLE(json_array)`**
  Transform arrays of objects into structured tables with automatic headers. Perfect for API lists.

- **`=JSON_FILTER(json_array, expression)`**
  Filter JSON arrays directly in your formula using simple expressions like `age > 21` or `status == "active"`.

- **`=JSON_VALIDATE(json_string, schema)`**
  Validate your JSON integrity against a defined schema to ensure data quality.

### 🔒 Secure & Private

- **Local Execution:** All data processing happens locally within your Google Sheets execution environment.
- **No External Servers:** Your data does not leave Google's infrastructure to be processed by our servers.

## Installation

1. Open a Google Sheet.
2. Go to **Extensions** > **Add-ons** > **Get add-ons**.
3. Search for **"JSON for Sheets"**.
4. Click **Install** and grant the necessary permissions.

_(Link to Google Workspace Marketplace coming soon)_

## Usage Examples

### 1. Extracting a Single Value

Got a cell `A1` with JSON content: `{"id": 101, "name": "Alice"}`?

```excel
=JSON_GET(A1, "name")
```

**Result:** `Alice`

### 2. Converting API Data to a Table

If cell `A1` contains a JSON array of users:

```excel
=JSON_TO_TABLE(A1)
```

**Result:** A dynamic table expanding to fit all rows and columns from the JSON data.

### 3. Filtering Data on the Fly

Filter a list of orders in `A1` where the total is greater than 100:

```excel
=JSON_FILTER(A1, "total > 100")
```

## Why Choose JSON for Sheets?

- **SEO & Data Analysis Friendly:** Perfect for SEO professionals importing structured data (Schema markup) or analysts working with REST APIs.
- **No Coding Required:** You don't need to write Apps Script code to handle JSON.
- **Performance:** Optimized for speed and reliability within the Sheets environment.

## Support & Legal

- **Privacy Policy:** [Read here](privacy.html)
- **Terms of Service:** [Read here](terms.html)

---

_Google Sheets™ is a trademark of Google LLC._
