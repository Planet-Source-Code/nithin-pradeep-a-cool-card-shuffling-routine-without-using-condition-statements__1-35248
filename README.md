<div align="center">

## A cool card shuffling routine 'without using condition statements'


</div>

### Description

Hi friends. This is a good card shuffling routine.

Basically, what it does is it takes an aray containing the numbers form 1 to 52 and shuffles the array. This can be used for any purpose including shuffling cards.
 
### More Info
 
An array which containd the numbers form 1 to 52 in that order

This code works by choosing a random number between 1 & 52 and assigning it to an element of the array. Then it chooses another random number and assigns it to the next element. The code is pretty self explanatory. If you have some doubt, just mail me.

The same array with the order of the numbers shuffled


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Nithin Pradeep](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/nithin-pradeep.md)
**Level**          |Beginner
**User Rating**    |4.7 (28 globes from 6 users)
**Compatibility**  |VB 3\.0, VB 4\.0 \(16\-bit\), VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[Games](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/games__1-38.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/nithin-pradeep-a-cool-card-shuffling-routine-without-using-condition-statements__1-35248/archive/master.zip)





### Source Code

```
Dim deck(1 To 52) As Integer 'the array which holds the cards
'the following are just a few counters
Dim n As Integer
Dim temp As Integer
Dim i As Integer
Dim temp1 As Integer
'this statement is used to return different random numbers each time we run the application
Randomize Timer
'the following loop assigns the numbers 1 to 52 to the array in that order.
For n = 1 To 52
 deck(n) = n
 Next n
'time to do the shuffling
 For i = 0 To 9'this llop just repeats the shuffling process 10 times
 For temp = 1 To 52
 n = Int((52 * Rnd) + 1) this generates a random number in the range 1 to 52
'the following block of code interchanges the values of deck(temp) & deck(n). This is a very simple method of shuffling the array. If you read it carefully you will be able to understabd the logic.
 temp1 = deck(temp)
 deck(temp) = deck(n)
 deck(n) = temp1
 Next temp
 Next i
```

