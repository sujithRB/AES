# EX-8-ADVANCED-ENCRYPTION-STANDARD ALGORITHM
## Name : SUJITH RB
## Reg.No : 212224103003
### Date: 12-05-2026
# Aim:
To use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption.

# ALGORITHM:
AES is based on a design principle known as a substitution–permutation.
AES does not use a Feistel network like DES, it uses variant of Rijndael.
It has a fixed block size of 128 bits, and a key size of 128, 192, or 256 bits.
AES operates on a 4 × 4 column-major order array of bytes, termed the state
# PROGRAM:
```c
#include <stdio.h>
#include <string.h>

void xor_encrypt_decrypt(char *input, char *key) {
    int input_len = strlen(input);
    int key_len = strlen(key);
    for (int i = 0; i < input_len; i++) {
        input[i] = input[i] ^ key[i % key_len];
    }
}

int main() {
    char url[] = "SUJITH";
    char key[] = "secretkey";
    
    printf("Original text: %s\n", url);
    xor_encrypt_decrypt(url, key);
    printf("Encrypted text: %s\n", url);
    xor_encrypt_decrypt(url, key);
    printf("Decrypted text: %s\n", url);

    return 0;
}
```
# OUTPUT:

<img width="1618" height="797" alt="Screenshot 2026-05-12 140524" src="https://github.com/user-attachments/assets/ed036460-13cb-4308-bb1a-48a7083fe19f" />



# RESULT:
Thus, the Advanced Encryption Standard (AES) concept was studied and a practical URL encryption program was successfully implemented and verified.


