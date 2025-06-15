<h1>Encryption</h1>

I first converted my secret word into ASCII using the table. I got 116 104 105 110 107 as the values.
Then I converted to binary and got the values 01110100 01101000 01101001 01101110 01101011.

Afterward, I did the same with my key, "moves". The ASCII values were 109 111 118 101 115.
Then, converting to binary, I got 01101101 01101111 01110110 01100101 01110011. 

Since both my key and my word are the same length, I do not need to change anything when I do the XOR encoding. For each pair, I looked at each corresponding digit and if it was the same (either both had a one or both had a zero) I put a zero. If the numbers were different I put a one.
By doing this, I got this in binary 00011001 00000111 00011111 00001011 00011000. 
Which I converted to hex 19 07 1F 0B 18

My encrypted value is 19071F0B18.

<h1>Decryption</h1>

I took my encrypted value: 19071F0B18 and I broke it up into 19 07 1F 0B 18.
Then I could convert the hex into binary and I got 00011001 00000111 00011111 00001011 00011000. This is the XOR encrypted binary. 

I converted the key, "moves" into ASCII and then binary to get 01101101 01101111 01110110 01100101 01110011.

Comparing the key values to the XOR values, I got 01110100 01101000 01101001 01101110 01101011 as the decrypted values. 
These I converted to the ASCII values and then to the letter values to get "think"
