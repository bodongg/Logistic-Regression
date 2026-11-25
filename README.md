# Delivery lateness with logistic regression

The [notebook](Logical%20Regression.ipynb) estimates whether a delivery will arrive late. It trains a logistic regression, compares warning cutoffs on a validation split using a 3:1 missed-delivery to false-alarm cost, then reports performance on held-out records.

## Run locally

From the repository root, install the dependencies in an activated virtual environment.

    python -m pip install -r requirements.txt
    python -m jupyterlab

Place an authorized copy of deliveries.csv in the repository root, then open the notebook and run the cells in order. The CSV is supplied separately.

The notebook expects delivery_id, distance_km, package_weight_kg, rush_hour, is_raining, driver_experience_years, vehicle_type, and delivered_late. The outcome is 1 for late and 0 for on time. Use 0 or 1 for rush_hour and is_raining.
