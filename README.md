# HDDL Semantics
This is a project for High Dimensionnal Deep Learning class of the Master 2 first semester at Insa Toulouse (ModIA).
During this class, we learned about state of the art deep learning methods.

We proposed a subject to the teachers: create a game like cementix https://cemantix.certitudes.org/ but with a model that we specialize to a specific book. The goal is that the software make us guess words specifics to the book. For exemple, a model trained on Harry Potter could make us guess the words: Dobby, wand, stupefix... with the meaning of the Harry Potter books.
We used the free access (excellent) book Warbreaker from Brandon Sanderson.
We used the free access model MiniLM-L6-v2 (https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) that we fine tuned with constrastive learning loss on successive sentence pairs.
The model didn't archive satisfactory performances. Due to the time limit in the project, we couldn't fix the problem but we hypothesized it was due to the collapse of the model. In the perspectives, we thoughts that psotive pairs only methods (like Dino in image) could help prevent collapse because some pairs taken in the same book, even if far appart can be positive while with constrastive methods, we consider them negatives. 

During the project we learned about sentence transformers, transformers specifically trained with self supervised methods to extract meaningful representations of sentences that we can compare with cosine similarities.

