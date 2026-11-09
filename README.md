# Transportation Optimization and Driver-Trip Assignment

Course project for Transportation & Logistics Planning, supervised by Dr. Ali Mirdar Harijani at Amirkabir University of Technology.

## Project components

| Component | Work completed | Original artifact |
| --- | --- | --- |
| Shortest paths | Compared a priority-queue implementation of Dijkstra's algorithm with a binary network-flow model in PuLP on a seven-node graph. | `1.ipynb` |
| Capacitated vehicle routing with time windows | Formulated the objective and constraints for routing, customer service, vehicle capacity, and time windows. The deliverable is a mathematical formulation. | `2.pdf` |
| Driver–trip assignment | Built a separate PuLP MILP to minimize assignment cost. Each trip is assigned to one driver, subject to trip-count and working-time limits. | `3.ipynb` |

The assignment notebook generates a synthetic instance with 12 trips and 15 drivers. Its stored solver output reports an optimal cost of 340.5 and uses six drivers. The separate 10-trip course workbook is a different input and is unused by this notebook.

## Run the notebooks

Open [the shortest-path notebook](notebooks/1.ipynb) or [the assignment notebook](notebooks/3.ipynb) in Jupyter and run all cells with the dependencies in `requirements.txt`. Both notebooks contain their inputs. The portfolio validation used PuLP 2.9.0 with CBC and reproduced the matching shortest-path distances and the assignment cost of 340.5.
