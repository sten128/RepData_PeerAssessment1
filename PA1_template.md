# Reproducible Research: Peer Assessment 1


###REMARK:
**To perform this analysis ggplot2 library is required

## Loading and preprocessing the data


```r
activity<-read.csv("activity.csv")

stepsday<-aggregate(activity$steps ~ activity$date, data=activity, sum)

names(stepsday)<-c("date", "totalsteps")
```


## What is mean total number of steps taken per day?


```r
meanpday<-mean(stepsday$totalsteps)

medianpday<-median(stepsday$totalsteps)

meanpday
```

```
## [1] 10766.19
```

```r
medianpday
```

```
## [1] 10765
```



## What is the average daily activity pattern?



## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?
