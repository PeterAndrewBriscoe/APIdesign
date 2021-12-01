# APIdesign

##The API
![image](https://user-images.githubusercontent.com/63236951/144217697-a2fdb44c-871a-4666-9f01-887fe23902d8.png)
Our database is here to store your addresses and family members, so anyone can know where you live! Yay!

##Actions you can do here
###Post
/people/new to post who you are!
/people/house/new to add a new house so everyone can visit you!

###Get
This is where you get to look up your friends (or enemies...)
/people/:id - this will show you the person you're looking for
/people/:id/:postcode - this shall tell you where they live
/:neighbourhoodPostcode/:ageBracket/:householdSize - this will return everyone in your neighbourhood

Id is the unique id of the person
Neighbourhood postcde is the first 4 letters of the postcode
Household size is the size of the household
