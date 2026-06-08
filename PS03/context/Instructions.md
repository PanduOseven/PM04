Platform Selection
Tool: UiPath

Reason:
- Enterprise-grade
- Secure credential management
- Strong logging

 High-Level Workflow
1. Read CSV
2. Loop through records
3. Validate SA ID
4. Open browser
5. Enter data
6. Retrieve status
7. Update file

Custom Code (SA ID Validation)
Function ValidateID(id As String) As Boolean
    If id.Length = 13 And IsNumeric(id) Then
        Return True
    Else
        Return False
    End If
End Function

Error Handling Table
| Scenario | Type | Handling |
|----------|------|---------|
| File missing | System | Stop + alert |
| Invalid ID | Business | Skip |
| UI error | Technical | Retry |

Logging Strategy
- Start process
- Each record processed
- Errors
- Completion summary

Dynamic Values
Stored in config:
- File path
- URL
- Credentials

Managed via:
- Orchestrator assets



