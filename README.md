# 📄 Get Next Line

## 📝 Description

**Get Next Line** is a project from **School 42**.  
The goal is to implement a function that reads a file descriptor line by line, returning one line at each call.  
The function must handle multiple file descriptors at the same time (bonus part).

---

## 🎯 Objectives

- Understand static variables
- Manage file descriptors
- Handle memory allocation and leaks
- Read data efficiently using buffers
- Write clean and norm-compliant code (42 Norm)

---

## 🛠️ Prototype

```c
char *get_next_line(int fd);
```

--- 

### ⚙️ How It Works

- The function reads from the given file descriptor until it encounters a newline (\n) or reaches EOF
- Each call returns the next line, including the newline if present
- If there is nothing more to read, the function returns NULL
- The bonus version supports multiple file descriptors simultaneously

---

### 📦 Files
### Mandatory

- `get_next_line.c`
- `get_next_line_utils.c`
- `get_next_line.h`

### Bonus

- `get_next_line_bonus.c`
- `get_next_line_utils_bonus.c`
- `get_next_line_bonus.h`

--- 

### ⚙️ Compilation & Usage

Compile with:


```bash
gcc -Wall -Wextra -Werror get_next_line.c get_next_line_utils.c
```

For bonus:

```bash
gcc -Wall -Wextra -Werror get_next_line.c get_next_line_utils.c
```

---

### ⚠️ Buffer Size

The function uses a buffer size defined at compilation:

```bash
-D BUFFER_SIZE=42
```

Example:

```bash
gcc -D BUFFER_SIZE=42 get_next_line.c get_next_line_utils.c
```

--- 

### 📐 Norm

- Fully compliant with the 42 Norm
- No forbidden functions used
- No memory leaks

--- 

### 👤 Author
- 42 Login: fmotte
- School: 42

--- 

### ✅ Status
✔️ Mandatory: validated  
⭐ Bonus: 125 / 125  