

<!-- === Source: MinerU_markdown_Linear_regression,_active_learning_1_2122709467580706821.md (Page 1) === -->

## Linear regression, active learning

We arrived at the logistic regression model when trying to explicitly model the uncertainty about the labels in a linear classifier. The same general modeling approach permits us to use linear predictions in various other contexts as well. The simplest of them is regression where the goal is to predict a continuous response $y _ { t } \in \mathcal R$ to each example vector. Here too focusing on linear predictions won’t be inherently limiting as linear predictions can be easily extended (next lecture). 

So, how should we model continuous responses? The linear function of the input already produces a “mean prediction” or $\theta ^ { T } \mathbf { x } + \theta _ { 0 }$ . By treating this as a mean prediction more formally, we are stating that the expected value of the response variable, conditioned on x, is $\theta ^ { T } \mathbf { x } + \theta _ { 0 }$ . More succinctly, we say that $E \{ y | \mathbf { x } \} = \theta ^ { T } \mathbf { x } + \theta _ { 0 }$ . It remains to associate a distribution over the responses around such mean prediction. The simplest symmetric distribution is the normal (Gaussian) distribution. In other words, we say that the responses y follow the normal pdf 

$$
N (y; \mu , \sigma^ {2}) = \frac {1}{\sqrt {2 \pi \sigma^ {2}}} \exp \left(- \frac {1}{2 \sigma^ {2}} (y - \mu) ^ {2}\right)\tag{1}
$$

where $\mu = \theta ^ { T } \mathbf { x } + \theta _ { 0 }$ . Our response model is therefore defined as 

$$
P (y | \mathbf {x}, \theta , \theta_ {0}) = N (y; \theta^ {T} \mathbf {x} + \theta_ {0}, \sigma^ {2})\tag{2}
$$

So, when the input is 1-dimensional, we predict a mean response that is a line in $( x , y )$ space, and assume that noise in y is normally distributed with zero mean and variance $\sigma ^ { 2 }$ Note that the noise variance $\sigma ^ { 2 }$ in the model does not depend on the input x. Moreover, we only model variation in the y-direction while expecting to know x with perfect precision. Taking into account the efect of potential noise in x on the responses y would tie parameters θ and $\theta _ { 0 }$ to the noise variance $\sigma ^ { 2 }$ , potentially in an input dependent manner. The specifics of this coupling depend on the form of noise added to x. We will discuss this in a bit more detail later on. 

We can also write the linear regression model in another way to explicate how exactly the additive noise appears in the responses: 

$$
y = \theta^ {T} \mathbf {x} + \theta_ {0} + \epsilon\tag{3}
$$

where $\epsilon \sim N ( 0 , \sigma ^ { 2 } )$ (meaning that noise � is distributed normally with mean zero and variance $\sigma ^ { 2 } )$ . Clearly for this model $E \{ y | \mathbf { x } \} = \theta ^ { T } \mathbf { x } + \theta _ { 0 }$ since � has zero mean. Moreover, adding Gaussian noise to a deterministic prediction $\theta ^ { T } \mathbf { x } + \theta _ { 0 }$ makes y normally distributed with mean $\theta ^ { T } \mathbf { x } + \theta _ { 0 }$ and variance $\sigma ^ { 2 }$ , as before. So, in particular, for the training inputs $\mathbf { x } _ { 1 } , \ldots , \mathbf { x } _ { n }$ and outputs $y _ { 1 } , \ldots , y _ { n }$ , the model relating them is 

$$
y _ {t} = \theta^ {T} \mathbf {x} _ {t} + \theta_ {0} + \epsilon_ {t}, t = 1, \ldots , n\tag{4}
$$

where $e _ { t } \sim N ( 0 , \sigma ^ { 2 } )$ and $e _ { i }$ is independent of $e _ { j }$ for any $i \neq i .$ 

Regardless of how we choose the write the model (both forms are useful) we can find the parameter estimates by maximizing the conditional likelihood. Similarly to the logistic regression case, the conditional likelihood is written as 

$$
L (\theta , \theta_ {0}, \sigma^ {2}) = \prod_ {t = 1} ^ {n} \frac {1}{\sqrt {2 \pi \sigma^ {2}}} \exp \left(- \frac {1}{2 \sigma^ {2}} (y _ {t} - \theta^ {T} {\bf x} _ {t} - \theta_ {0}) ^ {2}\right)\tag{5}
$$

