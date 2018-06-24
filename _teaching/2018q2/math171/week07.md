---
layout: course_notes
number: Math 171
quarter: Spring 2018
week: 7
topics:
  - Martingales
  - Optional Stopping
---

1. **{{ page.topics[0] }}**

    2. Let \\((X\_n)\_{n \ge 0}\\) be i.i.d. uniform on \\([-1, 0) \cup (0, 1]\\)

        3. Show that \\((M\_n)\_{n \ge 0}\\) with \\(M\_n = X\_0 + \dots + X\_n\\) is a Martingale.

        3. Show that \\((M\_n)\_{n \ge 0}\\) with \\(M\_n = \frac{1}{X\_0} + \dots + \frac{1}{X\_n}\\) is not a Martingale.

            * (<font color="red">Answer</font>) \\(\mathbb{E}\|M\_n\| = \infty\\)

    2. Let \\((X\_n)\_{n \ge 1}\\) be i.i.d. uniform on \\(\\{-1, 1\\}\\). AKA Rademacher distributed. Let \\(S\_n = X\_1 + \dots + X\_n\\), \\(S_0 = 0\\).

        3. Compute the moment generating function of \\(S\_n\\). That is, \\(\mathbb{E}[e^{tS\_n}]\\)

            * (<font color="red">Answer</font>) \\(\left(\frac{e^t + e^{-t}}{2}\right)^n\\)

        3. Find the odd moments of \\(S\_n\\). That is, \\(\mathbb{E}[S\_n^{2m+1}]\\). Explain briefly why the result makes sense.

            * (<font color="red">Answer</font>) 0. Makes sense because \\(S_n\\) is symmetric about 0.

        3. Find a formula for the even moments of \\(S\_n\\). That is, \\(\mathbb{E}[S\_n^{2m}]\\).

            * (<font color="red">Answer</font>) \\(\sum\_{k=0}^n \binom{n}{k}\left(\frac{1}{2}\right)^n (2k-n)^{2m}\\)

        3. For what values of \\(c\_n\\) is \\(M\_n = S\_n^2 - c\_n\\) a martingale?

            * (<font color="red">Answer</font>) \\(c_n = n\\)

        3. Find a formula for \\(\mathbb{E}[S\_{n+1}^{2m} \mid S\_n=t]\\) which depends only on \\(m\\) and \\(t\\)

            * (<font color="red">Answer</font>) \\(\sum\_{k=0}^m {2m \choose 2k} t^{2k}\\)

1. **{{ page.topics[1] }}**

    2. Problem 5.16 from the textbook (2nd edition) 

    2. Problem 5.17 from the textbook (2nd edition) 

    2. Problem 5.8 from the textbook (2nd edition) 
