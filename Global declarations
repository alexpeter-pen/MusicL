::notes cdefgabcCDEFGABC
\Declaring letters reserved for notes, later on, it can be declared what each case means

::key C#
\Key used throughout the composition

::speed 90
\Nominal speed. Normally defined in bit per minute, bpm

::duration 01234567 \ 1/2^n
::duration 1248    \ 1/n
\These are two standard ways of marking duration. For readability, it is not recomendable to use 16 or 32.
\A compound duration is achieved by concatenating durations like 12, 24, 124, so we assume that basic duration is just one character long
\It is possible to use 3,5,7,9 with the meaning clear from the context

::tempo:3:4
\Tempo used is three quarters

::tempo:3:2:4
\Compound tempo 5/4 = 3+2/4. It is assumed that the last number corresponds to the main unit, in the case above it is 4
\More complicated tempo cases might be defined using labels

::tempo:3:2:q
::tempo:2:3:t

::tempo:q:t

::transpose:e:2:><
::transpose:e:2:',
\Transpose is defining the first note, octave that does not require a special mark, and marks used for upper and lower octaves, the example is showing two possible choices
\For example, after this declaration a melody de'd means that e is taken from the third octave, one octave above
\efgabcd these letters if used would assume that they are from the same second octave
\e,f,g,a,b,c,d, these are from the octave bellow
\e'f'g'a'b'c'd' these are from the octave above
\e'' this e is from two octaves above

tone:octave:C:0:3
tone:octave:c:4:10
\To clarify how various cases can be used, this defines the usage of cases upper and lower depending on octave as in

Traditional	Helmholtz
0  subsubcontra	C͵͵͵ – B͵͵͵
1  sub-contra	C͵͵ – B͵͵
2  contra	C͵ – B͵
3  great	C – B
4  small	c – b
5  one-lined	c′ – b′
6  two-lined	c′′ – b′′
7  three-lined	c′′′ – b′′′
8  four-lined	c′′′′ – b′′′′
9  five-lined	c′′′′′ – b′′′′′
10 six-lined	c′′′′′′ – b′′′′′′
	
tone:chord:C:major
tone:chord:c:minor
\Within chords cases may have a different meaning

If a declaration of any kind is omitted, it is either arbitrary or most common.

