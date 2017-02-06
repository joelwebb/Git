<<<<<<< HEAD
#Readme for workflow of Unix assignment

First I used mkdir to create this Git repository
Then I used cd to move into it and I used touch to create this document
Then I used nano to edit this document

Then
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

Then I used grep to pull out each of the three genotype groups of Maize and Teosinte and placed into respective folders

Then I pulled out the first row as a header using the head function and then I used a simple cat function to combine them all with a header.

Then I used this command:
(head -n 1 Maize_genotypes.txt && tail -n +1 Maize_genotypes.txt| sort -n -k 1) > Sorted_Maize_genos.txt
to sort everything inside of the txt files without sorting through the header to yield a sorted genotype file. 

I did this process for both Maize and Teosinte and then I used AWK to transpose the genotypes and recombine a new column into the file.

Then I used join to join my genotype files with the chromosome number and bp location for each SNP. 

