<<<<<<< HEAD
#Readme for workflow of Unix assignment
#This document contains the step by step protocol that Joe Webb followed to analyze this SNP data and orient it to a file structure following this format:

Column 1 = SNP ID
Coulmn 2 = Chromosome Number
Column 3 = Base Pair Position
Column 4..N = Genetic Data for each subject. 

First I used mkdir to create this Git repository
Then I used cd to move into it and I used touch to create this document
Then I used nano to edit this document

=======
# Git
>>>>>>> 2fe619d293b2e6c28505d5d7470d3f3bee9e732c

Then I used git init
then git add . #to add all items in dir to git
then I typed git commit

Then I logged into github, made my new repository
then I typed git remote add origin git@github.com:joelwebb/Git
typed in my account name and password
Next, I coppied all of the unix exercise documents into my repository.

Then I used git push origin master to update my repo.

Then I used grep to pull out each of the three genotype groups of Maize and Teosinte and generated new textfiles. 

Then I used cat to generate a combined file and placed the Maize genotypes and Teosinte genotype files into respective folders

Then I pulled out the first row as a header using the head function and then I used a simple cat function to combine them all with a header.

Then I used this command:
(head -n 1 Maize_genotypes.txt && tail -n +1 Maize_genotypes.txt| sort -n -k 1) > Sorted_Maize_genos.txt
to sort everything inside of the txt files without sorting through the header to yield a sorted genotype file. 

I did this process for both Maize and Teosinte and then I used AWK to transpose the genotypes and recombine a new column into the file.

Then I used join to join my genotype files with the chromosome number and bp location for each SNP. 

Then I used the git add . command to add everything to the git que.
Then I used git commit to write myself a message that I was adding everything back to my folder

Then I used the git push origin master command to push it all to my repository on github.

Then I copied each of the joined full genotype files into their own directories and used GREP to split according to each chromosome

Then I copied the set into  dashes folder and another copy into questionmarks. 

In the dashes folder I used a sed command (sed -ie 's/\?/\-/g') to replace all questionmarks with "-"

Then I repeated this process for Maize after completing it for Teosinte.

Then I used awk to pull out each cromosome and generate new files in an orderly manner with the code ( awk '$2 == 2 { print $0 }' Test_join.txt > Sample_Chr2.txt).

Then I used the git add . command to add everything to the git que.

Then I used git commit to write myself a message that I was adding everything back to my folder

Then I used the git push origin master command to push it all to my repository on github.

Finally, I realized that for the Teosite data had an extra column, so I used awk to remove the column. 

Then I re ran git and uploaded my final project.
