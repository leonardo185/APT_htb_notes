# IP: 10.10.10.213 dead:beef::b885:d62a:d679:573f

## OS: Windows

## Nmap:

```
# Nmap 7.92 scan initiated Mon Nov 28 08:05:42 2022 as: nmap -vvv -p 80,135 -Pn -A -sC -sV -oN nmap 10.10.10.213
Nmap scan report for 10.10.10.213
Host is up, received user-set (0.048s latency).
Scanned at 2022-11-28 08:05:43 IST for 10s

PORT    STATE SERVICE REASON  VERSION
80/tcp  open  http    syn-ack Microsoft IIS httpd 10.0
|_http-server-header: Microsoft-IIS/10.0
|_http-title: Gigantic Hosting | Home
|_winrm: WinRM not exists (/wsman returns 404)
| http-methods: 
|   Supported Methods: OPTIONS TRACE GET HEAD POST
|_  Potentially risky methods: TRACE
135/tcp open  msrpc   syn-ack Microsoft Windows RPC
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Mon Nov 28 08:05:53 2022 -- 1 IP address (1 host up) scanned in 11.65 seconds
```

## Namp V6

```
Nmap scan report for dead:beef::b885:d62a:d679:573f
Host is up, received user-set (0.056s latency).
Scanned at 2022-11-28 19:26:25 IST for 76s

PORT      STATE SERVICE      REASON  VERSION
53/tcp    open  domain       syn-ack Simple DNS Plus
80/tcp    open  http         syn-ack Microsoft IIS httpd 10.0
| http-server-header: 
|   Microsoft-HTTPAPI/2.0
|_  Microsoft-IIS/10.0
|_http-title: Bad Request
|_winrm: WinRM not exists (/wsman returns 400)
88/tcp    open  kerberos-sec syn-ack Microsoft Windows Kerberos (server time: 2022-11-28 13:57:41Z)
135/tcp   open  msrpc        syn-ack Microsoft Windows RPC
389/tcp   open  ldap         syn-ack Microsoft Windows Active Directory LDAP (Domain: htb.local, Site: Default-First-Site-Name)
|_ssl-date: 2022-11-28T13:58:50+00:00; +1m10s from scanner time.
| ssl-cert: Subject: commonName=apt.htb.local
| Subject Alternative Name: DNS:apt.htb.local
| Issuer: commonName=apt.htb.local
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2020-09-24T07:07:18
| Not valid after:  2050-09-24T07:17:18
| MD5:   c743 dd92 e928 50b0 aa86 6f80 1b04 4d22
| SHA-1: f677 c290 98c0 2ac5 8575 7060 683d cdbc 5f86 5d45
| -----BEGIN CERTIFICATE-----
| MIIDJjCCAg6gAwIBAgIQQg664ORKu6FF1x3M6AR5FjANBgkqhkiG9w0BAQsFADAY
| MRYwFAYDVQQDDA1hcHQuaHRiLmxvY2FsMCAXDTIwMDkyNDA3MDcxOFoYDzIwNTAw
| OTI0MDcxNzE4WjAYMRYwFAYDVQQDDA1hcHQuaHRiLmxvY2FsMIIBIjANBgkqhkiG
| 9w0BAQEFAAOCAQ8AMIIBCgKCAQEApN9k/PGK7QcXjONuOeT7rIascD+bozXzfhli
| b4yHz6PfPrKMwp3AMcY5/M/iwDRoFOrYj3HNW4DlRkuBw5l//UGpjQcO4rkmxdIg
| 6Pqf7MOzLxF4jNGXyGlOq/hvki/+fsR9tq7e4O20w6LV3toLb5oKtitu3PW3pnKM
| lOTASkv1xt5E1+5cMo8NVEYgfHWdcLt6iY3PFKzN9HhjoZ1AmOToyb0RfgAyoJok
| QLkN3HJraOANzEPyq9NmGC/yRvdYQ299kXh+hCMU+M9EjBBvLFc8o7Ci5Zq1AgUm
| qf6XXz2QdwctXg2QJqqgMeElaxGJaoBg161EgEwftzy4yjobFwIDAQABo2owaDAO
| BgNVHQ8BAf8EBAMCBaAwHQYDVR0lBBYwFAYIKwYBBQUHAwIGCCsGAQUFBwMBMBgG
| A1UdEQQRMA+CDWFwdC5odGIubG9jYWwwHQYDVR0OBBYEFKCI+2TQc8sHDcWZMb2m
| 8BeIOhvNMA0GCSqGSIb3DQEBCwUAA4IBAQCYucbJiU6grEMT9a3NrUzW3SxCjW3i
| 9bYa1D/+Tlf6w627r03tL+tV/c0U2BzzztGMIUItOLfWyJCTcs6KUpSQUclaUTkG
| 7k59ABHj5z/OuOVRvP3qceJY69CNtwBaxYVni9ei8GZ22sIyg1WidFEP31CulJqm
| eMgrMOj5egS6jaiqaOUIk3wZk033Vk9ZeSEPi5Ur4qNa28pCxBDJ1k6s9yQWQFTF
| mHnp84Oc8orbALUePWiPt0IZKSXzptvHU0LRJE6aWB9pWKoEP+5ibZ7L7UxLVryH
| MP+pnqp9xiFaauqlwi2w8LmoX2KIat8obtDH/clQj6gu/UQ/7an+qErq
|_-----END CERTIFICATE-----
445/tcp   open  microsoft-ds syn-ack Windows Server 2016 Standard 14393 microsoft-ds (workgroup: HTB)
464/tcp   open  kpasswd5?    syn-ack
593/tcp   open  ncacn_http   syn-ack Microsoft Windows RPC over HTTP 1.0
636/tcp   open  ssl/ldap     syn-ack Microsoft Windows Active Directory LDAP (Domain: htb.local, Site: Default-First-Site-Name)
|_ssl-date: 2022-11-28T13:58:50+00:00; +1m10s from scanner time.
| ssl-cert: Subject: commonName=apt.htb.local
| Subject Alternative Name: DNS:apt.htb.local
| Issuer: commonName=apt.htb.local
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2020-09-24T07:07:18
| Not valid after:  2050-09-24T07:17:18
| MD5:   c743 dd92 e928 50b0 aa86 6f80 1b04 4d22
| SHA-1: f677 c290 98c0 2ac5 8575 7060 683d cdbc 5f86 5d45
| -----BEGIN CERTIFICATE-----
| MIIDJjCCAg6gAwIBAgIQQg664ORKu6FF1x3M6AR5FjANBgkqhkiG9w0BAQsFADAY
| MRYwFAYDVQQDDA1hcHQuaHRiLmxvY2FsMCAXDTIwMDkyNDA3MDcxOFoYDzIwNTAw
| OTI0MDcxNzE4WjAYMRYwFAYDVQQDDA1hcHQuaHRiLmxvY2FsMIIBIjANBgkqhkiG
| 9w0BAQEFAAOCAQ8AMIIBCgKCAQEApN9k/PGK7QcXjONuOeT7rIascD+bozXzfhli
| b4yHz6PfPrKMwp3AMcY5/M/iwDRoFOrYj3HNW4DlRkuBw5l//UGpjQcO4rkmxdIg
| 6Pqf7MOzLxF4jNGXyGlOq/hvki/+fsR9tq7e4O20w6LV3toLb5oKtitu3PW3pnKM
| lOTASkv1xt5E1+5cMo8NVEYgfHWdcLt6iY3PFKzN9HhjoZ1AmOToyb0RfgAyoJok
| QLkN3HJraOANzEPyq9NmGC/yRvdYQ299kXh+hCMU+M9EjBBvLFc8o7Ci5Zq1AgUm
| qf6XXz2QdwctXg2QJqqgMeElaxGJaoBg161EgEwftzy4yjobFwIDAQABo2owaDAO
| BgNVHQ8BAf8EBAMCBaAwHQYDVR0lBBYwFAYIKwYBBQUHAwIGCCsGAQUFBwMBMBgG
| A1UdEQQRMA+CDWFwdC5odGIubG9jYWwwHQYDVR0OBBYEFKCI+2TQc8sHDcWZMb2m
| 8BeIOhvNMA0GCSqGSIb3DQEBCwUAA4IBAQCYucbJiU6grEMT9a3NrUzW3SxCjW3i
| 9bYa1D/+Tlf6w627r03tL+tV/c0U2BzzztGMIUItOLfWyJCTcs6KUpSQUclaUTkG
| 7k59ABHj5z/OuOVRvP3qceJY69CNtwBaxYVni9ei8GZ22sIyg1WidFEP31CulJqm
| eMgrMOj5egS6jaiqaOUIk3wZk033Vk9ZeSEPi5Ur4qNa28pCxBDJ1k6s9yQWQFTF
| mHnp84Oc8orbALUePWiPt0IZKSXzptvHU0LRJE6aWB9pWKoEP+5ibZ7L7UxLVryH
| MP+pnqp9xiFaauqlwi2w8LmoX2KIat8obtDH/clQj6gu/UQ/7an+qErq
|_-----END CERTIFICATE-----
3268/tcp  open  ldap         syn-ack Microsoft Windows Active Directory LDAP (Domain: htb.local, Site: Default-First-Site-Name)
| ssl-cert: Subject: commonName=apt.htb.local
| Subject Alternative Name: DNS:apt.htb.local
| Issuer: commonName=apt.htb.local
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2020-09-24T07:07:18
| Not valid after:  2050-09-24T07:17:18
| MD5:   c743 dd92 e928 50b0 aa86 6f80 1b04 4d22
| SHA-1: f677 c290 98c0 2ac5 8575 7060 683d cdbc 5f86 5d45
| -----BEGIN CERTIFICATE-----
| MIIDJjCCAg6gAwIBAgIQQg664ORKu6FF1x3M6AR5FjANBgkqhkiG9w0BAQsFADAY
| MRYwFAYDVQQDDA1hcHQuaHRiLmxvY2FsMCAXDTIwMDkyNDA3MDcxOFoYDzIwNTAw
| OTI0MDcxNzE4WjAYMRYwFAYDVQQDDA1hcHQuaHRiLmxvY2FsMIIBIjANBgkqhkiG
| 9w0BAQEFAAOCAQ8AMIIBCgKCAQEApN9k/PGK7QcXjONuOeT7rIascD+bozXzfhli
| b4yHz6PfPrKMwp3AMcY5/M/iwDRoFOrYj3HNW4DlRkuBw5l//UGpjQcO4rkmxdIg
| 6Pqf7MOzLxF4jNGXyGlOq/hvki/+fsR9tq7e4O20w6LV3toLb5oKtitu3PW3pnKM
| lOTASkv1xt5E1+5cMo8NVEYgfHWdcLt6iY3PFKzN9HhjoZ1AmOToyb0RfgAyoJok
| QLkN3HJraOANzEPyq9NmGC/yRvdYQ299kXh+hCMU+M9EjBBvLFc8o7Ci5Zq1AgUm
| qf6XXz2QdwctXg2QJqqgMeElaxGJaoBg161EgEwftzy4yjobFwIDAQABo2owaDAO
| BgNVHQ8BAf8EBAMCBaAwHQYDVR0lBBYwFAYIKwYBBQUHAwIGCCsGAQUFBwMBMBgG
| A1UdEQQRMA+CDWFwdC5odGIubG9jYWwwHQYDVR0OBBYEFKCI+2TQc8sHDcWZMb2m
| 8BeIOhvNMA0GCSqGSIb3DQEBCwUAA4IBAQCYucbJiU6grEMT9a3NrUzW3SxCjW3i
| 9bYa1D/+Tlf6w627r03tL+tV/c0U2BzzztGMIUItOLfWyJCTcs6KUpSQUclaUTkG
| 7k59ABHj5z/OuOVRvP3qceJY69CNtwBaxYVni9ei8GZ22sIyg1WidFEP31CulJqm
| eMgrMOj5egS6jaiqaOUIk3wZk033Vk9ZeSEPi5Ur4qNa28pCxBDJ1k6s9yQWQFTF
| mHnp84Oc8orbALUePWiPt0IZKSXzptvHU0LRJE6aWB9pWKoEP+5ibZ7L7UxLVryH
| MP+pnqp9xiFaauqlwi2w8LmoX2KIat8obtDH/clQj6gu/UQ/7an+qErq
|_-----END CERTIFICATE-----
|_ssl-date: 2022-11-28T13:58:50+00:00; +1m10s from scanner time.
3269/tcp  open  ssl/ldap     syn-ack Microsoft Windows Active Directory LDAP (Domain: htb.local, Site: Default-First-Site-Name)
|_ssl-date: 2022-11-28T13:58:50+00:00; +1m10s from scanner time.
| ssl-cert: Subject: commonName=apt.htb.local
| Subject Alternative Name: DNS:apt.htb.local
| Issuer: commonName=apt.htb.local
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2020-09-24T07:07:18
| Not valid after:  2050-09-24T07:17:18
| MD5:   c743 dd92 e928 50b0 aa86 6f80 1b04 4d22
| SHA-1: f677 c290 98c0 2ac5 8575 7060 683d cdbc 5f86 5d45
| -----BEGIN CERTIFICATE-----
| MIIDJjCCAg6gAwIBAgIQQg664ORKu6FF1x3M6AR5FjANBgkqhkiG9w0BAQsFADAY
| MRYwFAYDVQQDDA1hcHQuaHRiLmxvY2FsMCAXDTIwMDkyNDA3MDcxOFoYDzIwNTAw
| OTI0MDcxNzE4WjAYMRYwFAYDVQQDDA1hcHQuaHRiLmxvY2FsMIIBIjANBgkqhkiG
| 9w0BAQEFAAOCAQ8AMIIBCgKCAQEApN9k/PGK7QcXjONuOeT7rIascD+bozXzfhli
| b4yHz6PfPrKMwp3AMcY5/M/iwDRoFOrYj3HNW4DlRkuBw5l//UGpjQcO4rkmxdIg
| 6Pqf7MOzLxF4jNGXyGlOq/hvki/+fsR9tq7e4O20w6LV3toLb5oKtitu3PW3pnKM
| lOTASkv1xt5E1+5cMo8NVEYgfHWdcLt6iY3PFKzN9HhjoZ1AmOToyb0RfgAyoJok
| QLkN3HJraOANzEPyq9NmGC/yRvdYQ299kXh+hCMU+M9EjBBvLFc8o7Ci5Zq1AgUm
| qf6XXz2QdwctXg2QJqqgMeElaxGJaoBg161EgEwftzy4yjobFwIDAQABo2owaDAO
| BgNVHQ8BAf8EBAMCBaAwHQYDVR0lBBYwFAYIKwYBBQUHAwIGCCsGAQUFBwMBMBgG
| A1UdEQQRMA+CDWFwdC5odGIubG9jYWwwHQYDVR0OBBYEFKCI+2TQc8sHDcWZMb2m
| 8BeIOhvNMA0GCSqGSIb3DQEBCwUAA4IBAQCYucbJiU6grEMT9a3NrUzW3SxCjW3i
| 9bYa1D/+Tlf6w627r03tL+tV/c0U2BzzztGMIUItOLfWyJCTcs6KUpSQUclaUTkG
| 7k59ABHj5z/OuOVRvP3qceJY69CNtwBaxYVni9ei8GZ22sIyg1WidFEP31CulJqm
| eMgrMOj5egS6jaiqaOUIk3wZk033Vk9ZeSEPi5Ur4qNa28pCxBDJ1k6s9yQWQFTF
| mHnp84Oc8orbALUePWiPt0IZKSXzptvHU0LRJE6aWB9pWKoEP+5ibZ7L7UxLVryH
| MP+pnqp9xiFaauqlwi2w8LmoX2KIat8obtDH/clQj6gu/UQ/7an+qErq
|_-----END CERTIFICATE-----
5985/tcp  open  http         syn-ack Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-title: Bad Request
|_http-server-header: Microsoft-HTTPAPI/2.0
|_winrm: WinRM not exists (/wsman returns 400)
9389/tcp  open  mc-nmf       syn-ack .NET Message Framing
47001/tcp open  http         syn-ack Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-server-header: Microsoft-HTTPAPI/2.0
|_winrm: WinRM not exists (/wsman returns 400)
|_http-title: Bad Request
49664/tcp open  msrpc        syn-ack Microsoft Windows RPC
49665/tcp open  msrpc        syn-ack Microsoft Windows RPC
49666/tcp open  msrpc        syn-ack Microsoft Windows RPC
49667/tcp open  msrpc        syn-ack Microsoft Windows RPC
49669/tcp open  ncacn_http   syn-ack Microsoft Windows RPC over HTTP 1.0
49670/tcp open  msrpc        syn-ack Microsoft Windows RPC
49674/tcp open  msrpc        syn-ack Microsoft Windows RPC
49698/tcp open  msrpc        syn-ack Microsoft Windows RPC
57493/tcp open  msrpc        syn-ack Microsoft Windows RPC
Service Info: Host: APT; OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
| smb2-security-mode: 
|   3.1.1: 
|_    Message signing enabled and required
| smb-security-mode: 
|   account_used: <blank>
|   authentication_level: user
|   challenge_response: supported
|_  message_signing: required
| smb-os-discovery: 
|   OS: Windows Server 2016 Standard 14393 (Windows Server 2016 Standard 6.3)
|   Computer name: apt
|   NetBIOS computer name: APT\x00
|   Domain name: htb.local
|   Forest name: htb.local
|   FQDN: apt.htb.local
|_  System time: 2022-11-28T13:58:37+00:00
|_clock-skew: mean: 1m10s, deviation: 0s, median: 1m09s
| smb2-time: 
|   date: 2022-11-28T13:58:40
|_  start_date: 2022-11-28T02:31:01

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Mon Nov 28 19:27:41 2022 -- 1 IP address (1 host up) scanned in 76.54 seconds

```