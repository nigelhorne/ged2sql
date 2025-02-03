# ged2sql

Import genealogical data from a GEDCOM file into an SQLite database.
It uses Gedcom for parsing, DBI for database interactions, and Lingua::EN modules for name normalization.

# Schema Design

Tables: people, siblings, children, spouses.

Foreign key constraints enforce relational integrity.
