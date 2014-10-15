Reproducible Research
by Roger D. Peng, PhD, Jeff Leek, PhD, Brian Caffo, PhD

Introduction

It is now possible to collect a large amount of data about personal movement using activity monitoring devices such as a Fitbit, Nike Fuelband, or Jawbone Up. These type of devices are part of the “quantified self” movement – a group of enthusiasts who take measurements about themselves regularly to improve their health, to find patterns in their behavior, or because they are tech geeks. But these data remain under-utilized both because the raw data are hard to obtain and there is a lack of statistical methods and software for processing and interpreting the data.

This assignment makes use of data from a personal activity monitoring device. This device collects data at 5 minute intervals through out the day. The data consists of two months of data from an anonymous individual collected during the months of October and November, 2012 and include the number of steps taken in 5 minute intervals each day.
Data

The data for this assignment can be downloaded from the course web site:

    Dataset: Activity monitoring data [52K]

The variables included in this dataset are:

    steps: Number of steps taking in a 5-minute interval (missing values are coded as NA)

    date: The date on which the measurement was taken in YYYY-MM-DD format

    interval: Identifier for the 5-minute interval in which measurement was taken

The dataset is stored in a comma-separated-value (CSV) file and there are a total of 17,568 observations in this dataset.
Assignment

This assignment will be described in multiple parts. You will need to write a report that answers the questions detailed below. Ultimately, you will need to complete the entire assignment in a single R markdown document that can be processed by knitr and be transformed into an HTML file.

Throughout your report make sure you always include the code that you used to generate the output you present. When writing code chunks in the R markdown document, always use echo = TRUE so that someone else will be able to read the code. This assignment will be evaluated via peer assessment so it is essential that your peer evaluators be able to review the code for your analysis.

For the plotting aspects of this assignment, feel free to use any plotting system in R (i.e., base, lattice, ggplot2)

Fork/clone the GitHub repository created for this assignment. You will submit this assignment by pushing your completed files into your forked repository on GitHub. The assignment submission will consist of the URL to your GitHub repository and the SHA-1 commit ID for your repository state.

NOTE: The GitHub repository also contains the dataset for the assignment so you do not have to download the data separately.
Loading and preprocessing the data

Show any code that is needed to

    Load the data (i.e. read.csv())

    Process/transform the data (if necessary) into a format suitable for your analysis

What is mean total number of steps taken per day?

For this part of the assignment, you can ignore the missing values in the dataset.

    Make a histogram of the total number of steps taken each day

    Calculate and report the mean and median total number of steps taken per day

What is the average daily activity pattern?

    Make a time series plot (i.e. type = "l") of the 5-minute interval (x-axis) and the average number of steps taken, averaged across all days (y-axis)

    Which 5-minute interval, on average across all the days in the dataset, contains the maximum number of steps?

Imputing missing values

Note that there are a number of days/intervals where there are missing values (coded as NA). The presence of missing days may introduce bias into some calculations or summaries of the data.

    Calculate and report the total number of missing values in the dataset (i.e. the total number of rows with NAs)

    Devise a strategy for filling in all of the missing values in the dataset. The strategy does not need to be sophisticated. For example, you could use the mean/median for that day, or the mean for that 5-minute interval, etc.

    Create a new dataset that is equal to the original dataset but with the missing data filled in.

    Make a histogram of the total number of steps taken each day and Calculate and report the mean and median total number of steps taken per day. Do these values differ from the estimates from the first part of the assignment? What is the impact of imputing missing data on the estimates of the total daily number of steps?

Are there differences in activity patterns between weekdays and weekends?

For this part the weekdays() function may be of some help here. Use the dataset with the filled-in missing values for this part.

    Create a new factor variable in the dataset with two levels – “weekday” and “weekend” indicating whether a given date is a weekday or weekend day.

    Make a panel plot containing a time series plot (i.e. type = "l") of the 5-minute interval (x-axis) and the average number of steps taken, averaged across all weekday days or weekend days (y-axis). The plot should look something like the following, which was creating using simulated data:

Your plot will look different from the one above because you will be using the activity monitor data. Note that the above plot was made using the lattice system but you can make the same version of the plot using any plotting system you choose.
Submitting the Assignment

To submit the assignment:

    Commit the your completed PA1_template.Rmd file to the master branch of your git repository (you should already be on the master branch unless you created new ones)

    Commit your PA1_template.md and PA1_template.html files produced by processing your R markdown file with knit2html() function in R (from the knitr package) by running the function from the console.

    If your document has figures included (it should) then they should have been placed in the figure/ directory by default (unless you overrided the default). Add and commit the figure/ directory to yoru git repository so that the figures appear in the markdown file when it displays on github.

    Push your master branch to GitHub.

    Submit the URL to your GitHub repository for this assignment on the course web site.

