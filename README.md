# Fordham Java coursework

Java projects from my computer science classes at Fordham University.

## Student records

`Student.java`, `CollegeStudent.java`, `HighSchoolStudent.java`, `Course.java`, `StudentBuild.java`, `StudentTest.java`

Classes for students and courses, from two different labs. `Student` keeps class-wide details in static fields and gives every student an auto-incremented ID. `CollegeStudent` and `HighSchoolStudent` extend it, and `StudentTest` stores both kinds in one `Student[]` array to show polymorphism. `StudentBuild.java` is the earlier lab and carries its own copy of `Student`, so compile it on its own.

`StudentTest` calls course methods (such as `addCourse`) from a later version of `Student.java` that isn't in this repo, so it doesn't compile as is.

## CSV analytics

`Analytics.java`, `AnalyticsUser.java`

Reads a CSV file into a 2D array, converts the values to numbers, and reports count, sum, average, median and mode for each row. The input path in `AnalyticsUser.java` points to a file on my old laptop and the dataset isn't included, so change `filename` to run it.

## Word sorter

`arraySort.java`

Reads three or more words from the console, splits them on whitespace and sorts them alphabetically.

## Running

Each program compiles separately:

```
javac arraySort.java && java arraySort
javac StudentBuild.java && java StudentBuild
javac Analytics.java AnalyticsUser.java && java AnalyticsUser
```
