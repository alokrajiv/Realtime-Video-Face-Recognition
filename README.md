# Realtime Face-Recognition on Live Streaming Videos

Realtime Face Recognition on Live Video Streaming coming into the server through an HTTP Tranport or from a Directly Connected Video-Camera or similar imaging device.

###### Remember to have OpenCV available as this is a mandatory dependency.
&nbsp;
## Instructions to setup.

compile:

    g++ $(pkg-config --cflags --libs opencv) main.cpp -o Test

run:

    ./Test data/cascades/haarcascade_frontalface_alt.xml data/csv/training_set.csv data/csv/label_names.csv 0


OR 

Run Together in 1-step:

    g++ $(pkg-config --cflags --libs opencv) main.cpp -o Test && ./Test data/cascades/haarcascade_frontalface_alt.xml data/csv/training_set.csv data/csv/label_names.csv 0
