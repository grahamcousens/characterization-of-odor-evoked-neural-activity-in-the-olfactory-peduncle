This repository contains single-unit neural activity recorded from the tenia tecta and anterior olfactory neucleus in the anesthetized mouse. Please see the manuscript for details on experimental design (to be updated once published).

Notes on data:

Data are contained in matlab .mat files (89 total, one for each cell) with the following variables:
cell, spike times in sequential list;
odors, matrix of odor onset times for up to 14 stimuli;
RESP_PKS, peaks of ongoing respiration cycles, if recorded along with the cell;
sessduration, duration of recording session.
All data are reported in seconds.

Notes on getting started with matlab code:

Matlab code branches from "run.m", and the data directory must be set in Line 4. 
Analysis windows referenced to odor onset and analysis bin size are specified in Line 8 - default selects an 8 sec interval centered on odor onset with a 4 sec bin size.
Cell selection is specified in Line 14 - default selects all cells. 

