
# AMPscript

## Overview

AMPscript is Salesforce Marketing Cloud's scripting language used to create dynamic and personalized email content. It helps marketers customize emails based on subscriber data, preferences, and behaviors.

## Skills Covered

* Personalization
* Dynamic Content
* Conditional Logic
* Data Extension Lookup
* Subscriber Data Management
* Email Customization

---

## Project 1: Personalized Greeting

### Objective

Display the subscriber's first name dynamically in the email.

### AMPscript

```ampscript
%%[
SET @FirstName = AttributeValue("FirstName")
]%%

Hello %%=v(@FirstName)=%%,
```

### Output

```text
Hello John,
```

### Outcome

Improved email personalization and customer engagement.

---

## Project 2: Conditional Content

### Objective

Display different content based on customer membership type.

### AMPscript

```ampscript
%%[
SET @MemberType = AttributeValue("MemberType")

IF @MemberType == "Premium" THEN
]%%

Thank you for being a Premium Member!

%%[
ELSE
]%%

Upgrade today to enjoy Premium Benefits.

%%[
ENDIF
]%%
```

### Outcome

Delivered targeted messaging based on customer segments.

---

## Project 3: Data Extension Lookup

### Objective

Retrieve customer information from a Data Extension.

### AMPscript

```ampscript
%%[
SET @Email = AttributeValue("EmailAddress")
SET @Rows = LookupRows("Customer_DE","EmailAddress",@Email)

IF RowCount(@Rows) > 0 THEN

SET @Row = Row(@Rows,1)
SET @City = Field(@Row,"City")

ENDIF
]%%

Your City: %%=v(@City)=%%
```

### Outcome

Displayed customer-specific information dynamically.

---

## Project 4: Birthday Email Personalization

### Objective

Send personalized birthday wishes.

### AMPscript

```ampscript
%%[
SET @FirstName = AttributeValue("FirstName")
]%%

Happy Birthday %%=v(@FirstName)=%%!

We wish you a wonderful year ahead.
```

### Outcome

Enhanced customer experience through personalized communication.

---

## Common AMPscript Functions

### AttributeValue()

Used to retrieve subscriber attributes.

```ampscript
AttributeValue("FirstName")
```

### LookupRows()

Retrieves records from a Data Extension.

```ampscript
LookupRows("Customer_DE","SubscriberKey",@SubscriberKey)
```

### RowCount()

Returns the number of rows.

```ampscript
RowCount(@Rows)
```

### Field()

Returns a field value from a row.

```ampscript
Field(@Row,"City")
```

### IF / ELSE

Used for conditional logic.

```ampscript
IF @Status == "Active" THEN
```

---

## Tools Used

* Salesforce Marketing Cloud
* Content Builder
* Email Studio
* Data Extensions
* AMPscript

---

## Outcome

Implemented personalized and dynamic email experiences using AMPscript, resulting in improved customer engagement, targeted communication, and enhanced campaign performance.
