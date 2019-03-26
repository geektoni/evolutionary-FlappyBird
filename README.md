# Evolutionary Flappy Bird

## Brief Overview

This project was about evolving an agent which had to be able to play Flappy Bird game as long as possible without 
hitting any pipes. The agend was controlled by a feed-forward neural network and the neural network was trained by
using **reinforcement learning** and **evolutionary algorithms** (more specifically, **differential evolution** and
**NEAT**). 

**[Here](https://github.com/geektoni/evolutionary-FlappyBird/blob/master/report/DeToni_Coman_Mousavi_BioProject.pdf) you can find a more detailed report about the techniques and the method used.**

![](https://media.giphy.com/media/1AIgP9e7zgjHIalKl6/giphy.gif)
![](https://media.giphy.com/media/iOsdaY31XoOlj7WrCc/giphy.gif)

The left image shows how a random agent performs, while the right image shows how a final evolved agent performs.

## Installation

The project was tested on **Ubuntu 16.04** and it is compliant with **Python 3.6**. We used **Pipenv** in order to manage
the various dependencies. They can be installed by issuing:
```bash
cd evolutionary-FlappyBird
pipenv install
pipenv shell
```

## Usage

The file `evo_flappy.py` can be used for training/evaluating the Flappy Bird agent. By issuing `python3 evo_flappy.py --
help`, the list of possible actions and flags will be displayed. For instance, the command shown below will train an agent 
using Differential Evolution and then it will play the game with the best individual found.
```bash
python3 evo_flappy.py --MODE_AGENT --MODE_LEARN --PLAY_BEST --MODE_NO_SCREEN --EA="DE"
```

## Contributors

Giovanni De Toni: [giovanni.detoni@studenti.unitn.it](mailto:giovanni.detoni@studenti.unitn.it)

Seyed Mahed Mousavi: [seyedmahed.mousavi@studenti.unitn.it](mailto:seyedmahed.mousavi@studenti.unitn.it)

Andrei Catalin Coman: [andreicatalin.coman@studenti.unitn.it](mailto:andreicatalin.coman@studenti.unitn.it)
