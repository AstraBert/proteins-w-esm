# Proteins with ESM
Predict the whole sequence and 3D structure of masked protein sequences with [ESM](https://github.com/evolutionaryscale/esm) by [Evolutionary Scale](https://www.evolutionaryscale.ai/).

## How to use it

### Locally - Build from scratch

> _The predictions are computationally-intense, you should have at least 16GB RAM and 4 core CPU_

1. Clone this repository:

```bash
git clone https://github.com/AstraBert/proteins-w-esm.git
cd proteins-w-esm
```

2. Rename `.env.example` to `.env` and modify it with your Hugging Face access token (`read` or `write` permissions, `fine-grained` is nut supported)
3. Launch the application and wait for it to load on `http://localhost:7860`
```bash
python3 app.py
```

### Locally - Use Docker image

1. Pull Docker image
```bash
docker pull astrabert/proteinswithesm:latest
```
2. Run the image and wait for it to load on `http://localhost:7860`:
```bash
docker run -p 7860:7860 astrabert/proteinswithesm:latest
```

### Online - Hugging Face demo
Use directly the Hugging Face Space demo that you can find [here](https://huggingface.co/spaces/as-cle-bert/proteins-with-esm).

### Online - Use GitHub CodeSpaces
Click the `<> Code` green button and then click on `CodeSpaces -> Create CodeSpace on 'main'`.

You should be redirected to a VSCode-based space connected to the port on which the app runs, directly accessible under the "Ports" section of the VSCode interface.
