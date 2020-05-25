#2.3
+ 2.17
    + we're dealing with EVEN numbers
    + 4 digit numbers that end in 0
        + pick 0, pick of 5 left, pick of 4 left, pick of 3 left
        + 1 * 5 * 4 * 3 = 60
    + 4 digit numbers that don't end in 0
        + must end in 2 or 6
        + let's make things simpler to reason with: pick the ending digit first,
          then the rest of the digits from L -> R
        + pick 2 or 6, pick from 4 left since can't start with 0, pick from 4 left
          since 0 is back in the mix, then pick from 3 left
        + 2 * 4 * 4 * 3 = 96
    + 96 + 60 = 156
+ the number of permutations of n objects arranged in a circle = (n - 1)!
+ 2.20
    + 10 players, so 10!
    + BUT only grades can be distinguished
    + e.g. first soph, second soph = second soph, first soph
    + so we have to divide 10! by number of repeating factors
    + 10! / (1! * 2! * 3! * 4!)
+ 2.22
    + 15 games, 10 arcade, 5 sports
    + choose 3 arcade, 2 sports
    + 10 choose 3 *  5 choose 2
    + number of ways to choose 3 from 10, and for each of those ways, we have
      the number of ways to choose 2 from 5
+ 2.25
    + S = {1 2 3 4 5 6}
    + 2 4 6, each has P = 2w
    + 1 3 5, each has P = w
    + P of 1 toss, num < 4, so 1 2 3
    + 1 2 3 = (w + 2w + w ) / (3w + 3 * 2w) = 4 / 9
+ 2.26
    + S = {1 2 3 4 5 6}
    + 2 4 6, each has P = 2w
    + 1 3 5, each has P = w
    + A = 2 4 6
    + B = 3 6
    + A OR B = 2 3 4 6 = (2w + w + 2w + 2w) / 9w = 7/9
    + we can't just add P(A) + P(B) since they're not mutually exclusive, 6 is
      in both sets
    + A AND B = P(A) * P(B)
    + P(A) = (2w + 2w + 2w) / 9w = 2/3
    + P(B) = (w + 2w) / 9w = 1/3
    + 2/3 * 1/3 = 2/9
+ 2.28
    + 5 cards, 2 aces, 3 jacks?
    + first find the total number of ways to choose a hand, 52 choose 5
    + so how many possible hands are there with 2 aces and 3 jacks?
    + (4 choose 2) * (4 choose 3)
    + multiply them together since for each way to choose the aces, we then
      choose jacks
    + so (4 choose 2) * (4 choose 3) / (52 choose 5)
+ 2.30
    + total of 7 or 11 when pair of dice tossed
    + P(7 or 11)
    + 7 sums = 1 6, 2 5, 3 4, 4 3, 5 2, 6 1 = 6 / 36 = 1 / 6
    + 11 sums = 5 6, 6 5 = 2 / 36 = 1 / 18
    + they're mutually exclusive, no overlap
    + so 1/6 + 1/18 = 4 / 18 = 2/9
+ 2.37
    + 4W 3B | 3W 5B
    + 2 scenarios: draw black from first or draw white from first
        + regardless, we place the drawn ball into the other bag, so the total
          count increases by 1
    + draw black from first: 3/7 * 6/9
    + draw white from first: 4/7 * 5/9
    + (3/7 * 6/9) + (4/7 * 5/9) since they're separate

6.4
+ standalone (even if it's in a sum, like P(X > a) + P(X < b))
    + P(X > a) = P(Z > k) = 1 - P(Z < k)
+ but when you have a joined inequality like P(a < X < b)
    + once you have calculated the corresponding Z's
    + P(X < b's z) - P(X < a's z)
