CC = gcc
CFLAGS = -Wall

ifeq ($(DEBUG), 1)
CFLAGS+=-g -O0
else
CFLAGS+=-O2
endif

TARGET = libkirk.a
OBJS = kirk_engine.o crypto.o amctrl.o bn.o ec.o ../common/utils.o

all: $(TARGET)

$(TARGET): $(OBJS)
	$(AR) rcs $@ $(OBJS)

clean:
	$(RM) *.o $(TARGET)

