Alpha Michi --- Minimalistic Go MCTS Engine with hueristics based off a neural network.
=====================================

So this is partially based on the simple michi go program
and partially attempted to go down the road that alphago went do. I don't have the resources or time
that google had so I am aiming at a simple reproduction that I am hoping could be a dan
level player on very modest hardware resources. In particular I want to aim at
being an good automated game review that I can use for improvement on my own games

Currently the project is mostly just michi but working on getting things revamped to use a proper neural network.

This will come in several phases.

1. Get the Policy network that just reproduces the likely human moves. This will likely be based off the gogod database.

2. Get a value network built through self play that gives a good prediction on the current value. I am actually hoping that this is the key
component. The MCTS will mostly be used in trying to improve the value network since on modest HW MCTS can get expensive so a single evaluation of the value network will
hopefully provide most of the strength increases.


