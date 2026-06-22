# Mini ML Metrics Calculator — Pure NumPy

> Built with NumPy only. No sklearn. No pandas. No shortcuts.

---

## What is this project?

Most people learning Machine Learning jump straight to sklearn and call `mean_squared_error()` without understanding what's happening inside.

This project builds every core ML metric from scratch using only NumPy — the same math that sklearn, PyTorch, and TensorFlow run under the hood.

---

## Metrics Built

### Regression Metrics
| Metric | Formula | Result |
|--------|---------|--------|
| MSE — Mean Squared Error | mean((actual - predicted)²) | 2.8 |
| MAE — Mean Absolute Error | mean(abs(actual - predicted)) | 1.6 |
| RMSE — Root Mean Squared Error | sqrt(MSE) | 1.673 |

### Classification Metric
| Metric | Formula | Result |
|--------|---------|--------|
| Accuracy | mean(actual == predicted) | 80.0% |

### Transformations
| Operation | What it does | Result |
|-----------|-------------|--------|
| Normalization | Scales values to 0-1 range | [0. 0.39 0.75 1. 0.5] |
| Sigmoid | Converts values to probabilities | [0.5 0.597 0.679 0.731 0.622] |

---

## NumPy Concepts Used

- `np.mean()` — average of array elements
- `np.abs()` — remove negative signs from errors
- `np.sqrt()` — square root for RMSE
- `np.exp()` — exponential function for sigmoid
- `np.min()` / `np.max()` — for normalization formula
- `np.isnan()` — detect missing values
- Boolean Indexing — filter arrays by condition
- Broadcasting — apply operations across different shaped arrays

---

## Why Build Metrics From Scratch?

When you call `sklearn.metrics.mean_squared_error()` you're trusting a black box.

When you build it yourself:
- You understand what the number actually means
- You can debug when results look wrong
- You know what's happening inside every ML framework
- You can explain it in any interview

---

## Project Structure
