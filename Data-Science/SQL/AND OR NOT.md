2024-09-29 14:04

Status:

Tags:
[[SQL]]

# logical operands

#### AND

	It's an operand that is used to filter two conditions, and specifies that both conditions must be met simultaneously.

SELECT firstname, lastname, email, country, supportrepid

FROM customers

WHERE supportrepid = 5 AND country = 'USA';

+-----------+----------+-------------------------+---------+--------------+
| FirstName | LastName | Email                   | Country | SupportRepId |
+-----------+----------+-------------------------+---------+--------------+
| Jack      | Smith    | jacksmith@microsoft.com | USA     |            5 |
| Kathy     | Chase    | kachase@hotmail.com     | USA     |            5 |
| Victor    | Stevens  | vstevens@yahoo.com      | USA     |            5 |
| Julia     | Barnett  | jubarnett@gmail.com     | USA     |            5 |
+-----------+----------+-------------------------+---------+--------------+

#### OR

	this is the operator that will check 2 conditions and will result in true if one of those two is found.

SELECT firstname, lastname, email, country

FROM customers

WHERE country = 'Canada' OR country = 'USA';

+-----------+------------+--------------------------+---------+
| FirstName | LastName   | Email                    | Country |
+-----------+------------+--------------------------+---------+
| François  | Tremblay   | ftremblay@gmail.com      | Canada  |
| Mark      | Philips    | mphilips12@shaw.ca       | Canada  |
| Jennifer  | Peterson   | jenniferp@rogers.ca      | Canada  |
| Frank     | Harris     | fharris@google.com       | USA     |
| Jack      | Smith      | jacksmith@microsoft.com  | USA     |
| Michelle  | Brooks     | michelleb@aol.com        | USA     |
| Tim       | Goyer      | tgoyer@apple.com         | USA     |
| Dan       | Miller     | dmiller@comcast.com      | USA     |
| Kathy     | Chase      | kachase@hotmail.com      | USA     |
| Heather   | Leacock    | hleacock@gmail.com       | USA     |
| John      | Gordon     | johngordon22@yahoo.com   | USA     |
| Frank     | Ralston    | fralston@gmail.com       | USA     |
| Victor    | Stevens    | vstevens@yahoo.com       | USA     |
| Richard   | Cunningham | ricunningham@hotmail.com | USA     |
| Patrick   | Gray       | patrick.gray@aol.com     | USA     |
| Julia     | Barnett    | jubarnett@gmail.com      | USA     |
| Robert    | Brown      | robbrown@shaw.ca         | Canada  |
| Edward    | Francis    | edfrancis@yachoo.ca      | Canada  |
| Martha    | Silk       | marthasilk@gmail.com     | Canada  |
| Aaron     | Mitchell   | aaronmitchell@yahoo.ca   | Canada  |
| Ellie     | Sullivan   | ellie.sullivan@shaw.ca   | Canada  |
+-----------+------------+--------------------------+---------+


#### NOT

	Unlike the previous operators, NOT is applied to a single operand and not multiple instances, so the query returns all records that dont contain the word.


SELECT firstname, lastname, email, country

FROM customers

WHERE NOT country = 'USA';

