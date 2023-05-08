# MAESTRO-Music-agent
Data mining project to predict classical music era from MIDI data
Originally performed as a class project for Georgia Tech graduate course ISYE7406 Data Mining & Statistical Learning

This analysis was performed on the MAESTRO dataset of classical music piano performances, sourced from:
https://magenta.tensorflow.org/datasets/maestro#dataset

From this paper:
Curtis Hawthorne, Andriy Stasyuk, Adam Roberts, Ian Simon, Cheng-Zhi Anna Huang,
  Sander Dieleman, Erich Elsen, Jesse Engel, and Douglas Eck. "Enabling
  Factorized Piano Music Modeling and Generation with the MAESTRO Dataset."
  In International Conference on Learning Representations, 2019.

Composer era was source from Wikipedia:
https://en.wikipedia.org/wiki/List_of_classical_music_composers_by_era 

Project files:
- MAESTRO metadata expanded3.csv contains the list of recordings, with year, composer & title, and file path information
- MAESTRO eras is a lookup table of major & minor classical music eras, sourced from Wikipedia.  It is not required to run the analysis.
- MAESTRO analysis.ipynb is a Jupyter notebook that analyzes each of the MIDI files and extracts features, which are saved to...
- stp_features.csv is the extracted features, one line per file analyzed, in the same order as the Metadata file
- MAESTRO data model.rmd is an R Markdown file that builds a variety of classification models to forecast major classical music era
