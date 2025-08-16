Hamming Code Using Verilog

This project implements Hamming Code in Verilog, covering encoding, decoding, and error correction for reliable digital communication. It demonstrates how single-bit errors in transmitted data can be detected and corrected using error-correcting codes.


Features

Hamming Code Generator/Encoder - takes 4 data bits and produces a 7-bit Hamming Code with parity bits.

Hamming Code Decoder - decodes the 7-bit Hamming Code and retrieves the original 4-bit data.

Error Correction Module - detects and corrects single-bit errors in the 7-bit Hamming Code.

Configurable Parity Type - supports odd and even parity (parity_type = 1 → Odd, parity_type = 0 → Even).

Testbenches Included - all modules are verified using dedicated testbenches.

Hamming Code Representation

The 7-bit Hamming Code layout is as follows:

Code Bit	H7	H6	H5	H4	H3	H2	H1
Position	D4	D3	D2	P3	D1	P2	P1

D → Data bits

P → Parity bits




Project Structure

Design Files

hamming_code_encoder.v - Hamming Code Generator/Encoder

hamming_code_decoder.v - Hamming Code Decoder

hamming_error_correction.v - Error Correction module

Testbench Files

hamming_encode_tb.v - Encoder Testbench

hamming_decode_tb.v - Decoder Testbench

hamming_error_correction_tb.v - Error Correction Testbench


