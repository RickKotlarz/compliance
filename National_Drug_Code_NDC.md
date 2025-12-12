#### National Drug Code (NDC) Regular Expression (RegEx)
 - References
   - [National Drug Code (NDC)](https://en.wikipedia.org/wiki/National_drug_code)
   - [FDA Format of the National Drug Code(NDC)](https://www.fda.gov/media/173715/download)
   - [Non-official NDC code lookup](https://ndclist.com/)


#### Finds 10-digit NDC (dashed) in 4-4-2 format:
RegEx: (?<!\d)\d{4}-\d{4}-\d{2}(?!\d) <br>
Example: 1111-2222-33 <br>
Example (embedded): (1111-2222-33)

#### Finds 10-digit NDC (dashed) in 5-3-2 format:
RegEx: (?<!\d)\d{5}-\d{3}-\d{2}(?!\d) <br>
Example: 12345-678-90 <br>
Example (embedded): (12345-678-90)

#### Finds 10-digit NDC (dashed) in 5-4-1 format:
RegEx: (?<!\d)\d{5}-\d{4}-\d{1}(?!\d) <br>
Example: 54321-9876-5 <br>
Example (embedded): (54321-9876-5)

#### Finds 10-digit NDC (dashed) in 6-3-2 format:
RegEx: (?<!\d)\d{6}-\d{3}-\d{2}(?!\d) <br>
Example: 654321-123-45 <br>
Example (embedded): (654321-123-45)

#### Finds 10-digit NDC (dashed) in 6-4-1 format:
RegEx: (?<!\d)\d{6}-\d{4}-\d{1}(?!\d) <br>
Example: 987654-3210-9 <br>
Example (embedded): (987654-3210-9)

#### Finds 11-digit NDC (no dashes), HIPAA/CMS padded 5-4-2
RegEx: (?<!\d)\d{11}(?!\d) <br>
Example: 01234567890 <br>
Example (embedded): (01234567890)

#### Finds 12-digit NDC (dashed), proposed uniform 6-4-2 format
RegEx: (?<!\d)\d{6}-\d{4}-\d{2}(?!\d) <br>
Example: 123456-7890-12 <br>
Example (embedded): (123456-7890-12)

#### Finds digit-only NDC strings of length 10, 11, or 12 (no dashes)
RegEx: (?<!\d)\d{10,12}(?!\d) <br>
Example (10): 1234567890 <br>
Example (11): 01234567890 <br>
Example (12): 123456789012 <br>
Example (embedded): (123456789012)
