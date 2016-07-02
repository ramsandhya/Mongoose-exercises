# Mongoose Exercises

## Basic Schema

1. Construct a Mongoose model for the student structure that we used yesterday. Example document:

{
  name: 'DeeAnn',
  links: {
    website: 'http://www.deeannkendrick.com/',
    github: 'https://github.com/dkendrick25'
  },
  gender: 'female',
  projects: ['Rate the Throne', 'Draw Together', 'Tic Tac Toe', 'Movie App'],
  points: 7
}

2. Construct a Mongoose model for the Jazz database we used yesterday. Example document:

{
  name: 'Lee Konitz/Bob Brookmeyer in Paris',
  artist: 'Lee Konitz',
  released: 1960,
  duration: 56,
  styles: ['Cool', 'Bop']
}

3. Construct a Mongoose model for the Zip code database used yesterday. Example document:

{
    "_id" : "01007",
    "city" : "BELCHERTOWN",
    "loc" : [
        -72.410953,
        42.275103
    ],
    "pop" : 10579,
    "state" : "MA"
}

## Basic CRUD (Create, Retrieve, Update, Delete)

1. Using the student model you made in the previous section, write a Node program to create a student in the DB.
2. Write a program to find all students in the collection.
3. Write a program to find the student you created by name.
4. Write a program to update a student's points value to 15.
5. Write a program to first find that student, retrieve his ID, then remove that student in the DB by id.

## Validation

Add data validation to the student model. Making:

* name required
* links.website required
* links.github required
* gender required and can only be 'female' or 'male'

1. Try saving an object that doesn't meet the requirements. Do you get an error? Print out the detailed validation errors.
2. Save an object that does meet the requirements.

## Aggregation

Use the zipcode model you made earlier. Write a Node program that performs an aggregation query to find the top 3 most populated cities and print them out to the console.
