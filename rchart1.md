# An example




```r
library(rCharts)
#names(iris) = gsub("\\.", "", names(iris))
#a<-rPlot(SepalLength ~ SepalWidth | Species, data = iris, color = 'Species', type = 'point')


hair_eye_male <- subset(as.data.frame(HairEyeColor), Sex == "Male")
n1 <- nPlot(Freq ~ Hair, group = "Eye", data = hair_eye_male, type = "multiBarChart")
```


```r
n1
```

```
Warning: cannot open file 'assets/fig/plot.html': No such file or
directory
```

```
Error: cannot open the connection
```

```r
#print(a)
```
knit2html("rchart1.Rmd")
