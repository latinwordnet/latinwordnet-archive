# Latin WordNet 2.0


## Mark-Up
For literal senses of words, no special mark-up is required. However, because synsets have been assigned to lemmas through an automated process, the possibility exists of mistaken or irrelevant attributions. Therefore it may be necessary to delete certain attributions, which can be indicated with strikethrough. Alternatively, if a known word sense is missing from the listed synset attributions, it can be added by supplying the relevent synset ID. If no appropriate synset exists, a new one will need to be created: in this case, provide a suitable gloss in English of the required meaning. To indicate a metonymic (within-domain) meaning extension, mark the synset with ‘~’. For metaphoric senses (if any), use ‘#’. Additionally, the primary sense(s) of a word -- the meanings that come most immediately to mind when thinking of the word -- should be indicated by ‘p’. (The primary sense of a word may be literal or figurative: in the latter case, both indications should be given). As with literal senses, missing figurative senses can be supplied by an English gloss for later addition to the database. 

##### Codes
     (none)    literal
     ~         metonymic
     \#        metaphorical
     p         primary
     -         (deletion)
     +         (addition)
Codes can be combined: e.g., '+#' (add a metaphorical sense, followed by the appropriate synset ID).

## Temporal relations
If a (literal, metonymic, or metaphorical) sense of a word is circumscribed temporally, this information can be included in the database by creating a Temporal Relation record. A Temporal Relation links a lemma and a synset (its sense) with a specification of period. Possible values are:
        old     Old Latin (-c. 75 BCE)
        cla     Classical Latin (c. 70 BCE-c. 200 CE)
        gld     Classical Latin 'Golden Age' (c. 70 BCE-18 CE)
        slv     Classical Latin 'Silver Age' (18-133 CE)
        ltr     Late Latin (c. 200-9th c. CE)
        ecl     Ecclesiastical Latin (c. 200 CE-)
        med     Medieval Latin (c. 9th c.-13th c. CE)
        ren     Renaissance Latin (c. 1300-1500 CE)
        neo     Neo-Latin (c. 1500-1800 CE)
        mod     Modern Latin (19th c. CE-)
For example, 
> ecl baculum (n) 'a support that steadies or strengthens something else (n#02327416)'

## Lexical and semantic relations
The WordNet can accommodate the encoding of both lexical (lemma-to-lemma) and semantic (synset-to-synset) relations, of several different kinds. As relations are exclusively binary, when coding a new relation it is easiest to classify the relation according to the part of speech of the originating element (the 'source') (where the 'target' can be of any of the permissible parts of speech). If the relation is lexical, source and target must be lemmas; if the relation is semantic, source and target must be synsets. Relations of antonymy, hypernymy, and hyponymy can be either lexical or semantic: if lexical, they must pertain to *all* senses of the relevant lemmas.

### Noun relations
##### Semantic
        !       antonym
        @       hypernym
        ~       hyponym
        #m	member-of
        #s	substance-of
        #p	part-of
        %m	has-member
        %s	has-substance
        %p	has-part
        =	attribute
        |	nearest
        +r	has-role
        -r	is-role-of
 ##### Lexical
        !       antonym
        @	hypernym
        ~	hyponym
        +c	composed-of
        -c	composes
        \	derived-from
        /	related-to
### Verb relations
##### Semantic
        !	antonym
        @	hypernym
        ~	hyponym
        *	entailment
        >	causes
        ^	also-see
        $	verb-group
        |	nearest
 ##### Lexical
        !       antonym
        @	hypernym
        ~	hyponym
        +c	composed-of
        -c	composes
        \	derived-from
        /	related-to
### Adjective relations
##### Semantic
        !	antonym
        &	similar-to
        =	is-value-of
        ^	also-see
        |	nearest
##### Lexical
        !       antonym
        <	participle
        +c	composed-of
        -c	composes
        \	derived-from
        /	related-to
### Adverb relations
##### Semantic
        !	antonym
        |	nearest
##### Lexical
        !	antonym
        +c	composed-of
        -c	composes
        \	derived-from
        /	related-to

###### Examples
(adjective relation) \, niveus, nix
(verb relation) !, maledico, benedico
(adjective relation) !, a#L9945509 ('capable of being placated or appeased'), a#01716198 ('impossible to placate')
