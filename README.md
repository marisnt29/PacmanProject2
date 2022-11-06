# The-Searchin-Pac-Man
## Depth-First Search (DFS)
Implemented the depth-first search (DFS) algorithm in the depthFirstSearch function in `search.py`. <br />
```
python pacman.py -l tinyMaze -p SearchAgent <br />
python pacman.py -l mediumMaze -p SearchAgent <br />
python pacman.py -l bigMaze -z .5 -p SearchAgent<br />
```

## Breadth-First Search (BFS)
Implemented the breadth-first search (BFS) algorithm in the breadthFirstSearch function in `search.py`.<br />
```
python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs<br />
python pacman.py -l bigMaze -p SearchAgent -a fn=bfs -z .5<br />
```
The above solution is a generic solution which also works on eight puzzle<br />
`python eightpuzzle.py`

## Uniform-cost Search (UCS)
Implemented the uniform-cost search (UCS) algorithm in the uniformCostSearch function in `search.py` <br />
```
python pacman.py -l mediumMaze -p SearchAgent -a fn=ucs<br />
python pacman.py -l mediumDottedMaze -p StayEastSearchAgent<br />
python pacman.py -l mediumScaryMaze -p StayWestSearchAgent<br />
```

## A* Search
Implemented A* graph search in the function aStarSearch in search.py. A* takes a heuristic function as an argument. Heuristics take two arguments: a state in the search problem (the main argument), and the problem itself (for reference information). The nullHeuristic heuristic function in `search.py` is a trivial example.<br />
`python pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic `


## Eating All The Dots
`python pacman.py -l testSearch -p AStarFoodSearchAgent<br />`

Implemented foodHeuristic in `searchAgents.py`<br />
`python pacman.py -l trickySearch -p AStarFoodSearchAgent`
