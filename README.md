# Accenture Skills Navigator

AI solution 06 of 14 · HR · built for **Accenture**

Prepared by **K Bhargav Raju**.

## Problem statement

A company has sufficient employees on paper but continues to miss project deadlines because the required skills are not available at the right time. Develop an AI workforce intelligence system that maps employee skills against business requirements, identifies critical skill gaps, and recommends hiring, training and internal allocation strategies.

## Why Accenture

Accenture staffs hundreds of thousands of people on client projects. Headcount can look fine while the specific skills a project needs next month are booked elsewhere. This tool maps skills to demand and decides hire, train or move.

## Algorithm

1. **Collect skills and pipeline**: Profiles, certifications, allocation, project pipeline
2. **Standardise skills**: Map free-text CV skills to one taxonomy
3. **Build skill matrix**: Proficiency 0-5 per person per skill
4. **Forecast demand**: Holt trend forecast per skill, 6 months ahead
5. **Find gaps**: Forecast demand vs available qualified people by month
6. **Match people to projects**: Cosine similarity on skill vectors + greedy assignment
7. **Hire, train or move**: Rule engine on gap size, lead time and near-ready staff
8. **Staffing plan**: AI analyst writes the plan

## Data

One delivery centre: 420 consultants, 14 skills, 24 months of demand history and 12 upcoming projects (sample data). All figures are illustrative and are not Accenture's actual numbers.

## How to use

Open `index.html` in any web browser. No installation is needed; the whole tool is one self-contained file.

The controls panel lets you change proficiency that counts as qualified, months to train a near-ready person, and the analysis reruns instantly. "New sample data" generates a fresh dataset.

## AI analyst panel

The "Ask the AI analyst" panel answers questions about the results in plain English through Claude. It works when the page is opened as a Claude artifact on claude.ai. Opened from GitHub, GitHub Pages or a local folder, all the models, charts and controls still run, and the panel shows that it is unavailable.