Note that $\sigma ^ { 2 }$ is also a parameter we have to estimate. It accounts for errors not captured by the linear model. In terms of the log-likelihood, we try to maximize 

$$
l (\theta , \theta_ {0}, \sigma^ {2}) = \sum_ {t = 1} ^ {n} \log \left[ \frac {1}{\sqrt {2 \pi \sigma^ {2}}} \exp \left(- \frac {1}{2 \sigma^ {2}} (y _ {t} - \theta^ {T} {\bf x} _ {t} - \theta_ {0}) ^ {2}\right) \right]\tag{6}
$$

$$
= \sum_ {t = 1} ^ {n} \left[ - \frac {1}{2} \log (2 \pi) - \frac {1}{2} \log \sigma^ {2} - \frac {1}{2 \sigma^ {2}} (y _ {t} - \theta^ {T} {\bf x} _ {t} - \theta_ {0}) ^ {2} \right]\tag{7}
$$

$$
{ = } { \mathrm{const.} - \frac { n } { 2 } \log \sigma ^ { 2 } - \frac { 1 } { 2 \sigma ^ { 2 } } \sum _ { t = 1 } ^ { n } ( y _ { t } - \theta ^ { T } \mathbf { x } _ { t } - \theta _ { 0 } ) ^ { 2 } }\tag{8}
$$

where ’const.’ absorbs terms that do not depend on the parameters. Now, the problem of estimating the parameters $\theta$ and $\theta _ { 0 }$ is nicely decoupled from estimating $\sigma ^ { 2 }$ . In other words, we can find the maximizing $\hat { \theta }$ and $\hat { \theta } _ { 0 }$ by simply minimizing the mean squared error 

$$
\sum_ {t = 1} ^ {n} (y _ {t} - \theta^ {T} \mathbf {x} _ {t} - \theta_ {0}) ^ {2}\tag{9}
$$

It is perhaps easiest to write the solution based on a bit of matrix calculation. Let X be a matrix whose rows, indexed by training examples, are given by $[ \mathbf { x } _ { t } ^ { T } , 1 ] \ ( \mathbf { x } _ { t }$ turned into a row vector and 1 added at the end). In terms of this matrix, the minimization problem 

6.867 Machine learning, lecture 5 (Jaakkola) 

becomes 

$$
\sum_ {t = 1} ^ {n} \left(y _ {t} - \left[ \begin{array}{c} \theta \\ \theta_ {0} \end{array} \right] ^ {T} \left[ \begin{array}{c} \mathbf {x} _ {t} \\ 1 \end{array} \right]\right) ^ {2} = \sum_ {t = 1} ^ {n} \left(y _ {t} - \left[ \mathbf {x} _ {t} ^ {T}, 1 \right] \left[ \begin{array}{c} \theta \\ \theta_ {0} \end{array} \right]\right) ^ {2}\tag{10}
$$

$$
= \left\| \left[ \begin{array}{c} y _ {1} \\ \dots \\ y _ {n} \end{array} \right] - \left[ \begin{array}{c} \mathbf {x} _ {1} ^ {T}, 1 \\ \dots \\ \mathbf {x} _ {n} ^ {T}, 1 \end{array} \right] \left[ \begin{array}{c} \theta \\ \theta_ {0} \end{array} \right] \right\| ^ {2}\tag{11}
$$

$$
= \left\| \mathbf {y} - \mathbf {X} \left[ \begin{array}{c} \theta \\ \theta_ {0} \end{array} \right] \right\| ^ {2}\tag{12}
$$

$$
= \mathbf {y} ^ {T} \mathbf {y} - 2 \left[ \begin{array}{l} \theta \\ \theta_ {0} \end{array} \right] ^ {T} \mathbf {X} ^ {T} \mathbf {y} + \left[ \begin{array}{l} \theta \\ \theta_ {0} \end{array} \right] ^ {T} \mathbf {X} ^ {T} \mathbf {X} \left[ \begin{array}{l} \theta \\ \theta_ {0} \end{array} \right]\tag{13}
$$

where $\mathbf { y } = [ y _ { 1 } , \dots , y _ { n } ] ^ { T }$ is a vector of training responses. Solving it yields 

$$
\left[ \begin{array}{l} \hat {\theta} \\ \hat {\theta} _ {0} \end{array} \right] = (\mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} \mathbf {X} ^ {T} \mathbf {y}\tag{14}
$$

