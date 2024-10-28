# voxel51_hello_world

# Word Vector Visualization with FiftyOne

This project creates visual representations of text data using Word2Vec embeddings and SVG images, organized in a FiftyOne dataset for easy exploration.

## Features

- Converts text into Word2Vec embeddings
- Visualizes word vectors as color-coded pixel grids in SVG format
- Organizes visualizations in a searchable FiftyOne dataset
- Multi-row layout with configurable parameters
- Handles large text documents efficiently

## Requirements

```
pandas
numpy
gensim
fiftyone
scikit-learn
sentence_transformers
```

## Usage

1. Place your input CSV file with a 'Body Text' column in the project directory
2. Run the SVG generation script to create visualizations:
   - Creates Word2Vec embeddings for each text
   - Generates color-coded SVG grid visualizations
   - Saves SVGs to 'content_images' directory

3. Run the FiftyOne dataset creation script to:
   - Import all SVGs into a searchable dataset
   - Add metadata and indexing
   - Launch the FiftyOne UI for visualization

## Configuration

Key parameters can be adjusted in the code:
- `SVG_WIDTH`: Width of SVG output (default: 800px)
- `PIXELS_PER_ROW`: Number of words per row (default: 100)
- `PIXEL_SIZE`: Size of each pixel (default: 8px)
- `PIXEL_SPACING`: Space between pixels (default: 1px)

## Output

- SVG files in 'content_images' directory
- FiftyOne dataset named 'svg_word_representation'
- Interactive visualization interface through FiftyOne
