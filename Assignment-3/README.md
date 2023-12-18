### Assignment #3 (0x4FFFFFFD) & (0x4FFFFFFE)


Assignment 2 and 3 code is in  assignment 2 code folder

1. **Team Contribution**
   
Anandu - Set up the environment for the nested VM and coded the leaf node 0x4FFFFFFD. 
Jeswanth - Coded the leaf node 0x4FFFFFFE, developed and tested the program, ensured result accuracy, and collaborated with Anandu in verifying the answers for the assignment questions.
  
2. **Describe in detail the steps you used to complete the assignment.** 
[GO TO ASSIGNMENT 2 for detailed steps ](https://github.com/AnanduSreekumar/CMPE-283-Virtulization-Technologies/blob/main/Assignment-2/README.md)

3. **Comment on the frequency of exits** – 
Some codes have no exits when using the minimum possible. Code 81 (VMMCALL) and code 3 (move to CR3) are examples of codes that do not have exits.

4. **Of the exit types defined in the SDM, which are the most frequent? Least?**
Exit code 124 was the most frequently used, with 683275 exits. Exit code 124 corresponds to VMEXIT_MSR.