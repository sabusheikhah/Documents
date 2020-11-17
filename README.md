# Documents


def diagonalDifference(arr):
    # Write your code here
    l = len(arr)
    d = int(l**0.5)
    jump = d + 1
    sl = [ ]
    sr = [ ]
    t = 0
    for i in range(1,jump):
        sl.append(arr[t])
        t += jump
    t = d - 1
    for j in range(1,jump):
        sr.append(arr[t])
        t += (d -1)
        
    count_f = 0
    count_b = 0
    ######################################333
    
    #Problem starts here,
    #sl and sr are lists that contain integers I want add up, but I am not allowed to because of the error mentioned on the subreddit.
    for i in sl:
        count_f += i
    
    for j in sr:
        count_b += j        
        
    return abs(count_f - count_b)
