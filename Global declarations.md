::notes cdefgabcCDEFGABC

$ Declaring letters reserved for notes, later on, it can be declared what each case means

::accidentals:C+C-Cn

$ Declaring accidentals used, Cn means C neutral

::accidentals:C#C♭C♮

$ Another option for accidentals

$ The above examples are typical. Notice that + and - might not be used easily somewhere else

::author Aleksandar Perisic
::date 2023-05-05
::name Land of S
::location Oslo Norway
::arrangement ST

$ These above are defining a set of typical attributes one composition may have, you can freely add more to it

$ We can use semi-accidentals too, but it must be specified with the corresponding symbol

::key C#

$ Key used throughout the composition

::pitch:A:440

$ Standard pitch used within the composition

::intonation:ET

$ Used intonation, ET stands for equal temperament

::scale:12

$ Standard 12-tone scale used

::scale:lydian

$ If this information is relevant, then it can be easily stated, notice that this is then combined with key or stated together like ::scale:lydian:C#

::scale:wwhwh3hh

$ Another way of defining the scale used, w - whole step, h - half step

::speed 90

::speed legatto

$ Nominal speed. If in numbers, normally defined in bit per minute, bpm, again it can be clarified

::duration 01234567 $  1/2^n

::duration 1248    $  1/n

$ These are two standard ways of marking duration. For readability, it is not recommendable to use 16 or 32.

$ A compound duration is achieved by concatenating durations like 12, 24, 124, so we assume that basic duration is just one character long

$ It is possible to use 3,5,7,9 with the meaning clear from the context

::tempo:3:4

$ Tempo used is three quarters. We can use ::tempo:c meaning common tempo.

::tempo:3:2:4

$ Compound tempo 5/4 = 3+2/4. It is assumed that the last number corresponds to the main unit, in the case above it is 4

$ More complicated tempo cases might be defined using labels

::tempo:3:2:q

::tempo:2:3:t

::tempo:q:t

::transpose:e:2:><

::transpose:e:2:',

$ Transpose is defining the first note, octave that does not require a special mark, and marks used for upper and lower octaves, the example is showing two possible choices

$ For example, after this declaration a melody de'd means that e is taken from the third octave, one octave above

$ efgabcd these letters if used would assume that they are from the same second octave

$ e,f,g,a,b,c,d, these are from the octave bellow

$ e'f'g'a'b'c'd' these are from the octave above

$ e'' this e is from two octaves above

tone:octave:C:0:3

tone:octave:c:4:10

$ To clarify how various cases can be used, this defines the usage of cases upper and lower depending on octave as in

Traditional	Helmholtz \
0  subsubcontra	C͵͵͵ – B͵͵͵ \
1  sub-contra	C͵͵ – B͵͵ \
2  contra	C͵ – B͵ \
3  great	C – B \
4  small	c – b \
5  one-lined	c′ – b′ \
6  two-lined	c′′ – b′′ \
7  three-lined	c′′′ – b′′′ \
8  four-lined	c′′′′ – b′′′′ \
9  five-lined	c′′′′′ – b′′′′′ \
10 six-lined	c′′′′′′ – b′′′′′′
	
tone:chord:C:major

tone:chord:c:minor

$ Within chords cases may have a different meaning

If a declaration of any kind is omitted, it is either arbitrary or most common.

Unless specified differently all declarations should be a full words. To avoid repetition or to shorten the usage we can declare what shorthand notation is

::key:k
::trill:r

and similar. Notice that the language assumes a level of context that is not spelled out. For this reason it is necessary to help the reader bz giving at least a hint in the declaration over what the notation, i.e. letter is used for.
