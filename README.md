# Product Table
## Date: 8/7/25
## Objective:

To create a structured HTML table that displays product-related information, including product names, prices, and descriptions, useful for catalogs, listings, or e-commerce prototypes.

## Tasks:

### 1. Set Up the Basic HTML Structure:

Use ```<!DOCTYPE html>```, ```<html>```, ```<head>```, and ```<body>``` tags to define the document layout.

Include a ```<title>``` such as "Product Table".

### 2. Create a Table Element:

Use the ```<table>``` tag to begin the product table.

### 3. Add a Table Header:

Use the ```<thead>``` section with a ```<tr>``` row and three ```<th>``` elements:

Product Name

Product Price

Description

### 4. Insert Table Body Rows:

Use the ```<tbody>``` section with multiple ```<tr>``` rows.

In each row, use three ```<td>``` cells for:

The name of the product (e.g., Laptop, Phone)

The price (e.g., ₹45,000, $499)

A short description (e.g., "High-speed performance", "Budget-friendly")

### 5. Ensure Semantic Structure:

Include ```<caption>``` if needed to describe the table purpose.

Use meaningful text inside the table for clarity.

### 6. No CSS or JavaScript:

Keep the table design strictly in HTML for simplicity.
## HTML Code:
```
index.html

<!DOCTYPE html>
<html>
<head>
    <title>Product Table</title>
</head>
<body>

    <h1>Product Catalog</h1>

    <table border="1">
        <caption>List of Available Products</caption>

        <thead>
            <tr>
                <th>Product Name</th>
                <th>Product Price</th>
                <th>Description</th>
            </tr>
        </thead>

        <tbody>
            <tr>
                <td>Laptop</td>
                <td>₹45,000</td>
                <td>High-speed performance for multitasking</td>
            </tr>
            <tr>
                <td>Smartphone</td>
                <td>$499</td>
                <td>Budget-friendly with great features</td>
            </tr>
            <tr>
                <td>Headphones</td>
                <td>₹2,999</td>
                <td>Wireless and noise-cancelling</td>
            </tr>
            <tr>
                <td>Tablet</td>
                <td>$299</td>
                <td>Lightweight and perfect for reading</td>
            </tr>
        </tbody>
    </table>

</body>
</html>
```
```
style.css

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: linear-gradient(to right, lightcyan, lightblue);
    margin: 40px;
    color: navy;
}

h1 {
    text-align: center;
    color: steelblue;
    font-size: 2.5em;
    margin-bottom: 20px;
}

table {
    width: 80%;
    margin: 0 auto;
    border-collapse: collapse;
    box-shadow: 0 8px 16px rgba(70, 130, 180, 0.2);
    background-color: aliceblue;
    border-radius: 8px;
    overflow: hidden;
}

caption {
    caption-side: top;
    padding: 12px;
    font-size: 1.3em;
    font-weight: bold;
    color: navy;
}

thead {
    background-color: steelblue;
    color: white;
}

th, td {
    padding: 16px 20px;
    text-align: left;
}

tbody tr:nth-child(even) {
    background-color: lightsteelblue;
}

tbody tr:hover {
    background-color: lightskyblue;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

td:nth-child(2) {
    font-weight: bold;
    color: deepskyblue;
}

@media (max-width: 768px) {
    table, thead, tbody, th, td, tr {
        display: block;
    }

    thead {
        display: none;
    }

    tr {
        margin-bottom: 20px;
        border-bottom: 1px solid skyblue;
    }

    td {
        position: relative;
        padding-left: 50%;
    }

    td::before {
        position: absolute;
        top: 16px;
        left: 16px;
        width: 45%;
        padding-right: 10px;
        white-space: nowrap;
        font-weight: bold;
        color: dodgerblue;
    }

    td:nth-child(1)::before { content: "Product Name"; }
    td:nth-child(2)::before { content: "Product Price"; }
    td:nth-child(3)::before { content: "Description"; }
}
```

## Output:
![image](https://github.com/user-attachments/assets/7612b851-26b3-4bf6-94c0-8d13ed6f0989)
![image](https://github.com/user-attachments/assets/9bfef6aa-1e82-4e49-86e4-06a0e4d8f6b7)


## Result:
A structured HTML table that displays product-related information, including product names, prices, and descriptions, useful for catalogs, listings, or e-commerce prototypes is created successfully.
