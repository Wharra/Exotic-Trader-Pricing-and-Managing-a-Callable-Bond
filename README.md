# $\color{DarkSlateBlue}{\textbf{Callable\ Bond\ Pricing\ and\ Risk\ Management}}$

## $\color{SteelBlue}{\textbf{1.\ Project\ Context}}$

This project develops a complete pricing and risk-management framework for a callable bond, aligned with interest-rate trading practices.
It covers term-structure modelling, discounted cash-flow valuation, call exercise logic, and hedging strategies.

The main deliverable is a Python notebook presenting the full workflow: data construction, model specification, implementation, scenario simulation, and performance analysis.

## $\color{SteelBlue}{\textbf{2.\ Functional\ Objectives}}$

### $\color{MidnightBlue}{\textbf{2.1.\ Pricing}}$

Develop valuation models for:

* a non-callable bond using discounted cash flows;
* a callable bond by comparing continuation value with call price.

Implement all required financial mathematics for cash-flow generation and discounting.

### $\color{MidnightBlue}{\textbf{2.2.\ Yield\ Curve\ Modelling}}$

Implement continuous term-structure interpolation (`interp1d`).
Generate meaningful rate scenarios, including:

* parallel shifts,
* twists and slope variations
* multi-factor curve dynamics affecting convexity.

### $\color{MidnightBlue}{\textbf{2.3.\ Call\ Exercise\ Analysis}}$

Determine optimal call exercise decisions based on:

* comparison with callable strike;
* sensitivity to interest-rate levels and dynamics.

Compute risk metrics:

* duration,
* convexity,
* call convexity.

### $\color{MidnightBlue}{\textbf{2.4.\ Hedging\ Strategy}}$

Provide tools to:

* price standard interest-rate swaps,
* calibrate hedges via notional sizing and curve-exposure alignment,
* mitigate negative convexity introduced by callability.

### $\color{MidnightBlue}{\textbf{2.5.\ Simulation\ and\ Performance\ Tracking}}$

Simulate daily rate movements over a chosen horizon.
Decompose PnL into:

* rate-driven effects,
* call-risk evolution,
* hedge performance contribution.

## $\color{SteelBlue}{\textbf{3.\ Technical\ Specifications}}$

### $\color{MidnightBlue}{\textbf{3.1.\ Technology\ Stack}}$

* Python 3.8+
* Required libraries:

  * numpy
  * scipy
  * matplotlib

### $\color{MidnightBlue}{\textbf{3.2.\ Code\ Architecture}}$

#### $\color{DarkSlateBlue}{\textbf{Pricing\ Module}}$

* Non-callable bond valuation
* Callable bond valuation with early-exercise logic

#### $\color{DarkSlateBlue}{\textbf{Yield\ Curve\ Module}}$

* Interpolation functions
* Deterministic and stochastic scenario generation

#### $\color{DarkSlateBlue}{\textbf{Risk\ Management\ Module}}$

* Swap pricing
* Hedge calibration
* PnL and sensitivity computations

#### $\color{DarkSlateBlue}{\textbf{Analysis\ and\ Visualization\ Module}}$

* Yield-curve visualisation
* Price evolution analytics
* Hedge performance comparison across scenarios
