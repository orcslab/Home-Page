---
output:
  html_document:
    mathjax         : default
---

## <a name="intro"></a>Introduction
This is a template for writing articles for the CampeLab home page. To keep our formatting standard, all articles must be written:

1. In (at least reasonably good) English. If you're not comfortable with the language, i) get the help of another student who is, and ii) go get yourself some more English lessons.
2. In [Markdown](http://daringfireball.net/projects/markdown/), preferrably **using this template**!

Warning: Github's Markdown viewer screws things a little bit (particularly images and equations), so don't worry if this template looks a bit rough around the edges - it will convert to HTML just fine (check the [Uploading the article](#uploading) for details).

## <a name="writing"></a>Writing the article

Use Rstudio's [R Markdown](http://rmarkdown.rstudio.com) capabilities if you need to embed code, or John Gruber's [Markdown:Dingus](http://daringfireball.net/projects/markdown/dingus) otherwise. If you choose to use other editors, the burden is on you to keep the standards of the home page.

For a good example of Markdown in action, check [this page](http://daringfireball.net/projects/markdown/syntax) and the [Markdown code that generates it](http://daringfireball.net/projects/markdown/syntax.text).

### Document header
Do not use the _title_, _author_, etc. fields in the document header. Actually, unless you really need something in particular, you can simply use (like I did in this template):

```
---
output:
  html_document:
    mathjax         : default
---
```

### Document body
Stick to the standard and keep it simple (the formatting, not necessarily the content). Markdown's _raison d'etre_ is to simplify formatting so that you can focus on content, so __don't overcomplicate things__! 

If you need to include equations, use LaTeX's "double dollar signs" for centered equations:

$$  
x = \frac{5^2}{y}
$$

There are two options for including figures:

1. If the figure is already hosted somewhere else in the net (do this only if you're really sure it is not going to suddenly disappear from that place. It is *always* better to use method 2 below, if possible.), you can include it using the HTML `<img>` tag, for instance:

```
<center>
<img src="http://150.164.32.10/joomla/images/members/Campelo_small.jpeg" alt="That's me!" 
height=150 width=200>
<br><font size="small"><strong>
Fig. 1: All hail the mighty advisor!
</strong></font><br><br>
</center>
```

2. If you want to include figures that are not hosted elsewhere, upload them to the [CampeLab/Home-Page/Figures](https://github.com/CampeLab/Home-Page/tree/master/Figures) repository, under a new folder with the following structure:

`CampeLab/Home-Page/Figures/YYYYMMDD-YourName/`

where `YYYYMMDD` is the date of the first figure upload for your article, and `YourName` is, well, your name. Place all figures for one particular article within this folder, and include them in your document using the appropriate HTML tag. The address for including your figure will be:  
`https://raw.githubusercontent.com/CampeLab/Home-Page/master/Figures/YYYYMMDD-YourName/FigureName.png`

```
<center>
<img src="https://raw.githubusercontent.com/CampeLab/Home-Page/master/Figures/20150503-Felipe/SiSu2015-1_EEUFMG_MaxMin.png"
alt="SiSU EEUFMG 2015">
<br><font size="small"><strong>
Fig. 2: Cutoff and maximum grades for UFMG's School of Engineering SiSU selection, 2015-1.
</strong></font><br><br>
</center>
```

## <a name="uploading"></a>Uploading the article

Here's the step-by-step of the process:

1. After you have written your article, you'll need to compile it to HTML before uploading it to the page:

    - If you used RStudio, click _Knit HTML_ in RStudio's editor and the HTML file will be generated. Open this file in the editor;

    - If you used Markdown Dingus, click the _Convert_ button and the HTML code will be displayed in a window;

2. Log into the CampeLab home page, click on the _Members Only_ tab and select the _New publication_ option (it's in the left bar);

3. Fill the fields. 
    - _Article Name_: the title of the article;
    - _Article Intro_: a first paragraph that will appear before the "Read More" button. Make it interesting and relatively short (300 to 800 characters, or 60 to 120 words). You can use your own article's first words, as long as there is no fancy formatting in there (some regular text formatting - _italics_, __bold__, etc.) is OK);
    - _Article Body_: the rest of your article. Just paste the HTML that you created in here. 

4. Click _Submit_.

5. Send a message to one of the __editors__ and ask him or her to publish your article. That is, unless you ARE an editor, in which case you should log into the Admin page and publish it yourself (in case of doubts contact either me or one of the other editors)

***
And that's it! I'll update this document every now and then, so make sure to come back eventually.

Cheers,  
Felipe

<div style="background-color:#eeeeee; width:400px">
<strong>Prof. Felipe Campelo, Ph.D.</strong><br/>
<i>Department of Electrical Engineering<br/>
Universidade Federal de Minas Gerais<br/>
Belo Horizonte, Brazil</i>
</div>
