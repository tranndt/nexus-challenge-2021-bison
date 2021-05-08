# nexus-challenge-2021-bison

## Due-date: May 14th, 2021

#### May 2nd, 2021
- Progress:
  - Cleaning data (today)
- Target: 
  - 2-3 days for coding algorithm.
  - 2-3 for the 5-pages summary paper.
- Meeting everyday around 9pm
#### May 3rd, 2021
- Questions:
-   Imporve the scheduling
    - can we departure early? how much earlier? what is the criteria?
    - balancing the inbound and outbound for every 3-4days?
Target:
- draw the graph, how bad/good it is regarding balance.
- how to flat the graph
- Meeting time changed to 8pm

#### May 4th, 2021
- Goal: balance the daily imbalances for the PQ region (= Outbound trailers - Inbound trailers)
- Assumptions:
  - Flexibility for scheduling: 24hrs. Can be parameterized if needed. 
  - Flexibility for trailer class: HEATER/REFFER/etc can be used as DRY if necessary
  - Start Date and Completion Dates are just estimate. If the date is unrealisticly long, we can shorten it (via some mechanism i.e >14 days)
  - Another layer of constraint: Initial number of drivers (~50). Can track along with the cumulative imbalance. Driver from incoming trailers can be factored into our calculation
- Todo:
  - Clean data
  - Come up with pseudo code
  - A method that figure out how dense our disturibution is/ how to measure
  - Load balancing algorithm:
    - Constraints: Look for candidates
    - Treating each day as a node with the imbalance as the value. Has edges to the day before and after.
- Thoughts:
  - After implementing the fundamental requirements. We can think of the rows that we have eliminated - those are not related to 'PQ' - can we use those to improve our algorithm?
  - For now, we clustered all the regions contains 'PQ' as a same region, can we narrow down more? e.g., 'PQ2S' and 'PQMON' as different regions.

#### May 5th,2021
- Evaluate how good our algorithm is:
  - Calculating the std (mean = 0) / Mean-squared error 
     - Be careful with the outlier
  - Visualize on a histogram
- To do: 
  - Modify the pseudocode if needed (easier to understand)
  - Implement greedy-approach pseudocode


#### May 6th, 2021
- To do:
  - Fixing bugs, visualize the result -> try to work on the basic dataset first (without the trailer_class)
  - Applying the trailer_class to the algorithm (working with the new dataset)
- Goal:
  - Finish fixing bugs and working on basic dataset


#### May 7th, 2021
- To do:
  - Finalize codes
  - Fix the bugs related to the starting date
  - Printing statements (add forecasting part)
- Goal:
  - Improving algorithms?
  - Proving this greedy algorithm (or how close it is to the optimal solution)  (*)
    - Start off: Think about the assumptions? What can be assumptions in the real-world (24hr)? 
  - Preparing at least 5-pages paper
    - a page for data cleaning/ data preprocessing
    - page for (*)
    - and so on ... 
