# Threat Intelligence Watchlists

This repository hosts two public threat intelligence watchlists in CSV format for use with SIEM and SOAR platforms such as Microsoft Sentinel.

These lists are provided for defensive and research purposes only.

## Files

- **rvt_blocklist_ip.csv** – CIDR/IP indicators  
- **rvt_blocklist_fqdn.csv** – FQDN indicators

- **rvt_blocklist_ip.csv** 
  CIDR-formatted network indicators (IPv4). Suitable for use with functions such as ipv4_is_in_range().

- **rvt_blocklist_fqdn.csv** 
  Domain-based indicators (FQDNs). Suitable for DNS, URL, and HTTP log matching.

## Format

All files use UTF-8 CSV with headers.

- `watchlist_block_ip.csv` columns:
  - `ip_address`
  - `network`
  - `asn`
  - `category`
  - `description`

- `watchlist_block_fqdn.csv` columns:
  - `fqdn`
  - `category`
  - `description`

## Usage

These watchlists are intended to be ingested into a SIEM watchlist or lookup table and joined against network, DNS, or proxy logs for detection and hunting.

## Disclaimer

No warranty is provided. Use at your own risk and only for defensive cybersecurity purposes.
