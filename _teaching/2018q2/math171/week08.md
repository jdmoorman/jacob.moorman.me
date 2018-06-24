---
layout: course_notes
number: Math 171
quarter: Spring 2018
week: 8
topics:
  - Exponential Distribution
  - Poisson Process Basics
---

1. **{{ page.topics[0] }}**

    2. Let \\(X \sim \mathrm{exp}(\lambda)\\).

        3. Find the distribution of \\(Y = \lceil X \rceil\\)

            * (<font color="red">Answer</font>) \\(\mathrm{geometric}(1-e^{-\lambda})\\)

        3. Show that \\(X\\) and \\(Y\\) are both memoryless

        3. Find the distribution of \\(\beta X\\)

            * (<font color="red">Answer</font>) \\(\mathrm{exponential}(\lambda/\beta)\\)

        3. Find the distribution of \\(e^{-X}\\)

            * (<font color="blue">Solution</font>) Let \\(Y = e^{-X}\\). Note since \\(X \in [0, \infty)\\) we have \\(Y \in (0, 1]\\). \\[\begin{aligned}F\_Y(y) &= P(Y \le y)\\\\ &= P(e^{-X}\le y)\\\\&=P(-X \le \log(y))\\\\&= P(X \ge -\log(y))\\\\&=1-F\_X(-\log(y))\end{aligned}\\] \\[\begin{aligned}f\_Y(y) &= \frac{d}{dy}F\_Y(y) \\\\ &= \frac{d}{dy}(1 - F\_X(-\log(y))) \\\\ &= -f\_X(-\log(y))\cdot \frac{-1}{y} \\\\ &= \frac{\lambda e^{-\lambda (-\log(y))}}{y} \\\\ &= \lambda y^{\lambda - 1}\end{aligned}\\]

    2. Let \\(U \sim \mathrm{uniform}[0,1]\\). Find the distribution of \\(-\alpha\log{U}\\)

        * (<font color="red">Answer</font>) \\(\mathrm{exponential}(1/\alpha)\\)

    2. Let \\(X\_1, X\_2, \dots\overset{\mathrm{i.i.d}}{\sim} \mathrm{exp}(\lambda)\\)

        3. (<font color="green">Discussed</font>) Suppose \\(N \sim \mathrm{geo}(p)\\). Find the distribution of \\(Z = \sum\_{i=1}^N X\_i\\).

        3. Find the distribution of \\(Q = \min(X\_1, X\_2, \dots X\_n)\\)

            * (<font color="red">Answer</font>) \\(\mathrm{exponential}(n\lambda)\\)

        3. Find the cumulative distribution of \\(V = \max(X\_1, X\_2, \dots X\_n)\\)

            * (<font color="red">Answer</font>) \\((1-e^{-v\lambda})^n\\)

1. **{{ page.topics[1] }}**

    2. Let \\(N(t)\\) be a poisson process with rate \\(\lambda\\)

        3. (<font color="green">Discussed</font>) Find the probability of no arrivals in \\((3,5]\\)

        3. (<font color="green">Discussed</font>) Find the probability that there is exactly one arrival in each of the intervals: \\((0,1], (1,2], (2,3], (3,4]\\)

        3. (<font color="green">Discussed</font>) Find the probability that there are two arrivals in \\((0,2]\\) and three arrivals in \\((1,4]\\)

        3. (<font color="green">Discussed</font>) Find the covariance of \\(N(t\_1)\\) and \\(N(t\_2)\\) for \\(0 < t\_1 < t\_2\\)




