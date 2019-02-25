# Ducling-Project
Obtained data on the following stations
# Our goal: Help examine current queuing operations at the DUC-ling using simulation
# Identify food stations with high service times and utilization to uncover opportunities for improvement
# High utilization rates observed for global market and grill, with high service times at self-serve stations like salads and deli

Services times at 12 food stations
Holding time at tables
Inter-arrival times at point-of-sale system

For other stations
Made reasonable assumptions e.g. 5 seconds to grab a tray
Excluded a few stations that have low traffic e.g. kosher

For each key station:

Used statistical modeling (goodness-of-fit test) to identify distributions that most closely fit the data

Sanity-checked the results visually, and based on what distributions are available in simulation platform

These distributions were then used to model the simulation inter-arrival and service times
# To create our model, we tested multiple capacity levels for self-serve stations to produce results in line with business operations
# To verify model functionality, we compared M/M/s model simulation output with analytical results by station
# To validate model results, we compared arrival rate predictions from simulation vs. results from observational data
For select stations, e.g. global market, water/juices and specials, simulation is reasonably similar to observational results
However, non-trivial differences in arrival rate observed for multiple stations especially pizza & beverages
In general, the model appears to underpredict arrival rates for most stations
This may be due to discrepancies in visit probability from survey vs. observational data


# Important Considerations
Model represents simplified view of DUC-ling operations, using a subset of all stations
Relies on limited data capture, with manual data collected during one weekday dinner time period only
Used self-reported routing for determining path probabilities, which may not be in line with reality – as observed during validation
Service time distributions may be overfitting on small sample of observational data
For employee-manned stations, a fixed capacity of 1 was used to readily design a simulation, does not capture rotating workers

# Potential nextsteps
Opportunity to explore ways to improve high utilization at grill and global market
Basic experiments indicate that doubling the number of servers will halve  station service times, although cost needs to be factored in
To improve the accuracy and applicability of queue simulation,
additional observation data is recommended, especially at other times/days. This will also help in distribution estimates.
Larger scale survey may be beneficial in getting more accurate path probabilities. Ideally, this should be validated via observational data
Ultimately, a more complex model could be built to capture additional nuances in operations
