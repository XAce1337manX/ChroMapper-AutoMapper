# AutoMapper

## ChroMapper plugin

Completely new automapper, audio to onsets and light generation algorithm.

### Features

-   Lightshow Generator (based on note timings)
-   Map Generator from Notes
-   Map Generator from Audio
-   Generate note in a specific audio range
-   Generate note as timing only
-   Note selection for each algorithm

### Options

**Audio**:
0.01 is the default value for an onset (note) to be placed by the algorithm
-   Max Speed : The minimum distance between two note generated.
-   Double Threshold : The onset value need to be above this value to generate a double note on same beat.
-   Max double speed : Remove double also known as gallops if there is a singular note too close to the double (in beat).
-   Onset Sensitivity : Threshold Multiplier for the average of an onset. If the onset is above that average, the onset is kept.
-   Indistinguishable Range : Value divided by to find the "Number of set of samples to ignore after an onset". Setting it higher will reduce that immunity period.
-   Audio Range : Min and Max value (in beat) where notes will be generated.

**Map** :
-   Bottom Row Only : All the notes are generated bottom row.
-   Up and Down Only : All the notes are either down or up cut direction (still flow).
-   Randomize Line : Randomise the line index of each note.
-   Fused Double Only : Make double notes the same line and layer.
-   Timing Only : Only dot notes, all aligned bottom left.
-   Wrist Limiter : When enabled, remove extreme wrist rotation.

**Light**:
-   Speed : Color will switch value every x (beat).
-   Offset : Add an offset from first note for the color switch (in beat).
-   Boost : Boost will turn on/off every x (beat).

### Credits

[Lolighter](https://github.com/Loloppe/Lolighter) by [Loloppe](https://github.com/Loloppe)
[ChroMapper-Lolighter](https://github.com/KivalEvan/ChroMapper-Lolighter) by [Kival Evan](https://github.com/KivalEvan/)
