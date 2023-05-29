# MusicL
Language for musical notation

This is a language for musical notation that is text-based but as capable as standard musical notation and interchangeable with it.
Regarding programming language part it is consisting of two symbols :: and : that are reserved and cannot be used for anything else and accepted symbols like cdefghc for notes.

:: describes context and this includes for example ::key ::tempo ::speed ::tranpose ::bars ::metronom

: describes specification or attribute for example ::transpose:e:2:>< means that the piece has a base note e in second octave, so all efgabcd in the notation belong to this octave, while octave above or bellow is marked with > and < respectively for example a melody part cde>c

Where used space means separation and no space means a potential grouping. A group is used where the same attribute is applicable to a series of concatenated notes.

Anything that is used in the notation should be defined within context. For example we can use 12345678 for marking duration or 1248, but this needs to be spelled out.

(It is a general aim to use only one character wherever possible in the notation for anything so it is not advisable to use 12481632 for marking duration.)

In this example, we introduce a notation for comment first and then duration. 0 in first, and 1 in the second line means a whole note.

::comment $ 

::duration 01234567 $ 1/2^n

::duration 1248    $ 1/n

Besides describing all the details as above, the language is based on vertical and horizontal synchronization context. For example, we can write a melody as

::notes cdefgahb p $ defines letters used for notes and pause

piano:g4a4p4h8c4p4d2

but we can write it as well

piano:gaphcpd:4448442

separating melody and rhythm.

Vertical synchronization allows writing parallel melody lines and instrument

An example of a series of chords

    piano:     cgac
               ebce
               gdeg

or instrumentation

              violin: a+4 h8  c-2  3fga 
              viola:  g   p   p4   f2
              bass:   h   d:l d:   d<

If vertical synchronization context is used, it is recommendable to have a font declaration that specifies how to read files, in this text we used Courier font but generally this is not known to the reader so it might be specified. Vertical content should be aligned to some degree, not necessarily note by note.

::font CourierNew

Equally, we can specify the encoding used

::encoding utf-8

In all these examples ::font:CourierNew or ::encoding:utf-8 is equivalent however : is used where we need to add more attributes like ::transpose:e:2.

This allows using extended Unicode notation, for example, we can use C𝄳 if we need to.

The language specification is strict in some sense, but as long as you do not assume that people understand what you mean, and properly define everything through the context, you can extend the language in any desired direction. So the language specification defines or suggests a couple of basic notational standards to learn how to properly describe the notation used, rather than explaining everything possible to annotate through the language.
