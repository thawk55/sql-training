# SQL Types

1. boolean - Represented as `true` or `false`
2. Characters -
  * CHAR(n) - is the fixed-length character with space padded. For example CHAR(5) allows five characters and will add spaces to anything less than 5 and error on anything over 5.
  * VARCHAR(n) - is the variable-length character string. It uses up to n characters and does not pad with spaces.
  * TEXT - is the variable-length character string. It has no limit aside from database storage space.
3. Numeric -
  * SMALLINT - is 2-byte signed integer that has a range from -32,768 to 32,767
  * INT - is 4-byte signed integer that has a range from -2,147,483,648 to 2,147,483,647
  * SERIAL - same as INT but postgres will auto populate with the next number. 1, 2, 3, etc
  * FLOAT(n) - is a floating-point number whose precision, at least, n, up to a maximum of 8 bytes.
  * REAL or FLOAT8 - is a 4-byte floating-point number.
  * NUMERIC(p, s) - is a real number with p digits with s number after the decimal point.
3. Time -
  * DATE - stores the dates only.
  * TIME - stores the time of day values.
  * TIMESTAMP - stores both date and time values.
  * TIMESTAMPTZ - is a timezone-aware timestamp data type. It is the abbreviation for timestamp with the time zone.
  * INTERVAL - stores periods of time. '2 weeks'
4. Misc -
  * ARRAY - Allows you to store a list of numbers or strings.
  * JSON - stores plain JSON data that requires reparsing for each processing,
  * JSONB - stores JSON data in a binary format which is faster to process but slower to insert. In addition, JSONB supports indexing, which can be an advantage.
  * UUID - stores a UUID (type 4 specified by RFC 4122).


