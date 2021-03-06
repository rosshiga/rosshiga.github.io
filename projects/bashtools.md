---
layout: project
type: project
image: images/bashtools.png
title: BashTools for CentOS7
permalink: projects/bashtools
# All dates must be YYYY-MM-DD format!
date: 2018-08-30
labels:
  - Bash
  - CentOS 7
  - Systemd
  - Certbot
  - NGINX
summary: A free open source set of bash scripts to deploy secure NGINX virtual domains.
---
GitHub: [BashTools_CentOS7](https://github.com/rosshiga/BashTools_CentOS7)

Demo: Used to deploy rosshi.ga, demo.rosshiga.com, and a number of small projects I have.
<div class="ui medium rounded images">
  <img class="ui image" src="../images/bashtools.png">
</div>

# BashTools_CentOS7 Usage
BashTools is a set of bash scripts to deploy and configure CentOS 7 and Nginx for IPv4 networks. The scripts also 
secure sites with free HTTPS certificates from [Let's Encrypt](https://letsencrypt.org/). The tools are focused on having
the latest version of packages and makes no consideration of stability. 
## Usage
All scripts will prompt for needed information or can be preconfigured in the script header. 
### firstSetup.sh
Non root user, timezone, optional yum packages, and public key for SSH can be specified in the header.

EPEL repo is enabled and sed is used to enable automatic yum updates which may impact stability.

fail2ban and ntpd are enabled and configured to work with firewalld to provide added security

Sysctl configurations for ASLR, SYN Cookies, TCP windows, and bogon/bad route protection are enabled and should be tuned to your application

Core limits on open handles and files have been removed and some kernel modules have been disabled 

### setupNGINX.sh
Certbot and nginx are installed from yum. Certbot is used to generate Let's Encrypt free certificates.

Port 80 and 443 are opened for nginx. OpenSSL is used to generate Diffie Hellman group of 2048 bits and is marked for rwx only by root,

Nginx is enabled to start on boot using systemd.

### addVHOST.sh

An TLS/SSL enabled host is created for a FQDN. Nginx is stopped and certbot is allowed to take over port 443 to verify DNS A records. A certificate is generated and OCSP is enforced. 

The configuration does not support host without SNI and is configured to A level grade per [SSL Labs](https://www.ssllabs.com/ssltest/analyze.html?d=demo.rosshiga.com) with perfect forward secrecy. 
