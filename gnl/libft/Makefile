# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: cfahey <cfahey@student.42.fr>              +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2018/11/23 03:46:28 by cfahey            #+#    #+#              #
#    Updated: 2018/12/11 18:03:35 by cfahey           ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

CC      = gcc

CFLAGS  = -Wall -Wextra -Werror

AR      = ar rc

RANLIB  = ranlib

NAME    = libft.a

HEAD    = libft.h

SRCS    = ft_bzero.c ft_memcpy.c ft_memchr.c ft_memcmp.c ft_memccpy.c \
ft_memmove.c ft_memset.c ft_strlen.c ft_strdup.c ft_strcpy.c ft_strncpy.c \
ft_strcat.c ft_strncat.c ft_strlcat.c ft_tolower.c ft_toupper.c ft_isprint.c \
 ft_isascii.c ft_isalnum.c ft_isdigit.c ft_isalpha.c ft_atoi.c ft_strcmp.c \
 ft_strncmp.c ft_strstr.c ft_strnstr.c ft_strchr.c ft_strrchr.c ft_memalloc.c \
 ft_memdel.c ft_strnew.c ft_strdel.c ft_strclr.c ft_striter.c ft_striteri.c \
 ft_strmap.c ft_strmapi.c ft_strequ.c ft_strnequ.c ft_strsub.c ft_strjoin.c \
 ft_strtrim.c ft_putstr.c ft_putchar.c ft_putendl.c ft_putnbr.c \
 ft_putchar_fd.c ft_putstr_fd.c ft_putendl_fd.c ft_putnbr_fd.c ft_itoa.c \
 ft_strsplit.c ft_lstnew.c ft_lstdelone.c ft_lstdel.c ft_lstadd.c \
 ft_lstiter.c ft_lstiter.c ft_lstmap.c ft_push.c ft_pow.c \
 ft_strtrim_delimeter.c ft_average.c ft_lstclear.c ft_bubble_sort.c \
 ft_joincatfree.c

OBJS    = $(SRCS:.c=.o)

.PHONY: all, clean, fclean, re

all: $(NAME)

$(NAME):
		@$(CC) $(CFLAGS) -c $(SRCS)
		@$(AR) $(NAME) $(OBJS)
		@$(RANLIB) $(NAME)
		@echo "[INFO] Library [$(NAME)] created!"

clean:
		@rm -f $(OBJS)
		@echo "[INFO] Objects removed!"

fclean: clean
		@rm -f $(NAME)
		@echo "[INFO] Library [$(NAME)] removed!"

re:		fclean all
