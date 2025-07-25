# Makemore: A Journey from Bigrams to WaveNet

This repository documents my journey following Andrej Karpathy's "makemore" series. The goal is to build character-level language models from scratch, starting with a simple statistical model and progressively building towards modern, deep neural network architectures.

This project is being built in public to track progress, share learnings, and demonstrate practical software engineering skills.

## Models Overview & Results

### Part 1: Bigram Model
A simple statistical model that predicts the next character based only on the single preceding character.

* **Limitations:** It has no concept of longer-term context, leading to unrealistic and often nonsensical names.
* **Final Loss:** 2.45
* **Sample Output:** `junide.`, `janasah.`, `cony.`
