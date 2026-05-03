# Experiment Summary

## Dataset

FAO wheat price data from Central Asia

## Model

Isolation Forest

## Initial problem

The model produced too many false positives.

## Why

Seasonality was ignored.

## Fix

Rolling median filtering was added before anomaly detection.

## Result

F1 score improved from 0.68 to 0.79.
