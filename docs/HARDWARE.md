# Hardware

This is the exact hardware used in the current OpenShelf prototype.

The build is intentionally simple, low-power, and easy to replicate.

---

## Core Compute

### D1 Mini (ESP8266)

Main controller.

Handles:

- Wi-Fi access point
- local web server
- SD file serving

Chosen for:

- low power use
- small footprint
- low cost
- easy replacement

---

## Storage

### 6-Pin SPI microSD Module

External file storage for hosted content.

Used to serve all files directly to connected users.

Connected over SPI.

---

### 32GB microSD Card

Stores the node’s local library.

Designed for lightweight files.

In practice, most hosted files are kept under 1MB for fast access.

---

## Power Stabilization

### 100uF Capacitor

Used across power rails for smoothing and stability.

Helps reduce voltage sag during Wi-Fi activity.

---

### 104 Ceramic Capacitor

Additional filtering for cleaner power delivery.

Used alongside the bulk capacitor.

---

## Power Interface

### Micro USB Male to USB-C Female Adapter

The D1 Mini can be powered directly through its built-in Micro USB port, which remains fully accessible inside the enclosure.

The current prototype uses a Micro USB to USB-C adapter for compatibility with modern cables.

Without the adapter, the power connection remains fully recessed and self-contained inside the unit.

With the adapter installed, the USB-C port protrudes slightly from the enclosure, as shown in the prototype photos.

---

## Mounting

### 51.5 x 32mm Perf Board Section

Cut from a larger perf board and used as the internal mounting base for the D1 Mini, SD module, and power filtering components.

Keeps the internal layout fixed and serviceable.

---

## Enclosure

### 70 x 45 x 29mm Project Box

Houses the full node.

The current enclosure size keeps the build compact while allowing enough room for internal wiring, storage, and power filtering.

Small enough for shelf placement, countertop deployment, or discreet wall mounting.
