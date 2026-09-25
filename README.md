# Enterprise Webhook Conditional Routing & Fallback Architecture (Make)

## Project Overview
An enterprise-grade automation workflow designed in **Make (Integromat)** that dynamically routes incoming webhook payloads based on business priority while implementing a native fallback path for standard or edge-case requests.

This project demonstrates robust logic branching, boolean filter conditions, execution tracking, and fault-tolerant data routing.

## Key Features
- **Dynamic Logic Branching:** Evaluates payload conditions in real time using logical OR rules (`tier = Enterprise` OR `priority = High`).
- **Native Fallback Handling:** Utilizes Make's native fallback router configuration to capture unhandled payloads, ensuring zero dropped requests.
- **Event-Driven Webhook Trigger:** Listens for real-time incoming JSON data.

## Technical Proof & Documentation

### Path 1: High-Priority / Enterprise Path
- `01_Enterprise_Route_Canvas.png` - Visual scenario execution showing top path activation.
- `02_Enterprise_Route_Bundle.png` - Data bundle verification confirming payload attributes.
- `03_Enterprise_Filter_Logic.png` - Logical OR filter configuration (`tier = Enterprise` OR `priority = High`).

### Path 2: Standard Fallback Path
- `04_Fallback_Route_Canvas.png` - Visual scenario execution showing fallback path activation.
- `05_Fallback_Route_Bundle.png` - Output bundle verification for fallback data.
- `06_Fallback_Filter_Setting.png` - Native fallback filter setting (`Set as fallback = Yes`).

## Tech Stack
- **Platform:** Make (Integromat)
- **Protocol:** Custom Webhooks (HTTP POST / JSON)
- **Control Flow:** Router, Filter Conditions (OR logic), Fallback Routing
