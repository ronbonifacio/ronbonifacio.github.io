# Working In Dev Containers
This is my first post on my AI blog!

Whilst this was a task that I had completed a while ago in my tutorial class, I've only ended up documenting on it on this blog now not long before the assignment is about to be due. Even though it may have been nicer to start documenting my journey earlier it is nonetheless good to write about what I have learnt.

Professor Lovell talked to our class about running python environments on the UQ lab computers using dev containers, they're an efficient way to work on projects with the same code bases and libraries. The dev container that Professor Lovell has provided has also been setup for deep learning on either the computer's CPU and GPU depending on which branch is chosen.
One of the assignment tasks was to compare the speedup the GPU has over the CPU when running deep learning training for a small image classifier. As expected training is a lot faster on GPU than on a CPU.

Some of the results from the training are shown below, with the training metrics output presented in a markdown table and some images of the GPU activity graphs.

Results from training:

| epoch | train_loss | valid_loss | error_rate | time |
|-------|------------|------------|------------|------|
| 0     | 0.736912   | 0.402907   | 0.106977   | 00:02 |

| epoch | train_loss | valid_loss | error_rate | time |
|-------|------------|------------|------------|------|
| 0     | 0.318343   | 0.289572   | 0.120930   | 00:02 |
| 1     | 0.195320   | 0.300568   | 0.102326   | 00:02 |
| 2     | 0.133876   | 0.296840   | 0.097674   | 00:02 |

GPU activity from training with a default batch size of bs=64

![](/images/default_batch_size.png)
