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
            * Show them [this code](https://gist.github.com/petervanwesep/e2c4a7201929f4bd864872e6fd574f5f) representing a single suit from a deck of cards.
            * Ask students what is represented by the variable `deck`.
        * Play the game
            * With the students' assistance, write the [gimme_a_card() function](https://gist.github.com/petervanwesep/503e33f80a5b28c33d7fcebee77fde27) to **print** a random card from the deck.
            * Get one volunteer to play the `gimme_a_card` function and another to play `randint`.
            * Use the board to write output.
            * One student from the class should "call" the function (by saying "Gimme a card!")
            * The student playing the function will in turn need to call `randint`
            * Trace through the function you wrote together.
            * Do this a few times.
        * Change the function to **return** a card instead of printing it out
            * Give a (physical) deck of sorted cards to the student playing the function, only including the cards from the programmed `deck`.
            * Have another student "call" the function, then trace through again as a class.
            * When the student reaches the `return` let them think for a moment about what they should do next.
            * If they don't figure it out, remind them that the caller of a function receives the returned value.
            * Student should hand the card to the person who called them.
        * Further exploration: How would we print out the value of the card after it is returned?
    	* Debrief the activity and talk about what was learned.
3. **Lab**
    * Given a shuffled deck list, students will create a program that plays the game 'War' with the user.

4. **Debrief**
    * Check student progress and completion of the lab, wrap up by taking any final questions.


###Accommodation/Differentiation
As an extension activity, ask students to research the shuffle function and the functions associated with it.


[Do Now]:do_now.md
[Lab - War (Card Game)]:lab.md