# Smart India Hackathon Workshop
# Date: 24-11-2026
## Reference Number: 26013948
## Name: Mohamed Riyaz Roshan M

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
Expected Solution:Expected Solution: Create a digital marketplace that:

Connects farmers/FPOs directly with consumers and bulk buyers. • Provides logistics support. • Uses AI for demand forecasting and route optimization.

Benefits:

Better prices for farmers. 
Lower prices for consumers. 
Reduced supply chain inefficiencies..




## Proposed Solution
Rupee Trail: a demand-first marketplace with price transparency

1. Detailed explanation

Most farm marketplaces begin with the farmer listing produce and hoping a buyer shows up. That leaves the farmer carrying the risk of unsold stock, and this risk is exactly what middlemen get paid to absorb. Rupee Trail reverses the flow: buyers commit first, and farmers harvest to order.

Community demand pools: hostels, college canteens, apartment communities and small retailers create a weekly pool, for example "300 kg tomatoes and 150 kg onions for Friday". Pools close 48 hours before delivery.
Farmer/FPO bidding: nearby farmers and Farmer Producer Organizations (FPOs) see the pooled demand and bid to fill it. A guaranteed buyer means no unsold stock and no distress selling.
Pooled delivery: one truck serves one drop point per community instead of many doorstep deliveries, which lowers last-mile cost.
Rupee Trail receipt: every order shows where each rupee went (farmer, transport, FPO, platform), compared with the typical mandi-and-retailer chain.

2. How it addresses the problem

Problem	How Rupee Trail addresses it
Middlemen absorb risk and take large margins	Guaranteed demand removes the risk, so the risk premium disappears
Farmers get low, uncertain prices	Fair-price band plus direct bids from FPOs and farmers
Consumers pay inflated prices	Fewer hops and pooled delivery reduce cost
Poor logistics	AI route optimization and community drop points
No visibility into pricing	Rupee Trail breakdown on every order

3. Innovation and uniqueness

It is a reverse marketplace where demand is the starting point, not a listing app.
Rupee Trail makes the middleman margin visible to both farmers and consumers.
Communities are the logistics unit, which cuts delivery cost structurally instead of relying on routing alone.
Demand forecasts are shared with farmers so they can plan what to grow.

## Technical Approach
1. Technologies to be used

Frontend: React web app (mobile-responsive), with Tamil and English
Backend: Python (Flask or FastAPI) with REST APIs
Database: PostgreSQL
Demand forecasting (AI): Prophet or scikit-learn
Route optimization (AI): Google OR-Tools
Fair-price engine (AI): regression model on public mandi price data
Maps: OpenStreetMap or Google Maps API
Payments: UPI (Razorpay sandbox)
Notifications: SMS / WhatsApp


2. Methodology and process

A community admin creates a weekly demand pool.
The forecasting model estimates quantities and flags likely shortfalls.
Farmers and FPOs within a set radius bid to fill the pool.
The price engine checks bids against the fair-price band.
The route optimizer groups pickups from several farms into one truck run.
The truck delivers to the community drop point; buyers collect.
A photo-based quality check is done at pickup, and payment is released through UPI.
A Rupee Trail receipt is generated for each order.

<img width="407" height="632" alt="image" src="https://github.com/user-attachments/assets/e2eb45f8-874e-4463-a7ec-f1c637036766" />

## Feasibility and Viability
## Feasibility and Viability

1. Feasibility

- Uses mature, low-cost technology (web app, standard forecasting and routing libraries).
- Mandi price data is publicly available, so the price engine can start without private data.
- FPOs already exist as aggregation bodies, so the supply side has a natural entry point.
- Can start as a pilot with a few communities and one or two FPOs in a single district.

2. Potential challenges and risks

- Farmers' trust and commitment to supply.
- Quality disputes between farmers and buyers.
- Demand volatility and perishability.
- Farmers with low digital literacy.
- Cold start: supply and demand are both needed to begin.

3. Strategies for overcoming these challenges
- **Trust and commitment:** FPO leaders act as guarantors, with small advance payments and ratings.
- **Quality disputes:** photo-based grading at pickup and a simple dispute flow.
- **Demand volatility:** pools close 48 hours ahead, with buffer lots and weekly forecast updates.
- **Low digital literacy:** Tamil UI, SMS/WhatsApp updates, and FPO agents as onboarding helpers.
- **Cold start:** begin with a few high-volume communities (hostels, canteens) and one local FPO.

## Impact and Benefits
1. Potential impact on the target audience

Farmers/FPOs: guaranteed buyers, better and more predictable prices, less unsold stock.
Consumers/bulk buyers: lower prices, fresher produce, transparent pricing.
Communities: a reliable weekly supply of vegetables and staples.

2. Benefits

Social: fairer income for small farmers, stronger FPOs, consumer trust through transparency.
Economic: fewer intermediaries, lower transport cost per kg, reduced distress selling.
Environmental: pooled deliveries mean fewer trips and lower emissions; demand-based harvesting reduces food waste

## Research and References
eNAM (National Agriculture Market): https://enam.gov.in
Agmarknet (mandi price data, Government of India): https://agmarknet.gov.in
SFAC, FPO promotion scheme: https://sfacindia.com
Google OR-Tools, vehicle routing: https://developers.google.com/optimization/routing
Prophet, time-series forecasting: https://facebook.github.io/prophet/
Problem statement source: SIH 26033, Ministry of Consumer Affairs, Food & Public Distribution