Note that the optimal parameter values are linear functions of the observed responses $\mathbf { y }$ . We will make use of this property later on. The dependence on the training inputs $\mathbf { x } _ { 1 } , \ldots , \mathbf { x } _ { n }$ (or the matrix $\mathbf { X } )$ is non-linear, however. 

The noise variance can be subsequently set to account for the remaining prediction errors. Indeed, the the maximizing value of $\sigma ^ { 2 }$ is given by 

$$
\hat {\sigma} ^ {2} = \frac {1}{n} \sum_ {t = 1} ^ {n} (y _ {t} - \hat {\theta} ^ {T} \mathbf {x} _ {t} - \hat {\theta} _ {0}) ^ {2}\tag{15}
$$

which is the average squared prediction error. Note that we cannot compute $\hat { \sigma } ^ { 2 }$ before knowing how well the linear model explains the responses. 

## Bias and variance of the parameter estimates

We can make use of the closed form parameter estimates in Eq.(14) to analyze how good these estimates are. For this purpose let’s make the strong assumption that the actual relation between x and y follows a linear model of the same type that we are estimating (we just don’t know the correct parameter values $\theta ^ { * } , \theta _ { 0 } ^ { * }$ , and $\sigma ^ { * 2 } )$ ). We can therefore describe the observed responses $y _ { t }$ as 

$$
y _ {t} = \theta^ {* T} \mathbf {x} _ {t} + \theta_ {0} ^ {*} + \epsilon_ {t}, t = 1, \ldots , n\tag{16}
$$

where $\epsilon _ { t } \sim N ( 0 , \sigma ^ { * 2 } )$ . In a matrix form 

$$
\mathbf {y} = \mathbf {X} \left[ \begin{array}{c} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right] + \mathbf {e}\tag{17}
$$

where $\mathbf { e } = [ \epsilon _ { 1 } , \hdots , \epsilon _ { n } ] ^ { T } , E \{ \mathbf { e } \} = 0$ and $E \{ \mathbf { e e } ^ { T } \} = \sigma ^ { * 2 } \mathbf { I }$ . The noise vector e is also independent of the inputs or X. Plugging this form of responses into Eq.(14) we get 

$$
\left[ \begin{array}{l} \hat {\theta} \\ \hat {\theta} _ {0} \end{array} \right] = (\mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} \mathbf {X} ^ {T} (\mathbf {X} \left[ \begin{array}{l} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right] + \mathbf {e})\tag{18}
$$

$$
= (\mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} \mathbf {X} ^ {T} \mathbf {X} \left[ \begin{array}{l} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right] + (\mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} \mathbf {X} ^ {T} \mathbf {e}\tag{19}
$$

$$
= \left[ \begin{array}{l} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right] + (\mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} \mathbf {X} ^ {T} \mathbf {e}\tag{20}
$$

In other words, our parameter estimates can be decomposed into the sum of correct underlying parameters and estimates based on noise alone (i.e., based on e). Thus, on average with fixed inputs 

$$
E \{\left[ \begin{array}{l} \hat {\theta} \\ \hat {\theta} _ {0} \end{array} \right] | \mathbf {X} \} = \left[ \begin{array}{l} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right] + (\mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} \mathbf {X} ^ {T} E \{\mathbf {e} | \mathbf {X} \} = \left[ \begin{array}{l} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right]\tag{21}
$$

Our parameter estimates are therefore unbiased or correct on average when averaging is over possible training sets we could generate. The averaging here is conditioned on the specific training inputs. 

Using Eq.(20) and Eq.(21) we can also evaluate the conditional co-variance of the parameter estimates where the expectation is again over the noise in the outputs: 

$$
C o v \{\left[ \begin{array}{c} \hat {\theta} \\ \hat {\theta} _ {0} \end{array} \right] | \mathbf {X} \} = E \left\{\left(\left[ \begin{array}{c} \hat {\theta} \\ \hat {\theta} _ {0} \end{array} \right] - \left[ \begin{array}{c} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right]\right) \left(\left[ \begin{array}{c} \hat {\theta} \\ \hat {\theta} _ {0} \end{array} \right] - \left[ \begin{array}{c} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right]\right) ^ {T} | \mathbf {X} \right\}\tag{22}
$$

