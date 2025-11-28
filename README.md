# Holee-Model-Interest-Rate-Term-Structure

This repository demonstrates the implementation and calibration of the Ho–Lee short-rate model, a foundational no-arbitrage term-structure model used in fixed-income analytics.
The notebook shows how to calibrate the model to real market zero-coupon rates sourced from the Indian bond market (e.g., the curve published by Clearcorp (CCIL)).

The Ho–Lee model defines short-rate dynamics as:
dr(t) = q(t) dt + s dW(t)

Key Components of the Project:
• Import and clean market zero-coupon rates.
• Convert zero rates into discount factors.
• Calibrate q(t) via nonlinear least squares.
• Simulate short-rate paths using Monte Carlo.
• Price zero-coupon bonds by discounting cash flows along simulated paths.
• Plot yield curve, model fit, q(t), and rate simulations.


The notebook uses zero-coupon yields for tenors 0.5Y to 2.5Y obtained from the CCIL Zero-Coupon Yield Curve.
This curve represents fair-value yields for government securities after bootstrapping and is widely used in the Indian fixed-income market.

These yields can be replaced  with:
Custom market data.
Bloomberg / Reuters zero curves.
US Treasury zero curve.
Swap curve bootstrapped rates.

Applications:
• Market Risk (VaR, interest-rate stress testing).
• Fixed-income analytics.
• Treasury and ALM rate forecasting.
• Derivatives valuation using short-rate models.
• Academic and interview-ready quant demonstrations.

Techstack: Jupyter,Numpy,Scipy,Matplotlib.

