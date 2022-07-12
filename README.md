Blockchain-THM-room-walkthrough-
Room to learn the basic concepts of blockchain, having fun.

For those fans of "Try Hack Me" and those who are interested in discovering blockchain from an easy and fun perspective, I have developed this "Try Hack Me" room about blockchain.
Here I leave you the complete walkthrough. 
Have fun!

![1](https://user-images.githubusercontent.com/109109176/178353266-7c3fdfde-29be-45ee-9d88-6b87c8f98544.jpg)


INSTRUCTIONS

IMPORTANT!! : You can do this room with the "Try Hack Me AttackBox" machine, only if you are a subscriber. If you are using a free account you have to use your own linux virtual machine.


Download the simulator

The first thing we have to do is start the machine "Bouncer Store", attached to this task.

To download the simulator we must connect to the machine via ftp.

Open your linux attack machine and run a terminal. Copy paste the following commands in the terminal:



ftp ip;

(ip= ip of "Bouncer Store")

Introduce the user:

bouncer

Enter the password:

cyberbouncer

![1](https://user-images.githubusercontent.com/109109176/178448664-1864684b-3f29-4ec2-84a3-f9d74f2bcd15.PNG)


Download the simulator with the command:

get blockchain-demo-master.zip;

We can exit from ftp with:

Ctl + D 



Now we are in possession of the simulator the next step is to install it in our linux attack machine:

The file is in zip format...

Unzip the simulator: 

unzip blockchain-demo-master.zip; 

Move to the simulator directory:

cd blockchain-demo-master;

Create a server using "docker":

sudo docker-compose up -d;

Give it time to execute the server...

![2](https://user-images.githubusercontent.com/109109176/178450668-4d3a84e7-e5ee-4aa2-9b93-a8a1b08e8c51.PNG)


Point a web browser at the simulator

Copy this url in your attack box browser to move to the "Hash" part of the simulator, in your localhost under port:3000-->   http://localhost:3000/hash

![3](https://user-images.githubusercontent.com/109109176/178451406-0695884d-f882-4210-bb1a-0b007e8fe110.PNG)


!Do the following only in case of error:

If you are not using the "THM attack box" it may be that you have problems starting the server, in that case try to install docker-compose with the follow commands and start the server again:

sudo apt update;

sudo apt install docker-compose -y;

sudo docker-compose up -d;


Question #1: 
A hash is a function that meets the encrypted demands needed to solve for a blockchain computation. Hashes are of a fixed length since it makes it nearly impossible to guess the length of the hash if someone was trying to crack the blockchain. The same data will always produce the same hashed value.
When you are in the simulator ...
In the "data" box: Write random letters. Is the hash changing? Yes or no ("y" or "n")

Answer #1: 
y

Question #2:
"Nonce" is a portmanteau of "number used only once." It is a four-bit number added to a hashed—or encrypted—block in a blockchain that, when rehashed, meets the difficulty level restrictions. The nonce is the number that blockchain miners are solving for.
Write what you want  in the "nonce" box.

![4](https://user-images.githubusercontent.com/109109176/178451948-64eda2d5-40c5-4ed5-89da-fcab119130c6.PNG)

Mine the block...
is the nonce changing? And the hash? ("y" or "n","y" or "n")

Answer #2:
n,n

Question #3:
Now try it with the data part, write "distributed" in the data box. 
Mine the block.
Whats the new hash? (copy paste all hash)

Answer #3:
00009718b21748a9b14da4603ab9f289dc500b20be3fdf9715d32f6803a440c4

![5](https://user-images.githubusercontent.com/109109176/178456658-a9b628ad-332c-419f-afcc-a289ee28248c.PNG)


Question #4:
Now write  "distriBUTED", is the hash changing? ("y" or "n")

Answer #4:
y

Question #5:
The security of a blockchain is that if any of the blocks is modified, even with a blank space, the rest of the chain also changes... true or false (t or f)

Answer #5:
t

Question #6:
In the "peer A" block 3, write in the data box: "Peer-to-peer" 
In the "peer B" block 5, write in the data box: "Peer to peer" 
Mine the blocks until all blocks turn green.

![6](https://user-images.githubusercontent.com/109109176/178458420-0078a320-2e82-4296-96a4-cffcab94d29b.PNG)

Answer #6

Question #7:
Do you think that this is a valid blockchain? (y or n)

Answer #7:
n

Question #8:
What is the most famous way attack for a blockchain?("a" or "b" or "c" or "d")
a) brute force attack
b) 51% attack
c) blockchain injection attack
d) a blockchain can't be overcome in any way

Answer #8:
b

Question #9:
In order to refresh the webpage, write this link in the browser: http://localhost:3000/distributed
In the "peer B" block 4, write: "crypto"
In the "peer C" block 4, write the same.

![7](https://user-images.githubusercontent.com/109109176/178459467-543c41f9-00c3-4429-bb46-22744d7902e9.PNG)

Mine the blocks until all blocks turn green.

Answer #9:


Question #10:
Do you think that this is a valid blockchain? (y or n)

Answer #10:
y

Question #11:

Answer #11:
BLOCKCHAIN IS FUTURE











