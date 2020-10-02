# ATM

The first part (C1 -> C23) consists in identifying the card and checking the pin: the expiration date is extracted from the ROM memory and compared with the date entered by the user, then the pin is extracted from the RAM memory and compared with the one entered by the user. If these operations are performed successfully, the desired operation is chosen with the help of the demultiplexer. <br />
  The balance query part (C24 -> C29) consists of extracting the balance from the RAM memory, decoding it and displaying it.<br />
  The pin change part (C30 -> C31) consists of extracting the pin from the RAM memory and displaying it.<br />
  The cash withdrawal part (C32 -> C49) consists of: the comparator with 1000 euros which compares the amount required with the maximum amount allowed for withdrawal, extracting the balance from RAM and comparing it with the amount required by the user, the 5 counters for each type of the banknote, the verification by a comparator of the existing types of banknotes and if all these operations are performed successfully, the balance decreases, its addition in the RAM memory and the decrease of the number of banknotes.<br />
  The cash deposit part (C50 -> C60) consists of: first a banknote decoder, an adder for adding the amount entered and then adding it to RAM, then a demultiplexer for selecting the type of banknotes entered and the 5 counters to could make the deposit, count the money successfully.<br />
  
