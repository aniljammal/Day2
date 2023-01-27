def countWays(n):
    # declaring  two variables to store the count
    prev = 1
    prev2 = 1
    # Running for loop to count all possible ways
    for i in range(2, n+1):
        curr = prev + prev2
        prev2 = prev
        prev = curr
    return prev
 
n = 4
print("Number of Ways : ", countWays(n))
