# LibASM
Recoding certain functions of the standard C Library, but in x86-64 Intel Assembly.
## Final grade : 115/125

Mandatory part : 100/100

Bonus : 15/25
### How to use it
Using ``make`` will create the ``libasm.a`` binary.
To include the library in your project, clone the repository in your working tree and compile with the following flags :
```
gcc  main.c libasm.a
```
Using ``make bonus`` will create the ``libasm.a`` binary.
```
gcc  main_bonus.c libasm.a
```
### Available functions
```
size_t		ft_strlen(const char *s);
int		ft_strcmp(const char *s1, const char *s2);
char		*ft_strcpy(char *dst, const char *src);
char		*ft_strdup(const char *s1);
ssize_t		ft_read(int fildes, void *buf, size_t nbyte);
ssize_t		ft_write(int fildes, const void *buf, size_t nbyte);

int		ft_list_size(t_list *lst);
int		ft_list_push_front(t_list **begin_list, void *data);
void		ft_list_sort(t_list **begin_list, int (*cmp)());

```
