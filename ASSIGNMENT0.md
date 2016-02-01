**ASSIGNMENT 0 - SRT 411**
==========================

Student Information :

-   Github name : mooven
-   Name : Mooven Soobaroyen
-   Student No : 042-853-143

**Introduction**
================

In this assignment, I will be creating a document using knitr to publish
my report for assignment 1 on Github. I used Rstudio to write my code.
This assignment contains all the ToDos in the "short introduction to R".
I will be doing them in order as per the link provided.

**ToDo**
========

**- `ToDo 1` **

This is the first ToDo which consists of calculating the percentage of
my life I have spent at college. The current year is 2016, I started
college in 2014 and I was born in 1995. The percentage is calculated as
shown:

    ((2016-2014)/(2016-1995))*100

    ## [1] 9.52381

As shown above by the calculation, we can see that the percentage I have
spent at college of my life is 9.52381%.

**- `ToDo 2` **

Here I will be calculating the percentage of my life I have spent at
college just as the one above, but this time I will be using variables.

    UniYear = (2016-2014) #Defining the numbers of years I have spent at school as UniYear
    MyAge = (2016-1995) #The variable MyAge is for my age
    Percentage = ((UniYear/MyAge) * 100) #Percentage is the variable to give the percentage
    Percentage #calling the variable 

    ## [1] 9.52381

As you can see the answer is the same. It is just this time we are
making use of variables.

**- `ToDo 3` **

Here we will be creating a vector with the numbers 4,5,8 and 11. We will
then proceed to calculate the sum of the vector.

    x=c(4, 5, 8, 11) #saving the vector as a variable called x
    sum(x)

    ## [1] 28

The sum of the vector is 28 as shown above which is 4 + 5 + 8 + 11.

**- `ToDo 4` **

We will now generate 100 random numbers using the function rnorm and
plot the 100 numbers on a graph.

    x = rnorm(100) #saving the 100 numbers as a variable called x
    plot(x) # plotting the graph

![](SRT411-Assignment-0/unnamed-chunk-4-1.png)<!-- -->

The graph once plotted is as shown below. We will show in the later
steps how to plot graphs using different colors and different size and
symbols of coordinates.

**- `ToDo 5` **

We will now be using the help command which tells us what does a
particular function. The following example shows the help command on the
square root function (sqrt).

    help(sqrt)

**- `ToDo 6` **

In this step we will be saving the code for ToDo 4 as a script namely
'firstscript.R'. We will then be showing how to use the source command
in calling a script.

    source("firstscript.R")

![](ASSIGNMENT0_files/figure-markdown_strict/unnamed-chunk-6-1.png)<!-- -->

As shown by the results above, we can see that it plots the exact same
graph as ToDo 4 as the content of 'firstscript.R' is the same as the
code in ToDo 4.

**- `ToDo 7` **

Here I will be creating a vector called 'P' which consists of numbers
starting from 31 to 60 that is altogether 30 numbers. I will then create
a matrix with it and save it in a variable namely 'Q'. The matrix will
be consisting of 6 rows and 5 columns. The code is as shown below.

    Q = matrix((P = seq(from=31, to=60, by=1)), nrow=6, ncol=5)
    Q # calling the variable Q that is the matrix

    ##      [,1] [,2] [,3] [,4] [,5]
    ## [1,]   31   37   43   49   55
    ## [2,]   32   38   44   50   56
    ## [3,]   33   39   45   51   57
    ## [4,]   34   40   46   52   58
    ## [5,]   35   41   47   53   59
    ## [6,]   36   42   48   54   60

The matrix is as shown above consisting of 6 rows and 5 columns.

**- `ToDo 8` **

