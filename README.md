# Purdue Aviation Management Practice: Airline

This is a small personal project I developed while studying at Purdue University. It is not an official Purdue project and is not endorsed by the university.

This project plans narrowbody international routes and low-seat-count narrowbody routes out of North American airports, and compares them on demand, cost and fit.

## Business question
For a narrowbody aircraft, which international routes from North American hubs are worth flying, and which low-seat-count routes can still cover their costs?

## Planned scope
1. **Route universe**: nonstop international city pairs served or plausibly servable by narrowbody aircraft from North American airports, with the aircraft type and range assumed for each.
2. **Demand estimate**: passenger demand per route from public traffic statistics (for example, US DOT and Statistics Canada), split by origin and destination.
3. **Seat-count scenarios**: each route tested at standard and low seat configurations, comparing load factor, revenue per trip and break-even seats.
4. **Cost model**: trip cost from block time, fuel, crew, and airport charges, with every input and its source recorded.
5. **Route comparison**: a ranked table of routes by estimated contribution per departure, with sensitivity to fuel price and load factor.
6. **Assumptions and limits**: a section listing every assumption and what it would change in the result.

7. **Seasonal routing**: route demand is split by season. Winter (Dec–Mar) tests sun and resort destinations, with Mexico as the core case. Summer (Jun–Aug) tests Alaska and northern leisure routes. Each season is scored on load factor and contribution per departure separately, so a route can be a winter-only or summer-only option.
8. **International student flows**: routes are also scored on their value in moving students (for example, Canada and US origins to and from student-heavy source markets in South and East Asia, and the reverse in the academic calendar). Demand is taken from public student-mobility statistics (for example, IRCC study-permit data and IIE Open Doors), and this route group is kept separate in the ranking so its results can be read alone.

9. **Fare forecast**: a fare model per route and season, built from public fare data (for example, US DOT DB1B fare samples and Statistics Canada air-fare series). Inputs are fuel price, load factor, booking lead time, and season. The model is tested on held-out months and reports the error next to each forecast. Results are published as a Tableau dashboard with route, season and scenario filters, so the fare path can be compared against the contribution ranking.
10. **Student-to-seat conversion (assumption)**: study-permit and enrolment counts from IRCC and IIE are not airline passengers. Demand from student flows is estimated by converting a count of students into trips per year (assumed trips per student per year, and share who fly on the route), and every conversion rate is listed in the assumptions table with its source and the result it would change.

## Status
Project started. No analysis has been completed or published yet. Results will be added to this repository as they are finished.
