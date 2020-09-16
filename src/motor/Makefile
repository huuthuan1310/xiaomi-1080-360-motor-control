LDFLAGS=-ldl -pthread -w -static

all: 
	$(CC) motord.c $(LDFLAGS) -o motord  

test:
	$(CC) motord.c $(LDFLAGS) -o motord  
	$(CC) -shared ./mocks/libdevice_kit.c -o libdevice_kit.so

clean:
	$(RM) motord libdevice_kit.so event status
