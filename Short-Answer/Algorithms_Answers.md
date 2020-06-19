#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)
    O(n). at first glance I considered that this would be O(n^3) due to it only being a while loop will run n^3 times if a grew linearly. however, A grows at (n^2) so the complexity is actually O(n^3/n^2) which simplifiys to O(n). when n is n it runs: [1,2,3,4,5...] times

b)
    O(n log(n)) is my first guess. so for the first loop, it will always run n times. then for the while loop, it runs that n times, but no where near as many times as n. logically it just works out to run log(n) times.

c)
    O(n), singly recursive funcions are naturally O(n) since it is called once. if the same function called itself twice it would be 2^n 

## Exercise II

so this is an excellent use case of our binary search. you could find the perfect floor in log(n).
the first step would be to go to the middle floor (rounded up or down if even number of floors). then drop and egg.
if it breaks, you cut your current amount of floors in half (if on floor 8/15, go to floor 4) and make note that you can't drop it from that floor or higher. if you drop the egg and it's fine, you moveup half the floors left (from floor 8/15 to 12/15) also making note that you have to drop the egg from higher than your current position to maximize your drop. you then repeat this process of moving up half of what's left, or down of what's left. 

this ends up being log(n) time to find the optimum egg drop floor. so you wouldnt even need that many eggs!
