compile:

g++ $(pkg-config --cflags --libs opencv) main.cpp -o Test

run:

./Test data/cascades/haarcascade_frontalface_alt.xml data/csv/training_set.csv data/csv/label_names.csv 0


Together in 1-step:

g++ $(pkg-config --cflags --libs opencv) main.cpp -o Test && ./Test data/cascades/haarcascade_frontalface_alt.xml data/csv/training_set.csv data/csv/label_names.csv 0