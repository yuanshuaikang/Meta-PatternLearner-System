# Meta-PatternLearner: A Meta-Learning Enhanced Interactive Recommendation System

## Overview
Meta-PatternLearner is an interactive recommendation system that leverages meta-learning to efficiently discover meaningful patterns with minimal user feedback. The system learns from historical user interactions across multiple datasets to rapidly adapt to new recommendation tasks.

Key features:
- Meta-learning framework for few-shot adaptation
- Interactive visualization of pattern relationships
- User-adjustable sampling strategy
- Efficient pattern discovery with limited feedback

## Installation

### Prerequisites
- Python 3.8+
- PyQt5
- TensorFlow 2.x
- scikit-learn
- networkx (for visualization)
- matplotlib

### Installation Steps
```bash
git clone https://github.com/yuanshuaikang/Meta-PatternLearner-System.git
cd Meta-PatternLearner-System
pip install -r requirements.txt
```

## Usage

### Data Preparation
Prepare your pattern data in the following format:
```python
pattern_data = {
    "interesting": [
        [1, 0, 1, 0, 1, 0, 1, 0, 1, 0],  # Example pattern 1
        [0, 1, 0, 1, 0, 1, 0, 1, 0, 1]   # Example pattern 2
    ],
    "uninteresting": [
        [1, 1, 1, 1, 1, 0, 0, 0, 0, 0],  # Example pattern 3
        [0, 0, 0, 0, 0, 1, 1, 1, 1, 1]   # Example pattern 4
    ]
}
```

### Running the System
1. Launch the GUI application:
```bash
python main.py
```

2. The interface consists of:
   - Left panel: Data loading and parameter configuration
   - Right panel: Training metrics visualization
   - Bottom panel: Pattern relationship network

3. Key operations:
   - Load your pattern data
   - Adjust meta-learning parameters (epochs, learning rates)
   - Provide feedback on recommended patterns
   - Explore pattern relationships through interactive visualization

### Meta-Learning Parameters
```python
# Example configuration
params = {
    "num_tasks": 10,       # Number of meta-tasks per epoch
    "n_shot": 20,         # Support set samples per class
    "n_query": 40,        # Query set samples per class
    "k_way": 2,           # Number of classes per task
    "inner_lr": 0.01,     # Inner loop learning rate
    "outer_lr": 0.001,    # Outer loop learning rate
    "epochs": 50,         # Meta-training epochs
    "inner_steps": 5      # Inner loop update steps
}
```
