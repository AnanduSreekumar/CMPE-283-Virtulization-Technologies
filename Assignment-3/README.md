### Assignment #3 (0x4FFFFFFC) & (0x4FFFFFFE)

1. **Contribution**
   
   > Answer: <br> Aishwarya - Completed the environment setup for the nested VM and implemented the code for leaf node 0x4FFFFFFC. <br> <br> Sanjay - Implemented the code for leaf node 0x4FFFFFFC, developed the testing program, and confirmed the accuracy of the results; created the test program and verified the results for the assignment questions along with Aishwarya. <br> <br> Sanjay - Executed the coding for leaf node 0x4FFFFFFE, formulated and tested the program, ensuring result accuracy, and collaborated with Aishwarya in verifying the outcomes for the assignment questions.
  
2. **Describe in detail the steps you used to complete the assignment.** 
   > Please Read the step mentioned above

3. **Comment on the frequency of exits** – does the number of exits increase at a stable rate? Or are there more exits performed during certain VM operations? Approximately how many exits does a full VM boot entail?
 
   <br> The quantity of exits does not exhibit a consistent growth pattern. For instance, at exit number 31, there was a doubling of total exits, whereas at exit number 1, there was only a slight increase, and at exit number 47, there was no change at all. <br> <br> Observing exits during a full VM boot, the count was 739532 before booting and 1450170 afterwards. <br> <br> In an experiment with the VM operation of pinging 8.8.8.8, most exit types showed no significant change in the total number of exits following this activity.

4. **Of the exit types defined in the SDM, which are the most frequent? Least?**

    > Answer: <br> The most frequent exit for us is exit number 30, with total exits as 1510473 and the least was 29 and 55, with 5 total exits. There were many exit numbers with 0 exits.