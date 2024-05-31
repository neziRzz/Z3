- Initialize Bitvec
  `Input = [BitVec('x[%d]' % i, 8) for i in range(44)]` (depends on datatype use diffrent bitsize, use 8 here since the initialized datatype here is char and a char equals 8 bits, the for loop is to determine the amount of characters)
- Adding conditions and constrains
    `s.add(constrains here)`
- Create the Solver() object using the following initialization
    `s = Solver()`
- Check if whether a solution exists
  `if(s.check == unsat: #sat or unsat,same logic but different syntax)
      print("No solution exists.")
    else:
      m = s.model()`
- Print out the result
    `print(m) #this will return a list of bitvecs so remember to convert it back to your desired format`
