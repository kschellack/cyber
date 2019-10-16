[Go back to readme](./README.md)


# This is a review of the first five weeks of IT 0075 

## Concentration has been on syntax and algorithms

I have tried (mostly successfully) to hone fast algorithm development. 
   First by the use of specific comments that delineate the sections of code to be somewhat independently 
   written and debugged.
   
   I have used the Python IDLE (integrated development and learning environment). It has been easy
   to learn and very functional.
   
   The most challenging of the given tasks was the extra credit --- removing the duplicate letters in password. The
   below code, which mostly works, challenged my ability to visualize the needed algorithm. Somehow I did not "see" that 
   the last letter would always be "correct". As expected, the solution came from collaborating with a classmate.
   
```python3
p='hezzo'

newpass=''

for i in range(len(p)-1):             #a loop that walks through entered password
    incr=i+1                          #set incr to look at the "next" letter of password
    print('line 3 p(i)= ',p[i],',i =',i)      #debug print
    while incr < (len(p)):            #loop to compare password letter to next letter to look for duplicates
        print('i= ',i,',incr= ',incr)  #debug print
        if p[i]==p[incr]:             #loop to look for duplicates
            print('found a dupe',p[i],p[incr],i) 
            i=i+1                     #increment the index that looks at "next letters"
            incr=incr+1
        elif incr==(len(p)-1):        #if incr is at end of p, append p(i) to newpass
            newpass=newpass+p[i]                        #if next letter is not a duplicate, go to next letter
            i=i+1
            print('added to newpass i= ', i, ',incr ', incr, newpass)        #debug print of building newpass
            incr=incr+1               #if no dupe, increment incr
        else:
            if i==(len(p)-1):
                newpass=newpass+p[i]
                print(newpass)
        incr=incr+1

```   
   
In conclusion, seems like Python is the most popular programming language. It is easy to learn, I look forward to 
progressing to the specific modules.
