# Local Inflation Histories and Mortgage Delinquency

**A State-Dependent Analysis Across U.S. Metropolitan Areas**

Honors thesis submitted in partial fulfillment of the requirements for the B.A. in Economics with Honors, University of California, Berkeley (2026).

## Overview

Why does the same inflation episode hit some places harder than others? This paper asks whether a metro area's prior local inflation history changes how *new* local inflation pressure transmits into future mortgage delinquency.

Using a monthly panel of 25 U.S. metropolitan areas, I find that the marginal effect of a new local inflation gap on future delinquency is **smaller in metros that have been running persistently above the national inflation rate** — a state-dependent pattern that pooled national estimates wash out entirely.

## Research Question

Does prior local inflation exposure moderate the effect of new local inflation pressure on realized mortgage delinquency?

## Approach

- **Panel:** 25 U.S. metros, monthly, ~2016–2025 (raw data 2013–2026)
- **Key variable:** local inflation *gap* (metro CPI inflation minus national CPI inflation), with prior *exposure* defined as the rolling average of past local gaps (6, 12, 24, and 36-month windows)
- **Dependent variable:** 12-month cumulative change in mortgage delinquency rate
- **Specification:** two-way fixed effects (metro and month) with lagged controls for unemployment, house-price growth, and nominal wage growth; HC1 robust standard errors
- **Identification:** within-metro variation around national conditions, with the gap-by-exposure interaction as the coefficient of interest

Five samples are compared: all metros, the baseline five (Baltimore, Miami, Phoenix, San Francisco, Tampa), Sun Belt (12 metros), top-exposure tercile (8 metros), and bottom/middle exposure (17 metros).

## Key Findings

1. **State-dependent attenuation.** The gap × exposure interaction is negative and significant in the baseline five, the Sun Belt, and the top-exposure samples. Prior exposure attenuates the marginal impact of a new local inflation gap on future delinquency.

2. **Sign flip in low-exposure metros.** In bottom/middle exposure metros, the same interaction is *positive* and significant — consistent with new inflation pressure carrying more information where local priors are weak.

3. **Persistence matters.** Attenuation deepens monotonically as the exposure window lengthens (6 → 12 → 24 → 36 months), pointing to a sustained inflation history rather than recent noise.

4. **Timing.** The negative interaction is weak at short horizons, sharpest at 12–18 months, and unstable by 24 months — consistent with delayed transmission from price pressure to mortgage distress.

5. **Robustness.** The result survives interactions with unemployment, house-price growth, and wage growth, as well as discrete high-exposure indicator specifications and direct mean-reversion controls (lagged delinquency levels and changes, metro-specific time trends).

## Interpretation

Two mechanisms from the existing literature each pick out one feature of the data uniquely:

- An **inflation-experience expectations channel** explains the bottom/middle sign flip — when local priors are weak, a new gap arrives as fresh information rather than confirmation.
- A **real debt-erosion channel under fixed-rate mortgages** explains the monotone deepening with longer exposure windows — sustained inflation gradually erodes the real value of fixed nominal payments.

Neither channel alone fits both patterns; together they do.

## Limitations

Aggregate metro-level data cannot fully separate true behavioral adaptation from residual recovery dynamics, and the sample sizes are small enough that inference rests on consistency across specifications rather than any single coefficient. Household-level panel data on income, debt, and consumption is the natural next step.

## Data

- Local CPI inflation, mortgage delinquency rates, unemployment, house-price growth, and nominal wage growth at the metro-month level
- Sources: BLS, Federal Reserve, FHFA, and other public series
