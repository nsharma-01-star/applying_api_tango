# TangoApplyingAPIs

## Note This is a reproduction project as part of the MSR course 2021/22 at UniKo, CS department, SoftLang Team

## Names of team/students Team: Tango 
## Members: 
* Nisha Sharma (nsharma01@uni-koblenz.de) 
* Pavithree shetty (pavithreerai@uni-koblenz.de) 
* Shweta Mishra (smishra@uni-koblenz.de ) 

## Baseline study: 
### Aspect of the reproduction project: Data collection and recognition of one dependency pair

### Input data: 
The java code aims at mining git repositories with following criteria
* A repository with 100 stars and 100 commits
* A repository with more than two contributors
* A repository with  at least one source directory

### Output data: 
Collected repositories
* Please find Temp folder which contains all the output jar files for the collected repo - https://drive.google.com/drive/folders/1jn0jsFZPQl-6vnHop8-VUNA1Lmps3DD5?usp=sharing
* The csv generated can be found in the output folder - https://github.com/nsharma-01-star/applying_api_tango/tree/main/applying-apis-main/output

## Findings of replication 
### Process delta:
* Original work found 19000 repositories with at least 100 stars, we found 19878 Java git repositories with at least 100 stars.
* Original work filtered 4018 repositories with 100 stars, 2 contributors, 100 commits and one POM file, we found 4288 Java GitHub repositories with at least 100 stars and one POM file.
* 3778 out of the 4018 repositories were found to be parsable in original work, we were able to filter 3777 parsable GitHub reposotories with src/main/java.

### Output delta:
* The code crashed after it was up for close to 72 hours. However, the following csv files were generated
  *  dependencies.csv - Original work produced 43798 different dependencies out of 3542 repositories, We found 46101 different dependencies out of 3783 repositories.
  *  dependencies_with_mcrTags.csv - We found 30704 entries with mcrTags.
  *  repositories_collected.csv - We found 4288 repositories.
  *  repositories_with_dependencies.csv - We found 3783 repositories with dependencies.
  *  repositories_with_mcrTags.csv - Original work found 3532 repositories with mcrTags. We found 3766 repositories with mcrTags.

### Implementation of replication: 
* Hardware requirements: 
  * OS: Windows, Linux or MacOS 
  * Memory: 16 GB RAM recommended 
  * Processor : Core(TM) i7
* Software requirements 
  * Java 11 (Maven project) 
  * Python 3.9.6 (plotly==5.1.0, pyspark==3.1.2)
* Validation
  * One can compare the above mentioned csv files with the original work, one would infer that the work is replicated.
* Data
  * The data replication was able to produce the csv files mentioned in the output delta section along with a temp folder consisting of necessary files required for the generation of the above mentioned csv files.
