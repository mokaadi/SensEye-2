# Russ Bielawski
# 2012-11-15

NAME=senseye_websocket

CC=gcc
CFLAGS=-O2 -Wall -g


OPENCV_INC=/usr/local/include/opencv
OPENCV_LIBS=-lopencv_core -lopencv_highgui -lopencv_imgproc

SENSEYE_DEFS_INC=../../uclinux/senseye_serv/

#LIBGLASSES_INC=../libglasses
#LIBGLASSES_SRC=$(LIBGLASSES_INC)/glasses.c

#INC=-I$(OPENCV_INC) -I$(LIBGLASSES_INC)
INC=-I$(OPENCV_INC) -I$(SENSEYE_DEFS_INC)
SRC=$(NAME).c
#SRC=$(NAME).c $(LIBGLASSES_SRC)
BIN=$(NAME)

#LIBDIR=-L/usr/local/lib
LIBS=$(OPENCV_LIBS)


all:	$(NAME)

$(NAME):	$(SRC)
	$(CC) $(CFLAGS) $(INC) $(SRC) $(LIBS) -o $(BIN)

clean:
	rm -f $(BIN)