$$
= E \left\{\left((\mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} \mathbf {X} ^ {T} \mathbf {e}\right) \left((\mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} \mathbf {X} ^ {T} \mathbf {e}\right) ^ {T} | \mathbf {X} \right\}\tag{23}
$$

$$
= E \left\{\left(\mathbf {X} ^ {T} \mathbf {X}\right) ^ {- 1} \mathbf {X} ^ {T} \mathbf {e e} ^ {T} \mathbf {X} \left(\mathbf {X} ^ {T} \mathbf {X}\right) ^ {- 1} | \mathbf {X} \right\}\tag{24}
$$

$$
= \left(\mathbf {X} ^ {T} \mathbf {X}\right) ^ {- 1} \mathbf {X} ^ {T} E \{\mathbf {e e} ^ {T} | \mathbf {X} \} \mathbf {X} \left(\mathbf {X} ^ {T} \mathbf {X}\right) ^ {- 1}\tag{25}
$$

$$
= (\mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} \mathbf {X} ^ {T} (\sigma^ {* 2} \mathbf {I}) \mathbf {X} (\mathbf {X} ^ {T} \mathbf {X}) ^ {- 1}\tag{26}
$$

$$
= \sigma^ {* 2} (\mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} \mathbf {X} ^ {T} \mathbf {X} (\mathbf {X} ^ {T} \mathbf {X}) ^ {- 1}\tag{27}
$$

$$
{ = } { \sigma ^ { * 2 } ( \mathbf { X } ^ { T } \mathbf { X } ) ^ { - 1 } }\tag{28}
$$

So the way in which the parameters vary in response to noise in the outputs is a function of the inputs or X. We will use this property in the next section to select inputs so as to improve the quality of the parameter estimates or to reduce the variance of predictions. 

Based on the bias and variance calculations we can evaluate the mean squared error of the parameter estimates. To this end, we use the fact that the expectation of the squared norm of any vector valued random variable can be decomposed into a bias and variance components as follows: 

$$
E \left\{\| \mathbf {z} - \mathbf {z} ^ {*} \| ^ {2} \right\} = E \left\{\| \mathbf {z} - E \{\mathbf {z} \} + E \{\mathbf {z} \} - \mathbf {z} ^ {*} \| ^ {2} \right\}\tag{29}
$$

$$
= E \left\{\| \mathbf {z} - E \{\mathbf {z} \} \| ^ {2} + 2 (\mathbf {z} - E \{\mathbf {z} \}) ^ {T} (E \{\mathbf {z} \} - \mathbf {z} ^ {*}) + \| E \{\mathbf {z} \} - \mathbf {z} ^ {*} \| ^ {2} \right\}\tag{30}
$$

$$
= E \left\{\| \mathbf {z} - E \{\mathbf {z} \} \| ^ {2} \right\} + 2 E \left\{(\mathbf {z} - E \{\mathbf {z} \}) ^ {T} \right\} (E \{\mathbf {z} \} - \mathbf {z} ^ {*}) + \| E \{\mathbf {z} \} - \mathbf {z} ^ {*} \| ^ {2}
$$

$$
= \overbrace {E \left\{\| \mathbf {z} - E \{\mathbf {z} \} \| ^ {2} \right\}} ^ {\text {variance}} + \overbrace {\| E \{\mathbf {z} \} - \mathbf {z} ^ {*} \| ^ {2}} ^ {\text {bias} ^ {2}}\tag{31}
$$

where we have assumed that $\mathbf { z } ^ { \ast }$ is fixed. Make sure you understand how this decomposition is derived. We will further elaborate the variance part to better use the result in our context: 

$$
E \left\{\| \mathbf {z} - E \{\mathbf {z} \} \| ^ {2} \right\} = E \left\{(\mathbf {z} - E \{\mathbf {z} \}) ^ {T} (\mathbf {z} - E \{\mathbf {z} \}) \right\}\tag{32}
$$

$$
= E \left\{T r \left[ (\mathbf {z} - E \{\mathbf {z} \}) ^ {T} (\mathbf {z} - E \{\mathbf {z} \}) \right] \right\}\tag{33}
$$

$$
= E \left\{T r \left[ (\mathbf {z} - E \{\mathbf {z} \}) (\mathbf {z} - E \{\mathbf {z} \}) ^ {T} \right] \right\}\tag{34}
$$

$$
= T r \left[ E \Bigg \{(\mathbf {z} - E \{\mathbf {z} \}) (\mathbf {z} - E \{\mathbf {z} \}) ^ {T} \Bigg \} \right]\tag{35}
$$

