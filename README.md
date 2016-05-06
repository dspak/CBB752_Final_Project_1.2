# Fastq Quality Statistics Plots
***

Tool that generates “quality control statistics” from FastQ file.

Note: This tool is part of a set of bioinformatic and biological structure tools created for CBB752 at Yale University in the Spring 2016. The website containing links to the set of tools can be found at: <https://github.com/CBB752Spring2016/CBB752Spring2016.github.io>.

__The tool that accomplishes this task is named qualitystats.R__

***

### General
The script take one required input (name of the fastq file to be processed) and one optional input (the name of the txt file to which the filename and titles of the corresponding plots are output).  This tool creates png files of the following plots:
  
  * Distribution of Read Lengths
  
  * Per base quality score containing the median, quartiles, mean, and standard deviation
  
  * Distribution of mean quality per sequence


### Usage
  
  Usage:      Rscript qualitystats.R -i < input file > -o < output file >
  
  Examples:  
  ```
  	     Rscript qualitystats.R -i sample-input.fastq -o sample-output.txt
         Rscript qualitystats.R -i sample-input.fastq
  ```
  
### Input and Output formats
  
  Input Formats:	
                  
    -i  string of corresponding fastq file
    -o  string containing the name of the file to which the output information is saved

  Output Format:	txt file containing the file name, the number of sequences and the titles of corresponding plots

### Sample Output

Quality Score Statistics and Figure names for sample-input.fastq

Number of Sequences = 100000

For the Distribution of read lengths see: Sequence_Length_Distribution.png

![Fig1](https://github.com/peter-mm-williams/CBB752_Final_Project_1.2/blob/master/Sequence_Length_Distribution.png)

For a plot of the per base quality score see: Per_Base_Sequence_Quality.png

![Fig2](https://github.com/peter-mm-williams/CBB752_Final_Project_1.2/blob/master/Per_Base_Sequence_Quality.png)

For a plot of the distribution of mean quality per sequence see: Per_Sequence_Mean_Quality_Distribution.png

![Fig3](https://github.com/peter-mm-williams/CBB752_Final_Project_1.2/blob/master/Per_Sequence_Mean_Quality_Distribution.png)

