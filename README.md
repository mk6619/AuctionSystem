# AuctionSystem

This is a smart contract build in solidity which can be used as a **reference** for a decentralized auction system.  
Contract has a constructor, 2 struct and 5 functions.  
Constructor is used for initializing the organizer address for safety purposes so that no other than organizer can use the code.  
There are 2 structs User and Item. You can edit these structs according to your need.    
There are 5 functions :-  
  1. **function addItemToAuction(string name, uint256 cost) public ()** :-
       This function takes 2 arguments to define an Item in auction. First Argument is name of the item which is string type and other argument is cost of that item.
  2. **function addUserToAuction(string name, address userAddress, uint256 coins) public ()** :- This function takes 3 arguments to define an User. First argument is name of the user, second is the address of the User (Ethereum address of the user) and third argument is the maximum coins or currency that user can use in auction.
  3. **function itemBuy(uint itemID, address userAddress) public ()** :- This function takes 2 argument to sell item to the user with the address userAddress.
  4. **function getItem(uint itemID) public constant returns (string,uint256,address)** :- This constant function will take one argument itemID and will return name, cost and owner of the particular item associated with this id.
  5. **function getUser(address userAddress) public constant returns (string,uint256,uint[])** :- This constant function will take one argument userAddress and will return name, coins and array of itemID of the items user owns.
  
  **Note**  
  itemID of particular item I which would have turn i in the auction, will have id i. It is taken care of in addItemToAuction function.
