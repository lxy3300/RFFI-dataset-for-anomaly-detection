# RFFI Dataset Repository

This repository contains two distinct datasets used for device authentication and anomaly detection research:

1. **Signal-level Data**  
2. **Protocol-level Data**

<br>

Due to file size constraints, the full raw and partially processed protocol-level data are not stored directly in this repository. You can download the data from the following link: [Download link](https://dalu-my.sharepoint.com/:f:/g/personal/xn394804_dal_ca/EploaLsr_D1OjS4jiAbLbpEBXwqIsrReWKmG99Yc9z4rqg?e=4sm12e).


## Dataset Structure

- `signal_level/` - Contains signal-level data samples.
- `protocol_level/` - Contains protocol level data samples.

## How to Load the Data

All dataset files are stored in Python pickle format (`.pkl`).  
Use the following function to load any pickle file:

```python
import pickle

def load_pickle_data(file_name):
    with open(file_name, 'rb') as file:
        data = pickle.load(file)
    return data
