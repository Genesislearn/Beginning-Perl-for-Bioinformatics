# Beginning Perl for Bioinformatics · 生物信息学 Perl 语言入门（中文版）
James D. Tisdall
---

该书向只有很少、甚至没有编程经验的生物学家展示了如何使用 Perl 这一理想的编程语言进行生物学数据分析。每一章都集中解决特定的问题或者问题集，所以当你读完本书后，你会对 Perl 的基础知识有一个深刻的理解，收集到解析 BLAST 和 GenBank 等任务的程序，同时习得处理更加高级的生物信息学问题的技能。

![Beginning Perl for Bioinformatics](https://github.com/M-Mono/Beginning-Perl-for-Bioinformatics/raw/master/Frontmatter.jpg)
---
编译环境：
+ **Fork**
  + [Yixf-Education](https://github.com/Yixf-Education/BP4B)

    ```
    译文版权声明

        - 本书的中文翻译（含封面）未得到原作者和原出版社的许可，中译本的翻译错误与原作者无关！
        - 本书的中译本封面由原书封面修改而成，仅供该中译本使用！
        - 本书的中译本初衷是作为天津医科大学、生物医学工程与技术学院、生物信息学专业、《分子生物计算》课程的教材。
        - 本书的中译本仅供参考学习只用，严禁贩卖、流通，后果自负！
        - 本书的翻译仍处于草稿阶段，疏漏、错误之处在所难免，欢迎读者予以指正。
        - 本书的中译本解释权归译者所有，如有任何疑问，请发邮件至yixfbio@gmail.com 与译者本人联系。

      伊现富

      2015 年 8 月 14 日

      天医-生医-208
      ```

+ **TeX Distribution**
    + [MacTeX 2019](https://www.tug.org/mactex/) [(License)](https://www.tug.org/mactex/src/License.rtf)
        + for Apple macOS


    + [TeX Live 2019](https://www.tug.org/texlive/) [(License)](https://www.tug.org/texlive/copying.html)
       + for GNU/Linux & Microsoft Windows


+ **Fonts**
  + [be5invis 更纱黑体 Sarasa Gothic 0.10.2](https://github.com/be5invis/Sarasa-Gothic) [(License)](https://github.com/be5invis/Sarasa-Gothic/blob/master/LICENSE)
  + [Adobe Source Code Pro 2.030](https://github.com/adobe-fonts/source-code-pro) [(License)](https://github.com/adobe-fonts/source-code-pro/blob/master/LICENSE.md)


+ **Editor**
    + [Visual Studio Code 1.40.1](https://code.visualstudio.com/) [(License)](https://code.visualstudio.com/License/)
        + [LaTeX Workshop 8.4.1](https://github.com/James-Yu/LaTeX-Workshop) [(License)](https://github.com/James-Yu/LaTeX-Workshop/blob/master/LICENSE.txt)
            + Configuration for LaTeX Workshop extension to complie XeTeX source code into PDF Version 1.7 (Acrobat 8.x)

                ```Visual Studio Code``` ⇢ ```File``` ⇢ ```Preferences``` ⇢ ```Settings``` ⇢ ```Extensions``` ⇢ ```LaTeX``` ⇢ ```Recipes```


                ```JSON
                {
                        "latex-workshop.view.pdf.viewer": "tab",
                        "latex-workshop.latex.tools": [
                                {
                                        "name": "latexmk",
                                        "command": "latexmk",
                                        "args": [
                                                "-synctex=1",
                                                "-interaction=nonstopmode",
                                                "-file-line-error",
                                                "-pdf",
                                                "%DOC%"
                                        ]
                                },
                                {
                                        "name": "xelatex",
                                        "command": "xelatex",
                                        "args": [
                                                "-synctex=1",
                                                "-interaction=nonstopmode",
                                                "-file-line-error",
                                                "--output-driver=xdvipdfmx -q -E -V 7",
                                                "%DOC%"
                                        ]
                                },
                                {
                                        "name": "pdflatex",
                                        "command": "pdflatex",
                                        "args": [
                                                "-synctex=1",
                                                "-interaction=nonstopmode",
                                                "-file-line-error",
                                                "%DOC%"
                                        ]
                                },
                                {
                                        "name": "bibtex",
                                        "command": "bibtex",
                                        "args": [
                                                "%DOCFILE%"
                                        ]
                                }
                        ],
                        "latex-workshop.latex.recipes": [
                                {
                                        "name": "XeLaTeX / XeTeX",
                                        "tools": [
                                                "xelatex"
                                        ]
                                },
                                {
                                        "name": "latexmk",
                                        "tools": [
                                                "latexmk"
                                        ]
                                },
                                {
                                        "name": "pdflatex -> bibtex -> pdflatex*2",
                                        "tools": [
                                                "pdflatex",
                                                "bibtex",
                                                "pdflatex",
                                                "pdflatex"
                                        ]
                                }
                        ],
                        "workbench.startupEditor": "newUntitledFile",
                        "window.zoomLevel": 0,
                        "editor.minimap.enabled": false
                }
                ```