$$
= T r [ C o v \{\mathbf {z} \} ]\tag{36}
$$

where $T r [ \cdot ]$ is the matrix trace, the sum of its diagonal components, and therefore a linear operation (exchangeable with the expectation). We have also used the fact that $T r [ { \bf a } ^ { T } { \bf b } ] =$ $T r [ \mathbf { a b } ^ { T } ]$ for any vectors a and b. 

6.867 Machine learning, lecture 5 (Jaakkola) 

Now, adapting the result to our setting, we get 

$$
\begin{array}{r l} E \left\{\left\| \left[ \begin{array}{c} \hat {\theta} \\ \hat {\theta} _ {0} \end{array} \right] - \left[ \begin{array}{c} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right] \right\| ^ {2} | \mathbf {X} \right\} & = \overbrace {T r \left[ C o v \left\{\left[ \begin{array}{c} \hat {\theta} \\ \hat {\theta} _ {0} \end{array} \right] | \mathbf {X} \right\} \right]} ^ {\text {variance}} + \overbrace {\left\| E \left\{\left[ \begin{array}{c} \hat {\theta} \\ \hat {\theta} _ {0} \end{array} \right] | \mathbf {X} \right\} - \left[ \begin{array}{c} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right] \right\| ^ {2}} ^ {\text {bias} ^ {2} = 0} \\ & = \sigma^ {* 2} T r [ (\mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} ] \end{array} \tag {37}
$$

Let’s understand this result a bit further. How does it depend on n, the number of training examples? In other words, how quickly does the mean squared error decrease as the number of training examples increases, assuming the input examples x are sampled independently from some underlying distribution $P ( \mathbf { x } ) !$ To answer this let’s start by analyzing what happens to the matrix ${ \bf X } ^ { T } { \bf X }$ 

$$
\mathbf {X} ^ {T} \mathbf {X} = \sum_ {t = 1} ^ {n} \left[ \begin{array}{c} \mathbf {x} _ {t} \\ 1 \end{array} \right] [ \mathbf {x} _ {t} ^ {T}, 1 ]\tag{38}
$$

$$
= n \cdot \frac {1}{n} \sum_ {t = 1} ^ {n} \left[ \begin{array}{c} \mathbf {x} _ {t} \\ 1 \end{array} \right] [ \mathbf {x} _ {t} ^ {T}, 1 ]\tag{39}
$$

$$
\approx n \cdot E _ {\mathbf {x} \sim P} \left\{\left[ \begin{array}{l} \mathbf {x} \\ 1 \end{array} \right] [ \mathbf {x} ^ {T}, 1 ] \right\} = n \cdot \mathbf {C}\tag{40}
$$

where for large n the average will be close to the corresponding expected value. For large n the mean squared error of the parameter estimates will therefore be close to 

$$
\frac {\sigma^ {* 2}}{n} \cdot T r [ \mathbf {C} ^ {- 1} ]\tag{41}
$$

The variance of simply averaging the (noise in the) outputs would behave as $\sigma ^ { * 2 } / n$ . Since we are estimating $d + 1$ parameters where d is the input dimension, this dependence would have to be in $T r [ \mathbf { C } ^ { - 1 } ]$ . Indeed it is. This term, a trace of a $( d + 1 ) \times ( d + 1 )$ matrix $\mathbf { C } ^ { - 1 }$ is directly proportional to $d + 1$ 

## Penalized log-likelihood and Ridge regression

When the number of training examples is small, i.e., not too much larger than the number of parameters (dimension of the inputs), it is often beneficial to regularize the parameter estimates. We will derive the form of regularization here by assigning a prior distribution over the parameters $P ( \theta , \theta _ { 0 } )$ . The purpose of the prior is to prefer small parameter values (predict values close to zero) in the absence of data. Specifically, we will look at simple zero mean Gaussian distributions 

$$
P (\theta , \theta_ {0}; \sigma^ {\prime 2}) = N (\left[ \begin{array}{l} \theta \\ \theta_ {0} \end{array} \right]; \left[ \begin{array}{l} 0 \\ 0 \end{array} \right], \sigma^ {\prime 2} \mathbf {I}) = N (\theta_ {0}; 0, \sigma^ {\prime 2}) \prod_ {j = 1} ^ {d} N (\theta_ {j}; 0, \sigma^ {\prime 2})\tag{42}
$$

