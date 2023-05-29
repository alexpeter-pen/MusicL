$ Instruments are introduced directly without any prefix and simply followed by the melody

piano:melody:a2d4c2e2

$ This can be shortened to

piano:a2d4c2e2

$ Equally we can split melody and rhythm and write it as

piano:adce:2422

$ Instead of melody, we can use chords, which again can be shortened because the usage is obvious

guitar:chords:Am7 a7 C G7d9

guitar:Am7 a7 C G7d9

::bars                b			b 

$ Bars are used to mark the first note just after where a bar should be. Here it is important to have things aligned because bars are just visual cues, any symbol can be used, but just that symbol then on. 

::metronom                m		m 

$ Metronom is giving the accents within a bar if tempo notation is not sufficient

::vertical:<name>

$ Vertical is defining a segment that is meant to be vertically synchronized, similarly how the staff is synchronized

::staff:<name>

$ Synonym for ::vertical

    ::staff:q
    ::transpose:e:2:',
    ::bars            b			    b 
    ::metronom            m		  m 
              violin: a+4 h8  c-2  3fga 
              viola:  g:q p:q p4:q f2
              bass:   h   d:l d:   d,

::dynamic:f

$ Dynamic describes dynamics with expected standard notation using ppp,ppp,pp,p,mp,mf,f,ff,fff,fff or similar extension of the same \
$ Dynamics are attached to the melody above by default and we can use ::d:u ::d:b ::d:s if we want to clarify what dynamic is attached to, :s meaning staff or segment. We shortened ::dynamic to just ::d in the examples
  
              violin: a+4 h8  c-2  3fga 
              ::d     p
              viola:  g:q p:q p4:q f2 
              ::d     f
  
::segment:k

$ Segment is splitting staff into vertical areas, where we can specify something, like dynamics, an apply to the entire segment
  
              violin: a+4 h8  c-2  3fga 
              viola:  g:q p:q p4:q f2
              ::segment:k
              ::d:k   ff
  
All neighboring lines belong to the same instrument as long as a new instrument is not specified.

::phrase:r

$ Phrase is introducing a part that may be used again in its entirety. For example
 
::phrase:a2g3 hg g2d4 42:k

piano:kc2kkd2k
  
$ Again, all elements that are not defined are arbitrary. For example, if we just specify melody, the instrument is arbitrary, or not even relevant. \
$This language can be extended with more declarations, but their usage must be clearly stated in the comment regardless of its assumed clarity.
