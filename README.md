# digital-coin-flip
A hardware project, my first experience with circuit design and PCB layout. 

My "digital coin flip" is a circuit that simulates flipping a coin and randomly lights up a "heads" or "tails" LED. When you press the "flip" button, it connects a fast oscillator to the clock input of a JK flip-flop with J and K held high, which rapidly flips the JK flip-flop's output, Q, between high and low. When you release the button, the flip-flop's state is held, with a roughly equal chance of ending up in either the high or low state (given the rapid clock speed and unpredictable length of a button-press). Then, Q and !Q are fed into the gates of two transistors, which switch power to the "heads" and "tails" LEDs, respectively.
