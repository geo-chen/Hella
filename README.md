# Hella

Product: https://www.hella.com/hella-sg/en/Driving-Video-Recorders-1370.html

Version: Hella Driving Recorder (DR) 820

## Finding 1 - CVE-2025-30115: Default Credentials Cannot be Changed. [CWE-1393]
The HELLA 820 dashcam uses a fixed default SSID and password <REDACTED>

## Finding 2 - CVE-2025-30113: Hardcoded credentials in APK to ports 9091 (API) and 9092 (RTSP)
The HELLA 820 dashcam’s Android APK (Hella Bulb v1.3) contains hardcoded credentials that allow unauthorized access to device settings through <REDACTED>

## Finding 3 - CVE-2025-30114: Bypassing of device pairing [CWE-798]
The HELLA 820 dashcam’s pairing mechanism relies solely on the connecting device’s <REDACTED>

## Finding 4 - CVE-2025-30116: Remotely Dump Video Footage and Live Video Stream
Once connected and authenticated, we are able to list all video recordings <REDACTED>

## Finding 5 - CVE-2025-30117: Managing Settings to Obtain Sensitive Data and Sabotaging Car Battery
After connecting to the dashcam, an attacker can obtain sensitive user and vehicle information through the HELLA DR 820’s settings interface. The attacker can then read configuration settings, including sensitive car and driver information, and modify various system parameters. <REDACTED>

## Finding 6: Public Domain Used for Internal Domain Name
Inspecting the DNS traffic, we also noticed that a configured internal domain name was using the .com tld and that domain name wasn't registered. We've registered that and notified the manufacturer within 24 hours.


## Disclosure
16 Feb 2025 - Disclosure to Hella's securemail
17 Feb 2025 - Also contacted Hella's generic inbox
7 Mar 2025 - Follow up to get Hella's response
17 Mar 2025 - Coordinated with Mitre to publish this writeup and get the CVE assignments
17 Mar 2025 - Hella's security team reached out requesting for temporary takedown
18 Mar 2025 - Redacted repo for 3 months
