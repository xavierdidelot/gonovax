# gonovax 0.3.4

* allow setting of initial coverage in XVW model

# gonovax 0.3.3

* improve tests and add checks for bad parameter inputs

# gonovax 0.3.2

* add three-stratum waning model with no re-vaccination: X -> V -> W 

# gonovax 0.3.1

* add vignette
* add fixed parameter transform function

# gonovax 0.3.0

* add vaccine effects vea (acquisition), vei (infectiousness),
ved (duration of infection), ves (symptoms)
* rename ve -> vbe to avoid confusion

# gonovax 0.2.9

* reduce input size from run_grid

# gonovax 0.2.8

* rename strategies

# gonovax 0.2.7

* fix bug QALY cost bug

# gonovax 0.2.6

* move transform function into package

# gonovax 0.2.5

* run_grid uses length of baseline to determine time horizon

# gonovax 0.2.4

* Allow efficacy to be varied in run_onevax

# gonovax 0.2.3

* move compare function used in paper into package

# gonovax 0.2.2

* refactor to run based on strategy
* allow XVWR model to have two different vaccines (i.e. eff / dur profile)

# gonovax 0.2.1

* add four-stratum waning model: X -> V -> W <-> R

# gonovax 0.2.0

* move globals into package

# gonovax 0.1.24

* allow model restart from a future point (necessary for time-varying params)

# gonovax 0.1.23

* add GRASP 2020 data

# gonovax 0.1.22

* add varying screening rate by group

# gonovax 0.1.21

* data starts in 2010
* add beta binomial function

# gonovax 0.1.20

* add time-varying beta and eta
* add option to change compare function

# gonovax 0.1.19

* add GRASP % symptomatic data
* export data easily
* add user function for running novax

# gonovax 0.1.18

* add mcmc thinning and sampling tools

# gonovax 0.1.17

* add mcmc fitting method to gumcad data

# gonovax 0.1.16

* bug-fix: extract flows now correctly attributes vaccination / re-vaccination
* re-code model so treatment of VbE is now the same structure as VoD / VoA

# gonovax 0.1.15

* output vaccination and revaccination separately
* use parsimonious numbers of compartments in waning model

# gonovax 0.1.14

* output full time series in run_grid()
* extend baseline to 30 years

# gonovax 0.1.13
* add time-varying vaccination parameter

# gonovax 0.1.12

* export aggregate() 
* export set_strategy()

# gonovax 0.1.11

* output asymptomatic and symptomatic diagnoses

# gonovax 0.1.10

* extend baseline to 20 years
* take plot method out of package
* export format_grid

# gonovax 0.1.9

* allow vaccination of activity groups at differing rates

# gonovax 0.1.8

* add onevax_waning model

# gonovax 0.1.7

* remove n_par index as running multiple parameter sets in vectorised mode is
inefficient in ode solver.

# gonovax 0.1.6

* add option to output full results in grid_search()
* add ability to input baseline in grid_search()

# gonovax 0.1.5

* fix bug in novax_baseline()
* fix model bug that caused people to go missing in VoD
* update plot method to avoid ggplot2 warnings

# gonovax 0.1.4

* cache baseline (novax) incidence parameters
* add run_grid_onevax() which run the model with cached parameters across an
eff x dur vaccination grid
* add plot methods for grid objects

# gonovax 0.1.3

* rename model to separate novax, onevax (and in future, dualvax / dualvax_wane)
* add run_novax() and run_onevax() which run the model with cached parameters
from equilibrium if specified
* add VbE to vaccination output

# gonovax 0.1.2

* add novax_equilib() which returns the cached equilibrium compartments for all
parameters in gono_params()

# gonovax 0.1.1

* export gono_params() and allow selection of specific parameter sets
* export dualvax_initial()
* add dualvax_restart() for restarting the model from a previous position

# gonovax 0.1.0

* initial version of the model tested with Bexsero only
