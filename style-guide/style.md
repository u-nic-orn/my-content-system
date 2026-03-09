# Style

The devil's in the details. Stick to these style rules for consistent texts.

## Abbreviations
If you use an abbreviation that isn't generally known, explain what it means. If it appears several times, write out the full term the first time and include the abbreviation in brackets next to it. After that, you can use the abbreviation on its own.

| ✓ Do | ✗ Don't |
|------|---------|
| API (Application Programming Interface) | LTD (Limited Company)<br/>LLC (Limited Liability Company)<br/>SMB (Small and Medium-sized Business) |

## User names — order of first and last name
This documents the current situation. Ideally, it would be consistent everywhere. Due to organic growth, this serves as a reminder not to introduce further inconsistencies.

### Office
`[Last name][Space][First name]`

| ✓ Do |
|------|
| Honeybadger Harriet |

### Payroll
`[Last name][Comma][Space][First name]`

| ✓ Do |
|------|
| Honeybadger, Harriet |

### Cockpit
`[First name][Space][Last name]`

| ✓ Do |
|------|
| Harriet Honeybadger |

## Receipt, scan, file or document

### Receipt
Specialist jargon used by fiduciaries and accountants. If you're speaking to end users as well, avoid this term.

### Scan
Use this term in bexio Go for scans created with the scanner function.

### File
Use "file" whenever multiple file formats can be uploaded.

### Document
Documents are quotes, orders, invoices and delivery notes. Bills and expenses are accounting transactions. The real-world documents behind them are called invoice and receipt.

## Sections in bexio
When referring to a part of bexio, call it a section.

| ✓ Do | ✗ Don't |
|------|---------|
| Purchase section<br/>Sales section<br/>Contacts section<br/>Banking section | Module<br/>Component |

## bexio [department] team
Name all departments consistently. If you explicitly label teams as belonging to bexio, write either "bexio support team" or "support team at bexio".

| ✓ Do | ✗ Don't |
|------|---------|
| Product team<br/>Support team<br/>Consulting team<br/>Fiduciary partner team<br/>Marketing team<br/>Development team<br/>HR and Finance team | Sales team<br/>bexio Marketing Team<br/>bexio-Marketing-Team<br/>bexio Marketing-Team<br/>XY department |

## bexio-[noun]
When combining bexio with a German noun, always use a hyphen.

| ✓ Do | ✗ Don't |
|------|---------|
| bexio-Support<br/>bexio-Team<br/>bexio-Schulung<br/>bexio-Support-Team | bexio Team<br/>bexio Support<br/>bexio Zukunftstag |

## Button texts

### Create a new item
Always start with the verb "New" and add the name of the item afterwards. As usual, there are exceptions, such as inviting another user or adding standard positions to a quote, invoice etc.

| ✓ Do | ✗ Don't |
|------|---------|
| New invoice<br/>New contact<br/>New time tracking | Create new invoice<br/>Add new contact<br/>+ time tracking |

## Contractions
Our users' time is precious and space in UIs is limited. Always use contractions.

| ✓ Do | ✗ Don't |
|------|---------|
| Can't<br/>Won't<br/>Don't | Can not<br/>Will not<br/>Do not |

## Empty states
Empty states are a sales opportunity. Good empty states contain 3 things:

- A clear title stating that no content is available
- Text explaining what would be shown if content existed and what purpose that content serves
- A call to action with a link or button leading directly to a new data entry

