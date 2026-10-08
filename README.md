# Blinkit Monthly Ration Analyzer

An AI-assisted grocery planning application that analyzes historical Blinkit orders and recommends household essentials for the current month's ration list.

> [!IMPORTANT]
> This repository is an implementation blueprint and may require selector updates before it works with the current Blinkit website. Use it only with your own account, review the site's applicable terms, and do not bypass CAPTCHA, access controls, or rate limits.

## Problem

Households often buy the same staples repeatedly but do not maintain a consistent replenishment list. This project converts past orders into a structured purchase history, estimates monthly usage, and generates an explainable ration recommendation.

## What the Application Does

1. Opens the Blinkit order-history page in a user-controlled browser session.
2. Expands available historical orders.
3. Extracts order dates, product names, pack sizes, quantities, and units.
4. Cleans and normalizes product data.
5. Aggregates purchases by product and month.
6. Identifies recurring household essentials.
7. Uses an LLM to interpret ambiguous patterns and explain recommendations.
8. Exports the proposed ration list to JSON, CSV, or Excel.
