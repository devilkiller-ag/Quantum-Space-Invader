# Quantum Breakout

[Download from Itch.io](https://jaisarita.itch.io/quantum-breakout)

Quantum Version of Classic Breakout Game

Inspired by QPong

I am happy to announce The Quantum Breakout Game which I built as a part of Team Abraxas for showcasing at Fest Nimbus, the annual technical fest of the National Institute of Technology Hamirpur. This is a quantum version of the Classic Breakout Game by Atari, Inc. built using Pygame and Qiskit. In the Classic Breakout Game, the player has to knock down as many bricks as possible by using a single ball and the paddle below to hit the ball against the bricks and eliminate them. In this quantum version of the game, players have to control the paddle by constructing a three-qubits circuit such that the probability of the paddle being above the state vector where the ball is about to come is maximum. The probability of the paddle being above a certain state is indicated by the opacity of the paddle, 100% opacity (pure white) indicates the 100% probability and 0% opacity (transparent) indicates the 0% probability of the state. As the ball comes near the paddle the measurement is done and the position of the paddle collapses to a being above a certain state which was in superposition before the measurement.

I have built this game to help school students and college freshmen understand the basic concept of quantum computing: Qubit manipulation by Quantum Gates.

This game is highly inspired by the QPong game developed by Junye Huang. I am thankful to him and Qiskit for releasing a basic tutorial for building QPong in a YouTube series: 12 Days of Qiskit (https://youtube.com/playlist?list=PLOFEBzvs-VvodTkP_rfrs3RWdeWE9aNRD) without which it would have been hard for me to develop this game.

# Game Demo
https://user-images.githubusercontent.com/43639341/232225302-bed08bac-010c-4569-94d2-819d7329568d.mp4

# Download & Install Instruction
1) Unzip the Downloaded Zip File
2) Open the Game Folder
3) Create a virtual enviornment using the command: `python -m venv qenv` on your terminal.
4) Activate the virtual enviorment: 
   - For windows: `.\qenv\Scripts\Activate.ps1`
   - For linux: `source qenv/bin/activate`
5) Install the requirements using the command: `pip install -r requirements-dev.txt​` on your terminal.
6) Run the `main.py` file using the command: `python main.py`

# Play Instruction
- Use the W, A, S, and D keys to move the marker on the circuit for adding gates at appropriate places.
- Use the X key to apply the X-Gate, the Y key to apply the Y-Gate, the Z key to apply the Z-Gate, and the H Key to apply the H-Gate.
- Use the C key to activate the control qubit, use the UP, DOWN, RIGHT, and LEFT keys to reach the target qubit, and then click the key representation (X, Y, Z, and H Keys) for the gate which you want to be controlled.
