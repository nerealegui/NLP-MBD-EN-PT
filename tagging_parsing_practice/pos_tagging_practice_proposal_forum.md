## Exercise 1.1

The best tag is the noun - it's the most common type
```
Default tagger accuracy for ADJ:  0.05291005291005291
Default tagger accuracy for ADV:  0.025573192239858905
Default tagger accuracy for CONJ:  0.02072310405643739
Default tagger accuracy for DET:  0.12301587301587301
Default tagger accuracy for X:  0.0
**Default tagger accuracy for NOUN:  0.31790123456790126**
Default tagger accuracy for PROPN:  0.0
Default tagger accuracy for NUM:  0.017195767195767195
Default tagger accuracy for PRON:  0.021164021164021163
Default tagger accuracy for ADP:  0.1128747795414462
Default tagger accuracy for AUX:  0.0
Default tagger accuracy for INTJ:  0.0
Default tagger accuracy for VERB:  0.1693121693121693
Default tagger accuracy for PART:  0.0
Default tagger accuracy for SCONJ:  0.0
Default tagger accuracy for SYM:  0.0
```


## Exercise 2.1.1 && 2.1.2 && 2.1.3 

Unigram tagger accuracy:  0.9448853615520282

The accuracy is way higher, we've gone from a 0.31 to a 0.94.

The unknown words are being tagged as nouns as I've set up the backoff default tagger with NOUN tag. When not set, the accuracy dropt to 0.88 - I'm assuming when we don't have any backoff, it's not tagger in the [doc](https://tedboy.github.io/nlps/generated/generated/nltk.UnigramTagger.html) there's no clear mention to it.

We are improving the accuracy of the default tagger by using a backoff tagger, but we could still get a better accuracy.


## Exercise 2.2.1

The combined tagger increases the accuracy up to 52.9% but I find it's still too low compared to our previous attempts.

## Exercise 2.2.2

It improves slightly the accuracy the cmbination of UnigramTagger and affixTagger compared to the exercise 2.1.3 -  0.9541446208112875. But it's not a huge improvement.

## Exercise 2.3.1

I get an accuracy of  0.8963844797178131 with the ngram_tagger tagger with default unigram. I've tested several context sizes but I don't see any changes.
