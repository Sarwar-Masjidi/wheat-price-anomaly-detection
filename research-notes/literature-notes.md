# Literature Notes

While working on wheat price anomaly detection, I reviewed research on:

- anomaly detection in sparse time series
- forecasting with small datasets
- preprocessing methods for noisy temporal data

## My observations

A major lesson from the literature and experiments is that preprocessing strongly affects results.

Examples from this repository:

- ignoring seasonality created false positives
- rolling median filtering improved anomaly detection
- small changes in preprocessing sometimes changed results significantly
