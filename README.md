# Needleman-Wunsch-Algorithm
## Description
This function implements the Needleman-Wunsch algorithm for global alignment of two nucleotide or amino acid sequences. It calculates the optimal alignment including the best score by considering match, mismatch, and gap penalties.

## Parameters
- `A` (string): First sequence to align.
- `B` (string): Second sequence to align.
- `match_score` (int, optional): Score for matching characters. Default is 2.
- `mismatch_penalty` (int, optional): Penalty for mismatching characters. Default is -1.
- `gap_penalty` (int, optional): Penalty for gaps. Default is -2.

## Returns
- `F` (matrix): Alignment score matrix with the scores of the best paths.
- `Trace_back` (matrix): Directions taken during traceback to find the optimal alignment. Indicated by "D" for diagonal (match/mismatch), "U" for up (gap in A), and "L" for left (gap in B).
- `A_aligned` (string): Aligned version of sequence A, including gaps.
- `B_aligned` (string): Aligned version of sequence B, including gaps.
- `Score` (int): Total alignment score.
