# Workout-application
First application for personal use 

Take in information from user through manual entries (maybe we can update this into a more gui/check mark interface once recommendations have been made)

Take in information from user, put this document into a JSON file that can be input into Azure Cosmos (or just Mongo DB since, upgradeable into cosmos through the API) that can then be extrapolated into Azure SQL studio (or just reagular SQL DB)

ELT format for this. 

Have a feature that will recommend what exercises to do, order, and intensity. 

The order will go by what you want to improve on the most, if you want your squat to be better it will be first in the line-up. 

Intensity will be based off of initial numbers given, and how you're feeling today. (If you're feeling great recommend @ 90% of 1rpm if you're not feeling so great recommend @ 80%)

Initial user-pass with no personally identifiable authentication for testing? 



https://www.myfitnesspal.com/api 

Take food ideas from here 

https://www.eatthismuch.com/ 



# Data flow


User will give what exercises they wish to do and their baseline weights & Reps. 


# If User is a beginner 

Recommend Starting Strength 5x5

If they know some baseline information: 

Take that information and assign it a progressive overload value aiming for 5/lb's everyweek. 

If They do not know baseline:

Assign empty barbell weights and then instruct to add 10 lb's to bar for deadlift and squats until they feel that the weight's growth rate is becoming uncomfortable. 

Assign user workouts for every week, that when they complete the exercise they mark it down. If they fail on the exercise we repeat once, if they fail again we use the same values from 2 weeks ago. 

# If user is not a beginner

Ask them what exercises they would like to do, how many times a week, and what order.  Example, workout A & B would be done in order A(monday), B(wednesday), A(friday). The day of the week would not be a hard requirement, only just push them to do the next one in the order. 

Get baseline stats on their exercises chosen and start their program off like that. 

Ask user if they want to explore options of progression methods or they would like to self-pace. 

# If opt in

Educate user on different kinds of methodology for progression and have them pick. 

Initial offerings - Madcow and texas method 

# If opt out 

Use baseline for workout recommendation and allow user to edit weights done, give the highest weight as recommendation next workout. 