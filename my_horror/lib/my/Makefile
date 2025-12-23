##
## EPITECH PROJECT, 2025
## my_horror
## File description:
## Makefile
##

NAME = libmy.a

CC = epiclang

SRC = 

OBJ = $(SRC:.c=.o)

AR = ar rc

CFLAGS = -Wall -Wextra -I../../include

RM = rm -f

all: $(NAME)

$(NAME): $(OBJ)
	@$(AR) $(NAME) $(OBJ)
	@ranlib $(NAME)

clean:
	@$(RM) $(OBJ)

fclean: clean
	@$(RM) $(NAME)

re: fclean all

.PHONY: all clean fclean re
