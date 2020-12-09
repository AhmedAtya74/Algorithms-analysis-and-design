# Masters theorem
## Masters theorem for decreasing function:
**Recurrence relation form:** T(n)=a* T(n-1)+f(n), assume that a > 0 and b > 0 and f(n) = O(N^k)  and k≥0

> ### We have three cases:
> -	Case1: if a < 1 → O(f(n))

> -	Case2: if a = 1 → O(n*f(n))

> -	Case3: if a > 1 → O(n^k * a^(n/b))

> ### Examples:
> - 1. T(n) = 1
>>
>> F(n) = O(1) = O(n^0 ), k = 0
>>
>> a = 0 , b = 1 
>>
>> since a = 0 then order of recurrence relation = O(f(n)) = O(1) 
>>
> - 2. T(n) = T(n-1) + n
>>
>> f(n) = O(n) = O(n^1 ), k = 1
>>
>> a = 1, b = 1
>>
>> since a = 1 then order of the recurrence relation = O(n*n)
>>
> - 3. T(n) = 2 * T(n-2) + 1
>>
>> f(n) = O(1) = O(n^0 ), k = 0
>>
>> a = 2, b = 2
>>
>> since a > 1 then order of the recurrence relation = O(n^0*2^(n/2)) = O(2^(n/2))
>>


## Masters theorem for dividing function:

**Recurrence relation form:** T(n)=a* T(n/b)+f(n)  assume that a≥1 and b>1 and f(n)=O(n^k * log^p⁡n)

> ### We have three cases:
> - Case1: if log a > k then order of recurrence relation=O(n^(log ⁡a) )

> - Case2: if  log ⁡a = k and
> > - p > -1 then order of recurrence relation=O(n^k * log^(p+1)⁡n) 
> > - p = -1 then order of recurrence relation=O(n^k * log⁡(log⁡⁡n))
> > - p < -1 then order of recurrence relation=O(n^k )                   

> - Case3: if  log a < k and
> > - p ≥ 0 then order of recurrence relation = O(n^k * log^(p)⁡n)
> > - p < 0 then order of recurrence relation = O(n^k) 

> ### Examples:
> - 1. T(n) = 2 * T(n/2) + 1 
>> a = 2 ,b = 2, log ⁡a = 1
>>
>> f(n) = O(1) = O(n^0 * log^(0)⁡n ), k = 0 ,p = 0
>>
>> since log a > k then order of recurrence relation=O(n^(log ⁡a)) = O(n^2)
>>
> - 2. T(n) = T(n/2) + 1
>>
>> a = 1, b = 2, log a = 0
>>
>> f(n) = O(1) = O(n^0 * log^(0) ⁡n ), k = 0, p = 0
>>
>> since log ⁡a = k and p> -1 then order of recurrence relation=O(n^k * log^(p+1)⁡n) = O(log⁡ n)
>>
> - 3. T(n) = 2 * T(n/2) + n/log⁡ n
>>
>> a = 2, b = 2, log a = 1
>>
>> f(n) = O(n * log^(-1)⁡ n), k = 1, p = -1
>>
>> since log a = k and p = -1 then order of recurrence relation = O(n * log⁡(log⁡(n)))
>>
> - 4. T(n) = 2 * T(n/2)+ n/log^(2)⁡n 
>>
>> a = 2, b = 2, log a = 1
>>
>> f(n) = O(n * log^(-2)⁡n ), k = 1, p = -2
>>
>> since log a = k and p < -1 then order of recurrence relation = O(n)
>>
> - 5. T(n) = T(n/2) + n^3
>>
>> a = 1, b = 2 ,log a = 0
>>
>> f(n) = O(n^3 * log^0⁡n ), k = 3, p = 0
>>
>> since log a < k  and p ≥ 0 then order of recurrence relation = O(n^3)
>>
> - 6. T(n) = 2 * T(n/2)+ n^3 * log n
>>
>> a = 2 , b = 2, log a = 1
>>
>> f(n) = O(n^3 * log^(1)⁡n ), k = 3, p = 1
>>
>> since log ⁡a < k and p ≥ 1 then order of recurrence relation = O(n^3 * logn )
>>
> - 7. T(n) = 2 * T(n/2) + n^3/log^2⁡n 
>>
>> a = 2, b = 2, log a = 1
>>
>> f(n) = O(n^3 * log^(-2)⁡n ), k = 3, p = -2
>>
>> since log ⁡a < k and p< 0 then order of recurrence relation = O(n^3)



 

