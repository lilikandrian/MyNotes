#MarkDown #TipsandTrik #Help
# Welcome to MWeb for iOS

MWeb is Pro Markdown writing, note taking and static blog generator App for Mac, iPad and iPhone. MWeb use of Github Flavored Markdown, referred to as GFM, which is one of the most widely used Markdown syntax. If you do not know what Markdown is, it is recommended to take a look at the [Markdown Syntax.md](Markdown%20Syntax.md) documentation. GFM in addition to support the official syntax, but also extended a lot of grammar. 

[Markdown Mat](Markdown%20Mat.md)
[Markdown MWeb](Markdown%20MWeb.md)
[Markdown Reference](Markdown%20Reference.md)
[Markdown Syntax](Markdown%20Syntax.md)

*[[Markdown Help I#^d9cba2]]*
**[[Markdown Help]]**
**[[Markdown MWeb]]**
**[[Markdown Help I]]**
**[[Markdown Mat]]**
**[[Markdown Syntax]]**

-----------

## GFM syntax guide

### Newlines

End a line with two or more spaces + enter.
Just typing enter to newline,please go to Settings and enable "Translate newlines to `<br>` tags" ( default is enable ).

### Task lists

**Example:**

```
- [ ] task one not finish `- + SPACE + [ ]`
- [x] task two finished `- + SPACE + [x]`
```

**Result:**

- [ ] task one not finish `- + SPACE + [ ]`
- [x] task two finished `- + SPACE + [x]`

### Image size and alignment **(Only in MWeb)**

Setting image width, align left, align right, align center syntax. For example: `![image description-w450](pic.jpg)`, -w450 mean set the image width: 450. `![-l500](pic.jpg)` --> align left, width:500. `![-r500](pic.jpg)` --> align right, width:500. `![-c500](pic.jpg)` --> align center, width:500.

### Multi-line code

**Example:**

    ```js
	function fancyAlert(arg) {
	  if(arg) {
	    $.facebox({div:'#foo'})
	  }

	}
    ```

**Result:**

```js
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }

}
```

### Tables

**Example:**

```
First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column
```

You can create tables by assembling a list of words and dividing them with hyphens - (for the first row), and then separating each column with a pipe |:

**Result:**

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column


### Strikethrough

**Example:**

	 (like ~~this~~)

**Result:**

Any word wrapped with two tildes (like ~~this~~) will appear crossed out.

### LaTeX

Markdown syntax:

    Block-level formula:
    ```math
    x = \dfrac{-b \pm \sqrt{b^2-4ac}}{2a}
    ```
    
    In-line formula: ``\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N``


The resut is (enable LaTeX in the settings page):

Block-level formula:

```math
x = \dfrac{-b \pm \sqrt{b^2-4ac}}{2a}
```

In-line formula: ``\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N``

Note: For compatibility with MWeb 3, $\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$ is also supported
And block-level syntax
$$ x = \dfrac{-b \pm \sqrt{b^2-4ac}}{2a} $$

- [ ] But it is recommended to use the new syntax.

## MWeb drawing

### mermaid

mermaid is a popular drawing gallery. It supports flowcharts, sequence diagrams and Gantt charts. Its official website is: <https://mermaidjs.github.io/>. The syntax of mermaid in MWeb is to declare code blocks. The language is mermaid, and the mermaid drawing grammar can be written in the code block. You can copy the following grammar to MWeb to view the result.

    ```mermaid
    sequenceDiagram
        participant Alice
        participant Bob
        Alice->John: Hello John, how are you?
        loop Healthcheck
            John->John: Fight against hypochondria
        end
        Note right of John: Rational thoughts <br/>prevail...
        John-->Alice: Great!
        John->Bob: How about you?
        Bob-->John: Jolly good!
    ```
 
**The result is:**
 
```mermaid
sequenceDiagram
    participant Alice
    participant Bob
    Alice->John: Hello John, how are you?
    loop Healthcheck
        John->John: Fight against hypochondria
    end
    Note right of John: Rational thoughts <br/>prevail...
    John-->Alice: Great!
    John->Bob: How about you?
    Bob-->John: Jolly good!
```
### echarts

echarts is a js drawing gallery produced by Baidu. Its website is: <https://echarts.apache.org/zh/index.html>. It has very powerful functions. MWeb supports some basic usages of echarts, but not too advanced. . You can copy the following syntax to MWeb to try. You can also go to <https://echarts.apache.org/examples/zh/index.html> to view some examples. Note that MWeb can only parse the simple `option = {}`, but it should It is enough to use.

    ```echarts
    option = {
        xAxis: {
            type:'category',
            data: ['Mon','Tue','Wed','Thu','Fri','Sat','Sun']
        },
        yAxis: {
            type:'value'
        },
        series: [{
            data: [820, 932, 901, 934, 1290, 1330, 1320],
            type:'line'
        }]
    };
    ```

**The result is:**

```echarts
option = {
    xAxis: {
        type:'category',
        data: ['Mon','Tue','Wed','Thu','Fri','Sat','Sun']
    },
    yAxis: {
        type:'value'
    },
    series: [{
        data: [820, 932, 901, 934, 1290, 1330, 1320],
        type:'line'
    }]
};
```

### Footnote

**Example:**

```
This is a footnote:[^1]
```

**Result:**

This is a footnote:[^1]

[^1]: footnote text detail...

![](media/16297923273991.jpg)


Ini adalah image pertama yang dimasukkan melalui md document.


### Comment And Read More..

<!-- comment -->
<!-- more -->




