Word Embeddings
One-hot encoding is massively inefficient because most values in one-hot vector will be set to 0. Embeddings are fully connected layers. 
Instead of doing the matrix multiplication, we use the weight matrix as a lookup table. e.g heart is encoded as 958, then to get the hidden layer values for heart, you just take the 958th row of the embedding matrix. This process is called an embedding lookup and the number of hidden units is the embedding dimension.


Word2Vec
Finds much more efficient representations by finding vectors that represent the word. These vectors also contain semantic information about the words.
*  Words that show up in similar contexts will have vectors near each other. 
* Different words will be further away from one another
* Relationships can be represented by distance in vector space
