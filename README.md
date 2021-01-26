# TopReconstruction

Top quark reconstruction work for Dr. Michael Fenton

The goal is to reconstruct top-antitop quark interactions and to identify the down jet for spin-correlation experiments.
The codes are implemented on Jupyter notebooks and require PyRoot to function.

MC16e is a dataset with both real and simulated data representing data-taking conditions at the LHC for the year 2018.

The primary codes are in the MC16e_pt_selection and MC16e_pt_selection_strict ipynb files. They primarily implement a Pt cutoff (default is 35 GeV) and a mass-window method for finding the down quark jet, although other methods are also available in the code and can be used instead. 

MC16e_pt_selection requires that the down jet have a Pt above the Pt cutoff.

MC16e_pt_selection_strict requires that all the jets in an event must have a Pt above the Pt cutoff.

Both files will output a root file with all events that pass the selection process and for which the t-tbar interaction can be reconstructed.

plot_weak and plot_strict create histograms of the results from MC16e_pt_selection and MC16e_pt_selection_strict, respectively.
