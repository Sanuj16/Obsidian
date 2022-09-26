We turn now to a formal mathematical setting for analyzing the randomized algorithm. Any probabilistic statement must refer to the underlying probability space.

In most of this course, we are using discrete probability spaces. In a discrete probability space, the sample space $\Omega$ is finite or countably infinite, and the family $F$ of allowable events consists of all subsets of $\Omega$. In a discrete probability space $F=2^\Omega$.

## [[Definition 1.1]]
## [[Definition 1.2]]
## [[Lemma 1.1]]
## [[Lemma 1.2]]
## [[Lemma 1.3]]

$Pr(algorithm fails) = Pr(E) \le \frac{d}{100d} = \frac{1}{100}$
Two ways to decrease the error:
- Increase the sample space
- Run the algorithm multiple times
	- with replacement : let us say the number of iterations is k, then the probability of chooosing roots of $F(x)-G(x)$, i.e., wrong answer for k iterations would be at most $(\frac{1}{100})^k$ 
	- without replacement

## [[Definition 1.3]]
## [[Theorem 1.8]]

