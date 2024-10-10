2024-10-03 09:45

Status:

Tags:
[[SQL]]
# WHERE

A command that is added to the string in order to further narrow down a search, it could be a column, a string, or a wildcard:

Examples of a wildcard:

- 'a%' = apple123, art, a
	This wildcard finds everything that starts with a hence a%

- 'a_' = as, an, a7
	This wildcard finds every coincidence that starts with a and contains 2 letters where the first one is a.
	
- 'a__' = and, add, a1c
	This wildcard finds every coincidence that starts with a and is followed by 2 letters.

- '%a' = pizza, Z6ra, a
	This wildcard find every coincidence that ends with a

- '_ a _' = ma, la, Ha
	this wildcard ends also with a _ _ and finds every coincidence that a in between 2 characters.

- '%a%' = Again, back, a 
	this wildcard finds every ocurrence of a between more letters.



References 