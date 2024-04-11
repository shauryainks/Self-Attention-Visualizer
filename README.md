# Self-Attention Visualizer

## Overview
This Python script provides functionality to visualize the self-attention scores of a pre-trained BERT-based language model, particularly useful for understanding which parts of the input text the model is focusing on.

The script takes an input text containing a masked token, generates predictions for the masked token, and then produces graphical representations of self-attention scores for each layer and head of the model.

## Dependencies
- TensorFlow (v2.x)
- Transformers (Hugging Face)
- PIL (Python Imaging Library)

## Installation
1. Install the required dependencies using pip:
   ```
   pip install tensorflow transformers pillow
   ```

2. Ensure you have the required font file in the `assets/fonts/` directory:
   - OpenSans-Regular.ttf

## Usage
1. Run the script `mask.py`.
2. Input a sentence containing a masked token (`[MASK]`).
3. The script will generate predictions for the masked token and produce graphical representations of self-attention scores for each layer and head of the model.
4. The images will be saved as PNG files in the current directory.

## Configuration
- `MODEL`: The pre-trained masked language model to use (default: "bert-base-uncased").
- `K`: Number of predictions to generate (default: 3).
- `FONT`: Path to the font file for rendering text in the diagrams (default: "assets/fonts/OpenSans-Regular.ttf").
- `GRID_SIZE`: Size of each grid cell in the attention diagrams (default: 40 pixels).
- `PIXELS_PER_WORD`: Space allocated for each word in the attention diagrams (default: 200 pixels).

