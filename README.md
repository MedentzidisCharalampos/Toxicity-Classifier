# Toxicity-Classifier
The toxicity model detects whether text contains toxic context. More about this model can be found there: https://github.com/tensorflow/tfjs-models/tree/master/toxicity . We will use the pre-trained Toxicity model to detect whether a given piece of text contains toxic content such as threatening language, insults, obscenities, identity-based hate, or sexually explicit language.    
We define a threshold which is a minimum prediction confidence.  
Every prediction has two values one for not-insult and one for insult

if prediction < not-insult then match = false and the comment is not toxic
else if prediction > insult then match = true and the comment is toxic
else if not-insult = insult the match = none and it is a tie

.
