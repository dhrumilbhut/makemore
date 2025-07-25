# Makemore: A Journey from Bigrams to WaveNet

This repository documents my journey following Andrej Karpathy's "makemore" series. The goal is to build character-level language models from scratch, starting with a simple statistical model and progressively building towards modern, deep neural network architectures.

This project is being built in public to track progress, share learnings, and demonstrate practical software engineering skills.

## Models Overview & Results

### Part 1: Bigram Model
A simple statistical model that predicts the next character based only on the single preceding character.

* **Limitations:** It has no concept of longer-term context, leading to unrealistic and often nonsensical names.
* **Final Loss:** 2.45
* **Sample Output:** `junide.`, `janasah.`, `cony.`

## Setup & Usage

1.  **Clone the repository:**
    ```bash
    git clone <your-repo-url>
    cd makemore-project
    ```
2.  **Install requirements:**
    ```bash
    pip install -r requirements.txt
    ```
3.  Place the `names.txt` file in the `data/` directory.

### How to Run

The training and sampling scripts are now unified and controlled via command-line arguments.

1.  **To train a model:**
    Specify the model using the `--model` flag (`bigram`, `mlp`, etc.).
    ```bash
    # Train the Bigram model
    python src/train.py --model bigram

    # (Future) Train the MLP model
    # python src/train.py --model mlp
    ```

2.  **To sample from a trained model:**
    ```bash
    # Sample from the Bigram model
    python src/sample.py --model bigram
    ```