+-----------+-------------+-------------------------------+----------------+
| FirstName | LastName    | Email                         | Country        |
+-----------+-------------+-------------------------------+----------------+
| Luís      | Gonçalves   | luisg@embraer.com.br          | Brazil         |
| Leonie    | Köhler      | leonekohler@surfeu.de         | Germany        |
| François  | Tremblay    | ftremblay@gmail.com           | Canada         |
| Bjørn     | Hansen      | bjorn.hansen@yahoo.no         | Norway         |
| František | Wichterlová | frantisekw@jetbrains.com      | Czech Republic |
| Helena    | Holý        | hholy@gmail.com               | Czech Republic |
| Astrid    | Gruber      | astrid.gruber@apple.at        | Austria        |
| Daan      | Peeters     | daan_peeters@apple.be         | Belgium        |
| Kara      | Nielsen     | kara.nielsen@jubii.dk         | Denmark        |
| Eduardo   | Martins     | eduardo@woodstock.com.br      | Brazil         |
| Alexandre | Rocha       | alero@uol.com.br              | Brazil         |
| Roberto   | Almeida     | roberto.almeida@riotur.gov.br | Brazil         |
| Fernanda  | Ramos       | fernadaramos4@uol.com.br      | Brazil         |
| Mark      | Philips     | mphilips12@shaw.ca            | Canada         |
| Jennifer  | Peterson    | jenniferp@rogers.ca           | Canada         |
| Robert    | Brown       | robbrown@shaw.ca              | Canada         |
| Edward    | Francis     | edfrancis@yachoo.ca           | Canada         |
| Martha    | Silk        | marthasilk@gmail.com          | Canada         |
| Aaron     | Mitchell    | aaronmitchell@yahoo.ca        | Canada         |
| Ellie     | Sullivan    | ellie.sullivan@shaw.ca        | Canada         |
| João      | Fernandes   | jfernandes@yahoo.pt           | Portugal       |
| Madalena  | Sampaio     | masampaio@sapo.pt             | Portugal       |
| Hannah    | Schneider   | hannah.schneider@yahoo.de     | Germany        |
| Fynn      | Zimmermann  | fzimmermann@yahoo.de          | Germany        |
| Niklas    | Schröder    | nschroder@surfeu.de           | Germany        |
+-----------+-------------+-------------------------------+----------------+


#### Combining Logical Operators

 Logical operators can be combined in several ways in order to further improve the query logic and get the results we want from the database.

SELECT firstname, lastname, email, country

FROM customers

WHERE NOT country = 'Canada' AND NOT country = 'USA';

+-----------+-------------+-------------------------------+----------------+
| FirstName | LastName    | Email                         | Country        |
+-----------+-------------+-------------------------------+----------------+
| Luís      | Gonçalves   | luisg@embraer.com.br          | Brazil         |
| Leonie    | Köhler      | leonekohler@surfeu.de         | Germany        |
| Bjørn     | Hansen      | bjorn.hansen@yahoo.no         | Norway         |
| František | Wichterlová | frantisekw@jetbrains.com      | Czech Republic |
| Helena    | Holý        | hholy@gmail.com               | Czech Republic |
| Astrid    | Gruber      | astrid.gruber@apple.at        | Austria        |
| Daan      | Peeters     | daan_peeters@apple.be         | Belgium        |
| Kara      | Nielsen     | kara.nielsen@jubii.dk         | Denmark        |
| Eduardo   | Martins     | eduardo@woodstock.com.br      | Brazil         |
| Alexandre | Rocha       | alero@uol.com.br              | Brazil         |
| Roberto   | Almeida     | roberto.almeida@riotur.gov.br | Brazil         |
| Fernanda  | Ramos       | fernadaramos4@uol.com.br      | Brazil         |
| João      | Fernandes   | jfernandes@yahoo.pt           | Portugal       |
| Madalena  | Sampaio     | masampaio@sapo.pt             | Portugal       |
| Hannah    | Schneider   | hannah.schneider@yahoo.de     | Germany        |
| Fynn      | Zimmermann  | fzimmermann@yahoo.de          | Germany        |
| Niklas    | Schröder    | nschroder@surfeu.de           | Germany        |
| Camille   | Bernard     | camille.bernard@yahoo.fr      | France         |
| Dominique | Lefebvre    | dominiquelefebvre@gmail.com   | France         |
| Marc      | Dubois      | marc.dubois@hotmail.com       | France         |
| Wyatt     | Girard      | wyatt.girard@yahoo.fr         | France         |
| Isabelle  | Mercier     | isabelle_mercier@apple.fr     | France         |
| Terhi     | Hämäläinen  | terhi.hamalainen@apple.fi     | Finland        |
| Ladislav  | Kovács      | ladislav_kovacs@apple.hu      | Hungary        |
| Hugh      | O'Reilly    | hughoreilly@apple.ie          | Ireland        |
+-----------+-------------+-------------------------------+----------------+


References 