In this step I will be creating 3 vectors (x1, x2 and x3), each of them
of length 100. I will then call them. In addition, I will create a data
frame with a (a = x1), b (b = x1 + x2) and c (c = x1 + x2 + x3). I will
save the data frame as a variable called 't'. I will proceed to plot 't'
and calculate the standard deviation.

    #Create the 3 vectors x1,x2 and x3 of length 100
    x1 = c(rnorm(100))
    x2 = c(rnorm(100))
    x3 = c(rnorm(100))
    #Calling the vectors
    x1

    ##   [1]  1.3528455631  1.1784143914  0.8984158991  0.6337413303  0.3676727285
    ##   [6]  1.1336579440 -0.7670781162  0.1207035482  0.0337388314  1.0261164383
    ##  [11]  0.8126044739 -1.1809505847 -0.1582879978 -0.1715543687  1.6455885527
    ##  [16]  0.5590297111 -1.0876480937 -1.3270595717  0.3702692708 -0.3026316227
    ##  [21] -1.5640487940 -0.0871977922 -0.4171684127  0.0690611098  1.4828056154
    ##  [26]  0.7237709143  0.5403606399  0.2654888071  0.2990343647  0.0401956671
    ##  [31]  0.2329653168  0.2886010061 -2.3032259418  0.8816253819 -0.7836404540
    ##  [36]  0.2293309575 -0.2512436999  0.0760864763  1.1729526265  0.4070728875
    ##  [41] -0.7012398091 -0.8738935720 -0.9920961135 -1.5059285629  0.1590805086
    ##  [46] -0.0105936313  1.5382405105  0.7145666862 -0.0609973671  0.6163249610
    ##  [51] -0.9272017147  0.3061776017  0.4661643773 -1.3563966075  0.8390134271
    ##  [56]  0.5861640196  2.9973749558 -0.0182126133  0.3991913551  0.7408541809
    ##  [61] -0.3780474445 -0.1166336794 -0.1394697318  1.6739756949 -1.4353399253
    ##  [66] -0.3901959969  3.3974522258 -0.7117067544 -1.2130764982 -0.4357352432
    ##  [71]  0.1587115952  2.4726553425  0.8587709044 -0.6409439293 -0.4024231150
    ##  [76] -0.5721665247 -0.7666997614  0.6134361490  1.0745340291  0.7729650890
    ##  [81]  0.2023276541  0.7975743431 -0.1752939788 -1.7802241520 -0.1902183731
    ##  [86] -0.4636142749  1.4640714988 -1.1072091417 -0.0914069796  0.0002975789
    ##  [91] -1.1577545061  0.4332670923  0.8474535206  0.4563381411 -0.3879912482
    ##  [96] -1.5186700201 -0.3857651744 -0.0358349610  1.6940413819  0.3849257515

    x2

    ##   [1]  0.21336918  0.77115398  2.11709807 -1.35050719 -1.12315164
    ##   [6] -0.90148880  0.32651860 -0.48136015 -1.76215951 -0.89885216
    ##  [11] -2.88569903 -0.15384334  0.04089840  0.36657554  1.62071146
    ##  [16] -1.37264676  0.04320298 -0.46640249  0.59580381  0.90611960
    ##  [21]  0.25781234  0.92592497  1.18818984  0.29903853  0.90424377
    ##  [26]  0.05258338  0.02799478 -0.62570910  0.57662401  0.05791369
    ##  [31]  0.14848602  0.10620486  0.12389102  0.29609774 -0.39796196
    ##  [36] -1.67798224  0.28407493  1.45688648 -0.73476507 -0.79324825
    ##  [41] -0.68923781 -0.46520099  0.39349700  1.11563554 -0.74782049
    ##  [46] -0.72683090 -0.88394347  0.76135303  0.06279650  1.98136562
    ##  [51] -0.78012481 -0.85542701  0.80801467  1.43319110  1.05060029
    ##  [56]  1.79398486 -1.22295434 -1.39095649  0.29397219 -0.17146185
    ##  [61] -0.89787488  0.53235094 -0.89820946  0.94975137 -0.08799666
    ##  [66] -1.07780265 -0.74681825 -1.33169772 -0.30380795  1.50999858
    ##  [71]  0.23142015  0.45286780  0.03468987  0.88824001 -0.44881794
    ##  [76]  1.08615369  0.30034448 -0.27411379  1.01845448  0.13454223
    ##  [81] -0.58688983 -0.03887064  0.89754738  0.12125731 -0.09630185
    ##  [86]  0.35649035  0.45442756  0.08381513 -1.42049061 -0.21387115
    ##  [91]  0.05559621  1.63277074 -0.15064410  1.63675571  1.13358647
    ##  [96] -2.24754328 -0.61658954 -0.07345672 -0.81740132 -1.26082079

    x3

    ##   [1] -0.079391910  0.679206253 -0.451959924  0.323534418  1.137975158
    ##   [6]  1.265307588 -0.297857727  0.912561865  0.170075130  0.913190035
    ##  [11]  0.313974065 -1.083456400  0.778964787  0.216900173 -0.638778233
    ##  [16]  1.745344165  1.703535715  1.373488201  0.182817958  1.076659977
    ##  [21] -1.139657684 -1.212798598 -0.604193562 -0.615146415  0.223137621
    ##  [26] -0.258458471  0.358415711 -0.263876129 -0.736076685 -0.467186322
    ##  [31] -0.387154736 -0.968996567  0.913214835  0.441857771 -0.716571622
    ##  [36] -0.081312045 -0.137727893  0.449114101 -1.556559594  0.576438098
    ##  [41]  0.554833885 -0.909140695 -0.261647643  0.442543284 -0.081881017
    ##  [46] -0.434765926 -0.185690103  0.631133795  0.566500149 -1.025814124
    ##  [51]  0.657132426 -0.253442190  0.032123482  0.602280545 -0.490611868
    ##  [56] -0.457609310  0.001678880  1.528897322  1.788192992 -0.515667530
    ##  [61] -0.005578035 -0.895082311  2.486532216  0.200659949 -1.721359524
    ##  [66] -0.130391031  0.834655142  0.809481580 -2.806211781  1.011443284
    ##  [71] -0.910782678  1.293638240  1.104649854 -0.542955546 -1.055121383
    ##  [76]  0.341685860 -0.651906685 -0.565272715  0.827232601  0.794338411
    ##  [81] -0.817094881 -0.727797352 -1.396857186  0.601355500 -0.200543120
    ##  [86] -1.790311022 -0.628911101 -1.474163613  0.548691842 -0.361222293
    ##  [91]  0.363387419 -1.607091656 -0.300284071  0.810788875  0.273432816
    ##  [96] -0.012670659 -1.280770384 -1.157984483  1.913316860 -0.406340437

    #create a data frame with 3 columns
    t = data.frame(a = x1, b = x1+x2, c = x1+x2+x3)
    plot(t)

