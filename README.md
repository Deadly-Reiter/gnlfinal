/* ************************************************************************** */
/*                                                                            */
/*                                                        :::      ::::::::   */
/*   get_next_line.h                                    :+:      :+:    :+:   */
/*                                                    +:+ +:+         +:+     */
/*   By: eborunov <eborunov@student.42.fr>          +#+  +:+       +#+        */
/*                                                +#+#+#+#+#+   +#+           */
/*   Created: 2023/01/24 21:12:52 by eborunov          #+#    #+#             */
/*   Updated: 2023/01/24 21:12:52 by eborunov         ###   ########.fr       */
/*                                                                            */
/* ************************************************************************** */

#ifndef GET_NEXT_LINE_H
# define GET_NEXT_LINE_H

# include <stdlib.h>
# include <sys/types.h>
# include <sys/uio.h>
# include <unistd.h>
# include <limits.h>

char		*ft_strcpy(char *line);
int			get_next_line(int fd, char **line);
size_t		ft_strlen(char *str);
int			ft_save_to_line(char **line, char *str_buff, size_t line_size);
int			ft_free(char *s_buff, char *rem, int s_b_flag, int r_flag);

#endif