# Drake-AI

Welcome to Drake-AI, a fine-tuned 3b parameter mini language model that spits heat like Drake! 🎤🔥

## Overview

Drake-AI is a custom language model based on the dolly-v2-3b architecture on huggingface. It has been fine-tuned with 3 billion parameters to capture the lyrical essence and style of the renowned artist Drake.


## Getting Started

To get started with Drake-AI, follow these steps:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/Drake-AI.git
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Model:**
   ```python
   python generate_text.py
   ```

   Feel free to customize the input prompts to generate text that resonates with Drake's style.

## Example Usage

```python
from drake_ai import DrakeAI

# Initialize the model
drake_model = DrakeAI()

# Generate text with a custom prompt
text = drake_model.generate_text(prompt="I'm feeling like...")

print(text)
```

## Contributions

Contributions are welcome! If you have ideas for improvement, encounter any issues, or want to add new features, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

- Special thanks to OpenAI for providing the GPT-3.5 architecture.
- Inspired by the lyrical genius of Drake.

Enjoy using Drake-AI and let the creativity flow! 🎶🚀
