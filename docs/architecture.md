# Technical-product architecture

This document describes architecture choices at a product level. It does not publish the commercial application source code.

## Local-first core

The application is designed so core project data and image processing can remain on the user's machine. This reduces dependency risk for production work and avoids making cloud upload a prerequisite for handling client artwork.

## Frontend and desktop direction

The application uses a React + TypeScript + Vite frontend and is packaged toward a Tauri desktop model using the same core product code.

## Domain logic separated from presentation

Crochet and product-domain logic is kept outside the interface layer where practical. This supports:

- automated tests
- desktop packaging
- multiple export formats
- future worker/background processing
- reusable logic across editor and production views

## Grid as data

The pattern is stored as structured grid data referencing palette entries. The canvas is a renderer, not the source of truth.

This enables the same pattern data to support:

- editing
- written instructions
- production mode
- yarn calculations
- SVG/PDF/PNG exports
- construction-aware views

## Versioned projects

Saved projects carry schema versions and normalisation/migration logic so older projects can receive defaults for newer settings without intentionally discarding surviving user data.

## Multi-panel project model

A project can hold front, back, sleeve and custom panels with panel-specific design state. This replaced the earlier single-chart mental model once full garments became the real unit of work.

## Cloud stage gate

Accounts, sync, subscriptions and team collaboration are deliberately downstream of local production validation. The intended SaaS architecture should extend the local-first core rather than replace it.
