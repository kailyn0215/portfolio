---
# ═══════════════════════════════════════════════════════════════
# Groovy Proxy — Local Development Proxy Tool
# ═══════════════════════════════════════════════════════════════
name: "Groovy Proxy"
title: "Groovy Proxy"
tagline: "Local development proxy tool for testing"
description: |
  A lightweight proxy server tool built to assist with local development and API testing. 
  Created to streamline the development workflow and make testing easier.

# Basic info
category: "dev_tool"
status: "maintaining"
featured: true
year: 2024

# Tech stack
stack:
  - "Node.js"
  - "JavaScript"
  - "Express"

# Links (leave empty if not available)
github: "https://github.com/kailyn0215/groovy-proxy"
live: ""

# Images
cover_image: ""  # TODO: Add cover image for gallery card
hero_image: ""   # TODO: Add hero screenshot for detail page
gallery:         # TODO: Add gallery screenshots
  # - /assets/images/projects/groovy-proxy/screenshot-1.png

# Detail page content
role: "solo_dev"
timeline: "personal_proj"

overview: |
  Groovy Proxy is a development tool I built to simplify API testing and local development 
  workflows. It acts as a proxy server that can intercept, log, and modify HTTP requests, 
  making it easier to debug and test applications during development.

problem: |
  During development, it's often necessary to test API integrations, debug request/response 
  cycles, and simulate different scenarios. Setting this up manually can be time-consuming 
  and error-prone.

solution: |
  Groovy Proxy provides a simple, configurable proxy server that can be run locally. It 
  logs all requests, allows for request modification, and provides a clean interface for 
  monitoring traffic during development.

features:
  - title: "Request Logging"
    description: "Detailed logging of all HTTP requests and responses"
  - title: "Easy Configuration"
    description: "Simple setup and configuration for different environments"
  - title: "Request Modification"
    description: "Ability to intercept and modify requests on the fly"
  - title: "Clean Interface"
    description: "User-friendly interface for monitoring traffic"

challenges:
  - title: "HTTP Protocol Handling"
    description: "Properly handling various HTTP methods and headers"
    solution: "Leveraged Express.js middleware for robust request handling"

outcomes:
  - "Streamlined personal development workflow"
  - "Gained deeper understanding of HTTP protocols"
  - "Created reusable tool for future projects"

next_steps: |
  TODO: Add any planned features or improvements for Groovy Proxy.
---