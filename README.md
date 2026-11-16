# FortiManager-SDWAN

## Description
Unofficial Jinja scripts for FortiManager Device Manager to quickly create SD-WAN provisioning templates in an ADOM or policy package – built for lab, demo and POC environments. Not affiliated with or supported by Fortinet.

## Variables
| Variable  | Description | Example Value |
| ------------- | ------------- | ------------- |
| ip_spoke_bgp_lo | "Lo-BGP" IP-adress of Spoke | 10.200.1.15 |
| ip_hub1_bgp_lo | "Lo-BGP" IP-address of Hub1 | 10.200.1.250 |
| net_spoke_lan | LAN with Subnet| 192.168.100.0/24 |
| net_bgp_lo | Summary LAN of "Lo-BGP" | 10.200.1.0/24 |
| pip1_hub1 | Public IP from Hub 1 - ISP 1 | 8.8.8.8 |
| sec_psk_ipsec | PSK Secret for IPSec | mySecretPSK11? |
| str_asn_emea | ASN of Region EMEA | 65002 |
| str_spoke_port_wan | Name of WAN Port | wan1 |

## Scripts


### Preparation Scripts
| Script Name  | Content | Type | Target |
| ------------- | ------------- | ------------- | ------------- |
| O metavariables.jinja | |  Jinja | ADOM Database |


### Spokes Scripts
| Script Name  | Content | Type | Target |
| ------------- | ------------- | ------------- | ------------- |
| D bgp-spoke-universal.jinja  | BGP Template for Spokes | Jinja | ADOM Database |
| D ipsec-spoke-1isp.jinja  | IPsec Template for Spokes with 1 ISP  | Jinja | ADOM Database |
| O ipsec-spoke-2isp.jinja  | IPsec Template for Spokes with 2 ISP  | Jinja | ADOM Database |
| O sdwan-spoke-1isp.jinja  | SDWAN Template for Spokes with 1 ISP  | Jinja | ADOM Database |
| O sdwan-spoke-2isp.jinja  | SDWAN Template for Spokes with 2 ISP  | Jinja | ADOM Database |
| D static-spoke-universal.jinja  | Static Routes for Spokes  | Jinja | ADOM Database |
| D system-spoke-universal.jinja  | Static Routes for Spokes  | Jinja | ADOM Database |


### Hubs Scripts
| Script Name  | Content | Type | Target |
| ------------- | ------------- | ------------- | ------------- |
| O bgp-hub-universal.jinja  | BGP Template for Spokes | Jinja | ADOM Database |
| O ipsec-hub-1isp  | IPsec Template for Spokes with 1 ISP  | Jinja | ADOM Database |
| O ipsec-hub-2isp  | IPsec Template for Spokes with 2 ISP  | Jinja | ADOM Database |
| O sdwan-hub-1isp  | SDWAN Template for Spokes with 1 ISP  | Jinja | ADOM Database |
| O sdwan-hub-2isp  | SDWAN Template for Spokes with 2 ISP  | Jinja | ADOM Database |
| O static-hub-universal  | Static Routes for Spokes  | Jinja | ADOM Database |
| O system-hub-universal  | Static Routes for Spokes  | Jinja | ADOM Database |
