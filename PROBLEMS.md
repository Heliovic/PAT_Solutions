# 1001 A+B Format（20 分）
[Java (20/20)](https://github.com/Heliovic/My_PAT_Answer/blob/master/1001/Main.java)

Calculate a+b and output the sum in standard format -- that is, the digits must be separated into groups of three by commas (unless there are less than four digits).

## Input Specification:
Each input file contains one test case. Each case contains a pair of integers a and b where -10^6≤a,b≤10^6. The numbers are separated by a space.

## Output Specification:
For each test case, you should output the sum of a and b in one line. The sum must be written in the standard format.

## Sample Input:
```
-1000000 9
```
## Sample Output:
```
-999,991
```

# 1002 A+B for Polynomials（25 分）
[Java (25/25)](https://github.com/Heliovic/My_PAT_Answer/blob/master/1002/Main.java)

This time, you are supposed to find A+B where A and B are two polynomials.

## Input Specification:
Each input file contains one test case. Each case occupies 2 lines, and each line contains the information of a polynomial:

K N1 a1 N2 a2 ... Nk ak

where K is the number of nonzero terms in the polynomial, Ni and ai(i=1,2,⋯,K) are the exponents and coefficients, respectively. It is given that 1≤K≤10，0≤Nk<⋯<N2<N1≤1000.

## Output Specification:
For each test case you should output the sum of A and B in one line, with the same format as the input. Notice that there must be NO extra space at the end of each line. Please be accurate to 1 decimal place.

## Sample Input:
```
2 1 2.4 0 3.2
2 2 1.5 1 0.5
```
## Sample Output:
```
3 2 1.5 1 2.9 0 3.2
```

# 1003 Emergency（25 分）
[Java (25/25)](https://github.com/Heliovic/My_PAT_Answer/blob/master/1003/Main.java)

As an emergency rescue team leader of a city, you are given a special map of your country. The map shows several scattered cities connected by some roads. Amount of rescue teams in each city and the length of each road between any pair of cities are marked on the map. When there is an emergency call to you from some other city, your job is to lead your men to the place as quickly as possible, and at the mean time, call up as many hands on the way as possible.

## Input Specification:
Each input file contains one test case. For each test case, the first line contains 4 positive integers: N (≤500) - the number of cities (and the cities are numbered from 0 to N−1), M - the number of roads, C1 and C2 - the cities that you are currently in and that you must save, respectively. The next line contains N integers, where the i-th integer is the number of rescue teams in the i-th city. Then M lines follow, each describes a road with three integers c1, c2 and L, which are the pair of cities connected by a road and the length of that road, respectively. It is guaranteed that there exists at least one path from C1 to C2.

## Output Specification:
For each test case, print in one line two numbers: the number of different shortest paths between C1 and C2, and the maximum amount of rescue teams you can possibly gather. All the numbers in a line must be separated by exactly one space, and there is no extra space allowed at the end of a line.

## Sample Input:
```
5 6 0 2
1 2 1 5 3
0 1 1
0 2 2
0 3 1
1 2 1
2 4 1
3 4 1
```
## Sample Output:
```
2 4
```

# 1004 Counting Leaves（30 分）
[Java (30/30)](https://github.com/Heliovic/My_PAT_Answer/blob/master/1004/Main.java)

A family hierarchy is usually presented by a pedigree tree. Your job is to count those family members who have no child.

## Input Specification:
Each input file contains one test case. Each case starts with a line containing 0<N<100, the number of nodes in a tree, and M (<N), the number of non-leaf nodes. Then M lines follow, each in the format:
```
ID K ID[1] ID[2] ... ID[K]
```
where ID is a two-digit number representing a given non-leaf node, K is the number of its children, followed by a sequence of two-digit ID's of its children. For the sake of simplicity, let us fix the root ID to be 01.

The input ends with N being 0. That case must NOT be processed.

## Output Specification:
For each test case, you are supposed to count those family members who have no child for every seniority level starting from the root. The numbers must be printed in a line, separated by a space, and there must be no extra space at the end of each line.

The sample case represents a tree with only 2 nodes, where 01 is the root and 02 is its only child. Hence on the root 01 level, there is 0 leaf node; and on the next level, there is 1 leaf node. Then we should output 0 1 in a line.

## Sample Input:
```
2 1
01 1 02
```
## Sample Output:
```
0 1
```