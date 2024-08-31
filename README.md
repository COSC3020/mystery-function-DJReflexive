# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```


# My Answer

I believe the `mystery()` function is a recursive algorithm that returns 
the greatest value of any given array. The first line is the base case
which just returns the first element if the array size is only 1 element.
The second line is the recursive call that shrinks the array by 1 (removing
the first element) and continually calls the function. The third and fourth
line are checking whether the var foo (which will be a single value after all 
the recursive calls) is the greatest value, but if not it will return the next 
value within the recursive call.


# My Sources

-www.w3schools.com: for a quick description of what the .slice() function does



# Plagiarism Acknowledgement

I certify that I have listed all sources used to complete this exercise, 
including the use of any Large Language Models. All of the work is my own, 
except where stated otherwise. I am aware that plagiarism carries severe 
penalties and that if plagiarism is suspected, charges may be filed against 
me without prior notice.
