# **Python program to display Fibonacci Sequence.**
* This program displays fibonacci sequence using a recursive function.<br>
* The Fibonacci sequence is the series of numbers where each number is the sum of the two preceding numbers.<br>
* The first two terms are 0 and 1. All the other terms are obtained by adding the preceding two terms. This means that the nth term is the sum of (n-1)th and (n-2)th term.<br>
* For example **nterms** = 10 will give a sequence 0, 1, 1, 2, 3, 5, 8, 13, 21, 34<br>
 
 ```python
 num = int(input(Enter a number: ))
 ```
 The *num* alerts the user to enter a number,

 ```python
 def recur_fibo(n):
    if n <= 1:
         return n
    else:
        return(recur_fibo(n-1) + recur_fibo(n-2))
    nterms = num
```
A recursive function recur_fibo() is used to calculate the nth term of the sequence. <br>
We store the number of terms to be displayed in *nterms*.<br>

```python
    if nterms <= 0:
        print('Enter a positive integer')
    else:
        print('Fibonacci sequence: ')
        for i in range(nterms):
            print(recur_fibo(i))
```
We use a *for* loop to iterate and calculate each term recursively.