where the variance parameter $\sigma ^ { \prime 2 }$ in the prior distribution specifies how strongly we wish to bias the parameters towards zero. 

By combining the log-likelihood criterion with the prior we obtain a penalized log-likelihood function (penalized by the prior): 

$$
\begin{array}{r c l} {l ^ {\prime} (\theta , \theta_ {0}, \sigma^ {2})} & = & {\sum_ {t = 1} ^ {n} \log \left[ \frac {1}{\sqrt {2 \pi \sigma^ {2}}} \exp \left(- \frac {1}{2 \sigma^ {2}} (y _ {t} - \theta^ {T} \mathbf {x} _ {t} - \theta_ {0}) ^ {2}\right) \right] + \log P (\theta , \theta_ {0}; \sigma^ {\prime 2})} \\ & = & {\mathrm{const.} - \frac {n}{2} \log \sigma^ {2} - \frac {1}{2 \sigma^ {2}} \sum_ {t = 1} ^ {n} (y _ {t} - \theta^ {T} \mathbf {x} _ {t} - \theta_ {0}) ^ {2}} \\ & & {- \frac {1}{2 \sigma^ {\prime 2}} (\theta_ {0} ^ {2} + \sum_ {j = 1} ^ {d} \theta_ {j} ^ {2}) - \frac {d + 1}{2} \log \sigma^ {\prime 2}} \end{array}\tag{43}
$$

(44) 

It is convenient to tie the prior variance $\sigma ^ { \prime 2 }$ to the noise variance $\sigma ^ { 2 }$ according to $\sigma ^ { \prime 2 } = \sigma ^ { 2 } / \lambda$ This has the efect that if the noise variance $\sigma ^ { 2 }$ is large, we penalize the parameters very little (permit large deviations from zero by assuming a large $\sigma ^ { \prime 2 } )$ . On the other hand, if the noise variance is small, we could be over-fitting the linear model. This happens, for example, when the number of training examples is small. In this case most of the responses can be explained directly by the linear model making the noise variance very small. In such cases our penalty for the parameters will be larger as well (prior variance is smaller). 

Incorporating this parameter tie into the penalized log-likelihood function gives 

$$
l ^ {\prime} (\theta , \theta_ {0}, \sigma^ {2}) = \mathrm{const.} - \frac {n}{2} \log \sigma^ {2} - \frac {1}{2 \sigma^ {2}} \sum_ {t = 1} ^ {n} (y _ {t} - \theta^ {T} \mathbf {x} _ {t} - \theta_ {0}) ^ {2}
$$

$$
- \frac {\lambda}{2 \sigma^ {2}} (\theta_ {0} ^ {2} + \sum_ {j = 1} ^ {d} \theta_ {j} ^ {2}) - \frac {d + 1}{2} \log (\sigma^ {2} / \lambda)\tag{45}
$$

$$
= \mathrm{const.} - \frac {n + d + 1}{2} \log \sigma^ {2} + \frac {d + 1}{2} \log \lambda\tag{46}
$$

$$
- \frac {1}{2 \sigma^ {2}} \left[ \sum_ {t = 1} ^ {n} (y _ {t} - \theta^ {T} {\bf x} _ {t} - \theta_ {0}) ^ {2} + \lambda (\theta_ {0} ^ {2} + \sum_ {j = 1} ^ {d} \theta_ {j} ^ {2}) \right]
$$

(47) 

where again the estimation of θ and $\theta _ { 0 }$ separates from setting the noise variance $\sigma ^ { 2 }$ . Note that this separation is achieved because we tied the prior and noise variance parameters. The above regularized problem of finding the parameter estimates $\hat { \theta }$ and $\widehat { \theta } _ { 0 }$ is known as Ridge regression. 

As before, we can get closed form estimates for the parameters (we omit the analogous derivation): 

$$
\left[ \begin{array}{l} \hat {\theta} \\ \hat {\theta} _ {0} \end{array} \right] = (\lambda \mathbf {I} + \mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} \mathbf {X} ^ {T} \mathbf {y}\tag{48}
$$

It is now useful to understand how the properties of these parameter estimates depend on λ. For example, are the parameter estimates unbiased? No, they are not: 

