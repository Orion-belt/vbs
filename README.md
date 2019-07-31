### Juju charm for IEEE P1930 vBS
This juju charm is under developement and collabrations are welcomned.
Charm is targeted to build vBS instance for 802.11 type of base stations.
It need to be complianced with IEEE P1930.1 requirement for vBS.

`git clone https://github.com/orion-belt/vBS.git`
`git clone https://github.com/orion-belt/floodlight-charm.git`
`juju deploy ./floodlight-controller`
`juju deploy ./vBS`
`juju add-relation vBS floodlight-controller


     ____________                         ___________
    |Charm       |                       |Charm      |
    |            |      (NBI)            |           |
    |            |  Standard protocol    |           |
    |  SDN CTL   |<--------------------->|    vBS    |
    |(floodlight)|                       |           |
    |            |                       |           |
    |____________|                       |___________|
						|       (SBI)
						|  Vendor Protocol
					    ____|______
					   |           |
					   |           |
					   |           |
					   |     BS    |
					   |           |
					   |           |
					   |___________|
