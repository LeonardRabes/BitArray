# BitArray
Manages a compact array of bit values, which are represented as Booleans. Similar to .Net System.Collections.BitArray.
## Functionality:
```c#
            BitArray bitArray = new BitArray();
            bitArray.AddRange(new bool[] { true, false, false, false, false, true});

            bitArray[2] = true;
            bool val = bitArray[2];

            bool[] bits = bitArray.GetBits(); // contains: true, false, true, false, false, true
            byte[] bytes = bitArray.GetBytes(); // contains: 164 (10100100)
            
            foreach (var bit in bitArray)
            {
                Console.Write(bit + " "); // Prints: true false true false false true 
            }       
``` 
