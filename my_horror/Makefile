##
## EPITECH PROJECT, 2025
## my_horror
## File description:
## Makefile
##

NAME    =   my_horror

CC      =   epiclang

SRC     =   src/main.c

OBJ     =   $(SRC:.c=.o)

CFLAGS  =   -Wall -Wextra -I./include

LDFLAGS =   -L./lib/my -lmy

RM      =   rm -f

all:    $(NAME)

make_lib:
	make -C ./lib/my

$(NAME): make_lib $(OBJ)
	@$(CC) $(OBJ) -o $(NAME) $(LDFLAGS)
	@echo "✅ Compiled: $(NAME)"

clean:
	@$(RM) $(OBJ)
	@make clean -C ./lib/my

fclean: clean
	@$(RM) $(NAME)
	@make fclean -C ./lib/my
	@echo "🧹 Cleaned: $(NAME)"

re:     fclean all

.PHONY: all clean fclean re make_lib
