# Counterparty_Credit_Risk
CVA project for CQF 2017 cohort
The aim of this project is to demonstrate techniques used to calculate a Credit Valuation Adjustment (CVA)
for a fixed income instrument, an interest rate swap (IRS). An hypothetical scenario has been assumed where
two different counterparties enter into an IRS written over 6 month LIBOR at T0 for 5 years maturity and then
credit value adjustments (CVA) are calculated to reflect the credit risk on the horizon until the end of fixed
income instrument. The counterparty A receives the fixed leg and pays the floating leg where as counterparty
B (Deutsche Bank) pays the fixed leg and receives the floating leg of the IRS. The mark to market (MTM) of
the IRS has been simulated by using Heat-Jarrow-Morton framework model (HJM) over the recent data
obtained from the Bank of England’s (BOE) statistics on bank liability curve. Then, the yield curve structure
has been simulated for different scenarios in order to obtain MTM values on future horizons. This process
then followed by generating an expected exposure profile for the underlying fixed income instrument where
the fair price of credit risk taken by counterparty A has been calculated using below formula set;
CVA = 
0
T
(1 - R) * EEt * DFt * dPDt
where;
EEt = EQ[max (MTMt , 0]
dPDt = ΔPDt = PD(ti-1,ti) = P(0, ti-1) - P(0, ti)
