Data Types
Structured: CSV (billing data)
Unstructured: PDF (tenders)

VAT Calculation (UiPath)
VAT = AmountDue * 0.15
Total = AmountDue + VAT


Average Usage
avg = dt.AsEnumerable().Average(Function(x) x("ElectricityUnits"))


Collections
Array → Customer IDs
Dictionary → Monthly totals

Regex
[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-z]{2,}

