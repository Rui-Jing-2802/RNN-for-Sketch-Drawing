
# Drawing Stroke Extraction


## Project Overview

The project encompasses the following steps:

1. **Image Preprocessing**: Convert hand-drawn images into black-and-white binary format.
2. **Vectorization**: Utilize `Potrace` to convert raster images to SVG format, extracting vectorized drawing strokes.
3. **Format Conversion**: Transform the extracted strokes into the Sketch-RNN format `(dx, dy, p1, p2, p3)`.
4. **Data Storage**: Store the processed stroke data in `.npz` format for seamless integration into model training workflows.

## Installation

To set up the project environment, follow these steps:

1. **Clone the Repository**:

    ```bash
    git clone https://github.com/your_username/your_repository_name.git
    cd your_repository_name
    ```

2. **Install Python Dependencies**:

    Ensure you have Python installed. Then, install the required Python packages:

    ```bash
    pip install -r requirements.txt
    ```

3. **Install Potrace**:

    - **Linux (Ubuntu/Debian)**:

        ```bash
        sudo apt install potrace
        ```

    - **macOS**:

        ```bash
        brew install potrace
        ```

    - **Windows**:

        Download the [Potrace executable](http://potrace.sourceforge.net/) and add it to your system's PATH.

## Citations
```
@ARTICLE{sketchrnn,
  author          = {{Ha}, David and {Eck}, Douglas},
  title           = "{A Neural Representation of Sketch Drawings}",
  journal         = {ArXiv e-prints},
  archivePrefix   = "arXiv",
  eprinttype      = {arxiv},
  eprint          = {1704.03477},
  primaryClass    = "cs.NE",
  keywords        = {Computer Science - Neural and Evolutionary Computing, Computer Science - Learning, Statistics - Machine Learning},
  year            = 2017,
  month           = apr,
}
```