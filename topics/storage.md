# Storage

## Email - advice to Val Junker Munn Rabot

Val,

It was a pleasure speaking with you today.  A quick summary to file with your notes:

1. Current solution covers most of the bases but my concerns would be, A. physical stress on the component drive interfaces, and B. the amount of "Val time" required to run it.  Additionally, while it allows for a relatively short Recovery Time Objective ("RTO") of ~one day the Recovery Point Objective ("RPO") could be as long as seven days.  The RPO could be shortened, but that would require more "Val time".

2. A possible alternative avenue would be to use a larger-capacity (~50-100 tapes) robotic tape library (IBM TS3500 Tape Library series, Quantum Scalar i500 series, HP MSL8096 series) combined with IBM's Tivoli Storage Manager ("TSM") software and Recall (or similar) off-site storage and tape rotation.  Main drawback here being initial CapX on the library of ~$30,000-$40,000.

3. Another alternative would be something like AWS Storage Gateway combined with Symantec BackupExec.  Would require setting up a relatively small virtualized environment to host the AWS Storage Gateway VM, and approximately 14 days (assuming ~50TB data set and ~500mbps upload bandwidth) to seed the initial backup set.

## Please let me know if you have any questions, and good luck!