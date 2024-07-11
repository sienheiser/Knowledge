Yesterday I said I should focus on trying to make an objective of the piano. For the time being I will old off doing this idea.

Instead I want to generate some chords randomly. For now a tuple of numbers will represent a chord.

I have made a procedure that will 
1. Take three random keys.
2. Generate the major chords with those keys as tonic.
3. Choose an inversion for each chord randomly.

Now I really need to define a mapping because these numbers for name make sense to me.

I have defined a Piano class that contains a list with numbers 1 to 88. Then I have defined another list with letters starting from A0 and ending at C8. There is a mapping attribute which is a hash map.

I should focus on abstracting what a triad is. Maybe if possible a four note chord also.