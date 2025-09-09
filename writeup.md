# Write Up for Infinity Calculator Challenge

## Steps to solve

The calculator is written to operate like an actual calculator. It will not do advanced arithmetic. Additionally, it will not calculate things that are not a number (NaN). As you could guess infinity is not a number.

The simplest solution is to enter `infinity` as your number. This will give you the flag.

```
Congratulations! You have reached infinity!
The flag is: ciahackedme{infinity_is_not_a_number}
```

Other methods are to use the strings command on the binary file to look for any text strings that are readable.

```
strings main | grep infinity
Congratulations! You have reached infinity!
The flag is: ciahackedme{infinity_is_not_a_number}
infinity
infinity+infinity
infinity-infinity
infinity*infinity
infinity/infinity
_Z8infinityv

```
In this approach, we use the strings command followed by grep to search the output for infinity. This leads us right to the flag.

Hope you enjoyed this very easy level ctf challenge. Let me know if you want a harder one.