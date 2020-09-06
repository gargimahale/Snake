# Snake

The project focuses on the artificial intelligence of the [Snake][wiki-snake] game. The snake's goal is to eat the food continuously and fill the map with its bodies as soon as possible. 

***[Algorithms >][doc-algorithms]***

## Experiments

We use two metrics to evaluate the performance of an AI:

1. **Average Length:** Average length the snake has grown to (*max:* 64).
2. **Average Steps:** Average steps the snake has moved.

Test results (averaged over 1000 episodes):

| Solver | Demo (optimal) | Average Length | Average Steps |
| :----: | :------------: | :------------: | :-----------: |
|[Hamilton][doc-hamilton]|![][demo-hamilton]|63.93|717.83|
|[Greedy][doc-greedy]|![][demo-greedy]|60.15|904.56|
|[DQN][doc-dqn]<br>(experimental)|![][demo-dqn]|24.44|131.69|

## Installation

Requirements: Python 3.5+ (64-bit) with [Tkinter][doc-tkinter] installed.

```
$ pip3 install -r requirements.txt

# Use -h for more details
$ python3 run.py [-h]
```

Run unit tests:

```
$ python3 -m pytest -v
```

[wiki-snake]: https://en.wikipedia.org/wiki/Snake_(video_game)
[doc-tkinter]: https://docs.python.org/3.6/library/tkinter.html
[doc-algorithms]: ./docs/algorithms.md
[doc-greedy]: ./docs/algorithms.md#greedy-solver
[doc-hamilton]: ./docs/algorithms.md#hamilton-solver
[doc-dqn]: ./docs/algorithms.md#dqn-solver

[demo-hamilton]: ./docs/images/solver_hamilton.gif
[demo-greedy]: ./docs/images/solver_greedy.gif
[demo-dqn]: ./docs/images/solver_dqn.gif
