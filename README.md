# Qiskit
Quantum  stuff

#link https://t.me/Ox7eck

```
from qiskit import QuantumCircuit, execute, Aer

# Create a Quantum Circuit with one qubit and one classical bit
qc = QuantumCircuit(1, 1)

# Apply a Hadamard gate to put the qubit in superposition
qc.h(0)

# Measure the qubit
qc.measure(0, 0)

# Run the circuit using the Qasm simulator
simulator = Aer.get_backend('qasm_simulator')
result = execute(qc, simulator, shots=1).result()

# Get measurement result
counts = result.get_counts(qc)
print("Hello, Quantum World! Measurement result:", counts)
```
