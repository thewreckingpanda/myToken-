
# Create a Token using Solidity

The project involves the creation of a smart contract for a custom cryptocurrency in Remix IDE. The contract is designed to manage the token's properties and operations. It includes public variables to store essential details such as the Token Name, Token Abbreviation, and Total Supply of the cryptocurrency. The contract further employs a mapping structure to associate addresses with their corresponding token balances.

Here, Token Name is 'PANDA' and Token Abbreviation. The initial total supply would be 0. A mapping function is intialized named 'balances' (addresses=>uint) which will tell the current balance of the corresponding address.


## Functionality

Key functionalities are implemented through two main functions:

Mint Function: This function allows the creation of new tokens. It takes two parameters: an address and a value. The value specified is added to the total supply of the cryptocurrency, consequently increasing the balance of the provided address by the same amount.

Burn Function: The burn function serves the purpose of token destruction. Similar to the mint function, it requires an address and a value. The value indicated is subtracted from the total supply, reflecting a reduction in the overall token count. Additionally, the balance of the provided address is decreased by the specified value.
## Special feature

A conditional statement is implemented in burn function to make sure the balance of the address is greater than or equal to the amount that is supposed to be burnt.

if(balances[_address] >= _value){
    ...
    ...
    ...
}    
## Deployment

To deploy this smart contract follow the steps given below:

Step 1 : Open REMIX IDE
Step 2 : Create a new file 
Step 3 : Type or paste the code in the file 
Step 4 : Click on compile
Step 5 : Deploy it

To execute the key functions, copy the addresses provided by REMIX IDE in the deployment section and paste it in the deployed contracts UI.
## License

This contract is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Credits
This project is created by ***[Rajat Verma](https://github.com/thewreckingpanda)***.

## Disclaimer

This contract is provided for educational purposes only. Use it in a controlled environment and do not use it in a production environment without proper security audits and testing.
