# Exotic Trader – Pricing and Managing a Callable Bond

## Overview

This project presents a complete workflow for pricing a callable bond and managing the associated call risk over time. It is designed from the perspective of an exotic interest rate trader and provides both theoretical background and a Python-based implementation.

The notebook walks through bond pricing fundamentals, callable structures, yield curve modeling, scenario generation, and hedging strategy design using standard fixed-income instruments such as swaps.

## Objectives

* Price a callable bond using discounted cash flows and call schedule constraints.
* Generate realistic synthetic yield curves and model rate dynamics over a quarter.
* Evaluate call risk and simulate call exercise decisions.
* Design and backtest a risk-management strategy using swaps or bonds.
* Provide clean, modular Python functions for pricing, simulation, and hedging.

## Financial Background

A callable bond price is the minimum between:

1. The price of the non-callable bond discounted on the yield curve.
2. The value implied by the call price when the issuer exercises its option.

The notebook details:

* Discounting conventions
* Cash-flow structures
* Yield curve interpolation
* Callability features
* Rate-shift modeling for scenarios
* Trader-oriented risk management considerations

## Features

* Yield curve interpolation using `scipy.interpolate.interp1d`
* Synthetic rate scenario generation (parallel shifts, steepening, flattening)
* Callable bond pricing engine
* Call decision logic simulation
* Strategy design: entering fixed-payer swaps to hedge the downside if rates fall
* PnL monitoring and scenario analysis
* Visualizations using Matplotlib

## Code Structure

The implementation is organized into clear components:

1. **Pricing Functions**

   * Non-callable bond pricing
   * Callable bond pricing with call schedule

2. **Curve and Scenario Tools**

   * Yield curve interpolation
   * Stochastic/structured rate shifts

3. **Risk Management Module**

   * Swap valuation
   * Hedge adjustments based on rate moves
   * Quarter-long PnL tracking

4. **Visualization & Analysis**

   * Yield curves
   * Price evolution
   * Hedge performance
