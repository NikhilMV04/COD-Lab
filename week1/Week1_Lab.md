# Program 1: 
### Statement:  Assembly Program for addition of 2 words

### Name of file:
Week1_Lab.s

### Observation - Single Cycle
- The code uses base address x5 and offsets to load specific words from the array, demonstrating how to access array elements in memory.

- The result of adding two 32-bit words (x6 and x7) is stored in the third position of the array (a[2]), showcasing the use of arithmetic and memory operations.

- The .data section initializes the array with specific values and updates the third element with the result of the addition, illustrating data setup and manipulation.
 
### Register Mapping
- **x5:** 0x10000000
- **x6:** 0xabcd1234
- **x7:** 0x5678ef90
- **x8:** 0x024601c4

### Data Mapping
- **0x10000000:** 10000297
- **0x10000004:** 00028293
- **0x10000008:** 0002a303





# Program 2: 
### Statement:  Assembly Program for addition of 2 half words

### Name of file:
Week1_Lab.s

### Observation - Single Cycle
- The .data section initializes an array a with three 16-bit half-words: 0x1234, 0x5678, and 0x0000. The last element is initially set to zero for storing the result.

- The code uses lh to load signed half-words from memory and add to compute their sum. The result is stored in x12.

- The sh instruction is used to store the result of the addition into the third element of the array (a[2]), demonstrating how to update array elements.
 
### Register Mapping
- **x9:** 0x10000000
- **x10:** 0x00001234
- **x11:** 0x00005679
- **x12:** 0x000068ac

### Data Mapping
- **0x10000000:** 10000497
- **0x10000004:** 00048493





# Program 3: 
### Statement:  Assembly Program for addition of 2 bytes

### Name of file:
Week1_Lab.s

### Observation - Single Cycle
- The .data section initializes an array a with three 8-bit bytes: 0x12, 0x34, and 0x00. The last byte is set to zero for storing the result.

- The code uses lb to load signed bytes from memory and add to compute their sum. The result is stored in x17.

- The sb instruction is used to store the result of the addition into the third byte of the array (a[2]), showing how to update byte values in an array.
 
### Register Mapping
- **x15:** 0x10000000
- **x15:** 0x00000012
- **x16:** 0x00000034
- **x17:** 0x00000048

### Data Mapping
- **0x10000000:** 10000717





# Program 4: 
### Statement:  Assembly Program and analyse the format of storing signed and unsigned words, half words and byte data types

### Name of file:
Week1_Lab.s

### Observation - Single Cycle
- The code loads a 32-bit word, a signed and unsigned 16-bit half-word, and a signed and unsigned 8-bit byte from memory, using appropriate instructions for each data type.

- It stores these values into separate memory locations, with the 16-bit half-word result being stored at different offsets within the same address to illustrate handling both signed and unsigned half-word storage.

- Registers are used to temporarily hold data loaded from memory and to specify where results are to be stored, demonstrating efficient data handling and memory operations in RISC-V assembly.
 
### Register Mapping
- **x15:** 0x12345678
- **x16:** 0x10000004
- **x17:** 0xffff9abc
- **x18:** 0x00009abc
- **x19:** 0x10000006
- **x20:** 0x1000003f
- **x21:** 0x1000003f
- **x22:** 0x10000007
- **x23:** 0x1000000b
- **x24:** 0x1000000b
- **x25:** 0x1000000d
- **x26:** 0x1000000d

### Data Mapping
- **0x10000000:** 10000797
- **0x10000004:** 0007a783

