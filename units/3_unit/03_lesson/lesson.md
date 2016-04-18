# Lesson 3.03: Return vs Print

##Learning Objectives
Students will be able to...
* Define and identify: **return, none, void**
* Explain and demonstrate the difference between printing and returning

##Materials/Preparation
* [Do Now]
* [Lab - War (Card Game)]
* Read through the do now, lesson, and lab so that you are familiar with the requirements and can assist students.
* Note that this lesson may take two days.

## Pacing Guide
| **Duration**   | **Description** |
| ---------- | ----------- |
| 5 Minutes  | Do Now      |
| 10 Minutes | Lesson      |
| 35 Minutes | Lab         |
| 5 Minutes | Debrief  |
| **Day 2**  |             |
| 10 Minutes | Recap & Review     |
| 40 Minutes | Finish Lab  |
| 5 Minutes | Debrief  |

## Instructor's Notes
1. **Do Now**
    * Students experiment with a function that returns a value, but they must add a print command to output that value.
2. **Lesson**
    * Ask students about what they think the difference between returning and printing is.
        * Get a volunteer to describe how they rewrote the code in the Do Now to get a value output.
        * Ask a student to write the code on the board.
    * Discuss the concept of the function contract again, explaining that the functions we will work with have both inputs and outputs.
    * Returning is a concept in Snap!, just with a different name: reporting.
        * ![BJC Reporint](http://bjc.berkeley.edu/bjc-r/img/building-blocks/max-code-buggy.png)
    * If students appear to be struggling with the return vs. print concept, try this activity:
        * Introduction to "Gimme a Card" Activity
            * Show the students [this code](https://gist.githubusercontent.com/petervanwesep/e2c4a7201929f4bd864872e6fd574f5f/raw/2dc98f880dd423d974d9d7a7a5e4144cd78e2134/lesson_3_03.py) representing a single suit from a deck of cards.
            * Ask students what is represented by the variable `deck`.
        * Play the game
            * With the students' assistance, write the [gimme_a_card() function](https://gist.githubusercontent.com/petervanwesep/503e33f80a5b28c33d7fcebee77fde27/raw/5f37b0a36cad8703a915a99cc05e30ca4d4caff7/lesson_3_03.py) to **print** a random card from the deck.
            * Get one volunteer to play the `gimme_a_card` function and another to play `randint`.
            * Give a (physical) deck of sorted cards to the student playing the function, only including the cards from the programmed `deck`.
            * One student from the class should "call" the function (by saying "Gimme a card!")
            * The student playing the function will in turn need to call `randint`
            * Trace through the function you wrote together, using the board/projector to write down output.
            * Repeat two or three times.
        * Change the function to **return** a card instead of printing it out
            * Have another student "call" the function, then trace through it again as a class.
            * When the student reaches the `return` let them think for a moment about what they should do next.
            * If they don't figure it out, remind them that the **caller** of a function receives the returned value.
            * Student should then hand the card to the person who called them.
        * Further exploration: How would we print out the value of the card after it is returned?
        * Debrief the activity and talk about what was learned.
        * Optional: **Follow-up Lab**
            * Using [this code](https://gist.githubusercontent.com/petervanwesep/451de0a3b37d8cde94b7515b8930d425/raw/a915433cd4081d34fe8525df7a838b6769ad200e/gistfile1.txt), implement the following two functions:
                * `gimme_a_suit` should require no input and should randomly return one of the four possible suits.
                * `gimme_a_card_value` should require no input and should randomly return one of the 13 possible card values.
            * Rewrite the `gimme_a_card` function to use these two new functions.
            * **Hint:** You won't need the old deck anymore, but the rest of `gimme_a_card` could be useful in writing your new functions.
            * Further exploration: Write a method `gimme_a_list_value` that takes a list and returns a random element from that list. Re-write `gimme_a_suit` and `gimme_a_card_value` to use this new function.

3. **Lab**
    * Given a shuffled deck list, students will create a program that plays the game 'War' with the user.

4. **Debrief**
    * Check student progress and completion of the lab, wrap up by taking any final questions.


###Accommodation/Differentiation
As an extension activity, ask students to research the shuffle function and the functions associated with it.


[Do Now]:do_now.md
[Lab - War (Card Game)]:lab.md