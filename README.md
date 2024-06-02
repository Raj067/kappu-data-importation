### Data Import Guide for Kikoba System

This document provides instructions for preparing and importing data into the Kikoba system. The data will be prepared in an Excel spreadsheet, and non-technical users are expected to follow this structure closely. The template structure provided here ensures that the data is correctly formatted and easily importable.

#### Overall Structure

The data must be structured in a JSON-like format within the Excel sheet, which includes information about the Kikoba group, users, and various transactions. Here is a detailed explanation of each section and its required fields.

### Kikoba Group Details

This section contains the primary details of the Kikoba group.

- **kikoba_name**: The name of the Kikoba group. This field is required.
- **kikoba_number**: A unique identifier for the Kikoba group. This field is required.
- **location**: The location of the Kikoba group. This field is optional.

### Users

This section lists all users associated with the Kikoba group. Each user has several fields:

- **phone**: The user's phone number. This field is required.
- **email**: The user's email address. This field is optional.
- **first_name**: The user's first name. This field is optional.
- **middle_name**: The user's middle name. This field is optional.
- **last_name**: The user's last name. This field is optional.
- **status**: The user's status, which can be either "active" or "banned". This field is required.

### Transactions

This section contains various types of transactions related to the Kikoba group.

#### Withdrawals

- **amount**: The amount of the withdrawal. This field should be a number.
- **description**: A description of the withdrawal. This field is optional.

#### Hisa (Shares)

- **phone**: The phone number of the user associated with the hisa. This field is required.
- **amount**: The amount of the hisa. This field is required.

#### Fines

- **phone**: The phone number of the user associated with the fine. This field is required.
- **amount**: The amount of the fine. This field is required.

#### Michango Category

- **name**: The name of the michango category. This field is required.
- **amount**: The amount associated with the michango category. This field is required.

#### Michango

- **phone**: The phone number of the user associated with the michango. This field is required.
- **amount**: The amount of the michango. This field is required.

#### Loans

- **phone**: The phone number of the user associated with the loan. This field is required.
- **amount**: The amount of the loan. This field is required.
- **status**: The status of the loan. This field is required.
- **repayment**: The repayment amount of the loan. This field is required.

### Excel Template Structure

The Excel file should have the following columns and corresponding data. Each row should represent a unique entry for users or transactions.

#### Sheet: Kikoba Group

| kikoba_name | kikoba_number | location |
|-------------|---------------|----------|
| ExampleGroup | 12345         | Location1|

#### Sheet: Users

| phone       | email          | first_name | middle_name | last_name | status  |
|-------------|----------------|------------|-------------|-----------|---------|
| 1234567890  | user@example.com | John       | A.          | Doe       | active  |

#### Sheet: Transactions

##### Withdrawals

| amount | description      |
|--------|------------------|
| 100.00 | Withdrawal Note  |

##### Hisa

| phone       | amount |
|-------------|--------|
| 1234567890  | 50.00  |

##### Fines

| phone       | amount |
|-------------|--------|
| 1234567890  | 20.00  |

##### Michango Category

| name        | amount |
|-------------|--------|
| Category1   | 30.00  |

##### Michango

| phone       | amount |
|-------------|--------|
| 1234567890  | 40.00  |

##### Loans

| phone       | amount | status | repayment |
|-------------|--------|--------|-----------|
| 1234567890  | 200.00 | active | 20.00     |

### Preparing the Data

1. **Create a new Excel file** with multiple sheets named "Kikoba Group", "Users", "Withdrawals", "Hisa", "Fines", "Michango Category", "Michango", and "Loans".
2. **Fill in the data** according to the structure provided above. Ensure all required fields are populated and optional fields are filled as needed.
3. **Save the Excel file** and review it to ensure the data is accurate and correctly formatted.

### Example Excel Layout

Here is an example of how your Excel file should be structured:

#### Kikoba Group Sheet

| kikoba_name  | kikoba_number | location |
|--------------|---------------|----------|
| ExampleGroup | 12345         | ExampleLocation |

#### Users Sheet

| phone       | email            | first_name | middle_name | last_name | status |
|-------------|------------------|------------|-------------|-----------|--------|
| 1234567890  | user1@example.com | John       | A.          | Doe       | active |
| 2345678901  | user2@example.com | Jane       | B.          | Smith     | banned |

#### Withdrawals Sheet

| amount | description         |
|--------|---------------------|
| 100.00 | Example Withdrawal  |

#### Hisa Sheet

| phone       | amount |
|-------------|--------|
| 1234567890  | 50.00  |

#### Fines Sheet

| phone       | amount |
|-------------|--------|
| 1234567890  | 20.00  |

#### Michango Category Sheet

| name        | amount |
|-------------|--------|
| Category1   | 30.00  |

#### Michango Sheet

| phone       | amount |
|-------------|--------|
| 1234567890  | 40.00  |

#### Loans Sheet

| phone       | amount | status | repayment |
|-------------|--------|--------|-----------|
| 1234567890  | 200.00 | active | 20.00     |

### Importing the Data

Once the data is prepared and saved in the Excel file, it can be imported into the Kikoba system using the provided import script. Ensure that the data adheres to the structure and format detailed above to avoid any import errors.
