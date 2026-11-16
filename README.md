# FortiManager-SDWAN

## Description

## Script

### Variables
| Variable  | Description | Example Value |
| ------------- | ------------- | ------------- |
| ip_spoke_bgp_lo | "Lo-BGP" IP-adress of Spoke | 10.200.1.15 |
| ip_hub1_bgp_lo | "Lo-BGP" IP-address of Hub1 | 10.200.1.250 |
| net_spoke_lan | LAN with Subnet| 192.168.100.0/24 |
| net_bgp_lo | Summary LAN of "Lo-BGP" | 10.200.1.0/24 |
| str_asn_emea | ASN of Region EMEA | 65002 |

### Spokes
| Script Name  | Content | Type | Target |
| ------------- | ------------- | ------------- | ------------- |
| metavariables.jinja | |  Jinja | ADOM Database |
| bgp-spoke-universal.jinja  | BGP Template for Spokes | Jinja | ADOM Database |
| ipsec-spoke-1isp  | IPsec Template for Spokes with 1 ISP  | Jinja | ADOM Database |
| ipsec-spoke-2isp  | IPsec Template for Spokes with 2 ISP  | Jinja | ADOM Database |
| sdwan-spoke-1isp  | SDWAN Template for Spokes with 1 ISP  | Jinja | ADOM Database |
| sdwan-spoke-2isp  | SDWAN Template for Spokes with 2 ISP  | Jinja | ADOM Database |
| static-spoke-universal  | Static Routes for Spokes  | Jinja | ADOM Database |
| system-spoke-universal  | Static Routes for Spokes  | Jinja | ADOM Database |


### Hubs
