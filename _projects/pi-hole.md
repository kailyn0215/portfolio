---
# ═══════════════════════════════════════════════════════════════
# PI-HOLE — Network-Wide Ad Blocking
# ═══════════════════════════════════════════════════════════════
name: "Pi-hole Setup"
title: "Pi-hole Setup"
tagline: "Network-wide ad blocking using a Raspberry Pi"
description: |
  A home networking project where I set up Pi-hole on a Raspberry Pi to block ads and 
  trackers at the DNS level for all devices on my network. In addition to the Pi-hole, 
  I also created a dashboard on an ESP32 with a touchscreen. This project taught me about 
  DNS, networking fundamentals, Linux server administration, as well as Arduino.

# Basic info
category: "networking"
status: "maintaining"
featured: false
year: 2024

# Tech stack
stack:
  - "Raspberry Pi"
  - "Pi-hole"
  - "Linux"
  - "DNS"
  - "Docker"
  - "SSH"
  - "Arduino IDE"

# Links (leave empty if not available)
github: ""
live: ""

# Images
cover_image: ""  # TODO: Add cover image for gallery card
hero_image: ""   # TODO: Add hero image of Pi-hole dashboard
gallery:         # TODO: Add screenshots
  # - /assets/images/projects/pi-hole/dashboard.png
  # - /assets/images/projects/pi-hole/raspberry-pi.jpg
  # - /assets/images/projects/pi-hole/query-log.png

# Detail page content
role: "Network Administrator"
timeline: "initial setup in a weekend, ongoing maintenance"

overview: |
  Pi-hole is a network-level ad blocker that acts as a DNS sinkhole, blocking advertisements
  and tracking domains before they even reach your devices. I set this up on a Raspberry Pi
  connected to my home network, providing ad-blocking benefits to every device — phones, 
  tablets, smart TVs, and computers — without needing to install anything on each device.

problem: |
  Online ads are intrusive, slow down browsing, and often come with privacy-invasive trackers.
  Browser-based ad blockers only work on that specific browser and device. I wanted a solution
  that would protect all devices on my network, including ones that can't run traditional
  ad blockers like smart TVs and IoT devices.

solution: |
  I configured a Raspberry Pi running Pi-hole as my network's primary DNS server. When any 
  device requests a known advertising or tracking domain, Pi-hole returns a blank response
  instead of connecting to the ad server. The setup also includes a web dashboard for 
  monitoring queries and managing blocklists.

features:
  - title: "Network-Wide Blocking"
    description: "Blocks ads and trackers for all devices automatically"
  - title: "Web Dashboard"
    description: "Real-time statistics and query logging via web interface"
  - title: "Custom Blocklists"
    description: "Added community-maintained lists for comprehensive coverage"
  - title: "Whitelist Management"
    description: "Easy whitelisting for sites that break without ads"

challenges:
  - title: "Router Configuration"
    description: "Had to configure router to use Pi-hole as DNS server"
    solution: "Accessed router admin panel and set custom DNS to Raspberry Pi's IP address"
  - title: "Some Sites Breaking"
    description: "Certain websites stopped working due to overly aggressive blocking"
    solution: "Used query log to identify blocked domains and added them to whitelist"
  - title: "Reliability Concerns"
    description: "Worried about internet going down if Pi fails"
    solution: "Set up secondary DNS fallback and configured Pi for automatic updates"

outcomes:
  - "Blocked over 30% of DNS queries as ads/trackers"
  - "Noticeably faster page load times across all devices"
  - "Improved privacy by blocking tracking domains"
  - "Gained practical experience with Linux, networking, and DNS"

next_steps: |
  Planning to add Unbound as a recursive DNS resolver for additional privacy (no upstream
  DNS provider), and potentially setting up a second Pi-hole for redundancy. Also considering
  adding WireGuard VPN to use Pi-hole protection when away from home.

layout: project
---