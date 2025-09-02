# Robot Trust Modeling

This project contains various models and experiments related to robot trust modeling. The goal is to explore and implement probabilistic models that simulate and analyze trust dynamics between robots and humans in decision-making scenarios.

## Folder Structure

- **PYMC_Simple_Model.ipynb**: A simple PyMC model for trust dynamics, using basic priors and trust thresholds.
- **PYMC_Expanded_Model.ipynb**: An expanded PyMC model that incorporates additional factors such as health, damage, and coin collection into the trust decision-making process.
- **PYMC_Complete_Model.ipynb**: A comprehensive PyMC model that integrates all available data and factors to simulate trust evolution over time.
- **1009_event_hardcoded_07_19_2024.csv**: A dataset used for training and testing the models. It contains columns such as `trust_level`, `current_health`, `proposed_damage`, and `move_approved`.

## Key Features

1. **Probabilistic Modeling**:
   - The models use PyMC to define probabilistic relationships between trust levels, health, damage, and decisions.
   - Time-series modeling is implemented to capture the evolution of trust thresholds over time.

2. **Data-Driven Analysis**:
   - The models are trained on real or simulated datasets to analyze how trust decisions are influenced by various factors.

3. **Customizable Parameters**:
   - Hyperparameters such as priors, thresholds, and weights can be adjusted to test different scenarios.

## How to Use

1. **Install Dependencies**:
   - Ensure you have Python installed along with the required libraries:
     ```sh
     pip install pymc pandas numpy matplotlib
     ```

2. **Run the Models**:
   - Open the Jupyter notebooks (`PYMC_Simple_Model.ipynb`, `PYMC_Expanded_Model.ipynb`, `PYMC_Complete_Model.ipynb`) in your preferred environment.
   - Update the `file_path` variable in the notebooks to point to the correct location of the dataset.

3. **Analyze Results**:
   - The models output posterior distributions for trust thresholds and other parameters.
   - Use the visualizations provided in the notebooks to interpret the results.

## Dataset Description

The dataset (`1009_event_hardcoded_07_19_2024.csv`) contains the following columns:
- `trust_level`: The trust level of the robot at a given time.
- `current_health`: The robot's health at the time of decision-making.
- `proposed_damage`: The damage proposed by the user's command.
- `move_approved`: Whether the robot approved the user's command.

## Future Work

- Extend the models to include additional factors such as environmental conditions and user behavior.
- Implement real-time trust adaptation in a simulated robot environment.
- Compare the performance of PyMC models with other probabilistic frameworks.

## References

- PyMC Documentation: [https://www.pymc.io/](https://www.pymc.io/)
  
## Contact

For questions or contributions, please contact peiyiw@andrew.cmu.edu
