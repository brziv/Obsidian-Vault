#theory

We want to find the maximum profit from a rod, by deciding if we should cut it or not, and if we cut, where to cut and how many times.

The idea is to go from the very bottom, slowly solve the sub-problems, use the results to solve larger sub-problems, and eventually the problem will be solved.

For length i, we compare the profit you get from all combinations of *two* cuts and choose the maximum value. For each combination, one value we get from the price for that one length, and the other from the *previous* computation we've already done. The previous solutions are just achieved by doing the same until we reach 1.

`dp[i] = max(price[j - 1] + dp[i - j])` from 1 to i (bottom-up)
