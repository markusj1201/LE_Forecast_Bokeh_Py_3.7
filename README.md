# LE_Forecast_Bokeh_Py_3.7
 Decline Curve Analysis¶ Python and Bokeh can be used to perform a decline curve analysis on an example dataset. This demonstration of DCA in Python borrows heavily from excellent work done by Lukas Mosser. This uses the same methodology of curve fitting, but uses Bokeh for plotting, which is more appropriate for interacting with DCA analysis.



DCA Theory
Decline curves provide us with an empirical method to predict expected ultimate recovery and cummulative production of a reservoir.

There are three classic types of decline curves:

Exponential decline
Hyperbolic decline
Harmonic decline
The production rate as a function of time is given as follows:

Exponential Decline
$$q(\Delta t)=q_i e^{-a\Delta t}$$
where $q_i$ is the initial rate, and $a$ is the decline rate. The exponential decline curve has one fitting parameter: $a$

Hyperbolic Decline
$$q(\Delta t)=\frac{q_i}{(1+ba_i\Delta t)^{(\frac{1}{b})}}$$
where $q_i$ is the initial rate, and $a_i$ is the decline rate, $b$ fractional exponent. The hyperbolic decline curve has two fitting parameters: $a_i$ and $b$

Harmonic Decline
$$q(\Delta t)=\frac{q_i}{(1+a_i\Delta t)}$$
where $q_i$ is the initial rate, and $a_i$ is the decline rate. The harmonic decline curve has one fitting parameter: $a_i$
