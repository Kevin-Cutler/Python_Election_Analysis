# Python Election Analysis




                          # Written Analysis of the Election Audit 

    
        ## Overview of Election Audit: 
        

  The purpose of the election analysis was to help Seth and Tom submit the election audit results to the election commission. As an analyst Tom and Seth have requested my partnership in developing a Python script runreport that will be delivered to the Colorado Board of Comissions. We need to analyze a CSV file of data [election_results] (https://github.com/Kevin-Cutler/Python_Election_Analysis/tree/master/Resources) by importing it into a text editor. We will be reviewing the data in VSCode and determining the best approach to assist in developing our final overview. The task is to determine the total number of votes cast. We will output a list of candidates who received votes. The last step for Seth and Tom will include calculating the percentage of votes each candidate won and the winner of the election based on popular vote. Additionally the election commission has requested an audit to include voter turnout for each county, percentage of votes from each county out of the total count, and
  the county with the highest turnout.

              ### Inspect the data before importing CSV file into a text editor

              <img width="300" alt="CSV_SnapShot" src="https://user-images.githubusercontent.com/88467263/133942909-9255b218-d0f0-4bf4-80dd-cf1e56cf7343.PNG">

![](Resources/CSV_SnapShot.png)

In my analysis I started by importing the CSV file from Seth and Tom and loading it into VSCode (Screen Shot Above). My focus is to determine, how many columns consist in the file, what type of data I am working with and if the data needed to be converted before reading the file into VSCode. The data consist of 3 columns provided, the 1st with the ballot ID of each person who casted their vote. The 2nd column listed the county and the 3rd lists the name of each candidate. After determining that there were no unusual gaps in the data, I was able to start developing the steps to work with in my text editor.

![](Resources/Example_Code_Importing_Variable_Assignment_List_Dictonaries.png)

After loading the CSV file and reviewing the data I created variables to import the data needed based on the request. To determine the total number of votes cast I used a couple variables which assisted while I looped through the data. I relied on a total votes counter that calculated each row in the CSV file. The total number of votes calculated is 369,711 which was helpful later when determining the percentages for each candidate and county votes. I used a loop that checked each row of the dataset whle also using a variable "candidate_name= row[2]", this checked the 3rd column in the row for each candidates name. I used this variable to store the candidates names in a list "candidate_options =[ ]" to output a list of candidates who received votes. I then added the candidate names using "candidate_options.append(candidate_name)" to add the candidate names into storage for later use. I used this same technique for the county in the additional requirement of this analysis. Using a dictonary called "candidate_votes" I was able to store each counted occurence of each candidates name through "candidate_votes[candidate_name]". In the final step of my analysis for candidate vote and county votes I calculated the percentage of votes by dividing each individual sum of votes by the total overall.



_________

# The voter turnout for each county and percentage of votes from each county out of the total count.
________________________________________

![](Resources/County_Votes.png)

_____________________
# The county with the highest turnout
______________________

![](Resources/Largest_County_Turnout.png)

___________
# Election-Audit Results

![](Resources/SS_Counties1.png)



________________________________

                        * Total Votes Cast in This Congressional Election

_______________


#### Below is the Total votes for this election and the script used to calculate and display the Total Votes to the Terminal.
![](Resources/Total_Votes.png)

![](Resources/Example_3.png)

________
                * Breakdown of the number of votes and the percentage of total votes for each county in the precinct.
_____________
![](Resources/Largest_County_Turnout.png)

_____________
         * Denver the county with the largest number of votes
___________

![](Resources/Largest_County_Turnout.png)

____________
         * Breakdown of the number of votes and the percentage of the total votes each candidate received.
_________________


![](Resources/SS_Candidates1.png)
____
# This Script was used to calculate and print the county votes to the terminal

![](Resources/Example_3.png)

___________
* Breakdown of The Winning Candidate  
    * Winning Candidate Vote Count 
        * Winning Candidate Percentage of Total Votes
_____________

![](Resources/Winner_Candidate.png)

______
# This Script to Print The Winning Candidate Votes
![](Resources/Example_4.png)



# Election-Audit Summary: 

In summary, I think we delievered a detailed analysis that can be reused for future elections. The format of the script can be used on other reports. The script is not limited to a change in the amount of data that can be held in a file. We can leverage python lists and dictonaries to output a variety of requirements with minor changes to the script we developed. This will allow the Colorado Commision Board to make key decisions that can be supported through a customized report that can be delievered in a short amount of time. 

___
### Example 1
__________________

This new reporting resources saves time on developing reports. We can change the requirements to develop reports on elections large and small. We can make decisions at a city level to determine the percentage of citizens that are for or aganist a new bill being passed based on the voter data. This can be used to buil a better repore with citizens by quickly reporting their votes through surveys or even elections.

______

### Example 2
_________
The second example I would use for the Colorado comissions is when looking to put new businesses or schools in specific locations. Now that we have this report we can develop a report to determine the best areas to spend money to improve the community but also maximize a return for future projects.








