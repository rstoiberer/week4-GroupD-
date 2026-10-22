# week4-GroupD-
In class competition week 4 - Anissa, Kay, Javier, Richard


### ✍️ Decision log, checkpoint 1: load and verify

**Driver:** (name) · **Navigator(s):** (names)

| What we found (with a count) | What we decided | Justification (one line) |
|---|---|---|
| Checksum matches the published SHA-256 | Use this file; read every column as text | The file is the one published, and reading as text hides nothing before we look |
| 131 rows against 127 published (4 extra) | Keep all rows for now; explain the extra 4 in checkpoints 2 and 5 | Deleting before we know why would hide the cause |
| Non-numbers in numeric columns: `""`, `n/a`, `..`, thousands separators; a `-999` population; a "Total" row | Carry the list forward to checkpoints 2, 7 and 8 | Each needs a different treatment, decided where it belongs |

*This is a model entry for the decision log: every row show invclude a count where applicable, a decision, and one line of justification.*

### ✍️ Decision log, checkpoint 2: structure and types

**Driver:** ____ · **Navigator(s):** ____

| What we found (with a count) | What we decided | Justification (one line) |
|---|---|---|
| There is a row Total (1) | We will remove this | This is not an observation |
| Leading and trailing spaces () | Strip the leading and trailing spaces |To ensure proper merging of data frames on the same keys |
| Non-conventional representation of missing values () | Make them all NA uniformly |To treat all the missing values the same|
| Some numbers have commas as thousands separators, others don't () | Remove the commas | To ensure uniform notation of numbers|
| Year is coded as an object Dtype() | We changed the type to int16 | To ensure that our objects have the proper data types|



### ✍️ Decision log, checkpoint 3: text and categories

**Driver:** ____ · **Navigator(s):** ____

| What we found (with a count) | What we decided | Justification (one line) |
|---|---|---|
|There are ISO3 country codes which were not capitalised() |Decided to capitalise them | We want to ensure consistency among country codes|
|We spot encoding errors for country names |Decided map all countries correctly with the country ISO3 country codes | We want to ensure consistent mapping between ISO3 and country names|
|We found inconsistencies in income group names() |Decided to lower case, replacing dashes with "", stripping leading and trailing whitespaces, and ensuring every label name ends with "income"| We want to ensure consistency among income groups|


### ✍️ Decision log, checkpoint 4: dates

**Driver:** ____ · **Navigator(s):** ____

| What we found (with a count) | What we decided | Justification (one line) |
|---|---|---|
| | | |


### ✍️ Decision log, checkpoint 5: duplicates

**Driver:** ____ · **Navigator(s):** ____

| What we found (with a count) | What we decided | Justification (one line) |
|---|---|---|
| | | |

### ✍️ Decision log, checkpoint 6: units and scales

**Driver:** ____ · **Navigator(s):** ____

| What we found (with a count) | What we decided | Justification (one line) |
|---|---|---|
| | | |

### ✍️ Decision log, checkpoint 7: impossible and implausible values

**Driver:** ____ · **Navigator(s):** ____

| What we found (with a count) | What we decided | Justification (one line) |
|---|---|---|
| | | |

### ✍️ Decision log, checkpoint 8: missing values ⚖️

**Driver:** ____ · **Navigator(s):** ____

| What we found (with a count) | What we decided | Justification (one line) |
|---|---|---|
| | | |

**Write your argument about the contested checkpoint (at most five sentences)**: State the evidence (share missing, pattern by income group, likely mechanism); say what the **other** option would have gained; state the consequence of your choice for an analysis that uses this variable.

*Our argument:*

### ✍️ Decision log, checkpoint 9: validate and save

**Driver:** ____ · **Navigator(s):** ____

| What we found (with a count) | What we decided | Justification (one line) |
|---|---|---|
| | | |
