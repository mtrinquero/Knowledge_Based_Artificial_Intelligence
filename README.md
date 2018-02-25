# Knowledge Based Artificial Intelligence

## Knowledge Based Artificial Intelligence Agent (adapted from masters coursework at Ga Tech)
* Overview: Python AI agent for reasoning over Raven's Progressive Matrices (RPM IQ test) via pattern recognition and other AI techniques
* Goal: gain a better understanding of human cognition to allow for modeling in python AI agent

## AI Techniques Leveraged
* Generate & Test
* Heuristics
* Problem Reduction (break image into quadrants / sub-sections)
* Visuospatial Reasoning
* Metacognition
* Analogical Reasoning
* Common Sense Reasoning
* Planning
* Cognitive System Architecture
* Means End Analysis
* Image processing and image comparison (Pillow, Python Image Library)

## Comparison Metrics used for reasoning over RPM problem set
* Similarity / Equality
* Increasing pixel density trend
* Decreasing pixel density trend
* Change in pixel darkness
* Change in pixels lightness
* Reflections: vertical, horizontal
* Symmetry Comparisons: Flip, Mirror, Diagonals Vertical / Horizontal Shifts: Up, Down, Left, Right (thresholds)

## Areas for improvement / TODOs:
* Mistake Type 1: My agent struggles in some situations with diagonal reasoning - problems that start with strong trends at the start (i.e. drastic changes from AB, AD, and AE), but these changes are not as significant at the end 
* Mistake Type 2: My agent currently does not have a good ability to detect rotations. Depending on the rotation, the metrics I use can still come to a correct conclusion based on the deltas they capture, but it would improve performance to develop better methods to handle rotations.
* Mistake Type 3: abstracting alternating patterns. This is a major issue in problem sets D and E where overall problem trends are not as clear cut / able to be determined based on mathematical methods. Especially when relationships skip a frame or alternate between frames. This mistake type is closely related to how humans vs. computers solve problems and their ability to adapt their approaches.  I would use analogical reasoning to implement my improvements on problem abstraction. As the problem sets increased in difficultly, this became a major issue for my agent as pixel/mathematical based approaches become less useful.
