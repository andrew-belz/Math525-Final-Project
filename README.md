# Math525 Final Project
## BYU Fall 2025

This repo holds the contents of my final project for my network theory class. I decided to analyze "control graphs" for chess positions to determine if meaningful insight could be extracted using typical network analysis tools, particularly those discussed in class.

### Project Goals

- Rigorously define the graph model and hypotheses. 
- Collect, wrangle and clean data. Construct graph models.
- Exploratory data analysis: Visualize graphs and compute network measures and metrics.
- Interpret the results: do any of these features have tangible chess interpretations?
- Stretch goal: Do any features correlate with Stockfish evaluations?

### Control Graphs

in progress

### Data

For this project I utilized [Lichess](lichess.org), a free chess website with open source resources.

#### Stockfish Evaluation API Endpoint:

[https://lichess.org/api/cloud-eval](https://lichess.org/api/cloud-eval)

Example usage: `https://lichess.org/api/cloud-eval?fen=r1bqkbnr/pp1ppppp/2n5/2p5/4P3/5N2/PPPP1PPP/RNBQKB1R w KQkq - 2 3`

#### Opening Explorer and Statistics API Endpoint:

[https://explorer.lichess.ovh/masters](https://explorer.lichess.ovh/masters)(Master-level games only)

Example usage: `https://explorer.lichess.ovh/lichess?fen=rnbqkbnr/pppp1ppp/8/4p3/4P3/8/PPPP1PPP/RNBQKBNR w KQkq - 0 2&speeds[]=blitz&ratings[]=2000`


#### Game Data

Bulk game data downloaded from [database.lichess.org](database.lichess.org).

Single game data retrieved using the Lichess single-game API endpoint [https://lichess.org/api/game/export/](https://lichess.org/api/game/export/)

Example usage: `https://lichess.org/api/game/export/mIu0wA9f?format=pgn`

### Python Dependencies

- `networkx`
- `chess`

### To-Do

- Define control graphs.
- Data collection and wrangling.
