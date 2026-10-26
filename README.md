# BESTFAB Atlas

**An interactive 3D atlas of a steel fabrication project.** Think of a human anatomy explorer, applied to a steel building: open a job, spin the structure, pull it apart down to the last purlin cleat, and click any piece to see what it is, what it's made of, where the steel came from, how far through the shop it is, and every certificate attached to it.

![BESTFAB Atlas](screenshots/atlas-overview.png)

## What it does

- **Reads real Tekla IFC4 exports.** Drop an `.ifc` file on the window and the atlas rebuilds around that job: geometry, part marks, assemblies, grades, section profiles, lengths and weights.
- **Detailed to the individual fastener.** The sample building has over 12,000 modelled parts, and every bolt, nut, washer, screw and weld is a clickable object with its own mark, mass, standard and certificates.
- **Explode, filter and inspect.** Toggle structural systems, explode the assembly from assembled to laydown, colour by system, fabrication stage, QA status or material, and fly through the model.
- **Runs the job, not just the model.** Tenders and quotes, takeoff and pricing, cutting lists and offcut stock, plate nesting, CNC files, shop loading, hold points and NCRs, QA register, truck loads and lift charts, programme dates, cash flow, and a tamper-evident audit trail.

## Tech stack

| Area | Tools |
| --- | --- |
| App | React, TypeScript, Vite, Zustand |
| 3D | three.js, web-ifc for IFC parsing |
| Documents | pdf-lib, pdfjs, Excel import and export, QR codes |
| Quality | Vitest test suite and stress tests on buildings up to 43,000 parts |

## Source code

Built for a steel fabrication business, so the source code is kept in a private repository. I'm happy to demo it in an interview.

**Built by Omar Al Azhari** · [LinkedIn](https://www.linkedin.com/in/omar-alazhari-028a6a203)
