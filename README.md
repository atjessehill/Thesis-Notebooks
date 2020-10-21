# Thesis-Notebooks

Collection of notebooks from my thesis research at Pace University.

Objective:

Use a dataset assembled from DJ sets of similar genres such as melodic techno/progressive house, versus songs scraped from beatport, to train a classifier which can autotag 
new as being "good enough" for a DJ set or not. 

Current approach: Divide each song into 30 second clips, feed mel spectrogram into CNN with 3 convolutional layers, employ ensemble voting on each clip to determine final tag for a song.

** Validation accuracy is currently ~70%, no test data yet.

Next steps: 
1. Adjust filter sizes used in musically-motivated CNN's such as in https://github.com/jordipons/musicnn
2. Validate whether the beginning and end clips (the harder clips for a human to determine), are being misclassified often. Adjust ensemble voting to ignore these clips, if so.
3. Explore source separation, training independent CNN's which vote. 

