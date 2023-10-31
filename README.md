# Optimization for Renewable-Energy-Community-members-pairing based on PV surplus generation

The Code determines the minimum PV generation surplus for collective self-consumption by analyzing a set of combinations of
 5 (modifiable) load diagrams (in z-score) in which, for each of the 96 observations within a 15-minute time frame of a day,
 the consumption values are summed and subtracted from the generation values. Then, the sum of all 96 values for each combination
 is calculated, and the minimum value is identified. This represents the best combination of options, but the code provides the
 top 5 combinations.

 The code operates on a table with 21 columns and 96 rows, with numeric values ranging from 0 to 1 in each cell.
 The first column represents a PV electricity generation profile (G). The other 20 columns correspond to electricity
 consumption profiles (P1 to P20). This Python code generates all possible combinations of 5 electricity generation profiles,
 calculates the values for each observation (row), subtracts them from the G value, and stores the result in the S variable.
 Each combination results in an STotal value, which is the sum of all 24 S values in that combination. The output of the Python
 code includes the STotal values for the 5 lowest combinations and displays the corresponding 5 P elements for each combination.
