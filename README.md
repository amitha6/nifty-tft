# nifty-tft

## Intent

The main aim is to use historical data from NIFTY as well as individual listed company statistics to predict future NIFTY indices. 

## Data

1. The data is available in separate sheets. 

2. For use with Temporal Fusion Transformer, every entry in the passed dataframe object must be related to a unique timestep. 

3. A time index column must be available, such that every successive time index differs from its predecessor by $+1$. 

4. The NIFTY index data must have one-hot columns for every company ever listed, so that in theory, the transformer will be able to learn the absence of companies from the index. 

5. Every time step is associated with a vector of information for all companies listed at that particular time.
