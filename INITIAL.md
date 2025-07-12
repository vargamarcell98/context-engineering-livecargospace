# Project Name: FreightSync Core

This project is a freight software tool to help transport carriers and freight forwarders optimize cargo space usage and increase visibility across the network.

## Core Concept

We want to build a basic but powerful SaaS system.

### Carrier Role

- Carriers can manually enter planned transports (pickup/drop-off time & location, capacity used, etc.).
- Vehicles can be registered with detailed cargo space (length/weight).
- Real-time vehicle location is retrieved via telematics API integration.
- Gantt chart and map view show live cargo space status.
- Gantt blocks can be edited (drag & drop or click).
- Carriers can register clients and assign them to transports.

### Freight Forwarder / Supplier Role

- FFs and suppliers can see shared cargo space from carriers they work with.
- No CRM features for this role.
- View is read-only: just Gantt chart and map of available space.

## Tech Stack

- Frontend: Next.js
- Backend: Supabase (PostgreSQL, Auth, Storage, Functions)
- Target environment: mobile-first responsive UI

## Objective

The MVP is focused only on cargo space visibility and manual transport entry. No bidding, no AI, no pairing algorithm yet.

The business model will be a SaaS subscription starting at 100–150 EUR/month.
