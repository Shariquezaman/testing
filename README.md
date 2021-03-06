# Sliding Window Protocol

Assignment for CZ 3006 - Net-Centric Computing at NTU, Singapore.

This repo implements the Sliding Window Protocol between two VMs running in a simulated network at different quality levels:

1. Level 0: Error-free transmission.
2. Level 1: Frame loss possible.
3. Level 2: Frame damage possible.
4. Level 3: Frame loss & damage possible.

### How to Run:
**Step 1:** Compile `SWP.java` by running:
```
javac SWP.java
```

**Step 2:** Next, start the Network Simulator by running the following where `X` is the service quality level [0 - 3].
```
java NetSim X
```

**Step 3:** Start the two VMs by running the following in separate windows:
```
java VMach 1
```
```
java VMach 2
```

After each run of the system, two output text files - `receive_file_1.txt` & `receive_file_2.txt` - will be automatically generated, with `receive_file_1.txt` being generated by VMach 1 and containing the texts received from VMach 2 & `receive_file_2.txt` being generated by VMach 2 and containing the texts received from VMach 1.

If the Sliding Window Protocol is correctly implemented, the contents in `receive_file_1.txt` should be the same as `send_file_2.txt` & the contents in `receive_file_2.txt` should be the same as `send_file_1.txt`.

<br>
**_Disclaimer:_** This repo is no longer maintained and was submitted as part of the coursework assignment for CZ 3006 at NTU in AY15/16 Semester 2.

Edited

Edited
 Edited