More on punctuation: see [No full stops in](#no-full-stops-in).

| ✓ Do |
|------|
| **((Title))**<br/>No invoices created<br/><br/>**((Body copy))**<br/>Here you can see whether invoices are outstanding, paid or overdue. You can also send multiple invoices by email from here.<br/><br/>**((Call to action))**<br/>Create an invoice now |

## Export

### File names
Always use this structure: `bexio_export_[area-name]_[timestamp].[file-format]`.<br/>Use the English name of the area.
The timestamp contains the year and the time. Use this format: `YYYYMMDDHHMMSS`.

If apostrophes are used, replace them with an underscore. This applies to French and Italian. Apostrophes sometimes cause errors.

| ✓ Do | ✗ Don't |
|------|---------|
| bexio_export_contacts_20220217125532.xlsx<br/>bexio_export_invoices_20220217125912.xlsx | contacts.xlsx |

## Formats

### Date
Use the European date format `DD.MM.YYYY`.

| ✓ Do | ✗ Don't |
|------|---------|
| 01.01.2020<br/>15.04.2020<br/>31.12.2020 | 15.4.20<br/>01.01.20<br/>4.15.20<br/>15 April 2020 |

### File formats
Write file formats in uppercase.

| ✓ Do | ✗ Don't |
|------|---------|
| ZIP<br/>XLSX<br/>PDF | zip<br/>xlsx<br/>pdf |

### Time
Always use the format `HH:MM`. This is easier to read when multiple times appear in a table.

| ✓ Do | ✗ Don't |
|------|---------|
| 05:40<br/>13:22<br/>03:53 | 5:40<br/>13:22<br/>3:53 |

## Error messages
How will the error be displayed? A toast, a dialog or something else? Write what is possible and follow these steps:

- Describe the problem as precisely as possible.
- Suggest a possible solution. If there's no solution, explain the next steps or who the users can contact.
- Add the error code as a placeholder, if available.

> **Note:** Always let your developer know when a placeholder should be used. Never write the error code directly.

| ✓ Do | ✗ Don't |
|------|---------|
| This invoice date is in a closed fiscal year. Change the date or ask our support to open the fiscal year.<br/><br/>Send us your company name and which year you want to open at support@bexio.com.<br/>Error code: XXX | You cannot create an invoice in a closed fiscal year. |

## Sentence case
Always use sentence case. You only use capital letters in the beginning of a sentence or text and for proper nouns. Proper nouns are days of the week, months, names etc.

| ✓ Do | ✗ Don't |
|------|---------|
| Add another shop<br/>View<br/>Save<br/>Dashboard<br/>Sales | add another shop<br/>view<br/>save<br/>dashboard<br/>sales |

## Downloadable content
Indicate the format and file size, if the size is clearly known. Use uppercase for the format and insert a space between number and format.

| ✓ Do | ✗ Don't |
|------|---------|
| Export the plug-in as a ZIP file (25 KB) | Export the plug-in |

## Input validation
Write the message in a positive way. State what needs to be done to make it work, instead of what is wrong. Avoid a full stop at the end. More on punctuation: see [No full stops in](#no-full-stops-in).

| ✓ Do | ✗ Don't |
|------|---------|
| Enter the same password in both fields<br/>Enter a valid email address | Password missing.<br/>Required.<br/>Incorrect email address. |

## No full stops in
- Mobile toast titles and text
- Labels — no colons either
- Titles of any kind
- Notes in the user interface
- Input validations
- Stand-alone calls to action in empty states

| ✓ Do | ✗ Don't |
|------|---------|
| This bank account is not connected<br/>Include invoices that are 10 days overdue<br/>Enter the same password in both fields | This bank account is not connected.<br/>Include invoices that are 10 days overdue.<br/>Enter the same password in both fields. |

## Addressing users
Always address users directly and use the polite form "Sie" in German. Use a conversational style. Write in the "we" form.

| ✓ Do | ✗ Don't |
|------|---------|
| Define in the settings that …<br/>Send your emails directly via …<br/>Which documents shall we create?<br/>How would you like to pay? | How can I help you? |

## Modals

### Texts
Texts in modals start with the most important information. What happens if the user continues? What are the consequences?

| ✓ Do | ✗ Don't |
|------|---------|
| Your credit will be charged if … | If you send this invoice via InvoCLOUD, your credit will be charged. |

### Buttons
Buttons always answer the question asked in the modal title. Imagine a conversation: what would you ask and what would the other person reply?

| ✓ Do | ✗ Don't |
|------|---------|
| **((Title))**<br/>Switch for all bank accounts?<br/><br/>**((Primary action))**<br/>Switch all<br/><br/>**((Secondary action))**<br/>No, only for this bank account | **((Title))**<br/>Switch for all bank accounts?<br/><br/>**((Primary action))**<br/>Yes<br/><br/>**((Secondary action))**<br/>Cancel |

## Password requirements
Always show the password requirements when users need to set a password. Few things are more annoying than an error message after coming up with a password. Learn more from our friends at Nielsen Norman Group: [Disclosing Password Constraints in the UI](https://www.nngroup.com/videos/disclosing-password-constraints/).

- Write what needs to be done so that it works, instead of everything the password must fulfil.
- Use bullet points — they are easier to scan.
- Use digits instead of written-out numbers.

## Tabs
Use the name of the section or the title of the opened page for browser tabs. The format is: `[Title][Space]|[Space][bexio]`. This ensures users can orient themselves when multiple tabs are open.

| ✓ Do | ✗ Don't |
|------|---------|
| Banking \| bexio<br/>Invoice 223-431 \| bexio<br/>New payment order \| bexio | bexio<br/>bexio \| Contacts |

## Toasts

### Mobile
Keep it short.

## Thousands and decimal separators
We follow the rules for Switzerland and the United Kingdom.

### Switzerland
Thousands separator = `'` (apostrophe)<br/>
Decimal separator = `.` (dot)

Group large numbers in sets of three: 1'000'000.50. We deviate from the Duden guidelines — like banks — because this format is easier to read.

See [Apostrophe](./typographical-signs.md#apostrophe) for how to insert a correct apostrophe.

### United Kingdom
Thousands separator = `,` (comma)<br/>
Decimal separator = `.` (dot)

Group large numbers in sets of three: 1,000,000.50.

### Exception
Before we had an accounting module and before we became part of Mobiliar, we intended to serve the German and Austrian markets as well. For this reason, there are certain localisation approaches for these two countries. In the profile settings you can choose between these three German variants:

- German (Switzerland)
- German (Germany)
- German (Austria)

This mainly affects thousand and decimal separators. We didn't get much further than that. In Germany and Austria, the separators are the same:

#### Germany and Austria
Thousands separator = `.` (dot)<br/>
Decimal separator = `,` (comma)

Group large numbers in sets of three: 1.000.000,50.

## Underlining
We operate in a web environment. Never underline normal text — underlining is reserved for links.

## Currency abbreviations with amounts
Use this format when you combine currencies and amounts: `[ISO currency code][non-breaking space][amount]`. In a list view with a fixed order, ensure that the currency code always comes before the amount.

See [Non-breaking space](./typographical-signs.md#non-breaking-space) for how to insert one.

| ✓ Do | ✗ Don't |
|------|---------|
| CHF 1'435.65 | 1'435.65 CHF<br/>1'435.65$ |

## Time or time tracking
When the user records a time, refer to it as time tracking. If times are already recorded, refer to them as time or times. So if the user is at a place where they record a time, that's time tracking. They can then find the times in the time overview. They can also import times.

| ✓ Do | ✗ Don't |
|------|---------|
| Import times to invoices<br/>You are in a time tracking view | Copy time trackings into a new project<br/>Create a new time to start recording |
