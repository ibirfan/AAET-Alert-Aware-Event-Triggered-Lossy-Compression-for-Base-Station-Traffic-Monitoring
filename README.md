# AAET-Alert-Aware-Event-Triggered-Lossy-Compression-for-Base-Station-Traffic-Monitoring

## Run in Thonny
1. Extract the ZIP into a writable folder.
2. Open main.py in Thonny.
3. If necessary, choose Tools > Manage packages, search for matplotlib, and install it.
4. Press F5. Close the original group's plot windows to continue to validation.

Command line: `python main.py --no-show`.
Install dependencies if needed: `python -m pip install -r requirements.txt`.

The script uses only the Python standard library and Matplotlib. It runs both seed groups with unchanged methods. Results are synthetic, and the code excludes headers, padding, and network overhead.

## Outputs
Each results/original and results/validation folder contains:
- alert_summary.csv: pooled alert counts and mean run cost/error
- run_alert_metrics.csv: metrics for each seed
- station_alert_counts.csv: station-level counts and errors
- sample_alerts.csv: every original and reconstructed sample by method
- alert_error_rates.png and alert_example.png

<img width="2700" height="990" alt="alert_error_rates" src="https://github.com/user-attachments/assets/da083737-f15c-4e66-b1ab-8210be6f78ee" />
<img width="1980" height="1080" alt="alert_example" src="https://github.com/user-attachments/assets/9025a641-1830-451a-8387-b54eb76670c1" />


Rerunning overwrites the corresponding result files. Bitstreams are strings used to count logical bits, not packed files.

## Key validation result
Alert-aware threshold 5: 78.31% logical bit saving, RMSE 2.282 percentage points, 0 missed high-load samples, 7 false alarms. This group contains 477 actual high-load samples.



## Provenance
Consolidated from the supplied Step 12 implementation, preserving generator and coding logic. Both original and validation result tables reproduce the prior displayed values at reported precision.
