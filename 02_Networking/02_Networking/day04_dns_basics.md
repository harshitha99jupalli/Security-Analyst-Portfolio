# Day 04 — DNS Basics and Security Risks

## What is DNS?
DNS (Domain Name System) converts website names into IP addresses.
Example: google.com → 142.250.xxx.xxx

## How DNS Works
1. User enters website name
2. DNS server looks up IP address
3. Browser connects to that IP
4. Website loads

## Common DNS Records
- A Record – Maps domain to IP
- MX Record – Email server
- CNAME – Alias
- TXT – Verification

## Why DNS matters in Security
- Phishing uses fake domains
- Malware connects to malicious domains
- DNS tunneling can hide attacks

## Example Attack
Fake domain: paypa1.com (looks like paypal.com)
Used in phishing emails.

## Learning Links
- https://www.youtube.com/watch?v=72snZctFFtA
- https://www.cloudflare.com/learning/dns/what-is-dns/

## My Notes
I should always check domain spelling and reputation during investigations.
