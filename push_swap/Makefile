NAME_M = push_swap

NAME_b = checker

SRCS_M = mandatory/equale.c mandatory/checkme.c  mandatory/ft_sort.c mandatory/ft_split.c  mandatory/indexing.c mandatory/main_folder.c mandatory/med_sort.c  mandatory/push_swap.c mandatory/push.c mandatory/rotate.c mandatory/small_sort.c mandatory/utils_1.c   

SRCS_b = bonus/action_zero.c bonus/checker.c bonus/get_next_line.c bonus/get_next_line_utils.c bonus/last_check.c bonus/push_stack.c bonus/rotate_b.c bonus/utils_again.c bonus/utils_bonus.c

OBJS_M = $(SRCS_M:.c=.o)

OBJS_b = $(SRCS_b:.c=.o)

FLAGS = -Wall -Wextra -Werror

cc = gcc

all : $(NAME_M)

$(NAME_M) : $(SRCS_M) $(OBJS_M) mandatory/push_swap.h
	@$(cc) $(FLAGS) $(SRCS_M) -o $(NAME_M)
	@echo ------mandatory compiled---------

bonus : $(NAME_b)

$(NAME_b) : $(SRCS_b) $(OBJS_b) bonus/push_swap_bonus.h
	@$(cc) $(FLAGS) $(SRCS_b) -o $(NAME_b)
	@echo ------bonus compiled---------

%.o : %.c
	@$(cc) $(FLAGS) -c $< -o $@

clean :
	rm -rf $(OBJS_b) $(OBJS_M)

fclean : clean
	rm -rf $(NAME_b) $(NAME_M)

re : fclean all