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

![](ASSIGNMENT0_files/figure-markdown_strict/unnamed-chunk-4-1.png)<!-- -->

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

    ##   [1] -0.27064998  0.09169226  0.66961861  1.28080911 -1.76691872
    ##   [6]  1.39883375 -0.84607250 -1.76131133  0.47446076  0.89602892
    ##  [11] -0.60625755  0.72716049 -1.04041844  0.32251405 -0.47216185
    ##  [16] -0.14787395  0.27995703 -0.92672461 -0.40076707  0.50065132
    ##  [21] -0.18315901 -0.09785465  0.70008871 -2.24508789 -0.67128850
    ##  [26] -0.27868952 -0.52742912 -1.74763231  0.64327644  0.01475245
    ##  [31] -0.10704345  0.81229341 -1.59223563  1.18115734 -1.19690232
    ##  [36] -0.16252258  1.17348806  0.62959015 -0.27659868  0.74095665
    ##  [41] -0.53952921 -0.23525233  1.70690878 -0.26050416 -0.78041643
    ##  [46] -0.65561880 -0.31229492 -0.94296422  0.95549727 -0.54075673
    ##  [51]  1.51612232 -0.56861731 -0.44706519 -0.88831786 -0.82277598
    ##  [56]  1.05187171  1.26545977 -0.14510460 -0.14006971  0.40108185
    ##  [61]  0.68210192  0.53697732 -0.39330882  0.49165341  0.38686638
    ##  [66]  1.11043541 -2.06247844 -1.01304738 -1.65291459 -0.98390120
    ##  [71] -0.48509257  0.51839518 -0.21970284  0.04648246 -0.22746086
    ##  [76]  0.18931126  0.46499415 -2.28940260 -0.51377816  0.24092987
    ##  [81]  1.83010072  0.67255285 -1.43393094  1.14848579  2.51927998
    ##  [86] -0.07645694  1.38852410  0.68415049 -0.16555712  1.36918005
    ##  [91]  0.08350132 -1.02814475 -0.04984004  0.71469442 -0.41821415
    ##  [96] -1.24177720  1.59792542 -0.59417735 -1.07935981  0.42729690

    x2

    ##   [1]  0.895376891 -0.006999903 -0.920397778  1.142085831  0.368725123
    ##   [6] -0.385879285 -0.062057612  0.639859994  0.717555021 -0.698674026
    ##  [11] -0.424928082 -0.393812733  1.269628532 -0.884385076 -0.134856218
    ##  [16]  1.265626864 -0.708208258 -1.124690756  1.388591010 -0.292492522
    ##  [21] -0.008024593 -0.721761827 -0.330008683  0.550443957  0.462292172
    ##  [26]  0.552006978 -1.096998461 -1.322963132 -0.120446789 -0.149208972
    ##  [31] -0.297074454 -0.890053380  0.041663968  1.743155511 -0.069357389
    ##  [36] -0.415295467  1.808349875 -0.263794790  2.094645517  0.600137052
    ##  [41]  0.159280034 -0.833145826 -0.034263726 -0.055767849  0.847302008
    ##  [46]  1.417698514 -0.751729317 -1.889221207  1.241300335 -2.294667109
    ##  [51]  0.505767683 -0.703529386 -0.608592598  2.423799395 -0.422920509
    ##  [56] -1.875358308 -1.149665130  1.472822100  0.821020439 -0.158601910
    ##  [61]  0.743278279 -0.832196692  0.649093787  0.646996717  1.156965125
    ##  [66] -1.259961346  0.318430018 -1.792887403 -0.272931206 -0.646405545
    ##  [71]  0.705641985 -0.434158935  0.402090980 -0.323450424  0.561013911
    ##  [76]  0.726224333 -0.902818633  0.648231714 -1.782043696  1.167623693
    ##  [81]  1.131925717  0.164275748  0.118048675  1.484857962  2.318815367
    ##  [86] -0.026790945  2.138412649  1.901995773 -0.396472528 -1.145420141
    ##  [91] -0.798456719  0.053838739 -0.494665502  0.076132216 -1.250874125
    ##  [96]  0.833540369  1.161839247  2.033931066 -0.986146419 -1.065994982

    x3

    ##   [1] -0.417760120 -0.746016550 -1.040435889 -0.233945866 -0.144389153
    ##   [6] -0.966254093  0.457101876  1.707063408  0.847358533  0.724957041
    ##  [11]  0.395878320  0.640741194  0.643753237 -1.142927137  0.492473085
    ##  [16]  1.389937181 -0.487401148 -0.657611972  1.320888021  0.207345237
    ##  [21] -0.588688065 -0.353458561  1.273255411 -0.167619245  1.028943809
    ##  [26] -2.006425768 -0.272698310  1.033038972 -1.009847302 -2.641135162
    ##  [31]  0.298247176 -0.826484958  1.242638025 -0.640229343 -0.420282016
    ##  [36] -0.501585042  0.937815712 -0.545680434 -0.947975458  1.265502508
    ##  [41]  0.765265678 -0.662889779 -0.521081437  2.048650951 -0.102291105
    ##  [46] -1.120402255 -0.774083574 -0.346043913  1.817036371  0.268799177
    ##  [51] -0.985421079 -0.060429522  1.211177588  0.528852933  1.290491498
    ##  [56]  1.292326893 -0.333294303 -1.269197919 -0.454590139  0.493943362
    ##  [61] -0.740660259 -0.869258274 -1.145323432  1.901070067  1.001420714
    ##  [66]  0.962038609  1.159977712 -1.551073606  0.226155536 -0.651181408
    ##  [71] -0.116205613  1.070841374  1.849819079 -0.005297623  0.206912660
    ##  [76]  0.271050903  0.365472737  0.321814205  0.331019446  1.604964437
    ##  [81]  0.539500330  1.226192710  0.854636333  0.228411778  0.512207064
    ##  [86] -0.498263444  0.931653737 -0.098383803 -0.325975678  1.042708808
    ##  [91]  1.152635778  0.733283561  0.652576179 -0.459791114 -0.878686951
    ##  [96] -1.584546348  0.944072590  0.884907315 -0.344091795  0.516285699

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

    ##   [1] 1.0811335       NaN       NaN       NaN 0.2288332       NaN 1.3796413
    ##   [8] 0.3874885       NaN 0.4237063 0.2451052 1.0611069       NaN 0.7390281
    ##  [15] 0.6692400       NaN 0.6237958       NaN 0.8498949 0.1299403 0.1378413
    ##  [22] 0.6398129       NaN 0.4694133       NaN 0.5991068       NaN 0.4119052
    ##  [29]       NaN       NaN 0.3340082 0.7154500 0.4645211 0.3877684 0.5758561
    ##  [36]       NaN 0.8866702       NaN       NaN       NaN       NaN       NaN
    ##  [43] 1.3919684       NaN 0.7396716 0.9026688 0.5361788       NaN       NaN
    ##  [50]       NaN 0.9689600 0.7220665       NaN       NaN       NaN 0.5511563
    ##  [57] 0.8425002 0.7016193       NaN 0.9625359       NaN       NaN       NaN
    ##  [64] 0.6562151       NaN 0.5277779 0.8817264       NaN       NaN 0.7392919
    ##  [71] 0.9610614 0.6697744       NaN 0.9083996 0.3572783       NaN 0.9405296
    ##  [78] 0.8528474       NaN 0.8253005       NaN       NaN 1.5023235       NaN
    ##  [85]       NaN 0.3990557 1.5856845 0.7904030 0.9783610       NaN 0.7766081
    ##  [92] 1.1624559 0.6071808       NaN       NaN       NaN 0.4671802 0.4312117
    ##  [99]       NaN       NaN

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
