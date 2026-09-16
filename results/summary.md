| metric | AdamW (lr 0.0001) | Muon (lr 0.0001) |
|---|---|---|
| test accuracy (%) | 89.07 ± 0.4 | 88.69 ± 0.93 |
| test accuracy at best val checkpoint (%) | 88.42 ± 0.6 | 88.11 ± 0.37 |
| test loss | 0.333 ± 0.011 | 0.372 ± 0.0096 |
| final train loss | 0.124 ± 0.0093 | 0.107 ± 0.0076 |
| ms per step | 45.7 ± 0.097 | 105 ± 0.24 |
| update size per step | 0.00024 ± 5.8e-06 | 0.0002 ± 2.2e-07 |
| cos(update, -gradient) | 0.28 ± 0.00077 | 0.11 ± 0.0019 |
| distance from pretrained weights | 0.075 ± 0.0017 | 0.1 ± 0.00053 |
| stable rank of W - W0 | 9.97 ± 0.052 | 111 ± 2.1 |
| probe loss | 0.0512 ± 0.005 | 0.0329 ± 0.0067 |
| probe confidence | 0.972 ± 0.0011 | 0.983 ± 0.0013 |
| Hessian largest eigenvalue | 17 ± 0.65 | 28 ± 3.2 |
| Hessian trace | 1.7e+02 ± 47 | 2.5e+02 ± 1.2e+02 |
| random sharpness (alpha 0.1) | 0.0015 ± 0.00042 | 0.0023 ± 0.00075 |
| worst-case sharpness (rho 0.2) | 0.0043 ± 0.00033 | 0.0059 ± 0.00045 |

Mean ± std over 3 seeds.
Paired test accuracy difference, Muon minus AdamW: -0.38 ± 1.1 points (one accuracy on 872 sentences has a standard error of about 0.45 points).
Loss barrier on the AdamW to Muon line: 0.014 ± 0.0042.