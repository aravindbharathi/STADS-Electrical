# STADS Electrical Repository
This repository contains all the codes intended to be used on hardware written during the process of development of the Star Tracker, including Verilog, Embedded C, C for HLS and bitstreams to program FPGAs.

This repository does not include codes for [in-loop simulation](https://github.com/aravindbharathi/STADS) of the Star Tracker and will not host the final flight codes.

## Organization of codes
1. Codes are to be hosted in their respective directories following the file nomenclature as explained in the [QA Guidelines](https://docs.google.com/document/d/1U63RPCxErLuVvC3BmJ-6Fqa9EqF_KslVQfur7OiazCk/edit).
2. Appropriate version control practices are to be followed as mentioned in the QA Guidelines.
3. Any arguments to be fed into C codes are to be given as arguments to `main()` and run from the command line. The `main()` should look as follows:
```
int main(int argc, char** argv)
{
    \\ insert main code here
}
```
4. Do not include any non-code / non-bitstream files (such as .txt, .jpg, .png, etc.) in the repository unless they are absolutely necessary.
