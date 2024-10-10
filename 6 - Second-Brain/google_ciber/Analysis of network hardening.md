2024-09-25 19:55

Status:

Tags: [[Cyber security]] 

# Analysis of network hardening

In this particular case so far we have dicovered four major vulnerabilities so far:

- employees share password.
- the admin password for the database is set to *default*.
- there are no rules for the *firewall*.
- they aren't using MFA (*Multi-Factor Auth).

Security Risk Assessment Report

Part 1: Select up to three hardening tools and methods to implement:

	My First suggestion would be to configure the firewall by disabling unused ports this would prevent malicious actors from being able to enter the network, taking in consideration that the first attack already happened it is one of the most important ones to implement since we dont know if during the breach malware was installed in the server/sistems, this would also include firewall maintenance, port filetering and siem tools usage to check the network for unauthorized access.

	My Second suggestion would be to implement password policies and MFA *multi factor authentification*, this would avoid password sharing among emplooyees while at the same time protect the company's data from a posible leak caused by just a password being stolen or a malicious actor utilizing the password of a colleague.

	My third suggestion would be to change the *admin password* asap, and also add MFA to it in order to avoid bad actors accessing the database.

part 2: Explain your recommendations:

	My recomendations so far are done to target the current problems found in the company, to avoid posible data leaks in the future, up to standards firewall/password policies are needed, the admin password being the top priority.

	I would also suggest after the changes are made that the company installs SIEM Tools in order to monitor their network, aside from enforcing the password policies. 

 part 3: Why is the recommended security hardening technique effective?

	By enfocring password policies and MFA we ensure that only the owner of the account can access it even if the password is shared or leaked it wont work since the MFA will also be needed, thus allow us to see posible bad actors within the company.

	By enforcing firewall stardars, disabling unused ports we limit the surface of attack area that the company must be aware of, aside from also installing SIEM tools in order to be able to monitor the network, it is important to also set a schedule for firewall maintenance.

	It is of the outmost importance that the password for the admin account to be changed and MFA be applied to it, if that admin account had access to roles inside of the company they would need to be checked aswell.

	For a last recomendation i highly suggest the analizis for viruses/malwares in the servers/computers of the company to discard a posible malware instalation done during the breach.


 part 4: How often does the hardening technique need to be implemented?

	All my suggestions would be best if done monthly.

References