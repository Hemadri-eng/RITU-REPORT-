# RITU-REPORT-
Rainfall forecasting across the Indian subcontinent is one of the most complex meteorological challenges in the world. Numerical Weather Prediction (NWP) models—such as the India Meteorological Department’s Global Forecasting System (IMD GFS at 12 km), the National Centre for Medium Range Weather Forecasting Unified Model (NCUM Global), and the European Centre for Medium-Range Weather Forecasts (ECMWF IFS)—serve as the foundation for operational forecasting. However, these dynamical models exhibit substantial, systematic forecast errors.

Crucially, rainfall forecast errors over India vary drastically across different weather regimes:

During Active Monsoon phases, coarse models systematically underestimate localized convective cloudbursts and extreme rainfall spikes along mountain barriers and core monsoon zones by 15% to 30%.
During Break Monsoon phases, the same models suffer from persistent false-wet bias, predicting continuous light drizzle across central India when the weather is actually dry.
Under Monsoon Depressions and Low-Pressure Systems, cyclonic vortex tracking and intense core convergence require asymmetric extreme-value loss modeling.
In Orographic (Western Ghats & Himalayas) and Coastal zones, boundary-layer interactions and steep topography trigger localized forced ascent that coarse grid resolutions smooth out.
A conventional, uniform bias-correction method (such as standard linear scaling or a single static machine-learning regressor applied year-round) cannot perform equally well across these fundamentally different physical conditions. Correcting for active monsoon underestimation causes severe false alarms during break periods, while correcting for break periods dampens real flood-producing downpours.

The objective of our project, developed under SIH Problem Statement 26142, is to build RITU (Regime-Intelligent Temporal Understanding for Rainfall): an end-to-end meteorological AI post-processing system that first diagnoses the prevailing synoptic weather regime from atmospheric dynamics, and then dynamically routes the raw NWP forecast through a dedicated, physics-guided AI correction model. The ultimate goal is to improve district- and grid-level rainfall forecasts, eliminate false alarms, and reliably capture heavy (>64.5 mm) and very heavy (>115.6 mm) extreme rainfall events.

