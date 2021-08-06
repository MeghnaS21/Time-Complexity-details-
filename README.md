# Time-Complexity-details-
We often get confused with the exact meanings of different kinds of asymptotic notations. In the case of beginners, we always find ourselves in the middle of this time complexity mess.  Feel free to edit this repository.

# What’s the Difference Between Big O, Big Omega, and Big Theta?
In Introduction to Algorithms, Cormen et al use Insertion Sort as an example to explain the difference between Big O, Big Omega, and Big Theta. We’ll do the same here.

# What is Big O?

## Big O describes the upper bound of an algorithm.

Using our Insertion Sort example, the rate of growth of our algorithm is at most quadratic, or O(n^2).

This is why, for us, as developers and practitioners, we are primarily concerned with Big O.

We want to know just how poorly an algorithm might perform.

To say that the Big O of Insertion Sort is O(n^2) doesn’t mean that Insertion Sort will always be O(n^2). The actual runtime will vary based on the input. What we are saying is that, in a worst case scenario, this is the upper bound of the performance of Insertion Sort.

Knowing this, we then need to ask ourselves the following questions:

    Are we okay with this?
    Can we do better?

# What is Big Omega?

## Big Omega describes the lower bound of an algorithm.

Using our Insertion Sort example, if the input is already sorted, then the rate of growth of our algorithm is at least linear, or Ω(n).

If only life always handed us sorted arrays. 🌼

We can also think of this as our best-case scenario.

# What is Big Theta?

## Big Theta describes the tight bound of an algorithm, it’s limit from above and below.

Using our Insertion Sort example, we know that the rate of growth is at most O(n^2) and at least Ω(n).

But Big Theta will change with our inputs. Returning to our Insertion Sort example, in a best case scenario, Big Theta is n, but in a worst case scenario, Big Theta is n^2. To say that Insertion Sort is Θ(n) or Θ(n^2) is incorrect as both of these imply that Insertion Sort will always run at either n or n^2.

# So what use is Big Theta?

## Big Theta is often used to describe the average, or expected, case for an algorithm. This isn’t exactly true, but it’s a useful shorthand.

*So for Insertion Sort, the average case for Big Theta is n^2.
So What’s the Difference Between Big O, Big Omega, and Big Theta?*

### We can think of Big O, Big Omega, and Big Theta like conditional operators:

    Big O is like <=, meaning the rate of growth of an algorithm is less than or equal to a specific value, e.g: f(x) <= O(n^2)
    Big Omega is like >=, meaning the rate of growth is greater than or equal to a specified value, e.g: f(x) >= Ω(n).
    Big Theta is like ==, meaning the rate of growth is equal to a specified value, e.g: f(x) = Θ(n^2).

But if we needed to make a blanket statement for all cases, we would use Big O, and, for example, say that Insertion Sort is O(n^2).
Best Case, Worst Case, and Expected Case

# What is the relationship between best case/worst case/expected case and Big O/Big Omega/Big Theta?

There isn’t one.

Equivalencies are often made between Big O and worst case, Big Omega and best case, and Big Theta and average case, but we can speak of best, worst, and average for each of these notations.

### For example, each of the following statements are true:

    Insertion Sort’s worst case rate of growth is at most O(n^2)
    Insertion Sort’s worst case rate of growth is at least Ω(n)
    Insertion Sort’s worst case rate of growth is exactly Θ(n^2)