![](ASSIGNMENT0_files/figure-markdown_strict/unnamed-chunk-8-1.png)<!-- -->

**- `ToDo 9` **

Here I will be adding the following lines to the previous ToDo. Check
the following:

    plot(t$a, type="l", ylim=range(t),
    lwd=3, col=rgb(1,0,0,0.3))
    lines(t$b, type="s", lwd=2,
    col=rgb(0.3,0.4,0.3,0.9))
    points(t$c, pch=20, cex=4,
    col=rgb(0,0,1,0.3))

I will now by explaining the meaning of rgb, lwd, pch and cex.

-   rgb

rgb stands for Red, Blue and Green. It gives an idea of what color you
want the graph to be and playing with the intensity of the colors, you
can create the color of your choice. The last argument is for the
intensity of the line.

-   lwd

Lwd is the thickness of the line. The higher the value, the thicker the
line.

-   pch

pch (graphic symbol) is the sign of the plot we use to plot the change.
Different number is for different shapes of plots such as circles,
triangles, cross etc.

-   cex

cex (size of pixel) is the size of the coordinates. The higher the
number, the bigger the coordinates.

**- `ToDo 10` **

I created a file in notepad called tst1.txt as shown by the picture
provided with the matrix consisting of 3 columns and 6 rows.

I will then create a script to read it the file and multiply the column
'g' by 5 and store the result in a file named as tst2.txt.

     d = data.frame(a = c(1,2,4,8,16,32), 
                   g = c(2,4,8,16,32,64),
                   x = c(3,6,12,24,48,96))
    #saving the matrix in a file named as tst1.txt
    write.table(d,file="tst1.txt", row.names=FALSE)
    #creating a script to call it 
    read.table(file="tst1.txt", header=TRUE)

    ##    a  g  x
    ## 1  1  2  3
    ## 2  2  4  6
    ## 3  4  8 12
    ## 4  8 16 24
    ## 5 16 32 48
    ## 6 32 64 96

As you can see above it prints the matrix.

    #multiplying the 'g' column by 5
    d[2] = d[2]*5
    #saving the results as a text file named as tst2.txt
    write.table(d,file="tst2.txt", row.name=FALSE)

**- `ToDo 11` **

