# Makemore 

This project trains a character-level Transformer language model on  and generates new name-like strings.

## Environment
- Python 3.12
- PyTorch (MPS or CPU supported)

## Data
- Input file:  (one name per line)

## Training
Example (Transformer 8 layers, 128 embedding, MPS):


- Periodic eval every 500 steps; best checkpoint saved to .
- Logs and samples are in .

## Sampling
Sample from the best checkpoint:


Adjust  and temperature for creativity (see ).

## Final Artifacts
- Best checkpoint:  (copy of )
- Training logs:  (and )
- Samples after 10k steps: 

## Notes
- Code instantiates Transformer unconditionally; other model code remains for reference.
- To run on CPU, set .
