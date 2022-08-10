## Introduction

**Lazy RLA Tools** provides multiple functions to simulate a lazy risk-limiting audit, as detailed in [Lazy Risk-Limiting Ballot Comparison Audits](https://arxiv.org/abs/2202.02607). There are four main options for this tool: 
1) Set up an election audit. This uses the name of a town, number of voters, and number of polling places in a town to create sample files used in a lazy RLA comparison audit. It outputs two sets of CVR files (one 'trusted' and one 'untrusted'), a ballot manifest, and ballot tabulation in csv format. 
2) Audit election. This uses either the files from option 1) or user-inputted files to conduct a lazy RLA comparison audit. It chooses a number of ballots to audit (using [Kaplan-Markov expected sample sizes](https://ucb-stat-159-s21.github.io/site/Notes/audit.html)), creates mock CVR files for each batch that a ballot is chosen from, and outputs the calculated risk limit based on the discrepancies found in the files. 
3) Set up and audit election. Runs option 1) and 2) detailed above.
4) Run simulation. This simulates both an election and an incremental ballot comparison audit. It creates a user-inputted number of ballots, distributes them to towns, then runs a ballot comparison audit and collects the data on a town level. It averages and outpus the data in a single csv file. This data is used for the efficiency argument of the lazy RLA comparison audit. 

This tool also provides a Jupyter notebook to act as a frontend for option 3). 

## Installation

This section provides instructions on how to run the python version of Lazy RLA Tools. To see how to set up a working Jupyter notebook, look at the following section.

First, install the necessary packages:
> pip install numpy==1.20.3

### Jupyter Notebook

TO DO: find *easiest* way to set up Jupyter notebook

To install the necessary packages in Jupyter, add this snippet to the import code block:

> import sys
> !{sys.executable} -m pip install numpy

After this code block runs the first time, you will receive a message that says: "Requirement already satisfied: numpy in dir"

## How to Use
### Set up an election audit
### Audit election
### Run simulation

