# APIdesign

## noSQL Schema
![image](https://user-images.githubusercontent.com/63236951/144217697-a2fdb44c-871a-4666-9f01-887fe23902d8.png)

Our database is here to store your addresses and family members, so anyone can know where you live! Yay!

## Actions you can do here
### Post
* /people/new to post who you are and any houses you own!
* /people/:id/house/new to add a new house so everyone can visit you!

### Get
This is where you get to look up your friends (or enemies...)
* /people - this will return an array of all people objects.
* /people/:id - this will show you the person you're looking for, returning an object.
* /people/:id/:postcode - this shall tell you all the places they live at, as an array of house objects.
* /:neighbourhoodPostcode/:ageBracket/:householdSize - this will return an array of all people in your postcode in the given age bracket and with the given household size.

#### Variables
* id: the unique id of the person.
* neighbourhoodPostcode: the first 4 letters of a postcode, e.g. EX11.
* ageBracket: e.g. "18-24".
* householdSize: the size of the household, e.g. 5.
