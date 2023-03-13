# Coding with ChatGPT - PostgreSQL

## [PostgreSQL] Lowercase

```dos
In my postgreSQL, I create a new table like this

CREATE TABLE TEST_TRTMT (
   TEST_TRTMT_ID        BIGSERIAL            NOT NULL
)

Why both the table name and column name became lowercase when I checked it with pgAdmin?
```

PostgreSQL automatically converts unquoted identifiers (such as table and column names) to lowercase, unless they are enclosed in double quotes. So in your CREATE TABLE statement, the table name and column name are not enclosed in double quotes, hence PostgreSQL automatically converts them to lowercase.

If you want to use a specific capitalization for your table or column names, you can enclose them in double quotes like this:

```sql
CREATE TABLE "TEST_Trtmt" (
   "TEST_Trtmt_ID"        BIGSERIAL            NOT NULL
);
```

However, it's generally not recommended to use quoted identifiers in PostgreSQL as they can make your SQL queries harder to read and may cause issues when referencing the table or column name in other parts of your code.
