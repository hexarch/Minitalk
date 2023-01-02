SERVER = server
CLIENT = clıent

SRC_client = client.c
SRC_server = server.c

CC = gcc

CFLAGS = -Wall -Werror -Wextra

all: $(SERVER) $(CLIENT)

$(CLIENT):
		$(CC) $(CFLAGS) $(SRC_client) -o $(CLIENT)
$(SERVER):
		$(CC) $(CFLAGS) $(SRC_server) -o $(SERVER)

clean:
		@rm -rf $(SERVER) $(CLIENT)
		@echo "\033[92mclean completed\033[om"
fclean: clean
		@rm -rf $(SERVER) $(CLIENT)
		@echo "\033[92m:)\033[0m"

re: clean all

.PHONY: all clean fclean re
