#### National Drug Code (NDC) Regular Expression (RegEx)
 - References
   - [National Drug Code (NDC)](https://en.wikipedia.org/wiki/National_drug_code)
   - [FDA Format of the National Drug Code(NDC)](https://www.fda.gov/media/173715/download)
   - [Non-official NDC code lookup](https://ndclist.com/)
   - [RegEx tool](https://regexr.com/)

#### Digit-only NDC strings of length 10, 11, or 12 (with or without dashes) format

(?<!\d)(?:\d{4}-\d{4}-\d{2}|\d{5}-\d{3}-\d{2}|\d{5}-\d{4}-\d{1}|\d{6}-\d{3}-\d{2}|\d{6}-\d{4}-\d{1}|\d{6}-\d{4}-\d{2}|\d{10}|\d{11}|\d{12})(?!\d)
Example (10): 1234567890 <br>
Example (11): 01234567890 <br>
Example (12): 123456789012 <br>
Example (12): 123456-7890-12 <br>
Example (embedded): (123456789012)

#### 10-digit NDC (dashed) in 4-4-2 format
(?<!\d)\d{4}-\d{4}-\d{2}(?!\d) <br>
Example: 1111-2222-33 <br>
Example (embedded): (1111-2222-33)

#### 10-digit NDC (dashed) in 5-3-2 format
(?<!\d)\d{5}-\d{3}-\d{2}(?!\d) <br>
Example: 12345-678-90 <br>
Example (embedded): (12345-678-90)

#### 10-digit NDC (dashed) in 5-4-1 format
(?<!\d)\d{5}-\d{4}-\d{1}(?!\d) <br>
Example: 54321-9876-5 <br>
Example (embedded): (54321-9876-5)

#### 10-digit NDC (dashed) in 6-3-2 format
(?<!\d)\d{6}-\d{3}-\d{2}(?!\d) <br>
Example: 654321-123-45 <br>
Example (embedded): (654321-123-45)

#### 10-digit NDC (dashed) in 6-4-1 format
(?<!\d)\d{6}-\d{4}-\d{1}(?!\d) <br>
Example: 987654-3210-9 <br>
Example (embedded): (987654-3210-9)

#### 11-digit NDC (dashed) in 5-4-2 format
(?<!\d)\d{5}-\d{4}-\d{2}(?!\d)
Example: 01234-5678-90 <br>
Example (embedded): (01234-5678-90)

#### 12-digit NDC (dashed), proposed uniform 6-4-2 format
(?<!\d)\d{6}-\d{4}-\d{2}(?!\d) <br>
Example: 123456-7890-12 <br>
Example (embedded): (123456-7890-12)