In addition to submitting the URL for your GitHub repository, you will need to submit the 40 character SHA-1 hash (as string of numbers from 0-9 and letters from a-f) that identifies the repository commit that contains the version of the files you want to submit. You can do this in GitHub by doing the following

    Going to your GitHub repository web page for this assignment

    Click on the “?? commits” link where ?? is the number of commits you have in the repository. For example, if you made a total of 10 commits to this repository, the link should say “10 commits”.

    You will see a list of commits that you have made to this repository. The most recent commit is at the very top. If this represents the version of the files you want to submit, then just click the “copy to clipboard” button on the right hand side that should appear when you hover over the SHA-1 hash. Paste this SHA-1 hash into the course web site when you submit your assignment. If you don't want to use the most recent commit, then go down and find the commit you want and copy the SHA-1 hash.

A valid submission will look something like (this is just an example!)

https://github.com/rdpeng/RepData_PeerAssessment1

7c376cc5447f11537f8740af8e07d6facc3d9645

Please submit the URL pointing to your GitHub repository containing the documents for this assignment. (NOTE: Please submit the URL for the entire repository, not for any individual files.)

On a separate line, submit the SHA-1 hash identifier corresponding to the commit that contains the full submission (the identifier should be a string of 40 characters containing numbers 0-9 and letters a-f).
Evaluation/feedback on the above work
Note: this section can only be filled out during the evaluation phase.
Was a valid GitHub URL containing a git repository submitted? 

0 points: A valid GitHub URL was NOT submitted (or URL is broken) 
1 point: The submitted URL points to a GitHub repository 
Does the GitHub repository contain at least one commit beyond the original fork? 

0 points: No, there are no commits beyond the original fork 
1 point: Yes, there is at least one commit beyond the original fork 
Was a SHA-1 submitted indicating a specific commit in the GitHub repository?

0 points: No, there was no SHA-1 submitted
1 point: Yes, a SHA-1 was submitted
If a SHA-1 was submitted along with the GitHub URL, does the SHA-1 correspond to a specific commit in the repository?

0 points: No, there is no commit in the repository corresponding to that SHA-1
2 points: Yes, there is a commit in the repository corresponding to that SHA-1
Overall evaluation/feedback
Note: this section can only be filled out during the evaluation phase.
Examine the submitted assignment PA1_template.md markdown file. Go to the specific version of the repository that corresponds to the SHA-1 submitted with the assignment. If no SHA-1 was submitted, go to the most recent commit in the repository.

Does the submission show code for reading in the dataset and/or processing the data?

0 points: There is no code presented for reading in the dataset
1 point: There is code presented for reading in the dataset
Does the submission contain a histogram of the total number of steps taken each day?

0 points: No, there is not histogram of the total number of steps taken each day
1 point: Yes, there is a histogram of the total number of steps taken each day
Are both the mean and median number of steps taken each day reported?

0 points: Neither the mean nor the median number of steps is reported (both mean and median must be reported or else 0 points are awarded)
1 point: Both the mean and median are reported
Is there a time series plot of the average number of steps taken (averaged across all days) versus the 5-minute intervals?

0 points: There is no plot included, or the included plot appears incorrect
1 point: A time series plot is included and it appears correct
Does the report give the 5-minute interval that, on average, contains the maximum number of steps?

0 points: No, the 5-minute interval containing the maximum number of steps is not reported
1 point: Yes, the 5-minute interval containing the maximum number of steps is reported
Does the report describe and show with code a strategy for imputing missing data?

0 points: No, there is no description of an imputation strategy for missing data
1 point: Yes, there is a description of a strategy for imputing missing data
Does the report contain a histogram of the total number of steps taken each day after missing values were imputed?

0 points: No, there is no histogram of the total number of steps taken each day after missing values were imputed
1 point: Yes, the histogram is present in the report.
Does the report contain a panel plot comparing the average number of steps taken per 5-minute interval across weekdays and weekends?

0 points: No, there is no panel plot
1 point: Yes, there is a panel plot
Does the report show all of the R code needed to reproduce the results (numbers, plots, etc.) in the report?

0 points: The report does not contain any R code
1 point: The report contains R code for **some** of the results presented
2 points: The report contains R code for **all** of the results presented
Use this space to provide constructive feedback to the student who submitted the work. Point out both strengths and weaknesses in the submission and provide advice about how the work could be improved in the future.