Here I will be calculating the square root of 100 randomly generated
numbers.

    sqrt(rnorm(100))

    ## Warning in sqrt(rnorm(100)): NaNs produced

    ##   [1]       NaN       NaN       NaN 0.2871820 0.3034987 0.8032293       NaN
    ##   [8] 0.6161814       NaN 1.0388966       NaN       NaN       NaN 0.6339222
    ##  [15] 0.8029803       NaN       NaN       NaN 0.5270194 0.1740938 0.8721307
    ##  [22]       NaN 0.9122690       NaN 0.6052778 1.2740489 1.3503688 1.0892865
    ##  [29]       NaN 1.3098542 0.3498507 0.5335532 0.5639094       NaN 1.3096167
    ##  [36]       NaN 0.5637257       NaN 0.2854836 1.0402789       NaN 0.2708514
    ##  [43]       NaN 0.4200843 0.2696455 0.5090004 0.1745294       NaN 1.2925700
    ##  [50]       NaN       NaN       NaN 0.7219103       NaN       NaN 1.2337369
    ##  [57] 0.7511589       NaN       NaN       NaN       NaN 1.0990145       NaN
    ##  [64]       NaN       NaN 1.0489848 0.6457599       NaN 0.4546785 0.8172287
    ##  [71]       NaN       NaN 1.1208618       NaN       NaN       NaN       NaN
    ##  [78] 0.8471739       NaN       NaN       NaN       NaN 0.4697357       NaN
    ##  [85] 1.2578337 0.8375753       NaN 1.2755098       NaN       NaN 0.8937119
    ##  [92]       NaN 0.6763192 0.4407516       NaN 0.7348908 0.6115596       NaN
    ##  [99] 0.8744744 1.1439530

As you can see it gives a warning saying that NaNs are produced. NaN
stands for not a number. It usually means that the output number is a
complex number that is it is an imaginary number.

**- `ToDo 12` **

We will now be making a graph with on the x-axis: today, Sinterklaas
2014 and your next birthday and on the y-axis the number of presents you
expect on each of these days. We will be making two vectors first as
shown below and plot the graph as shown below:

    year = strptime(c("20141205", "20150509"),format="%Y%m%d")
    No_of_presents = c(2,7)
    plot(year, No_of_presents)

![](ASSIGNMENT0_files/figure-markdown_strict/unnamed-chunk-12-1.png)<!-- -->

**- `ToDo 13` **

We will be making a vector from 1 to 100. A for-loop will also be in
place which runs through the whole vector. Elements which are smaller
than 5 and larger than 90 will be multiply by 10 and the other elements
with 0.1. Look at the code below to get an idea of how the code looks
like.

    f = seq(from=1, to=100) # creating a vector called 'f' with numbers ranging from 1-100
    for (i in 1:100)
    {
      if (f[i] < 5 | f[i] > 90)
      {
        f[i] = f[i] * 10
      }
      else
      {
        f[i] = f[i] * 0.1 
      }
    }

**- `ToDo 14` **

Here we will be writing the function for the previous ToDo but using an
argument so that we can feed it any vector you like. We will also be
using a for-loop in the function to do the computation with each
element. We will use the standard R function length in the specication
of the counter.

    vector = function(arg1)
    {
      for (i in 1:length(arg1))
      {
        if (arg1[i] < 5 | arg1[i] > 90)
        {
          arg1[i] = arg[i] * 10
        }
      else 
        {
          arg1[i] = arg1[i] * 0.1
        }
      }
    }

**- `ToDo 15` **

Here we will be doing the same ToDo as the previous one but without a
for-loop. We will only be using if and else statements. The code is as
follows.

    vector = c(1:100)
    ifelse(vector < 5 | vector > 90, vector * 10, vector * 0.1)

    ##   [1]   10.0   20.0   30.0   40.0    0.5    0.6    0.7    0.8    0.9    1.0
    ##  [11]    1.1    1.2    1.3    1.4    1.5    1.6    1.7    1.8    1.9    2.0
    ##  [21]    2.1    2.2    2.3    2.4    2.5    2.6    2.7    2.8    2.9    3.0
    ##  [31]    3.1    3.2    3.3    3.4    3.5    3.6    3.7    3.8    3.9    4.0
    ##  [41]    4.1    4.2    4.3    4.4    4.5    4.6    4.7    4.8    4.9    5.0
    ##  [51]    5.1    5.2    5.3    5.4    5.5    5.6    5.7    5.8    5.9    6.0
    ##  [61]    6.1    6.2    6.3    6.4    6.5    6.6    6.7    6.8    6.9    7.0
    ##  [71]    7.1    7.2    7.3    7.4    7.5    7.6    7.7    7.8    7.9    8.0
    ##  [81]    8.1    8.2    8.3    8.4    8.5    8.6    8.7    8.8    8.9    9.0
    ##  [91]  910.0  920.0  930.0  940.0  950.0  960.0  970.0  980.0  990.0 1000.0
