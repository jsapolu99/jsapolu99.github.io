---
layout: essay
type: essay
title: "ICS 414 Reflection"
# All dates must be YYYY-MM-DD format!
date: 2024-12-17
published: true
labels:
  - Software Engineering
  - Design Patterns
---
## Introduction:
In my final semester of my college career, I enrolled in ICS 414: Software Engineering II under Professor Cam Moore. As part of this course, I joined a team tasked with building a product for a real-world client. This experience allowed me to gain practical, hands-on exposure to the challenges of professional software development.

## The Client:
Our client was Spire Hawaii, an accounting firm specializing in a variety of financial services, including Performance Audits, Forensic Accounting, Insurance Examinations, Accounting Consulting, Financial Statement Audits, and Systems Implementation. They approached our team with an interest in modernizing a critical aspect of their workflow.

## The Product:
Spire Hawaii envisioned an online accounting dashboard that would streamline their financial forecasting process. While they currently rely on Excel for their calculations, they wanted a user-friendly web application that could easily import financial data, perform the necessary forecasts, and present the results in a clear, visually appealing format. The goal was to create a tool accessible not only to experts familiar with Excel, but also to clients and stakeholders who might be less comfortable navigating complex spreadsheets.

## How it Went:
At the outset, the task seemed straightforward: allow users to upload CSV files, run the imported data through forecasting formulas, and produce dynamic visualizations using a charting library. We successfully implemented CSV file uploads and leveraged Recharts, a React-based charting library, to display the imported financial data. However, the biggest hurdle we faced was the forecasting logic itself. We were never explicitly given the formulas required for these calculations—only their current, intricate Excel spreadsheets. Without clear guidance on how the projections were computed, it proved difficult to replicate their results within our application. This lack of clarity led to significant confusion, ultimately preventing us from delivering the forecast functionality.

## Conclusion: 
If I had the opportunity to tackle this project again, I would prioritize obtaining explicit, detailed forecasting formulas from the client. Failing that, I would request an in-depth explanation of the logic embedded in their spreadsheets. While the client’s requirements were not deliberately unclear, as developers, we should have asked more probing questions and insisted on the necessary information upfront. Doing so would have empowered us to build the dashboard they truly envisioned.
