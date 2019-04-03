### Juju charm for IEEE P1930 vBS
This juju charm is under developement and collabrations are welcomned.
Charm is targeted to build vBS instance for 802.11 type of base stations.
It need to be complianced with IEEE P1930.1 requirement for vBS.

`git clone https://github.com/kharade-rohan/vBS.git`

`juju deploy /vBS`


      ___________                         ___________
     |Charm      |                       |Charm      |
     |           |                       |           |
     |           |                       |           |
     |  SDN CTL  |<--------------------->|    vBS    |
     |           |                       |           |
     |           |                       |           |
     |___________|                       |___________|
						|
						|
					    ____|______
					   |           |
					   |           |
					   |           |
					   |     BS    |
					   |           |
					   |           |
					   |___________|
