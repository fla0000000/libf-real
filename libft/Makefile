# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: fbiondo <marvin@42.fr>                     +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/01/20 11:21:42 by fbiondo           #+#    #+#              #
#    Updated: 2023/01/27 15:25:41 by fbiondo          ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libft.a

SRCS = ft_isdigit.c ft_memset.c ft_isprint.c ft_atoi.c ft_tolower.c ft_bzero.c ft_strlen.c ft_toupper.c ft_calloc.c ft_memchr.c ft_isalnum.c ft_memcmp.c ft_strncmp.c ft_isalpha.c ft_memcpy.c \
ft_strchr.c ft_strnstr.c ft_isascii.c ft_memmove.c ft_strrchr.c ft_strlcpy.c ft_strlcat.c ft_itoa.c ft_strdup.c ft_putchar_fd.c ft_putstr_fd.c ft_split.c ft_substr.c ft_putendl_fd.c ft_putnbr_fd.c ft_striteri.c ft_itoa.c ft_strmapi.c\

OBJS = ${SRCS:.c=.o}

CC		= gcc
RM		= rm -f

CFLAGS = -Wall -Wextra -Werror

.c.o:
		${CC} ${CFLAGS} -g -c $< -o ${<:.c=.o}

$(NAME): ${OBJS}
		ar rcs ${NAME} ${OBJS}

all:	${NAME}

clean:
	${RM} ${OBJS}

fclean:	clean
		${RM} ${NAME}

re:		fclean all
