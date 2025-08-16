# Hamming Code Using Verilog  

This project implements **Hamming Code** in Verilog, including encoding, decoding, and error correction. It demonstrates how single-bit errors can be detected and corrected in digital communication systems.  

---

##  Features  
- **Hamming Code Encoder** - generates a 7-bit Hamming Code from 4-bit data.  
- **Hamming Code Decoder** - retrieves the original 4-bit data and raises an error flag if corruption is detected.  
- **Error Correction Module** - corrects single-bit errors in the received Hamming Code.  
- **Parity Type Selection** - supports **even** (`parity_type = 0`) and **odd** (`parity_type = 1`) parity.  
- **Complete Testbenches** - each module is tested using dedicated testbench files.  

---

##  Hamming Code Representation  

The 7-bit Hamming Code format:  

| Code Bit | H7 | H6 | H5 | H4 | H3 | H2 | H1 |  
|----------|----|----|----|----|----|----|----|  
| Position | D4 | D3 | D2 | P3 | D1 | P2 | P1 |  

- **D** → Data bit  
- **P** → Parity bit  

---

##  Project Structure  

### Design Files  
- `hamming_code_encoder.v` - Hamming Code Encoder  
- `hamming_code_decoder.v` - Hamming Code Decoder  
- `hamming_error_correction.v` - Error Correction Module  

### Testbench Files  
- `hamming_encode_tb.v` - Testbench for Encoder  
- `hamming_decode_tb.v` - Testbench for Decoder  
- `hamming_error_correction_tb.v` - Testbench for Error Correction  

---

##  Module Details  

###  Encoder  
- **Input:** 4-bit data  
- **Output:** 7-bit Hamming Code (with parity bits)  

###  Decoder  
- **Input:** 7-bit Hamming Code  
- **Output:** 4-bit corrected data + error flag  

###  Error Correction  
- **Input:** 7-bit Hamming Code (possibly erroneous)  
- **Output:** Corrected 7-bit Hamming Code + error flag  

---




