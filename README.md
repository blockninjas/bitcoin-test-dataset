# bitcoin-test-dataset
Testdataset for Bitcoin Analysis starting from Address 18V6vwHKoqVQWUB4FbPHcTmaqTLfnuNWRN

Extract the zip file first and you will get the data.dat file!

It does contain transactions from and to the above mentioned Address from and to depth 7. Use it for your own purposes.

The mentioned Bitcoin Adress does not have to do anything with me or other things I know. It was taken arbitrary. 

The format of the Dataset is the following. It is one file named "data.dat" which is a text file. It does NOT contain any Transaction Hashes
or something else. Each line contains the following data:

  [Bitcoin Adress From] [Bitcoin Address To] [Satoshi Amount]

Every transaction regarding the starting Bitcoin Adress mentioned above is resolved in a way that every input Address is in correlation to each output Address. 

ATTENTION: To get the Bitcoin Amount you have to devide the "Satoshi Amount" by 100.000.000!!!

Example:

A transaction contains the following input side:
```
  A 12.5
  B 10.2
  C 2
```

and the following output side:
```
  Y 12.2
  Z 12.5
```
The the data in the file would be
```
  A Y 12.5
  B Y 10.2
  C Y 2
  A Z 12.5
  B Z 10.2
  C Z 2
```
LaTeX citation:
```
  @misc{dinhobl_2017, title={TUViennaBitcoinSet}, url={https://github.com/mrqc/bitcoin-test-dataset.git}, publisher={Erhard Dinhobl}, author={Dinhobl, Erhard}, year={2017}, month={Dec}} 
```
