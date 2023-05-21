This contract first declares a struct for the Candidate which includes an id, name, and voteCount. It then declares three state variables: a mapping to track who has voted, another mapping to store the candidates, and a variable to keep track of the total number of candidates.

The contract also has an event which is emitted when a vote is cast.

In the constructor function, two candidates are added to the state.

Private function addCandidate creates a new candidate and adds it to the state.

Public function vote enables voting for candidates. It first checks that the caller has not voted before and that the candidate being voted for exists. If these conditions are met, the voter is marked as having voted, the vote count for the candidate is increased by one, and a votedEvent is emitted.
