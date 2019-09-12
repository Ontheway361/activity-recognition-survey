# survey taxonomy
<img src="https://github.com/Ontheway361/Human-Activity-Recognition/blob/master/assets/taxonomy.jpg" width="600" height="400" alt="首页"/>
In our survey paper, we group the approaches based on deep learning into three categories, e.g. sequence-based, view-based, depth-based. For the sequence-based approaches, their intrinsic characteristic is transforming the sequences with variable length to fixed dimension label. For the view-based approaches, which focus on the generation, combination and factorization of different views. For the depth-based approaches, they study the transformation of representation from one space to another.

# Introduction
This repo contains the brief introduction of our survey paper : A Gentle Review of Deep Learning based Human Activity Recognition. In this section we will introduce the outline of each categories.

## Sequence-based
In this section, we list the two streams of methods that transform the sequence with variable length to fixed dimension. One is RNN(LSTM)-related approaches, the other is temporal aggregation related approaches.

### Recurrent Nets and Attention Mechanism
Recurrent networks are ad hoc for sequential input, e.g. video, signal.
<p><img src="assets/sequential/fig7-rnn.jpg" width="300" height="180" alt="首页"/></p>

### Temporal Aggregation
Sampling and pooling are two major ways of temporal aggregation.
For sampling, it is the most intuitive method to convert a flexible length sequence to fixed-length representation by taking the constant number of observations from a sequence. We group the tricks that based on sampling into five classes, e.g. random sampling, uniform sampling, segment random sampling, shot-based sampling and adaptive sampling. Following figs illustrate those sampling tricks.
<p>a.random sampling</p>
<img src="assets/sequential/fig8a-random.jpg" width="600" height="150" alt="首页"/>

<p>b. uniform sampling</p>
<img src="assets/sequential/fig8b-uniform.jpg" width="600" height="150" alt="首页"/>

<p>c. segment random sampling</p>
<img src="assets/sequential/fig8c-segment.jpg" width="600" height="150" alt="首页"/>

<p>d. shot-based sampling</p>
<img src="assets/sequential/fig8e-shot_based.jpg" width="600" height="240" alt="首页"/>

<p>e. adaptive sampling</p>
<img src="assets/sequential/fig8d-adaptive.jpg" width="600" height="240" alt="首页"/>

Pooling as the common component CNNs, which performs on features to to generate the more semantic features. We classify pooling-based approaches into three groups, e.g. local pooling, global pooling, slow pooling, according to the place and the times a pooling operation was executed.
<table style="border:0px">
   <tr>
       a). local_pooling
       <td><img src="assets/sequential/fig10a-local_pooling.jpg" width="200" height="100" frame=void rules=none></td>
       b). global_pooling
       <td><img src="assets/sequential/fig10b-global_pooling.jpg" width="200" height="100" frame=void rules=none></td>
       c). slow_pooling
       <td><img src="assets/sequential/fig10c-slow_pooling.jpg" width="200" height="100" frame=void rules=none></td>
</table>
