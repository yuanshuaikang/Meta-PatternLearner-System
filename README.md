# Meta-PatternLearner: A Meta-Learning Enhanced Interactive Recommendation System

## Overview
Meta-PatternLearner is an interactive recommendation system that leverages meta-learning to efficiently discover meaningful patterns with minimal user feedback. The system learns from historical user interactions across multiple datasets to rapidly adapt to new recommendation tasks.

Key features:我无法读取《https://github.com/yuanshuaikang/Meta-PatternLearner-System/tree/main》、《https://youtu.be/Lnv4-0qZOAs》文件的内容。其他文件已阅读并为你总结如下：
Here's a README file for your Meta-PatternLearner system in code format:

```markdown
# Meta-PatternLearner: A Meta-Learning Enhanced Interactive Recommendation System

![System Framework](ECML_PKDD_2025_Author_Kit/meta-framework.pdf)

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
    "epochs": 25,         # Meta-training epochs
    "inner_steps": 5      # Inner loop update steps
}
```

## Documentation
For detailed technical information, please refer to our paper:
- [Meta-PatternLearner: A Meta-Learning Enhanced Interactive Recommendation System for Efficient Pattern Discovery](https://arxiv.org/abs/xxxx.xxxxx)

## Demonstration Video
[![System Demo](https://img.youtube.com/vi/Lnv4-0qZOAs/0.jpg)](https://youtu.be/Lnv4-0qZOAs)

## Citation
If you use this system in your research, please cite our work:
```bibtex
@article{bao2025meta,
  title={Meta-PatternLearner: A Meta-Learning Enhanced Interactive Recommendation System for Efficient Pattern Discovery},
  author={Bao, Xuguang and Yuan, Shuaikang and Chang, Liang and Gu, Tianlong},
  journal={ECML PKDD},
  year={2025}
}
```

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
For questions or suggestions, please contact:
- Xuguang Bao: [email@example.com]
- Shuaikang Yuan: [email@example.com]
- Liang Chang (corresponding author): changl@guet.edu.cn
```

This README provides a comprehensive overview of your system with installation instructions, usage guidelines, and citation information. You can adjust the content as needed for your specific repository structure.
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
