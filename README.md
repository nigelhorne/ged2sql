ged2sql
=======

Import genealogical data from a GEDCOM file into an SQLite database.
It uses Gedcom for parsing, DBI for database interactions, and Lingua::EN modules for name normalization.

# Command Line Options

| Flag | Meaning |
| ---- | ------- |
| -f   | treat warnings as fatal, implies -w |
| -s   |  Name of sqlite file (default is out.sql) |
| -w   | print warnings |

# Schema Design

Tables: people, siblings, children, spouses.

Foreign key constraints enforce relational integrity.
