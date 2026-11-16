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

### Preparation
| Script Name  | Content | Type | Target |
| ------------- | ------------- | ------------- | ------------- |
| O metavariables.jinja | |  Jinja | ADOM Database |


### Spokes
| Script Name  | Content | Type | Target |
| ------------- | ------------- | ------------- | ------------- |
| D bgp-spoke-universal.jinja  | BGP Template for Spokes | Jinja | ADOM Database |
| O ipsec-spoke-1isp  | IPsec Template for Spokes with 1 ISP  | Jinja | ADOM Database |
| O ipsec-spoke-2isp  | IPsec Template for Spokes with 2 ISP  | Jinja | ADOM Database |
| O sdwan-spoke-1isp  | SDWAN Template for Spokes with 1 ISP  | Jinja | ADOM Database |
| O sdwan-spoke-2isp  | SDWAN Template for Spokes with 2 ISP  | Jinja | ADOM Database |
| D static-spoke-universal  | Static Routes for Spokes  | Jinja | ADOM Database |
| D system-spoke-universal  | Static Routes for Spokes  | Jinja | ADOM Database |


### Hubs
### Spokes
| Script Name  | Content | Type | Target |
| ------------- | ------------- | ------------- | ------------- |
| O bgp-hub-universal.jinja  | BGP Template for Spokes | Jinja | ADOM Database |
| O ipsec-hub-1isp  | IPsec Template for Spokes with 1 ISP  | Jinja | ADOM Database |
| O ipsec-hub-2isp  | IPsec Template for Spokes with 2 ISP  | Jinja | ADOM Database |
| O sdwan-hub-1isp  | SDWAN Template for Spokes with 1 ISP  | Jinja | ADOM Database |
| O sdwan-hub-2isp  | SDWAN Template for Spokes with 2 ISP  | Jinja | ADOM Database |
| O static-hub-universal  | Static Routes for Spokes  | Jinja | ADOM Database |
| O system-hub-universal  | Static Routes for Spokes  | Jinja | ADOM Database |
