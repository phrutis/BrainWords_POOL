# Pool for searching Brainwallets BTC + ETH for sale ~~$1000~~ -> $400<br>
You can buy a pool at the link https://t.me/cuda8/270<br>
![Image](https://github.com/user-attachments/assets/1eb9242c-7c0c-4f92-b53a-e0117a25ad62)<br>

Pool for those who have many cards (rigs)<br>
Pool is based on the BrainWords program<br>
The client program has added support for multi GPU!<br>

| GPU card | Speed |
|----------|-------------|
| 5090     | 540 Mkeys/s |
| 4090     | 360 Mkeys/s |
| A100     | 180 Mkeys/s |
| A6000    | 180 Mkeys/s |
| 3090     | 180 Mkeys/s |
| 3080 Ti  | 170 Mkeys/s |
| 3080     | 150 Mkeys/s |
| 3070 Ti  | 120 Mkeys/s |
| 3070     | 110 Mkeys/s |
| 3060     | 70 Mkeys/s |
| 2080 S   | 70 Mkeys/s |
| 2070     | 50 Mkeys/s |

Pool supports up to 5000 cards and more.<br>
Each card executes its own chunk (a small segment from a given range)<br>
Automatic download and update of addresses from the server.<br>
The client can search for 4 types of BTC addresses (1 uncopressed, 1 compressed, 3, bc) at once or ETH.<br>
The address database is hashed, if it is changed by the client, it is downloaded again.<br>

When the client is first launched, it downloads the address database, then it takes 15 minutes to create the acceleration table ecmult_big-536870912-24.bin (5.7 GB)<br>
You can copy the table to another rig if it has a weak processor so you don't have to wait.<br>
When launched again, the client reads the table, starts immediately.

Support only CUDA cards (CMP cards work)<br>
Os: windows, ubuntu, lin, hive.

Only the speed is displayed in the client window.<br>
If it finds the found address, it is displayed<br>
![Image](https://github.com/user-attachments/assets/80b744a2-2afe-44a4-a070-71e89c8f1656)

The admin displays the password generation, speed, position suffix number.

## Simple and convenient admin panel.<br>
Edit, save button.<br>
1. Column for arguments (--root, --eth, --ethsha256, --camp2, --iteration...)<br>
By default, empty - this is a BTC search<br>
2. The name of the address database file<br>
3. Suffix (0) is the position from which to start the search.<br>
During operation, it is inqued at the current position.<br>
Pause, start button<br>

You can change the search position (suffix) without stopping the work.<br>

### The find is sent to 2 groups.<br>
1. Hunter group. A message is received indicating the user's nickname and the found address.<br>
2. Admin group receives a message password, nickname, address, private key, address type.

Clear WEB statistics, see the screenshot above.<br>
Statistics are updated automatically<br>
Length 8 all possible characters (93) passed.

Convenient launch<br>
```chmod +x bb```<br>
```./bb -u NickName```<br>
```bb.exe -u NickName```

You can run multiple rigs under one nickname<br>
A set of server sources, client sources, server installation instructions, and client compilation.<br>
If you have any questions, write them down @phrutis
