# OpenShelf

![Status](https://img.shields.io/badge/status-pilot-blue)  
![Type](https://img.shields.io/badge/type-offline%20micro--library-green)  
![Platform](https://img.shields.io/badge/platform-ESP8266-orange)  

<p align="center">
  <img src="images/openshelf-nodes.jpg" width="700">
</p>

Offline micro-libraries for small businesses and community spaces.

---

## What Is OpenShelf?

OpenShelf is a small self-hosted offline library system built on low-power Wi-Fi hardware.

Each node creates its own local access point and serves a lightweight collection of files directly to anyone nearby. Users connect to the node’s Wi-Fi, open the local interface, and browse whatever the host has chosen to share.

The system is designed for simple local distribution of useful information in physical spaces like cafés, community gardens, pop-ups, small businesses, and neighborhood events.

It does not require internet access, accounts, apps, or user tracking.

---

## Why It Exists

A lot of useful local information still depends on internet access, social media, or QR links that lead to external platforms.

That creates unnecessary barriers.

OpenShelf was built as a way to keep small, practical resources physically tied to the spaces they belong to. Instead of sending people outward to apps or websites, the information stays local and directly accessible on-site.

It also avoids the surveillance model most digital systems default to. OpenShelf does not collect user data, track activity, or require any form of account or login.

The goal is simple: make it easier for people to share useful things with the people already standing there.

---

## How It Works

Each OpenShelf node runs as a self-contained local Wi-Fi access point.

At a participating location, visitors will typically see a small sign showing the OpenShelf network name and a QR code.

They connect to the node’s Wi-Fi, scan the QR code, and are taken directly to the local web interface hosted on the device. From there they can browse and download whatever files have been loaded onto that node.

No internet connection is required.

Each node can be customized for its location and purpose, allowing hosts to curate their own collections based on the needs of their space.

---

## What Can Live On A Node?

OpenShelf is designed for small, lightweight files that are easy to access and quick to download.

In practice, files under 1MB tend to work best for fast transfers and low-friction access across a wide range of devices.

A node can host things like:

- event flyers and schedules

- menus and local coupons

- community guides and resource sheets

- multilingual information

- mutual aid contacts and safety information

- recipes, plant guides, and workshop notes

- zines, poems, and small art PDFs

- maps, directions, and neighborhood info

What lives on a node depends entirely on where it is placed and what its host wants to share.

---

## Hosting A Node

Running an OpenShelf node requires very little infrastructure.

At minimum:

- a small space to place or mount the node
- a visible sign with the Wi-Fi name and QR code
- a power outlet or battery pack

Nodes use very little power and are intended for continuous long-term operation. Actual uptime depends on power quality, enclosure, and deployment conditions. In typical indoor use, electricity cost should be very low, usually only a few dollars per year.

The system is meant to be lightweight, low-maintenance, and easy to integrate into existing community spaces.

---

## Current Status

OpenShelf is currently in active pilot development.

The public-facing site is live, prototype nodes are built and functioning, and small-scale real-world deployment is the current focus.

Core firmware and deployment tooling are being kept private for now while the project is tested and refined.

---

## Repository Structure

```text
OpenShelf/
├── README.md
├── images/
│   └── openshelf-nodes.jpg
├── docs/
│   ├── HARDWARE.md
│   ├── DEPLOYMENT.md
│   └── ROADMAP.md
└── firmware/
    └── README.md
```

---
## Documentation

- [Hardware](docs/HARDWARE.md)

- [Deployment](docs/DEPLOYMENT.md)

- [Roadmap](docs/ROADMAP.md)
