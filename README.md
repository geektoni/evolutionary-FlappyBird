# Evolutionary Flappy Bird

## Brief Overview

This project was about evolving an agent which had to be able to play Flappy Bird game as long as possible without 
hitting any pipes. The agend was controlled by a feed-forward neural network and this neural network was trained by
using **reinforcement learning** and evolutionary computation techiques (more specifically, **differential evolution** and
**NEAT**). 

**[Here](https://github.com/geektoni/evolutionary-FlappyBird/blob/master/report/DeToni_Coman_Mousavi_BioProject.pdf) you can find a more detailed report about the techniques and the method used.**

## Installation

The project was tested on **Ubuntu 16.04** and it is compliant with **Python 3.6**. We used **Pipenv** in order to manage
the various dependencies. They can be installed by issuing:
```bash
cd evolutionary-FlappyBird
pipenv install
pipenv shell
```

## Usage

The file `evo_flappy.py` can be used for train/evaluate the Flappy Bird agent. By issuing `python3 evo_flappy.py --help`, the 
list of possible actions and flags will be displayed. For instance, the command shown below will train an agent using Differential Evolution and then it will play the best individual found.
```bash
python3 evo_flappy.py --MODE_AGENT --MODE_LEARN --PLAY_BEST --MODE_NO_SCREEN --EA="DE"
```

## Contributors

Giovanni De Toni: [giovanni.detoni@studenti.unitn.it](mailto:giovanni.detoni@studenti.unitn.it)

Seyed Mahed Mousavi: [seyedmahed.mousavi@studenti.unitn.it](mailto:seyedmahed.mousavi@studenti.unitn.it)

Andrei Catalin Coman: [andreicatalin.coman@studenti.unitn.it](mailto:andreicatalin.coman@studenti.unitn.it)
