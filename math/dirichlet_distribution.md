- [Bayes theorem](#bayes-theorem)
- [Bernoulli distribution & beta distribution](#bernoulli-distribution--beta-distribution)
- [Multinomial distribution & dirichlet distribution](#multinomial-distribution--dirichlet-distribution)
- [结论](#结论)
- [附录](#附录)
  - [Beta distribution](#beta-distribution)
  - [Multinomial distribution](#multinomial-distribution)

## Bayes theorem
$$
P(q|x)P(x)=P(X=x|q)P(q)
$$

其中$P(q)$表示关于$q$的先验概率，$P(q|x)$是观测到x之后得到的关于$q$的后验概率，且$P(x)$为常量，方程两边由P(q)得到f(q)，而由P(q|x)得到f(q|x)，得到结论：**关于q的后验概率密度f(q|x)就和"关于q的先验概率密度乘以一个条件概率"成比**，即：
$$
f(q|x)\approx P(X=x|q)f(q)
$$

## Bernoulli distribution & beta distribution
一次试验有两个结果的重复试验称为Bernoulli trial，其分布为Bernoulli distribution，均匀分布的先验密度函数可以被Beta distribution描述；

## Multinomial distribution & dirichlet distribution
这时候上面的Bernoulli trial就要变成有一次trial有k个可能的结果； Bernoulli distribution就变成Multinomial distribution。而beta distribution所表述的先验分布，也要改写成一个多结果版本的先验分布。那就是dirichlet distribution。

## 结论
Beta分布是二项式分布的共轭分布，Dirichlet分布是多项式分布的共轭分布

## 附录
### Beta distribution


### Multinomial distribution