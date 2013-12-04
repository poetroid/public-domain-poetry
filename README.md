# Restore Poems Together

Thousands of poems in the public domain live buried in school libraries, archaic websites, journals gone out of print. We don't have a free, unified access. An open library.

Let's build one.

## Overview

Three parts: format, metadata, scripts.

1. Restore poems with a new format: for humans and machines.
2. Curate poems adding metadata, inline: humans and machines.
3. Run scripts to find, see, and print poem, offline.

### Poem format

[Plain Text](http://en.wikipedia.org/wiki/Plain_text) is still an excellent format supported by all editors by default: notepad, textedit, [iAWriter](http://www.iawriter.com/mac/), and others. Files must be saved in [UTF-8](http://en.wikipedia.org/wiki/UTF-8) 'encoding'-- a setting available as options in the 'save as' file-dialog. Saving a file in UTF-8 is a necessary, important step to preserve foreign-language characters across machines.

```
Every time I say "joy," joyous thing,
you will know that I am talking about you,
for you are the joy of all joyous beauty
and the joy of all joyous and beautiful pleasures,
```

### Metadata

The current format for metdata is [YAML](http://en.wikipedia.org/wiki/YAML), a humanly readable format. This format may change to [edn](https://github.com/edn-format/edn), and old poems will be upgraded, automatically.

Metadata will be curated *inline*, above the poem, for storing metadata and tags, to inform humans and machines of semantic data for further analysis.

```
---
title: Untitled
type: Sonnet
author: Guitton D'Arezzo
curator: Ata Moharreri
period: 1230-1294
country: Italy
tags:
- joy
- happiness
---
```

Note the `---` before and after the metadata.

Filenames are saved as `last-name-title-first-five-words-of-poem.txt`

Poems, metadata, and all the revisions are protected in (git)hub, for free, forever.

**Complete Example**

```
---
author: Walt Whitman
gender: male
title: from I Sing the Body Electric
curator: Ata
year: 19th century
country: America
tags:
 -  body
 -  women
 -  art
 -  love
 -  life
 -  soul
 -  meditative
 -  family
 -  beauty
 -  nature
 -  feminine
 -  narrative
---

This is the female form,
A divine nimbus exhales from it from head to foot,
It attracts with fierce undeniable attraction,
I am drawn by its breath as if I were no more than a helpless vapor,
all falls aside but myself and it,
Books, art, religion, time, the visible and solid earth, and what
was expected of heaven or fear'd of hell, are now consumed,
Mad filaments, ungovernable shoots play out of it, the response likewise ungovernable,
Hair, bosom, hips, bend of legs, negligent falling hands all diffused, mine too diffused,
Ebb stung by the flow and flow stung by the ebb, love-flesh swelling and deliciously aching,
Limitless limpid jets of love hot and enormous, quivering jelly of love, white-blow and delirious nice,
Bridegroom night of love working surely and softly into the prostrate dawn,
Undulating into the willing and yielding day,
Lost in the cleave of the clasping and sweet-flesh'd day.

This the nucleus—after the child is born of woman, man is born of woman,
This the bath of birth, this the merge of small and large, and the outlet again.

Be not ashamed women, your privilege encloses the rest, and is the exit of the rest,
You are the gates of the body, and you are the gates of the soul.

The female contains all qualities and tempers them,
She is in her place and moves with perfect balance,
She is all things duly veil'd, she is both passive and active,
She is to conceive daughters as well as sons, and sons as well as daughters.

As I see my soul reflected in Nature,
As I see through a mist, One with inexpressible completeness, sanity, beauty,
See the bent head and arms folded over the breast, the Female I see.

```

### Scripts

This library will include python scripts to help scholars, students, educators, and publishers research poetry, from the comfort of their pc, mac, or browser. 

## Status and Roadmap

Currently hosts ~34000 poems, some hand-curated by editors at Facjure.

For a webapp to search and view existing poems, visit [poetroid](https://github.com/poetroid), an open platform to discover poetry together.

## Resources

Thanks to the original sites that curated thousands of poems from the public domain: 

- [Project Gutenberg](http://www.gutenberg.org)
- [Public Domain Poetry](http://www.public-domain-poetry.com)

## Contributers

- Priyatam Mudivarti: fiction writer, engineer, and founder of [Facjure LLC](http://www.facjure.com)
- Ata Moharreri: poet, professor, and former managing editor of [The Massachusetts Review](http://www.massreview.org/editors)
- Sreeharsha Mudivarti: musician, engineer, and survivor of a space ship crash.

## Copyright & License

Copyright (c) Facjure LLC. All rights reserved.

Poems are available for free for personal or commerical use, provided this license is retained.

Scripts are available for free using Apache 2 Opensource License.
