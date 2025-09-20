# shamirsecretsharing
Hashira Placements Assignment - Secret Reconstruction
Description

This project implements the solution for reconstructing a secret from given shares using Shamir's Secret Sharing and Lagrange Interpolation.

You are given multiple points (roots) in a JSON format where each point is defined with a base and a value. The goal is to find the secret (the constant term of the polynomial) using a minimum number of points k.

Implementation Details

Language used: Java

Handles arbitrary large numbers and different numerical bases with BigInteger.

Parses input JSON to extract shares (points).

Applies Lagrange interpolation to reconstruct the secret.

Supports multiple test cases with varying parameters.

How to Use

Compile the Java program:

javac ShamirSecretSharing.java


Run the program with the appropriate input. The program reads from JSON-formatted test cases and prints out the reconstructed secret.

Sample Input Example
{
  "keys": {
    "n": 4,
    "k": 3
  },
  "1": {
    "base": "10",
    "value": "4"
  },
  "2": {
    "base": "2",
    "value": "111"
  },
  "3": {
    "base": "10",
    "value": "12"
  },
  "6": {
    "base": "4",
    "value": "213"
  }
}

Output (testcase 1) : 3


After processing the input, the program outputs the recovered secret as a BigInteger value.

Additional Notes

The program was implemented and tested within the 45-minute time limit.

The solution efficiently handles inputs with various numeric bases.

Ready to handle the second test case as mentioned in the assignment.
{
"keys": {
    "n": 10,
    "k": 7
  },
  "1": {
    "base": "6",
    "value": "13444211440455345511"
  },
  "2": {
    "base": "15",
    "value": "aed7015a346d635"
  },
  "3": {
    "base": "15",
    "value": "6aeeb69631c227c"
  },
  "4": {
    "base": "16",
    "value": "e1b5e05623d881f"
  },
  "5": {
    "base": "8",
    "value": "316034514573652620673"
  },
  "6": {
    "base": "3",
    "value": "2122212201122002221120200210011020220200"
  },
  "7": {
    "base": "3",
    "value": "20120221122211000100210021102001201112121"
  },
  "8": {
    "base": "6",
    "value": "20220554335330240002224253"
  },
  "9": {
    "base": "12",
    "value": "45153788322a1255483"
  },
  "10": {
    "base": "7",
    "value": "1101613130313526312514143"
  }
}


output (testcase 2) : -6290016743746469796

Submission

The complete source code is pushed to GitHub. Please find the repository link provided in the submission form.
