The time complexity of LightSort is O(n log n) in the average and worst cases.

To prove this, we can use the Master theorem, which provides a way to solve recurrence relations of the form T(n) = aT(n/b) + f(n), where a is the number of subproblems, n/b is the size of each subproblem, and f(n) is the time taken to divide and combine the subproblems.

For LightSort, the recurrence relation is T(n) = 2T(n/2) + O(n), where the O(n) term corresponds to the time taken to merge the sublists.

Using the Master theorem, we can see that a = 2, b = 2, and f(n) = O(n). The theorem states that if f(n) = O(n^d) for some constant d >= 0, then T(n) has the following time complexity:

If d < log_b(a), then T(n) = Theta(n^(log_b(a))).
If d = log_b(a), then T(n) = Theta(n^d * log(n)).
If d > log_b(a), then T(n) = Theta(n^d).
In the case of LightSort, we have a = 2, b = 2, and d = 1. Therefore, d < log_b(a), which means that the time complexity of LightSort is Theta(n^(log_2(2))) = Theta(n log n).

Thus, we can conclude that the time complexity of LightSort is O(n log n) in the average and worst cases.