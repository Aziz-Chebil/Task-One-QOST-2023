# Task-One-QOST-2023
The key idea of my solution is to compare integers using their binary representation.
These are the steps of my solution :
1. Determine the absolute values of the integers and the length of the longer integer's binary representation
2. Create our quantum circuit with the appropriate number of qubits initialized to |0>
3. Apply the controlled X gates to initially compare the binary representation of a & b Use Hadamard gates and controlled shift to implement the QPE algorithm to determine the relative phase between the binary integers of a & b
4. Apply a Toffoli gate to the two most significant qubits of the input registers, with the target qubit being an additional ancilla qubit initialized to |1⟩  to determine the relative phase between a & b
5. Encode the relative phase into an overall phase using a Hadamard gate 
6. Measure the additional ancilla qubit
7. Get the measurement outcome
8. Determine the larger number and return it with the determined sign
