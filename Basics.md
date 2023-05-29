MusicL is using : and :: for describing musical content. These symbols cannot be used for any other purpose.

:: is describing context like ::key ::tempo, so it is a definition name and is followed by description

In ::<<declaration>>, <<declaration>> is a word that is standardly adopted word that has the most common meaning \
There is no space in <declaration> name, and this is mandatory. \
An optional, but recommended rule, is that the only acceptable another symbol apart from ASCII letters is - or _, but just one of them in the same file. \
The reason for using another alphabet might be the audience the notation is intended for.

: is used to clarify the item, or to connect the item with the predefined context or among themselves. d:s could mean d with staccato. Equally 3:4 means 3-quarter rhythm.

The extension for the file containing this notation is .mlq

The basic rule in MusicL is that everything must be declared before it is used. \
If something is not declared, its usage is inferred and if so it must be consistent through the same file.

Any declaration can be shortened ::key to ::k and similar if its usage is clear.

If the item ends with not declared letter like :q, q is understood as a label, intended to use somewhere else. \
If the item ends with empty : it is inheriting whatever the previous item had for example d:l d: d: are showing three notes that are inheriting legato.
