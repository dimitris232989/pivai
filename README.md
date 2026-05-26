# Pivai Tech — Company Website

Official website for Pivai Tech, a technology company based in Columbia, SC. Designed and developed as part of my role as an IT Assistant at the company.

**Live site:** https://pivaitech.com

## About

A production website handling real traffic. I was responsible for the design, development, and ongoing maintenance of the site, including all web design decisions and user-facing components.

## Tech stack

- HTML / CSS / JavaScript
- Built with Squarespace
- Deployed via Netlify

## Pages

- Home
- About
- Team
- Case Studies
- News
- Careers
- Contact

## Case Studies — Architecture

The Case Studies page features an interactive map and detection viewer powered by a custom backend:

- **REST API** hosted on Render (`pivai-api.onrender.com`) serves dataset metadata and file paths via `/api/datasets`
- **Backblaze B2** bucket stores the actual RGB frames and depth frames captured during road inspections
- The frontend fetches dataset configs from the API, then loads inspection frame images (RGB + depth) directly from the Backblaze-backed image paths
- Each frame includes GPS coordinates, AI-detected object classes (potholes, signs, cracks), bounding boxes, and depth data
- The map is built with Leaflet.js, with clickable markers per detection frame and real-time class filtering

## Role

- Designed and built the website
- Responsible for ongoing updates and maintenance
- Integrated the Backblaze B2 bucket and Render API into the Case Studies page
- Part of my work as IT Assistant at Pivai (Aug 2025 – Present)
