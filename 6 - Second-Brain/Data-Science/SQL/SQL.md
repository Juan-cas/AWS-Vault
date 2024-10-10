2024-09-28 22:07

Status:

Tags:
[[Data science]]
# SQL

[SELECT](obsidian://open?vault=GluGlu&file=6%20-%20Second-Brain%2FData-Science%2FSQL%2FSELECT%20*) customerid, city, country [FROM](obsidian://open?vault=GluGlu&file=6%20-%20Second-Brain%2FData-Science%2FSQL%2FFROM) customers [ORDER BY](obsidian://open?vault=GluGlu&file=6%20-%20Second-Brain%2FData-Science%2FSQL%2FORDER%20BY) city;

would provide an output like:

+------------+--------------+----------------+
| CustomerId | City         | Country        |
+------------+--------------+----------------+
|         48 | Amsterdam    | Netherlands    |
|         59 | Bangalore    | India          |
|         36 | Berlin       | Germany        |
|         38 | Berlin       | Germany        |
|         42 | Bordeaux     | France         |
|         23 | Boston       | USA            |

you could make it sort in descend order:

+------------+---------------------+----------------+
| CustomerId | City                | Country        |
+------------+---------------------+----------------+
|         33 | Yellowknife         | Canada         |
|         32 | Winnipeg            | Canada         |
|         49 | Warsaw              | Poland         |
|          7 | Vienne              | Austria        |
|         15 | Vancouver           | Canada         |
|         27 | Tucson              | USA            |

another example would be:

[SELECT](obsidian://open?vault=GluGlu&file=6%20-%20Second-Brain%2FData-Science%2FSQL%2FSELECT%20*) customerid, city, country [FROM](obsidian://open?vault=GluGlu&file=6%20-%20Second-Brain%2FData-Science%2FSQL%2FFROM) customers [ORDER BY](obsidian://open?vault=GluGlu&file=6%20-%20Second-Brain%2FData-Science%2FSQL%2FORDER%20BY) country, city;

[[TODO]]: make more commands with the rest of the possible arguments.

References 