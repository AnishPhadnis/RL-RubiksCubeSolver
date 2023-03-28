multiThreadedRubiksCube.db - sqlite db containing table called states

states table schema:
- state TEXT PRIMARY KEY
  - string representation of state
  - py222.stateToString and py222.stringToState convert between string and py222 representations
- numMovesFromSolved INTEGER
  - number of moves this state is from being solved
- solveSequence TEXT
  - poorly named field, should be called scrambleSequence
  - the sequence of moves used to get to that state
  - "undoing" this sequence would be the solveSequence