$$
\begin{array}{r l r} {E \left\{\left[ \begin{array}{l} \hat {\theta} \\ \hat {\theta} _ {0} \end{array} \right] | \mathbf {X} \right\}} & = & {(\lambda \mathbf {I} + \mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} \mathbf {X} ^ {T} \mathbf {X} \left[ \begin{array}{l} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right]} \end{array}\tag{49}
$$

$$
= (\lambda \mathbf {I} + \mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} (\mathbf {X} ^ {T} \mathbf {X} + \lambda \mathbf {I} - \lambda \mathbf {I}) \left[ \begin{array}{l} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right]\tag{50}
$$

$$
= \left[ \begin{array}{l} \theta^ {*} \\ \hat {\theta} _ {0} ^ {*} \end{array} \right] \overbrace {- \lambda (\lambda \mathbf {I} + \mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} \left[ \begin{array}{l} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right]} ^ {}\tag{51}
$$

$$
= \left(\mathbf {I} - \lambda (\lambda \mathbf {I} + \mathbf {X} ^ {T} \mathbf {X}) ^ {- 1}\right) \left[ \begin{array}{c} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right]\tag{52}
$$

It is straightforward to check that $\left( \mathbf { I } - \lambda ( \lambda \mathbf { I } + \mathbf { X } ^ { T } \mathbf { X } ) ^ { - 1 } \right)$ is a positive definite matrix with eigenvalues all less than one. The parameter estimates are therefore shrunk towards zero and more so the larger the value of λ. This is what we would expect since we explicitly favored small parameter values with the prior penalty. What do we gain from such biased parameter estimates? Let’s evaluate the mean squared error, starting with the covariance: 

$$
{C o v \left\{\left[ \begin{array}{l} \hat {\theta} \\ \hat {\theta} _ {0} \end{array} \right] | \mathbf {X} \right\}} = {\sigma^ {* 2} (\lambda \mathbf {I} + \mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} \mathbf {X} ^ {T} \mathbf {X} (\lambda \mathbf {I} + \mathbf {X} ^ {T} \mathbf {X}) ^ {- 1}}\tag{53}
$$

$$
= \sigma^ {* 2} (\lambda \mathbf {I} + \mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} (\lambda \mathbf {I} + \mathbf {X} ^ {T} \mathbf {X} - \lambda \mathbf {I}) (\lambda \mathbf {I} + \mathbf {X} ^ {T} \mathbf {X}) ^ {- 1}\tag{54}
$$

$$
{ = } { \sigma ^ { * 2 } ( \lambda \mathbf { I } + \mathbf { X } ^ { T } \mathbf { X } ) ^ { - 1 } - \lambda \sigma ^ { * 2 } ( \lambda \mathbf { I } + \mathbf { X } ^ { T } \mathbf { X } ) ^ { - 2 } }\tag{55}
$$

The mean squared error in the parameters is therefore given by (we again omit the deriva-

tion that can be obtained similarly to previous expressions): 

$$
\begin{array}{r l r} {E \left\{\left\| \left[ \begin{array}{l} \hat {\theta} \\ \hat {\theta} _ {0} \end{array} \right] - \left[ \begin{array}{l} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right] \right\| ^ {2} | \mathbf {X} \right\}} & = & {\sigma^ {* 2} \cdot T r \left[ (\lambda \mathbf {I} + \mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} - \lambda (\lambda \mathbf {I} + \mathbf {X} ^ {T} \mathbf {X}) ^ {- 2} \right]} \\ & & {+ \lambda^ {2} \left[ \begin{array}{l} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right] ^ {T} (\lambda \mathbf {I} + \mathbf {X} ^ {T} \mathbf {X}) ^ {- 2} \left[ \begin{array}{l} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right]} \end{array}\tag{56}
$$

Can this be smaller than the mean squared error corresponding to the unregularized estimates $\sigma ^ { * 2 } \cdot T r \left[ ( \mathbf { X } ^ { T } \mathbf { X } ) ^ { - 1 } \right] ?$ Yes, it can. This is indeed the benefit from regularization: we can reduce large variance at the cost of introducing a bit of bias. We will get back to this trade-of in the context of model selection. 

Let’s exemplify the efect of λ on the mean squared error in a context of a very simple 1-dimensional example. Suppose, we have observed responses for only two points, $x = - 1$ and $x = 1$ . In this case, 

