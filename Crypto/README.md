# CTF Challenges

A collection of cryptography challenges from various CTFs I've participated in, along with my solutions.

## Crypto

### BabyXor
A simple XOR encryption challenge using a 6-byte key to encrypt the flag. The exploit involves determining the key length and brute-forcing possible key values.

**Files**:
- `chal.py` - Challenge script that XORs the flag with a random key
- `exploit.py` - Solution script
- `out.txt` - Output from the challenge

### Hash_and_Burn
A frequency analysis challenge where characters are hashed with a consistent salt. The solution involves analyzing hash frequencies to map back to the original characters.

**Files**:
- `chal.py` - Challenge script that hashes each character of the flag
- `exploit.py` - Solution script using frequency analysis
- `output.txt` - Hashed output to decode

### Pseudopredictable
An RSA challenge with a twist - the prime numbers are generated using a Linear Congruential Generator (LCG). The exploit involves:
1. Recovering the LCG parameters from sample outputs
2. Predicting the prime numbers used
3. Reconstructing the private key to decrypt the flag

**Files**:
- `chal.py` - Challenge script that generates primes using an LCG
- `exploit-part1.py` - Script to recover the LCG parameters
- `exploit-part2.py` - Script to reconstruct the RSA private key
- `out.txt` - Challenge output containing public parameters

### Corrupted
A challenge involving corrupted encryption.

**Files**:
- `chal.py` - Challenge script
- `exploit.py` - Solution script
- `output.txt` - Output to decode

---

*Note: These solutions are for educational purposes. Always solve challenges on your own before looking at solutions.*

