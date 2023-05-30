      <tuplet><tone><accidental><duration><transpose>:<attribute-1>:<attribute-2>:...:<attribute-n>:<scope>
  
  This is a general definition of tone and the attributes that tone may have. The attribute should be declared upfront so it is clear what each letter used means
  
  A pattern may consist of multiple tones, where duration is separated, or grouped in a tuplet
  
  3g+ag4 b8 p4

  This is equivalent to
  
  ![image](https://github.com/alexpeter-pen/MusicL/assets/118837759/07db6909-38b0-4f54-bdde-8ebc0e72d097)

Spaces are here added for clarification, the notation should generaly work even when they are removed. Anyway missing spaces suggest groupin and used space suggests separation. Notice that the second g has no accident, it is inherited, and this is one of the rules that is adopted from the standard notation.
  
  d4:l e: d:
  
  Inherited attributes are clarified by empty : \
  **l** in d4:**l** means (for example) legato here and these three tones have the same duration of a quarter and are connected. In standard notation that would be
  
  ![image](https://github.com/alexpeter-pen/MusicL/assets/118837759/487ad4ec-1e14-4121-a893-fe7fe055e107)

All other attributes are defined similarly, they are attached to a specific note, or a group of notes, where it is declared in the notation what meaning the used letter has. For example, somewhere we define an attribute description.

::legato:fluid:1234

$ This specifies that :l means legato and that overlapped appearances will be marked by l1 l2 l3 and l4, when necessary

::slur:rhythm

$ This specifies that :s means slur and is used to define a rhythmic local group.

s:a8b8d8 p8

![image](https://github.com/alexpeter-pen/MusicL/assets/118837759/448985ff-d652-4c3e-8d27-d5d9b7f571c6)

Notice a subtle difference that standard notation cannot easily express

s:a8b8d8p8

This would mean that the pause is a part of the same rhythmic local group.

All other elements like stress, and accent are added in the same manner.

g4':tr or g4':t means a trill on g in one octave above the predefined or just first (called one-lined) octave if nothing is predefined

Declaration should contain the definition of trill in a form that describes intention, alike

::trill:cdcd...
