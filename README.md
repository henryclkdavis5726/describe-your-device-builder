# Describe Your Device v2026 - browser-based prototype 2026

> **Describe Your Device is a web-based prototyping tool that converts natural-language descriptions into constraint programs, wiring diagrams, in-browser simulations, and downloadable firmware sketches for Arduino and ESP32.**

[![Platform](https://img.shields.io/badge/Platform-web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/henryclkdavis5726/describe-your-device-builder?style=flat-square)](https://github.com/henryclkdavis5726/describe-your-device-builder)

---

<p align="center">
  <a href="https://henryclkdavis5726.github.io/describe-your-device-builder/">
    <img src="https://img.shields.io/badge/Download-Describe%20Your%20Device%20Latest-brightgreen?style=for-the-badge" alt="Download Describe Your Device">
  </a>
</p>

> **[Download Describe Your Device v2026](https://henryclkdavis5726.github.io/describe-your-device-builder/)**

---

[Download Latest Build](https://henryclkdavis5726.github.io/describe-your-device-builder/)

---

## What is Describe Your Device?

Describe Your Device provides a browser-first workspace for shaping device concepts from ordinary language into structured models. Its constraint-programming workflow uses a CSP solver approach to describe system behavior, test constraints, and develop an initial idea into a more precise design.

The project is intended for makers, embedded programmers, and hardware enthusiasts building with Arduino or ESP32. Wiring diagrams, device simulation, and firmware sketch export are combined in a single web interface. Since the core workflow runs client-side, the tool does not rely on a server-side backend.

---

## Capabilities

- Turn natural-language device descriptions into constraint programs
- Check constraints with the AC-3 algorithm
- Produce SVG wiring diagrams that illustrate hardware arrangements
- Simulate device behavior directly in the browser
- Export firmware sketches for download
- Support prototyping workflows focused on Arduino and ESP32
- Run the primary experience without a server
- Apply PLATO prototyping ideas alongside constraint-solving methods

---

## Getting Started

1. Obtain the source by downloading or cloning the repository:
   - `git clone https://github.com/henryclkdavis5726/describe-your-device-builder.git
2. Open the project in a browser-based environment, or serve its files locally.
3. Load the main HTML entry point in a web browser.

A basic static server is sufficient for local testing:

- `python -m http.server`

After starting the server, visit the local address it reports and begin describing a device.

---

## How to Use It

1. Start the application in your browser.
2. Describe the device you want to prototype using plain language.
3. Examine the resulting constraint program and validate its model.
4. Review the generated wiring diagram and simulation results.
5. Export the firmware sketch once the design is ready.

The usual design loop is:

- Describe the device
- Verify the constraints
- Review the wiring
- Test the simulation
- Download the generated sketch

---

## Configuration

The application handles most configuration through the current browser session or project files loaded by the client.

To change its behavior, inspect the repository's main HTML file and associated client-side assets. When running locally, settings generally come from the static files and hosting environment rather than from a backend service.

Example structure:

    settings:
      mode: browser
      solver: AC-3
      target: arduino
      output: firmware sketch

---

## Requirements

- A current web browser
- Local static hosting when running the project outside a hosted page
- Sufficient browser memory for interactive simulation and diagram generation
- A development environment appropriate for Arduino or ESP32 sketches if you intend to compile the exported firmware

---

## Frequently Asked Questions

### Is a server required?

No. The main browser workflow is designed to operate without a server.

### Which embedded targets are supported?

The tool generates firmware sketches for embedded workflows including Arduino and ESP32.

### How can I get an updated version?

Use the latest repository release or the hosted download link. If you run the project locally, refresh or replace your local copy afterward.

### Why might the diagram or simulation be incorrect?

Begin by reviewing the device description and the assumptions expressed in its constraints. Even minor changes in wording may alter the generated model and the outputs that follow from it.

### Where is configuration kept?

Settings are typically managed in the browser session or in the project files served by the application.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
