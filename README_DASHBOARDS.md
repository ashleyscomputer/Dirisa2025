
# README – Driver Safety, Behaviour & Telematics Dashboards

This repository contains two complementary dashboards designed to demonstrate how telematics 
and behavioural analytics work together to understand and reduce road-accident risk.

---

# 1. Altron Telematics Dashboard  
**File:** `altron_telematics_dashboard_v3.html`  

## Purpose  
Shows how vehicle movement, speed discipline, g-forces, road conditions, and time-of-day 
patterns contribute to risk using real Altron telematics data.

## Main Features  
- Overspeeding analysis  
- High-risk record quantification  
- Average fleet risk score  
- Night-time driving exposure  
- Harsh event (braking, acceleration, cornering) analysis  
- Risk score distribution  
- Overspeed rate by road-speed band  
- Risk by hour of day  
- Harsh event patterns  
- Road condition impact (normal vs rough roads)  
- Town-level risk patterns & exposure  
- Trip-level example (speed vs risk)  

## What This Dashboard Demonstrates  
- Telematics shows **what**, **where**, and **when** risk increases.  
- It cannot explain **why** a driver behaves unsafely.  
- This gap is filled by behavioural monitoring.

---

# 2. Driver Behaviour, Fatigue & Road Risk Dashboard  
**File:** `driver_behaviour_dashboard_v2.html`

## Purpose  
Uses a behaviour-rich dataset (distraction, fatigue, drowsiness, seatbelt use, eating, smoking) 
to quantify how driver states directly influence accident risk.

## Main Features  
- Behavioural Safety Pulse (distraction %, drowsy %, seatbelt OFF %)  
- High-risk episode detection  
- Average risk by behaviour (phone use, fatigue, drowsiness, etc.)  
- Drowsiness vs risk (PERCLOS trend)  
- Distraction distribution  
- Seatbelt compliance & risk  
- Temporal & trip-level behavioural patterns  
- Behavioural risk profiles (radar chart)

## What This Dashboard Demonstrates  
- Behaviour is the **root cause** of many crash-risk spikes.  
- Fatigue, distraction, and non-compliance raise risk far more than vehicle signals alone.  
- Telematics alone cannot capture these states.  
- Behaviour + telematics = complete risk intelligence.

---

# How Both Dashboards Work Together

| Component | Telematics Dashboard | Behaviour Dashboard |
|----------|----------------------|----------------------|
| Measures vehicle behaviour | ✔️ | ❌ |
| Measures driver behaviour | ❌ | ✔️ |
| Shows where/when risk occurs | ✔️ | ✔️ |
| Shows why risk occurs | ❌ | ✔️ |
| Detects root causes | ❌ | ✔️ |
| Supports predictive prevention | ✔️ (with behaviour) | ✔️ |
| Justifies alerting system | Partial | Strongly |

Together, they form a complete narrative:  
**1. Telematics shows the risk surface.**  
**2. Behaviour identifies the underlying cause.**  
**3. Your app solves the missing piece through alerts and monitoring.**

---

# Files Included  
- `altron_telematics_dashboard_v3.html`  
- `driver_behaviour_dashboard_v2.html`  
- This README file  

