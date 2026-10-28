# Hyderabad Cafe Finder Dashboard

An end-to-end Power BI project that turns Google Places cafe data into an interactive dashboard for deciding which Hyderabad cafe to visit next, built to solve a real weekend problem: comparing cafes across a pile of browser tabs.

## 📌 Overview

I visit a new cafe almost every weekend, and choosing one meant searching Google, opening several options in separate tabs, then checking ambience, price and rating on each. This project replaces that routine with one dashboard: set a few filters, see the cafes that match, and open the one I like straight in Google Maps. The goal is to turn scattered listing data into clear, decision-ready reporting.

![Dashboard preview](docs/screenshots/dashboard.png)

## 📊 Dashboard: Hyderabad Cafe Finder

**Key Metrics:** Cafes (142) · Areas (18) · Avg. Rating (4.45) · Total Reviews (265K)

**What it shows:**
- Number of cafes per area, with Jubilee Hills (33), Banjara Hills (31) and Madhapur (20) covered most thoroughly
- Average rating by area, weighted by review count so cafes with few reviews don't distort the comparison
- Cafes by price range (Budget, Mid, Premium)
- A map of every cafe by location, sized by review count and coloured by rating
- A table of cafes to try next, with a one-click "Open in Maps" link
- KPI cards showing total reviews, average rating and visited status for a selected cafe
- Fully interactive with slicers for Area, Best For, Seating Type, Pet Friendly, Rating and Visited status

## 🛠️ Tools & Techniques Used

| Category | Details |
|---|---|
| Data Source | Excel (cafe details from Google Places search results, October 2026) |
| BI Tool | Power BI Desktop |
| Data Cleaning | Power Query: type corrections, de-duplication, splitting multi-value columns into tag tables |
| DAX | SWITCH for price bucketing, SUMX for review-weighted ratings, CALCULATE for visited counts |
| Visuals | KPI cards, map, bar and column charts, slicers, table with web URL links |
| Interactivity | Slicers for Area, Best For, Seating, Pet Friendly, Rating and Visited, with cross-filtering across all visuals |
| Design | Wireframe-first layout and a custom Power BI theme |

## ⚠️ Data Notes

- **Prices are simulated.** The Price for Two column holds placeholder values used to build and test the price-range visuals. They are not real prices.
- **Some labels are inferred.** Seating Type, Best For and Pet Friendly are first-draft labels based on venue type and reviews, not official data.
- **Snapshot data.** Ratings and review counts reflect October 2026 and will change over time.

## 🎯 What This Project Demonstrates

- Defining a problem from a real need and designing the dashboard around it, starting with a wireframe
- Modelling multi-value columns correctly by splitting them into separate tables with many-to-one relationships
- Writing DAX for custom segmentation and review-weighted ratings
- Designing a clean, consistent dashboard with a custom theme so the data stays the focus
- Being upfront about data limits, including which values are real and which are placeholders

## 👤 About Me

Data Science student based in Hyderabad, building hands-on projects to strengthen practical BI skills, from collecting and cleaning data to modelling and presenting it the way an analyst would in a real role.

**Your Name** · [LinkedIn](https://www.linkedin.com/in/your-profile) · [GitHub](https://github.com/your-username)
