Given numRows, generate the first numRows of Pascal's triangle.
Pascal's triangle : To generate A[C] in row R, sum up A'[C] and A'[C-1] from previous row R - 1.
Example:
Given numRows = 5,
Return
[
[1],
[1,1],
[1,2,1],
[1,3,3,1],
[1,4,6,4,1]
]
Constraints:
0 <= numRows <= 25

he outer loop iterates through each row from 0 to numRows-1.
For each row, create a list row with i + 1 elements, initially filled with 1.
The inner loop updates the elements in the row starting from index 1 up to i-1 by summing the corresponding values from the previous row.
Append the generated row to the result list.
Repeat the process until all rows are generated.
The example with numRows = 5 will produce the Pascal's Triangle as specified.
