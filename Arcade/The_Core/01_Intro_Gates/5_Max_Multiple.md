# Max Multiple



Given a divisor and a bound, find the largest integer N such that:

N is divisible by divisor.
N is less than or equal to bound.
N is greater than 0.
It is guaranteed that such a number exists.

### Example

For divisor = 3 and bound = 10, the output should be maxMultiple(divisor, bound) = 9.

The largest integer divisible by 3 and not larger than 10 is 9.



```javascript
function maxMultiple(divisor, bound) {
    for(var i = bound; i > 0; i--) {
        if(i % divisor === 0) {
            return i;
        }
    }
    
}
```

or

```javascript
maxMultiple = (divisor, bound) => bound - (bound % divisor);
```

