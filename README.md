# Six Degrees of Hollywood

## Background

According to the Six Degrees of Kevin Bacon game, anyone in the Hollywood film industry can be connected to Kevin Bacon within six steps. Each step consists of finding a film that two actors both starred in.

The goal is to find the shortest path between any two actors by picking a sequence of movies that connects them. For example, the shortest path between Jennifer Lawrence and Tom Hanks is 2 steps:

1. Jennifer Lawrence is connected to Kevin Bacon by both starring in "X-Men: First Class."
2. Kevin Bacon is connected to Tom Hanks by both starring in "Apollo 13."

## Problem Statement

We can frame this as a search problem:

- **States**: People (actors)
- **Actions**: Movies (that take us from one actor to another)
- **Initial State**: The first actor
- **Goal State**: The second actor

By using breadth-first search, we can find the shortest path between the two actors.

## Run Example

To run the program, use the following command:

```bash
$ python degrees.py large
Loading data...
Data loaded.
Name: Emma Watson
Name: Jennifer Lawrence
3 degrees of separation.
1: Emma Watson and Brendan Gleeson starred in Harry Potter and the Order of the Phoenix
2: Brendan Gleeson and Michael Fassbender starred in Trespass Against Us
3: Michael Fassbender and Jennifer Lawrence starred in X-Men: First Class
```
