# E-Commerce User Behavior & Funnel Analysis

## Overview
Analysis of user behavior on an e-commerce platform, tracing the full conversion funnel from page view through purchase to identify drop-off points, traffic source performance, and revenue drivers. Built using MySQL and Excel, with results cross-validated between both tools.

## Dataset
A sample dataset of ~9,400 events across 5,000 users, covering event type (page_view, add_to_cart, checkout_start, payment_info, purchase), traffic source (email, organic, paid_ads, social), product ID, purchase amount, and timestamp.

## Tools Used
- MySQL
- Microsoft Excel (Pivot Tables, Charts)

## Analysis Performed
- User funnel analysis (page_view → add_to_cart → checkout_start → payment_info → purchase)
- Traffic source analysis
- Conversion rate analysis (stage-by-stage and overall)
- Product performance
- Revenue analysis
- Customer journey timing (time taken between funnel stages)

## Key Findings
- Email converts best (~34% page view to purchase) despite the lowest traffic volume.
- Social has the weakest top-of-funnel conversion (~13.6% view-to-cart), suggesting a mismatch between social ad creative and actual product pages, not a checkout problem.
- Once a user adds to cart, conversion stays high (70-94%) across all traffic sources. The funnel's biggest leak is at the very first step, not checkout or payment.
- Organic traffic drives the most total revenue (~42%) through volume, even though it doesn't have the highest per-user conversion rate.
- All 6 products convert within a tight 15.5-17.8% range, performance is driven by traffic source, not product.
- Total revenue: $87,975.11 across 826 purchases.

## How to Use
1. Open User_Events_Analysis.xlsx to review the Pivot Tables and pre-built conversion/revenue breakdowns.
2. Run the queries in SQL_Queries.sql against a MySQL instance with a matching user_events table to reproduce the results.

## Files
- SQL_Queries.sql
- User_Events_Analysis.xlsx
