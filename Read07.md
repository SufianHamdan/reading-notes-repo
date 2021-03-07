# JavaScript, Comparison and logical operators

You can evaluate a situation by comparing one value in the script to what you expect it might be. The result will be a Boolean: true or false.

**== IS EQUAL TO IS NOT EQUAL TO This operator compares two values (numbers, strings, or Booleans) to see if they are the same.**


'Hello == 'Goodbye' returns false because they are not the same string.
'Hello' == 'Hello' returns true because they are the same string.



**!= This operator compares two values (numbers. strings, or Booleans) to see if they are not the same.**


'Hello' != 'Goodbye'
 returns true because they are not the same string
'Hello' != 'Hello' 
 returns false becauseithey are not the same string.

**It is usually preferable to use the strict method:**
**===**

**STRICT EQUAL TO**
This operator compares two values to check that both the data type and value are the same.

'3' === 3 returns false because they are not the same data type and value. 

'3' === '3' returns true because they are the same data type and value.

**STRICT NOT EQUAL TO**
This operator compares two values to check that both the data type and value are not the same.

'3' !== 3 returns true because they are not the same data type or value.

'3' !== '3' returns false because they are the same data type or value.

**Sea GREATER THAN `>`**
This operator checks if the number on the left is greater the number on the right.

4 > 3 return true 
3 > 4 returns false

**LESS THAN `<`**
This operator checks if the number on the left is less Adob than the number on the right.

4 < 3 returns false
3 < 4 returns true

**GREATER THAN OR EQUAL TO `>=`**
This operator checks if the number on the left is greater than or equal to the nunmber on the right.

`4 >= 3` return true 
`3 >= 4` returns false
`3 >= 3` returns true

**LESS THAN OR EQUAL TO `<=`**
This operator checks if the number on the left is less than or equal to the number on the right.

`4 <= 3` return false 
`3 <= 4` returns true
`3 <= 3` returns true

---
### Logical Operators

Comparison operators usually return single values of true or false. 
Logical operators allow you to compare the results of more than one comparison operator.

### && ||  LOGICAL AND 

This operator tests more than one condition
`((2 < 5) && (3 >= 2))` returns true.

If both expressions evaluate to true then the expression returns true. If just one of these returns false, then the expression will returns false


```

true && true returns true 
true && false returns false 
false && true returns false 
false && false returns false

```

LOGICAL OR 
`((2 < 5) || (2 < 1)) !(2 < 1)` returns true

If either expression evaluates to true, then the expression expressions return true,
if both return false, then the expression expressions return false
```

true || true returns true 
true || false returns true 
false || true returns true 
false || false returns false

```

LOGICAL NOT

This operator takes a single boolean value  and inverts it.
`!(2 < 1)` returns true
This reverses the state of an expression

!true returns false
!false returns true
