# Thesis-Notebooks

Collection of notebooks from my thesis research at Pace University.

Objective:

Use a dataset assembled from DJ sets of similar genres such as melodic techno/progressive house, versus songs scraped from beatport, to train a classifier which can autotag 
new as being "good enough" for a DJ set or not. 

Current approach: Divide each song into 30 second clips, feed mel spectrogram into CNN with 3 convolutional layers, employ ensemble voting on each clip to determine final tag.

** Validation accuracy is currently ~70%
