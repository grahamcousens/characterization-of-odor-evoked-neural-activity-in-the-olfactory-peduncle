# medial-olfactory-cortex
This repository contains single-unit neural activity recorded from the tenia tecta and anterior olfactory neucleus in the anesthetized mouse. Please see the manuscript for details on experimental design (to be updated once published).

Data are contained in matlab .mat files (89 total, one for each cell) with the following variables:
cell: spike times in sequential list
odors: matrix of odor onset times for up to 14 stimuli
RESP_PKS: peaks of ongoing respiration cycles, if recorded along with the cell
sessduration: duration of recording session
All data reported in seconds.

Matlab code branches from "run.m", and the data directory must be set in Line 4. 
Analysis windows referenced to odor onset and analysis bin size are specified in Line 8. Default selects an 8 sec interval centered on odor onset with a 4 sec bin size.
Cell selection is specified in Line 14. Default selects all cells. 
create_spontaneous returns mean interspike intervals and coefficients of variation. 
create_psth returns binned raw spike counts.
create_phases returns the distribution of binned spikes relative to respiration phase, along with population vector for each cell.
