### C 的令牌(Tokens)

C 程序由各种令牌组成，令牌可以是关键字、标识符、常量、字符串值，或者是一个符号。

```
printf("Hello, World! \n"); // 这句可分解成5个令牌如下：

// printf
// (
// "Hello, World! \n"
// )
// ;

```

### 分号

在 C 程序中，分号是语句结束符。也就是说，每个语句必须以分号结束。它表明一个逻辑实体的结束。

例如，下面是两个不同的语句：

```

printf("Hello, World! \n");
return 0;

```

### 注释

注释就像是 C 程序中的帮助文本，它们会被编译器忽略。

```
/* 我的第一个 C 程序 */

```

您不能在注释内嵌套注释，注释也不能出现在字符串或字符值中。

### 标识符

- 一个标识符以字母 A-Z 或 a-z 或下划线 _ 开始，后跟零个或多个字母、下划线和数字（0-9）。C 标识符是用来标识变量、函数，或任何其他用户自定义项目的名称。
- C 标识符内不允许出现标点字符，比如 @、$ 和 %。
- C 是区分大小写的编程语言。

命名规范：

1.标识符由字母、数字、下划线组成，并且首字母不能是数字。
2.不能把C的关键字作为用户的标识符，例如：if、for、while等。（注：标识符不能和C语言的关键字相同，也不能和用户自定义的函数或C语言库函数同名）
3.标识符长度是由机器上的编译系统决定的，一般的限制为8字符，(注：8字符长度限制是C89标准，C99标准已经扩充长度，其实大部分工业标准都更长)。
4.标识符对大小写敏感，即严格区分大小写。一般对变量名用小写，符号常量命名用大写。（注：C语言中字母是区分大小写的，因此score、Score、SCORE分别代表三个不同的标识符）
5.标识符命名应做到"见名知意"，例如，长度（外语：length），求和、总计（外语：sum），圆周率（外语：pi）

有效的标示符举例：
```
mohd       zara    abc   move_name  a_123
myname50   _temp   j     a23b9      retVal

```

### 关键字

下表列出了 C 中的保留字。这些保留字不能作为常量名、变量名或其他标识符名称。

```

auto	else	long	switch
break	enum	register	typedef
case	extern	return	union
char	float	short	unsigned
const	for	signed	void
continue	goto	sizeof	volatile
default	if	static	while
do	int	struct	_Packed
double	

```

C99新增关键字:

```
_Bool	_Complex	_Imaginary	inline	restrict
```

C11新增关键字:

```
_Alignas	_Alignof	_Atomic	_Generic	_Noreturn
_Static_assert	_Thread_local

```

C 中的空格: 只包含空格的行，被称为空白行，可能带有注释，C 编译器会完全忽略它。

在 C 中，空格用于描述空白符、制表符、换行符和注释。空格分隔语句的各个部分，让编译器能识别语句中的某个元素（比如 int）在哪里结束，下一个元素在哪里开始。因此，在下面的语句中：

```
int age;

```

在这里，int 和 age 之间必须至少有一个空格字符（通常是一个空白符），这样编译器才能够区分它们。另一方面，在下面的语句中：

```
fruit = apples + oranges;   // 获取水果的总数

```

fruit 和 =，或者 = 和 apples 之间的空格字符不是必需的，但是为了增强可读性，您可以根据需要适当增加一些空格。

