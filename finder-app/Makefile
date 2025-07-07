TARGET = writer
SRCS = writer.c
CC = gcc
CFLAGS = -g -Wall
LIBS = -lc
CROSS_COMPILER = aarch64-none-linux-gnu-

OBJS = $(SRCS:.c=.o)

$(TARGET): $(OBJS)
	$(CC) $(CFLAGS) -o $(TARGET) $(OBJS) $(LIBS)

%.o: %.c
	$(CC) -o $(TARGET) $(CFLAGS) -c $< -o $@
		
clean:
	rm -f $(OBJS) $(TARGET)
