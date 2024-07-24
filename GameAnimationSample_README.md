# Notes will be placed here regarding how Motion Matchcing works within Game Animation Sample.

## Revieweing Sparse Motion Matching Database and Chooser Table
1. Observation #1: Sparse Pose Databases are filled with the basic 8-way motions like you fill into a beginner-like database table.
2. Observation #2: The Sparse Chooser Table is filled with 4 Enum Columns (Movement Mode, Stance, Movement State, Gait) to differentiate what animation(s) get played. Comes with the basic Idle, Walk, Run, and InAir Animations.
3. Observation #3: The Enums are found within the `Update States` function within the `Event Graph` within the `Animation Blueprint`.
