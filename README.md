# Preheat Train Fouling Digital Twin

## Project Summary

This repository contains a refinery crude preheat train fouling digital twin developed as an industrial analytics, predictive maintenance, and asset performance management project.

The digital twin models thermal performance degradation in shell-and-tube heat exchangers due to fouling accumulation, simulates industrial instrumentation and historian data flows, estimates energy recovery losses, predicts maintenance requirements, and provides decision-support outputs for refinery operations.

The project incorporates a realistic industrial architecture including field instrumentation, PLC data acquisition, historian systems, SQL analytics, digital twin calculations, dashboard visualization, and maintenance forecasting.

The simulated refinery process consists of multiple crude preheat exchangers recovering thermal energy from hot process streams before crude oil enters the fired heater.

Synthetic datasets are generated using engineering assumptions and process-realistic operating ranges. The project is intended for engineering analytics demonstration, portfolio development, and educational purposes and is not a validated refinery operations system.

---

## Industrial Architecture

Field Instrumentation

↓

PLC Layer

↓

SCADA / DCS Layer

↓

Historian Database

↓

SQL Analytics

↓

Digital Twin Engine

↓

Power BI Dashboard

↓

Maintenance Decision Support

---

## Current Status

The current baseline model:

* Simulates continuous refinery preheat train operation.
* Models fouling accumulation in multiple heat exchangers.
* Tracks thermal and hydraulic performance degradation.
* Calculates heat transfer KPIs.
* Generates historian-quality process datasets.
* Simulates PLC and instrumentation tag structures.
* Produces asset health scores.
* Forecasts maintenance interventions.
* Generates Power BI-ready datasets.
* Supports SQL-based industrial analytics.
* Includes engineering validation workflows.

---

## Asset Register

| Asset ID | Equipment Description     | Service             |
| -------- | ------------------------- | ------------------- |
| E-101    | Crude Preheat Exchanger A | Crude Preheat Train |
| E-102    | Crude Preheat Exchanger B | Crude Preheat Train |
| E-103    | Crude Preheat Exchanger C | Crude Preheat Train |

---

## Simulated Instrumentation

Each exchanger includes:

### Temperature Measurement

TT101_IN

TT101_OUT

TT102_IN

TT102_OUT

TT103_IN

TT103_OUT

### Pressure Measurement

PT101_IN

PT101_OUT

PT102_IN

PT102_OUT

PT103_IN

PT103_OUT

### Flow Measurement

FT101

FT102

FT103

### Differential Pressure

DP101

DP102

DP103

---

## PLC Layer

The PLC layer simulates:

* Data acquisition
* Signal processing
* Alarm generation
* Historian logging
* KPI trigger conditions

Example logic:

IF DP101 > Fouling Threshold

THEN Fouling Alarm = TRUE

IF Asset Health Score < 60

THEN Maintenance Alert = TRUE

---

## SCADA / DCS Layer

The SCADA layer provides:

* Process monitoring
* Alarm management
* Equipment status visualization
* Operator dashboards
* Asset condition tracking

---

## Historian Layer

The historian stores time-series process information including:

* Temperatures
* Pressures
* Flow rates
* Differential pressures
* U-values
* Fouling resistance
* Asset health indicators

Data are generated at configurable sampling intervals to emulate industrial historian systems.

---

## Engineering Models

The digital twin calculates:

### Heat Duty

Q = mCpΔT

### Overall Heat Transfer

Q = UAΔTlm

### Fouling Resistance

Rf = (1/Uf) − (1/Uclean)

### Pressure Drop Growth

ΔP = f(Fouling Severity)

### Asset Health Score

Weighted score based on:

* U-value degradation
* Fouling resistance
* Pressure drop increase
* Energy recovery efficiency

---

## SQL Analytics Layer

The SQL layer supports:

* Historian queries
* KPI calculations
* Asset monitoring
* Maintenance forecasting
* Dashboard integration

---

## Core KPIs

| KPI                      | Description                   |
| ------------------------ | ----------------------------- |
| Heat Recovery Efficiency | Thermal recovery performance  |
| Fouling Resistance       | Fouling severity indicator    |
| Overall U-Value          | Heat transfer performance     |
| Pressure Drop Growth     | Hydraulic degradation         |
| Energy Loss Cost         | Estimated operating penalty   |
| Cleaning Priority Index  | Maintenance ranking metric    |
| Predicted Cleaning Date  | Forecasted intervention date  |
| Asset Health Score       | Composite condition indicator |

---

## Maintenance Forecasting

The maintenance module generates:

* Cleaning recommendations
* Predicted cleaning dates
* Asset ranking
* Risk classifications
* Cost avoidance estimates

---

## Power BI Dashboard

Dashboard pages include:

### Executive Overview

* Fleet health score
* Current maintenance risk
* Energy recovery efficiency
* Estimated annual losses

### Exchanger Health Monitoring

* Fouling growth trends
* U-value degradation
* Pressure drop analysis
* Equipment ranking

### Maintenance Planning

* Cleaning forecasts
* Maintenance priorities
* Intervention scheduling
* Cost avoidance analysis

---

## Validation Strategy

### Level 1: Engineering Validation

* Energy balance verification
* Heat transfer consistency checks
* Fouling resistance validation

### Level 2: Literature Validation

Comparison against published refinery fouling studies.

### Level 3: KPI Validation

Verification of:

* Asset health scores
* Cleaning priorities
* Forecast outputs

### Level 4: Industrial Benchmarking

Comparison against publicly available refinery case studies and industry performance benchmarks.

---

## Skills Demonstrated

* Chemical Engineering
* Process Engineering
* Heat Transfer
* Refinery Operations
* Industrial Automation
* Instrumentation Engineering
* PLC Systems
* SCADA Systems
* Predictive Maintenance
* Reliability Engineering
* Industrial Analytics
* Digital Twin Development
* Python
* SQL
* Power BI
* Asset Performance Management

---

## Handoff Note

Users should review engineering assumptions, validation studies, and generated datasets before relying on results. All outputs are provided as demonstration artifacts and are not intended for operational deployment without further engineering validation.

---
## Currently Under Development (VS Code)
> **Project Status:** This project is currently under active development in Visual Studio Code. The repository structure, engineering models, synthetic historian datasets, and documentation are being developed incrementally. New features, validation studies, and dashboard outputs will be added as the digital twin evolves.
