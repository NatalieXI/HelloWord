# MarkDown学习笔记
标题是每篇文章都需要也是最常用的格式，在 Markdown 中，如果一段文字被定义为标题，只要在这段文字前加 # 号即可。

# 一级标题

## 二级标题

### 三级标题

以此类推，总共六级标题，建议在井号后加一个空格，这是最标准的 Markdown 语法。

# 列表
熟悉 HTML 的同学肯定知道有序列表与无序列表的区别，在 Markdown 下，列表的显示只需要在文字前加上 - 或 * 即可变为无序列表，有序列表则直接在文字前加1. 2. 3. 符号要和文字之间加上一个字符的空格。
1. 有序列表1
2. 有序列表2
3. 有序列表3

# 引用

如果你需要引用一小段别处的句子，那么就要用引用的格式。
> 例如这样
 只需要在文本前加入 > 这种尖括号（大于号）即可
# 图片与链接

插入链接与插入图片的语法很像，区别在一个 !号

1. 图片为：![ ]( ){ImgCap}{/ImgCap}

2. 链接为：[ ]( )

插入图片的地址需要图床，这里推荐围脖图床修复计划 与 CloudApp 的服务，生成URL地址即可。
## 插入链接
[NatalieXI](https://github.com/NatalieXI/HelloWord)
# 粗体与斜体

Markdown 的粗体和斜体也非常简单，用两个 * 加一段文本就是粗体的语法，用一个 * 加一段文本就是斜体的语法。

例如：**这里是粗体 *这里是斜体
# 表格

表格是我觉得 Markdown 比较累人的地方，例子如下：

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

# 代码框

如果你是个程序猿，需要在文章里优雅的引用代码框，在 Markdown下实现也非常简单，只需要用两个`把中间的代码包起来
`public static boolean isDirExist(String dirPath, boolean bCreate) {
		File dir = new File(dirPath);
		if (dir.exists())
			return true;
		if (!bCreate)
			return false;

		// 创建目录
		File parent = dir.getParentFile();
		if (parent.exists()) {
			return dir.mkdir();
		} else {
			if (isDirExist(dir.getParent(), bCreate))
				return dir.mkdir();
			else
				return false;
		}
	}`
 
# 分割线

分割线的语法只需要三个 * 号，例如：
***





