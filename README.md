# Compliance Repo
A collection of various sensitive data types, faux data type sample sets, and their associated regular expression queries. Data sets such as these are useful for demonstrating and testing information protection and compliance tool rules.

### National Drug Code (NDC)
 - Reference [National Drug Code (NDC)](https://en.wikipedia.org/wiki/National_drug_code)

#### Finds 10-digit NDC (dashed) in 4-4-2 format:
RegEx: ```\d{4}-\d{4}-\d{2}$``` <br>
Example: 1111-2222-33

#### Finds 10-digit NDC (dashed) in 5-3-2 format:
RegEx: ```\d{5}-\d{3}-\d{2}$``` <br>
Example: 12345-678-90

#### Finds 10-digit NDC (dashed) in 5-4-1 format:
RegEx: ```\d{5}-\d{4}-\d{1}$``` <br>
Example: 54321-9876-5

#### Finds 10-digit NDC (dashed) in 6-3-2 format:
RegEx: ```\d{6}-\d{3}-\d{2}$``` <br>
Example: 654321-123-45

#### Finds 10-digit NDC (dashed) in 6-4-1 format:
RegEx: ```\d{6}-\d{4}-\d{1}$``` <br>
Example: 987654-3210-9

#### Finds 11-digit NDC (no dashes), HIPAA/CMS padded 5-4-2
RegEx: ```\d{11}$``` <br>
Example: 01234567890

#### Finds 12-digit NDC (dashed), proposed uniform 6-4-2 format
RegEx: ```\d{6}-\d{4}-\d{2}$``` <br>
Example: 123456-7890-12

#### Finds digit-only NDC strings of length 10, 11, or 12 (no dashes)
RegEx: ```\d{10,12}$``` <br>
Example (10): 1234567890 <br>
Example (11): 01234567890 <br>
Example (12): 123456789012 <br>