$$
\mathbf {X} = \left[ \begin{array}{c c} - 1 & 1 \\ 1 & 1 \end{array} \right], \mathbf {X} ^ {T} \mathbf {X} = \left[ \begin{array}{c c} 2 & 0 \\ 0 & 2 \end{array} \right], (\lambda \mathbf {I} + \mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} = \left[ \begin{array}{c c} 1 / (2 + \lambda) & 0 \\ 0 & 1 / (2 + \lambda) \end{array} \right]\tag{57}
$$

The expression for the mean squared error therefore becomes 

$$
\begin{array}{r l r} {E \left\{\left\| \left[ \begin{array}{l} \hat {\theta} \\ \hat {\theta} _ {0} \end{array} \right] - \left[ \begin{array}{l} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right] \right\| ^ {2} | \mathbf {X} \right\}} & = & {\sigma^ {* 2} \left(\frac {2}{(2 + \lambda)} - \frac {2 \lambda}{(2 + \lambda) ^ {2}}\right) + \frac {\lambda^ {2}}{(2 + \lambda) ^ {2}} (\theta^ {* 2} + \theta_ {0} ^ {* 2})} \\ & & {= \frac {4 \sigma^ {* 2}}{(2 + \lambda) ^ {2}} + \frac {\lambda^ {2}}{(2 + \lambda) ^ {2}} (\theta^ {* 2} + \theta_ {0} ^ {* 2})} \end{array}\tag{58}
$$

We should compare this to $\sigma ^ { * 2 } T r \left. ( \mathbf { X } ^ { T } \mathbf { X } ) ^ { - 1 } \right. = \sigma ^ { * 2 }$ obtained without regularization (corresponds to set ting $\stackrel { \triangledown } { \ = } 0$ In the noisy case $\sigma ^ { * 2 } > \theta ^ { * 2 } + \theta _ { 0 } ^ { * 2 }$ we can set $\lambda = 2$ and obtain 

$$
E \left\{\left\| \left[ \begin{array}{c} \hat {\theta} \\ \hat {\theta} _ {0} \end{array} \right] - \left[ \begin{array}{c} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right] \right\| ^ {2} | \mathbf {X} \right\} = \frac {4 \sigma^ {* 2}}{1 6} + \frac {4}{1 6} (\theta^ {* 2} + \theta_ {0} ^ {* 2}) <   \frac {8 \sigma^ {* 2}}{1 6} = \frac {1}{2} \sigma^ {* 2}\tag{59}
$$

The mean squared error of the parameters is therefore clearly smaller than without regularization. 

## Active learning

We can use the expressions for the mean squared error to actively select input points $\mathbf { x } _ { 1 } , \ldots , \mathbf { x } _ { n }$ , when possible, so as to reduce the resulting estimation error. This is an active learning (experiment design) problem. The goal is to get by with as few responses as possible without sacrificing the estimation accuracy. For example, in training a classifier we would like to minimize the number of training images we would have to label in order obtain a certain classification accuracy. In the regression context, we may be selecting among possible experiments to carry out (e.g., choosing diferent operating points for a factory or gauging market/customer responses to diferent strategies available to us). By letting the method guide the selection of the training examples (inputs), we will generally need far fewer examples in comparison to selecting them at random from some underlying distribution, database, or trying available experiments at random. Fewer responses means less human efort, less cost, or both. 

To develop this further let’s go back to the unregularized case where 

$$
E \left\{\left\| \left[ \begin{array}{c} \hat {\theta} \\ \hat {\theta} _ {0} \end{array} \right] - \left[ \begin{array}{c} \theta^ {*} \\ \theta_ {0} ^ {*} \end{array} \right] \right\| ^ {2} | \mathbf {X} \right\} = \sigma^ {* 2} T r \left[ (\mathbf {X} ^ {T} \mathbf {X}) ^ {- 1} \right]\tag{60}
$$

We do not know the noise variance $\sigma ^ { * 2 }$ for the correct model but it only appears as a multiplicative constant in the above expression and therefore won’t afect how we should choose the inputs. When the choice of inputs is indeed up to us (e.g., which experiments to carry out) we can select them so as to minimize $T r \left[ ( { \bf X } ^ { T } { \bar { \bf X } } ) ^ { - 1 } \right]$ . One caveat of this approach is that it relies on the underlying relationship between the inputs and the responses to be linear. When this is no longer the case we may end up with clearly suboptimal selections. 

We will discuss next time how we can find say n input examples $\mathbf { x } _ { 1 } , \ldots , \mathbf { x } _ { n }$ that minimize the criterion. 