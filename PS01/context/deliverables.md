PM04-PS01 – Model Answers
Task 1: PDD Analysis
### Process Breakdown

1. Monitor email inbox for new order emails
2. Download CSV attachment
3. Read CSV data into DataTable
4. Validate customer_id (8 digits)
5. Open browser → navigate to order system
6. Login using secure credentials
7. Loop through each order:
   - Enter customer_id, product_sku, quantity
   - Click "Add Item"
8. Submit order
9. Capture confirmation number
10. Send confirmation email
11. Handle errors (log + alert)

Task 1: Tool Selection
### Selected Tool: UiPath

### Justification:
- Strong web automation capabilities
- Built-in activities for email, CSV, browser
- Large community support in South Africa
- Easy integration with Orchestrator

Task 2: Validation Code (Pseudo)
If customer_id.Length = 8 And IsNumeric(customer_id) Then
    valid = True
Else
    valid = False
End If

Task 2: Problem-Solving (Dynamic UI)
Approach 1:
- Use dynamic selectors instead of fixed ID

Approach 2:
- Use Anchor Base or Find Element activity

Benefit:
- Handles UI changes automatically

Task 2: Handling Empty Quantity
If quantity Is Nothing OR quantity = "" Then
    quantity = 1
Else
    use original value
End If

Task 3: System Interaction
Components:
- Email → Outlook activity
- File System → Save CSV locally
- Web App → Browser automation
- Credentials → Orchestrator Assets

Task 3: Objects & Processes
Objects:
- Email
- CSV file
- Web browser
- Order system

Processes:
- Download file
- Read CSV
- Validate data
- Enter order
- Send confirmation

