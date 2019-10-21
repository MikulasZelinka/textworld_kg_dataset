# TextWorld KG Dataset
Dataset proposed in paper Building Dynamic Knowledge Graphs from Text-based Games


## Statistics
| #Train  | #Valid | #Test  |  Avg. Obs.  | Avg. #Operations | #Vertices | #Edges | Avg. #Connections |
| ---     | ---    | ---    | ---         | ---              | ---       | ---    | ---               |
| 267,031 | 13,442 | 41,865 | 29.3 tokens | 3.1              | 99        | 10     | 43.1              |

## Data Format
We have split the dataset into training, validation, and test sets, each of them is in a `.json` file. In a `.json` file, each line is a `json` dump, which is a single data point.

#### Each data point consists the follow elements: 

* `previous_triplets`: ground truth (partially observable) graph at previous game step represented by triplets;
* `previous_action`: text action an agent performed at previous game step;
* `observation`: observation at current game step, which is resulted by `previous_action`;
* `target_commands`: graph updates represented by text commands (operations).
