# qPCR Absolute Concentration Calculation

The code provided is for a python implementation of Fieller's Theorem for error calculation when fitting a standard curve described by S. Pizzamiglio et al (2007). The original paper [Confidence interval for DNA/mRNA concentration by real-time PCR](https://journals.sagepub.com/doi/pdf/10.1177/172460080702200312) describes the rationale for this approach and compares it to another popular approach.

The code implements the calculation of the upper and lower prediction intervals of the concentration and ct values of an unknown sample given a standard curve with multiple dilutions.

Plots are generated using the plotly library and examples are shown below.

## Usage

Provide a suitable .csv file in the same format as the example ('InternationalStandards.csv'). Some tweaking of the ranges for the residuals and standard curve plots will be necessary and can be done in the layout sections of the plotly specification, under xaxis=dict(range=[1,5.5], tickvals=[10, 100, 1000,10000,100000]).

## Example Plots

### Plotting of Residuals
![Residuals](https://github.com/mcrone/qpcr_abs_calibration/blob/master/images/residuals.svg)

### Plotting of Prediction Intervals of concentration of unknown sample
![Xpredintervals](https://github.com/mcrone/qpcr_abs_calibration/blob/master/images/std_curve.svg)

### Zoomed Plot of Prediction Intervals of concentration of unknown sample
![Xpredintervalszoom](https://github.com/mcrone/qpcr_abs_calibration/blob/master/images/std_curve_zoom.svg)


### Plotting of Prediction Intervals of concentration and Ct values of unknown sample
![Ypredintervals](https://github.com/mcrone/qpcr_abs_calibration/blob/master/images/ypred.svg)

### Zoomed Plot of Prediction Intervals of concentration and Ct values of unknown sample
![Ypredintervalszoom](https://github.com/mcrone/qpcr_abs_calibration/blob/master/images/ypred_zoom.svg)

## Funding

UKDRI  
Community Jameel  
UKRI-EPSRC (EP/R014000/1)  



