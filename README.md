# Simple part of speech tag fixer

### These functions are designed to fix POS tags.

### To install using pip:

    pip install tag-fixer

### To begin, import tag_fixer:

    from tag_fixer import tag_fixer as tf
	
	
### For tag_fixer(), the presumed format of the data is a list of [word,tag] or (word,tag) pairs
    
    l = [["The","DT"],["teacher","NNP"],["is","VBZ"],["awesome","JJ"]]
    fixed_list = tf.tag_fixer(l)

### For tag_fixer_sents(), the presumed format of that data is a list sentences that are lists of [word,tag] pairs.    
    
    l2 = [[["The","DT"],["teacher","NNP"],["is","VBZ"],["awesome","JJ"]],[["This","DT"],["is","VBZ"],["another","JJ"]]]
    fixed_sents = tf.tag_fixer_sents(l2)

### Note that either function will automatically capitalize tags (so the user doesn't have to hit the [shift] key)

