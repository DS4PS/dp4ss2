#### Data Programming for the Social Sciences (DP4SS)

<br>

<center>
  
A gentle introduction to data programming <br> 
in R for social science audiences. 

<br> <br> 

Jesse Lecy <br> 
& <br> 
Jamison Crawford

<br> 
<br> 
<br> 
<br> 

<img src="https://raw.githubusercontent.com/DS4PS/ds4ps.github.io/master/assets/img/cc.logo.png" alt="CC License" style="width:200px;">
<br> 
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Attribution · NonCommercial · ShareAlike</a>

<br>
<br>
<br>

<a rel="license" href="https://github.com/DS4PS/dp4ss-textbook">
<img src="https://cdn.freebiesupply.com/logos/large/2x/github-icon-logo-png-transparent.png" alt="GitHub" style="width:50px;">
<br> 
Source Code</a>
<br>
</center>

<br>
<br>

This textbook is being developed by adapting lecture notes and resources from a graduate-level introductory course in data science that is offered at the Watts College of Public Service at Arzona State University. 

Comments and suggestions are welcome!    ·  ·  ·   <a rel="license" href="https://github.com/DS4PS/dp4ss-textbook/issues/new">
<img src="https://image.flaticon.com/icons/png/512/813/813419.png" alt="new issue" style="width:30px;"></a> [Comments](https://github.com/DS4PS/dp4ss-textbook/issues/new)



<br>
<br>
<br>



**CONTENTS:**

-----------------------

* TOC
{:toc}

-----------------------

<br>
<br>
<br>
 
 












# Your Data Science Toolkit  
 
We will need three tools to manage your data science projects: a data programming language (R), a project management interfact (R Studio), and a way to create data-driven documents (R Markdown).  
 
 
## [Core R](http://ds4ps.org/dp4ss-textbook/ch-010-core-r.html)  

* What is R?  [ [video](https://player.vimeo.com/video/180644880) ]  
* Packages  
  - [CRAN Views](https://cran.r-project.org/web/views/)  
  - [Awesome R](https://awesome-r.com/)  
  - [R Bloggers](https://www.r-bloggers.com/) 



## [R Studio](http://ds4ps.org/dp4ss-textbook/ch-020-rstudio.html)   

* Installing R and R Studio  
* Tour of R Studio  


## [Data-Driven Docs](http://ds4ps.org/dp4ss-textbook/ch-030-data-driven-docs.html)   

* Automation & Flexibility   
* [The Importance of Reproducibility](https://www.nature.com/news/1-500-scientists-lift-the-lid-on-reproducibility-1.19970)  
* Formats [link](https://rmarkdown.rstudio.com/formats.html)  
* Gallery [link](https://rmarkdown.rstudio.com/gallery.html)  


## [Markdown](http://ds4ps.org/dp4ss-textbook/ch-031-markdown.html)  

* R Markdown Formats [overview](https://rmarkdown.rstudio.com/lesson-1.html)  
  * Headers and Chunks [link](https://ds4ps.org/docs/#how-do-data-driven-docs-work)  
  * Knitting [link](https://ds4ps.org/docs/#knitting-r-markdown-files)  
  * [Customization](https://holtzy.github.io/Pimp-my-rmd/) 
 
<br>
<br>

 
# Getting Started 

These are some useful resources and guides for learning how to program if you are new to R or data programming. 

## Starting to Code  
* [RMD File Styles and Knitting Tips](https://ds4ps.org/cpp-526-fall-2019/labs/r-markdown-files.html)  
* [Style Guides](https://jef.works/R-style-guide/)  


## [Getting Help](http://ds4ps.org/dp4ss-textbook/ch-021-help.html)  
* Help files   
* Error messages   
* Discussion boards  


## [The Learning Curve](http://ds4ps.org/dp4ss-textbook/ch-032-learning_r.html)   
* Vocabular and verbs  
* Learning to Learn R 

<br>
<br>



# Using R 

Functions, variables, and operators are the core components of any functional programming language. These first chapters are foundational for everything moving forward. 

## [R as a Calculator](http://ds4ps.org/dp4ss-textbook/ch-033-calculator.html)   
* Mathematical Operators 
* Objects
* Assignment 
 
## [Functions](http://ds4ps.org/dp4ss-textbook/ch-040-functions.html)  
* Input-Output Devices 
* Arguments 
* Values 
* Returns 

## [Logical Operators](http://ds4ps.org/dp4ss-textbook/p-050-business-logic.html)
* Logical operators 
  - equal
  - not equal 
  - greater than or less than 
  - opposite of

## Special Operators 
  - Unique values 
  - Duplicates 
  - Missing values (NA)
  - Maximum 
  - Minimum 

<br>
<br>



# One-Dimensional Datasets

Vectors are the building blocks of analysis in R. Vectors come in a variety of flavors - we cover the four most salient data types here: numbers, characters, categories, and logical or boolean. 

## [Vectors](http://ds4ps.org/dp4ss-textbook/ch-050-vectors.html)   
* Vector Types
  - Numeric (v)
  - Character (s)
  - Factor (ordered vs unordered) (f)
  - Logical (true/false) (L)
* Checking vector types
  - data class 
  - data mode 

## Converting Data Type   
* Casting  
  - explicit casting 
  - implicit casting (coercion)
* Information loss 
* Care with factors  


## Variable Transformations   
* Linear transformations 
  - vectorized functions 
  - recycling rules 
* Recoding values 
  - find and replace
  - recoding factors 
* Floors and ceilings 

<br>
<br>




# Two-Dimensional Datasets  

Vectors typically represent individual variables in the social science context. A dataset contains IDs for individuals, and multiple measures from each individual. Typically data is organized so that columns represent distinct variables and rows represent individuals in the dataset. This spreadsheet representation of data is operationalized as **data frames** in R. Here you learn how to construct and manipulate data frames. 

## Dataframes  

* Creating data frames from vectors  
  - rows and columns  
* the `$` operator 
* Checking and changing class types 


## Dataframe Subsets  

* Filter rows and select columns  
  - the `[]` operator 
  - `dplyr::filter` and `dplyr::select` 
* Reorder rows or columns
  - `sort()` versus `order()`
  - `dplyr::arrange` 

## Dataframe Constructors   
* Building data objects: 
  - `data.frame()` vs `cbind()` and `rbind()`
* Variable transformations in df's
  - assignment inside a df: `dat$x_squared <- x·x`
  - `dplyr::mutate` vs `dplyr::transmute()`

## Matrices and Lists 
* Matrix 
* Lists 
* Conversions: 
  - matrix to df 
  - list to df 

<br>
<br>



# Data IO

Data **import** and **export** *[ input / output ]*.

## Navigation 
* Working directories
  - paths: windows v linux 
  - current working directory: `getwd()` 
  - change working directory: `setwd()` 
  - check files in directory: `dir()`
  - create new folder: `dir.create("name")`
* Unzip files `unzip("filename")`
* Delete files [tutorial](http://theautomatic.net/2018/07/11/manipulate-files-r/)

## Built-In Datasets
* Core R datasets 
* Datasets in packages 
* Packages that are data 

## [Importing Data into R](http://ds4ps.org/dp4ss-textbook/ch-100-importing.html) 
* Read options   
* Copy and paste from Excel 
* Using rdata format 
* Read from csv or tsv
* Read text files
* Import from Excel
* Import from common format (foreign package)
* Import from the web (RCurl)
* Import from GitHub
* Import from DropBox
* [ [tutorial](https://www.datacamp.com/community/tutorials/r-data-import-tutorial) ]

## [Exporting Data](http://ds4ps.org/dp4ss-textbook/ch-101-exporting_files.html) 
* Write options 
  - CSV 
  - R Data Sets (RDS)
  - CSV vs RDS
  - Tables 
  - RData Format
  - SPSS or Stata 
* Copy to Clipboard 
* Copy to Excel 
* [ [tutorial](https://thomasleeper.com/Rcourse/Tutorials/savingdata.html) ]

## [APIs](http://www.storybench.org/how-to-access-apis-in-r/) 
* What is an API?
* Examples 
  - Census
  - Socrata
  - Twitter
* [ [Demo with DataUSA API](https://gist.github.com/lecy/0aa782a873cd174573f32d243233ca5b) ] 

<br>
<br>


<br>
<br>




# Data Wrangling (dplyr)

Data wrangling is the process of preparing data for analysis, which includes reading data into R from a variety of formats, cleaning data, tidying datasets, creating subsets and filters, transforming variables, grouping data, and joining multiple datasets. 

The goal of data wrangling is to create a **rodeo dataset** (clean and well-structured) that is ready for the big show (modeling and visualization)! 

## [Slicing Datasets](http://ds4ps.org/dp4ss-textbook/p-070-data-verbs.html) 
* Subset operator `[]`
  - by position 
  - by name 
  - by logical vector 
  - with recycling
* Selector vectors
* Subset by row 
  - `dat[ row_selector , ]`
  - `dplyr::filter( dat, row_selector )`
* Subset by column
  - `dat[ , column_selector ] `
  - `dplyr::select( dat, column_selector )`
* Reorder 
  - with index 
  - order / match

## [Data Wrangling Recipes](http://ds4ps.org/dp4ss-textbook/p-072-data-recipes.html) 
* Pipe operator 
* Window vs summary functions 
* dplyr [cheat sheet](https://rstudio.com/wp-content/uploads/2015/02/data-wrangling-cheatsheet.pdf) 

## [Combining Datasets](http://ds4ps.org/dp4ss-textbook/p-076-merging-data.html) 
* `merge()` and `match()`
* `join()` in dplyr
* inner, outer, right, left

<br>
<br>



# Explore and Describe

The first step in the data science process is to get to know your data through descriptive analysis and exploratory analysis that searches for useful patterns or trends. We accomplish this through summary statistics, and in the next section visualization. 

## Summarizing Vectors
* Counting things:  
  - `sum( logical statement )`
* Counting missing data: 
  - `sum( is.na(x) )`
* Categorical data:  
  - `table( f1, f2 )`
  - `prop.table()` and `margin.table()`
* Numeric data:  min, max, mean, median, summary, quantile
  - all vectors at once:  `summary( data.frame )`


## Summarizing Groups of Vectors
* `table( f1, f2 )` 
* `ftable( row.vars=c("f1","f2"), col.vars="f3" )`
* Function over groups:  `tapply( v1, f1 )`  or `dplyr:: group_by() + summarise()`
* Functions over levels of numeric data:  `tapply( v1, cut(v2) )`
* `tapply( v1, INDEX=list(f1,f2)`  or `dplyr:: group_by() + summarise()`
* `aggregate( dat, FUN, by=f1 )`
* https://cran.r-project.org/web/packages/DescTools/vignettes/DescToolsCompanion.pdf
* v1, v2 using `cor()` or visually with `pairs()` 

<br>
<br>




# Efficient Analysis With Groups

As you become proficient with descriptive analysis you will want to find ways to be more efficient. Unless you learn how to scale data exploration and modeling you will not be able to quickly identify patterns in your data. The most efficient way to scale your analysis is to understand the dimensionality or internal problem space in your data, and use **apply** functions in R to replicate analysis over many groups at once. 

## [Groups](http://ds4ps.org/dp4ss-textbook/p-050-business-logic.html) 
* Logical statements 
  - define group criteria 
  - TRUE signifies membership
* Group constructors 
  - from categorical variables
  - from numeric variables
  - from strings 
  - from missing values 
* Compound logical statements:  AND and OR
* Casting logical vectors 


## [Group Structure](http://ds4ps.org/dp4ss-textbook/p-073-group-structure.html) 
* Combining factors and numeric data for analysis 
* Faceting in plots 


## Counting Group Members  
* Mathematical operators with logical vectors
  - counts of members: sum( L1 )
  - proportions of members: mean( L1 )
* Conditional proportions 
  - subset then tabulate 
  - logical statement in numerator and demoninator 
 
 
## The Mathematics of Groups  
* Group structure 
  - generalizing logical statements 
* Group dimensionality 
  - how many unique groups are in the data? 
  - combinatorics of attributes
  - total groups from f1 and f2 `= nlevels(F1) · nlevels(F2)` 
* Groups as problem spaces 
  - complexity theory 
  - search 
  - dimension reduction 


## Analysis with Groups   
* Contingency tables  
  - counts of members:  `f1 · f2`
* Statistics by group
  - function applied over a group: `v1 ~ f1 · f2`
  - `apply()` functions 
  - dplyr `group_by()` and `summarize()` functions 


## Latent Groups 
  - clustering 
  - unsupervised learning approaches 

<br>
<br>











# Visualization 

For a great overview with examples of R code: 

*Wilke, C. O. (2019). Fundamentals of Data Visualization: A Primer on Making Informative and Compelling Figures. O'Reilly Media.* [FREE EBOOK](https://serialmentor.com/dataviz/)

## [Principles of Visual Communication](http://ds4ps.org/dp4ss-textbook/p-060-intro-to-data-viz.html)  
* Ground, figure, narrative (context, subject, action)
* Tufte’s rules 
* Visual tragedies 

## [Core Graphics Engine](http://ds4ps.org/dp4ss-textbook/p-061-plot-basics.html)  
* `plot()` function 
* Arguments:
  - plot point types 
  - colors 
  - size 
  - axis labels 
  - plot title 
  
## [Customizing Graphics](http://ds4ps.org/dp4ss-textbook/p-062-customized-graphics.html) 
* Defining a canvas: xlim, ylim
* Adding data
* Type (point, line, both)
* Symbols
* Color
* Size
* Adding grids
* Adding axes
* Adding titles / axes labels
* Adding data labels:  text()
* Margins

## Colors in R
* select by name: 
  - [pre-programmed pallete](http://www.stat.columbia.edu/~tzheng/files/Rcolor.pdf) 
  - [popular packages](https://www.datanovia.com/en/blog/the-a-z-of-rcolorbrewer-palette/) 
* [color theory](https://www.canva.com/colors/color-wheel/)
  - value
  - shade, tint, tone 
  - hue, saturation 
  - transparency 
* color values 
  - [RGB codes vs Hex codes](https://htmlcolorcodes.com/)
* [color functions](https://www.nceas.ucsb.edu/~frazier/RSpatialGuides/colorPaletteCheatsheet.pdf)

## Advanced Plot Features 
* Custom fonts 
* Math symbols 
* Multiple plots (core graphics)
  - incorrect:  https://en.wikipedia.org/wiki/File:Smallmult.png#/media/File:Smallmult.png
* Custom graph layouts

## [Grammar of Graphics and ggplot2](http://ds4ps.org/dp4ss-textbook/ch-102-ggplot2.html) 
* Grammar of graphics concept
* ggplot overview


## Animations 


<br>
<br>


# Dynamic Documents 

## [R shiny](https://github.com/DS4PS/cpp-526-fall-2019/raw/master/lectures/shiny-widgets.pdf) 
* What makes documents dynamic? 
* Widgets 
  - input objects
  - [Widgets Gallery](https://shiny.rstudio.com/gallery/widget-gallery.html)
* Render functions 
* Reactive functions 
* [ [tutorial](http://rmarkdown.rstudio.com/authoring_shiny.html) ] 


## [Dashboards in R](http://rmarkdown.rstudio.com/flexdashboard/) 
* Principles of good dashboard design 
* Layouts 
* Sidebars 
* Value boxes 
* [ [demo RMD](https://shiny.rstudio.com/gallery/kmeans-example.html) ]

## Customizing Styles 
* CSS: cascading style sheets

<br>
<br>
<br>






<style>
  
.post-content>ul {
font-family: monospace; 
  font-size: 16px; 
  font-style: normal; 
  font-variant: none; 
  font-weight: 100;
  line-height: 30px;
}

.post-content>h2 { 
  font-size: 20px;  
  color: maroon;
  font-weight: normal;
}

.post-content>h4 { 
  font-family: "Century Gothic", CenturyGothic, AppleGothic, sans-serif; 
  font-weight: bold;
  font-size: 48px;  
  color: maroon;
  line-height: 1.1em;
}

.post-content>h1 {
/*   background-color: #666; */
  color: #2c0c0c;
  font-weight: bold;
  font-size: 48px !important;
  padding: 0px;
  margin-top: 70px;
  margin-bottom: 10px;
}


.post-content a {
  color: maroon;
  font-weight: normal;
  text-decoration: underline steelblue;
} 

.post-content>ul a {
  font-weight: bold;
}
  
#markdown-toc a {
    color: black;
    font-size: calc(0.75em + 0.25vw);
    line-height: 1.2;
    font-weight: normal;
    text-decoration: none;
}
  
.navbar-nav>li>a {
    display: flex;
    justify-content: center;
    align-items: center;
    box-sizing: border-box;
    height: 80px;
    padding: 0 15px;
    font-size: .875rem;
    font-family: system-ui;
}

#markdown-toc ul {
  font-size:calc(0.85em + 0.25vw);
  line-height:1.2;
  font-weight: bold;
} 
#markdown-toc ul li {
  list-style-type: disc !important;
  font-size:calc(0.65em + 0.25vw);
  line-height:1.2;
  margin-left: 20px;
}  


/* #markdown-toc li ul li { */
/*   display:none; */
/* }   */

#markdown-toc a {
  color: black;
  font-size:calc(0.65em + 0.25vw);
  line-height:1.2;
  font-weight: normal;
}  
#markdown-toc a:hover {
    color: black;
    text-decoration: none;
    font-weight: bold;
}

pre, code {
  border: none;
}

code {
    font-size: 1.1em;
    font-family: "Andale Mono", AndaleMono, monospace;
    padding: 0px 1px;
    padding-top: 0px;
    padding-right: 1px;
    padding-bottom: 0px;
    padding-left: 1px;
    border-radius: 0px;
    font-weight: bold;
}

.collapsible {
  background-color: #fff;
  color: #444;
  cursor: pointer;
  padding: 18px;
  width: 20%;
  border: none;
  text-align: left;
  outline: none;
  font-size: 15px;
}

.active, .collapsible:hover {
  background-color: #ccc;
}

.active, .collapsible:hover {
  background-color: #ccc;
}

.content {
  display: none;
  overflow: hidden;
}




  /* Reset Basic Elements
 * ============================================== */
    body, h1, h2, h3, h4, h5, h6,
    p, blockquote, pre, hr,
    dl, dd, ol, ul, figure {
        margin: 0;
        padding: 0;
    }

h1 { color: black; }
    h2 {
        color: #337ab7; // blue
        font-weight:300;
    } 

/* Basic Styling
 * ============================================== */
    body {
        font-family: $base-font-family;
        font-size: $base-font-size;
        line-height: $base-line-height;
        font-weight: 300;
        color: $text-color;
        background-color: $background-color;
        -webkit-text-size-adjust: 100%;
    }

/* Set Margin Bottom for Vertical Rhythm
 * ============================================== */
    h1, h2, h3, h4, h5, h6,
    p, blockquote, pre,
    ul, ol, dl, figure,
    %vertical-rhythm {
        margin-bottom: $spacing-unit / 2;
    }

/* Images and Figures
 * ============================================== */
    img {
        max-width: 100%;
        vertical-align: middle;
    }

    figure > img {
        display: block;
    }

    figcaption {
        font-size: $small-font-size;
    }

/* Lists
 * ============================================== */
    ul, ol {
        margin-left: $spacing-unit;
    }

    li {
        > ul,
        > ol {
             margin-bottom: 0;
        }
    }

/* Headers
 * ============================================== */
    h1, h2, h3, h4, h5, h6 {
        font-weight: bold;
        margin: 0px;
    }

    h1 {font-size: 1.9em !important;}
    h2 {font-size:calc(2em + 0.25vw) !important; }  // font-size: 1.5em !important;}
    h3 {font-size: 1.3em;}
    h4 {font-size: 1em;}
    h5 {font-size: .9em;}
    h6 {font-size: .8em;}


/* Links
 * ============================================== */
    a {
        // color: darken($brand-color, 10%);
        color: rgba(229,144,42,.7);
        text-decoration: none;
        font-weight: bold;
        
        &:hover {
            color: darken($brand-color, 10%);
            text-decoration: none;
            font-weight: bold;
        }
    }

/* Block Quotes
 * ============================================== */
    blockquote {
        color: #BBB;
        border-left: 4px solid $brand-color;
        padding-left: $spacing-unit / 2;
        font-size: 17px;
        letter-spacing: -1px;
        // font-style: italic;

        > :last-child {
            margin-bottom: 0;
        }
    }

/* Code Blocks
 * ============================================== */
    pre,
    code {
        font-size: 13px;
        border: 1px solid $grey-color-light;
        font-family: Andale Mono, AndaleMono, monospace;
    }

    code {
        padding: 1px 3px;
        background-color: #FFF;
        border-radius: 5px;
        font-family: Andale Mono, AndaleMono, monospace;
    }

    pre {
        border-radius: 3px;
        padding: 8px 12px;
        overflow-x: scroll;
        background-color: #F5F5F5;

        > code {
            background-color: #F5F5F5;
            border: 0;
            padding-right: 0;
            padding-left: 0;
        }
    }

/* Wrapper
 * ============================================== */
    .wrapper {
        max-width: -webkit-calc(#{$content-width} - (#{$spacing-unit} * 2));
        max-width:         calc(#{$content-width} - (#{$spacing-unit} * 2));
        margin-right: auto;
        margin-left: auto;
        padding-right: $spacing-unit;
        padding-left: $spacing-unit;
        @extend %clearfix;

        @include media-query($on-laptop) {
            max-width: -webkit-calc(#{$content-width} - (#{$spacing-unit}));
            max-width:         calc(#{$content-width} - (#{$spacing-unit}));
            padding-right: $spacing-unit / 2;
            padding-left: $spacing-unit / 2;
        }
    }

/* Clear Fix
 * ============================================== */
    %clearfix {

        &:after {
            content: "";
            display: table;
            clear: both;
        }
    }

/* TABLES
 * =============================================== */
    table {
        border-collapse: collapse;
        border-spacing: 0
    }

    :not(.highlight)>table {
    margin: 0 auto 1.5em auto
    }

    :not(.highlight)>table tr {
        background-color: #fff;
        border-top: 1px solid #ccc
    }

    :not(.highlight)>table tr th, :not(.highlight)>table tr td {
        padding: 6px 13px;
        border: 1px solid #ddd
    }

    :not(.highlight)>table tr th {
        font-weight: bold
    }

    :not(.highlight)>table tr:nth-child(2n) {
        background-color: #f8f8f8
    }

/* Site Header
 * ============================================== */
    .site-header {
        min-height: 450px;
        background-color: $brand-color;
        background-image: url('');
        background-size: cover;
        background-position: center -170px;
        background-attachment: fixed;

        @include media-query($on-palm) {
            min-height: 250px;
            background-position: center -250px;
        }
    }


    .site-header a, a h1 {color: #FFF}; 
    .site-header a:hover, a h1:hover {color: black}; 

    .site-header h1 {
        display: block;
        font-size: 80px !important;
        line-height: 80px;
        letter-spacing: 3px;
        text-align: center;
        padding-top: 20px;
        clear: both;
        text-transform: uppercase;
        font-family: 'Open Sans';

        @include media-query($on-palm) {
            font-size:60px !important;
            letter-spacing: 0px;
        }
    }

    .site-header span {
        border: 10px solid #FFF;
        padding: 0.3em 0.5em;
        margin: 10px 20px;
        display: inline-block;

        @include media-query($on-palm) {
            margin: 10px 10px;
            padding: 0.15em 0.4em;
        }
    }


    .site-nav {
        // float: left;
        line-height: 56px;
        margin-left: 50px;
        padding-bottom: 100px;

        
        .page-link {
            line-height: $base-line-height;
            font-weight: bold;
            letter-spacing: 0.05em;
	    text-transform: uppercase;

            &:not(:first-child) {
                margin-left: 20px;
            } 
         }
            


        .page-link:hover {
            opacity: 0.8;
        }

        @include media-query($on-palm) {
            padding-bottom: 10px;
        }
    }

/* Site Footer
 * ============================================== */

.footerFloatOuter {
	width: 100%;
	float: none;
    }

.footerFloatInner1 {
	width: 100%;
	float: none;
        text-align: center;
	margin-left: 10px;
    }

.footerFloatInner2 {
	width: 100%;
	float: none;
        text-align: center;
    }

.footer {
        min-height: 300px;
        background-color: #696969;
        padding-bottom: 3em;
        padding-top: 6em;
        margin: auto;
	font-family:system-ui,-apple-system,"Segoe UI",Roboto,Helvetica,Arial,sans-serif;
        font-size:calc(0.75em + 0.25vw) !important;
        font-weight:300;
        line-height:1.6 !important;
        // font-size: 12px;
        // font-family: Open Sans;
        color: #FFF;
	text-transform: uppercase;
        // font-weight: bold;
               
        @media screen and (min-width: 800px) {
            
            .footerFloatInner1 {
	          width: 20%;
	          float: left;
		  align: left;
		  margin-left: 0px;
            }
            .footerFloatInner2 {
	          width: 20%;
	          float: left;
		  text-align: left;
            }
		
            .footerFloatOuter {
	          width: 30%;
	          float: left;
            }      
        } 
}

.footer ul li {
	font-family:system-ui,-apple-system,"Segoe UI",Roboto,Helvetica,Arial,sans-serif;
        font-size:calc(0.75em + 0.25vw) !important;
        font-weight:300;
        line-height:1.6 !important;
        color: #FFF;
	text-transform: uppercase;
	// text-align: left;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}




/* Individual Posts
 * ============================================== */
    .page-content {
        padding: $spacing-unit 0;
        text-align: justify;
    }

    .page-heading {
        font-size: 20px;
        padding-top: 2px;
    }

/* Archive
 * ============================================== */
    .post-list {
        margin-left: 0;
        list-style: none;

        > li {
            display: block;
            padding: 0.1em 1.5em;
        }

    }

    .post-link {
        font-family: 'Open Sans';
        font-weight: 300;
        font-size: 1.5em;
        letter-spacing: -1px;
        color: #454545;
        display: block;
        width: 100%;

        @include media-query($on-palm) {
            font-size: 1.33em;
        }
    }

    .post-meta {
        font-size: $small-font-size;
        color: $grey-color-light;
        text-transform: uppercase;
        display: inline-block;
    }

/* Post Format
 * ============================================== */
    .post-header {
        margin-bottom: $spacing-unit;
    }

    .post-title {
        font-size: 42px;
        letter-spacing: -1px;
        line-height: 1;

        @include media-query($on-laptop) {
            font-size: 36px;
        }
    }

    .post-content {
        margin-bottom: $spacing-unit;
        /*
        h2 {
            font-size: 32px;

            @include media-query($on-laptop) {
                font-size: 28px;
            }
        }

        h3 {
            font-size: 26px;

            @include media-query($on-laptop) {
                font-size: 22px;
            }
        }

        h4 {
            font-size: 20px;

            @include media-query($on-laptop) {
                font-size: 18px;
            }
        } */
    }

</style>  


<br>


