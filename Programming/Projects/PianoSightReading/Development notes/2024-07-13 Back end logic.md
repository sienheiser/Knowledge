I feel like crap today. I am not in the mood to code all the logic for displaying sheet music. Instead I will work on trying to integrate the chord lessons and see how to track the data.

Let us define the problem. I want to track data about **lessons**. What is a lesson? A lesson displays a number of chords and the student presses those chords.

## Idea 1 Simplest scheme
We track the displayed chord and the time it took to press that chord. E.g. if the student does not press the right keys of the chord then the timer keeps ticking until the student presses the correct keys.

If we model a lesson as a record and the lesson has $n$ chords then we need $2n$ fields for that record. Our lessons can have varying number of chords that means our records will have varying number of fields. 

### Gathering statistics
The most basic stat is the average time it takes to press each. If we had such an architecture it is hard to find the chord across all the fields. It is more convenient to search one fields. So I do not like this structure

## Idea 2 Tracking each note
Suppose we make a table with all the possible notes on a piano. It would have three fields a row id, character_display_sharp, character_display_flat.

let there be a lessons table where the first field of the table is a lesson id, the second fields counts the number of chords that were displayed and the third field counts the number of chords that were correctly pressed on the first try.

Then let there be each 88 other tables one for each note. In each table the first field will be a rowid the second a lesson id  and the third the time it took to press that key. 

To gather statistics in this case is easy we just go to one of the notes table and get the average time.