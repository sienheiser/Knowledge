## 07/08/2024
I want exploring what formats can I record a lesson. A lesson has the following parameters I want to keep track
1. The notes displayed in the lesson
2. The notes pressed in each lesson
3. The time it takes to press each note
I have implemented the above. Right now I have a basic way of randomly choosing displaying three notes on the piano and starting the specified information in an sqlite3 database.

The next question is working on the randomly choosing of three notes to display. **I believe** this aspect is the crux of this app. These are the impressions I have 
1. I need something that will look on the generate lessons given a some keys as input. So for example I need a model that can generate music notes that sound nice.


I am still lost on how to approach this problem of generating reasonably sounding music notes. 

### Using chords instead of singles notes
I have spent time trying to understand how one could make a box that generated natural sounding notes from using a dataset. When making a machine learning algorithm big consideration must be given to the data we use. The music data set found online cannot be used for commercial purposes.

I would like to try a different approach. What if I make a slightly smarter version of anki. Use rule of the octave as a starting point and branch out from there.

#### 1st method
In the rule of the octave each note in a scale has an associated triad chord with it and each triad has three variations

This basic pattern can be repeated for each of key on the piano.


## 09/08/2024
Today I will continue trying to make the note algebra work. 

So far I think I have a working system. Now I want to create the display for displaying notes. I have not done it yet so I should try working on it tomorrow.

Next thing to understand is the following what scheme should I use for representing a keyboard. Right now I am using numbers 1,2,3 to represent keys on a keyboard. Keyboards of different sizes will always have their left most key labelled number 1. This means for different keysboards 1 will mean different things. Maybe I should look at how a piano is tuned and make an absolute base. 