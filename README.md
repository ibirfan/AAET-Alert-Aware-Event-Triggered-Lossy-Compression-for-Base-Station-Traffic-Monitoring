# AAET-Alert-Aware-Event-Triggered-Lossy-Compression-for-Base-Station-Traffic-Monitoring

## Run in Thonny
1. Extract the ZIP into a writable folder.
2. Open main.py in Thonny.
3. If necessary, choose Tools > Manage packages, search for matplotlib, and install it.
4. Press F5. Close the original group's plot windows to continue to validation.

Command line: `python main.py --no-show`.
Install dependencies if needed: `python -m pip install -r requirements.txt`.

The script uses only the Python standard library and Matplotlib. It runs both seed groups with unchanged methods. Results are synthetic, and logical coding bits exclude headers, padding and network overhead.

## Outputs
Each results/original and results/validation folder contains:
- alert_summary.csv: pooled alert counts and mean run cost/error
- run_alert_metrics.csv: metrics for each seed
- station_alert_counts.csv: station-level counts and errors
- sample_alerts.csv: every original and reconstructed sample by method
- alert_error_rates.png and alert_example.png

Rerunning overwrites the corresponding result files. Bitstreams are strings used to count logical bits, not packed files.

## Key validation result
Alert-aware threshold 5: 78.31% logical bit saving, RMSE 2.282 percentage points, 0 missed high-load samples, 7 false alarms. There are 477 actual high-load samples in this group.



## Provenance
Consolidated from the supplied Step 12 implementation, preserving generator and coding logic. Both original and validation result tables reproduce the prior displayed values at reported precision.
