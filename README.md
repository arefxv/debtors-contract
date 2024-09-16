# debtors-contract
This repository contains a set of smart contracts for managing debtors using the Solidity programming language. The contracts allow you to create and manage debtor records, storing details like the debtor's name and amount owed. There is also a factory contract that can create multiple debtor contracts and interact with them.
Contracts
1. Debtors
This contract keeps a list of debtors and allows storing, retrieving, and adding new debtors.

Functions:
store(uint256 _amount): Stores the amount provided.
retrieve(): Retrieves the stored amount.
addDebtor(string memory _name, uint256 _amount): Adds a debtor to the list with their name and amount owed.
Data Structures:
Debtors: Struct that holds debtor's name and amount owed.
listOfDebtors: Public array storing all debtors.
nameToAmount: Mapping of debtor names to amounts owed.
2. johnDebtors
This contract is similar to the Debtors contract but is specific to an individual named John.

Functions:
srote(uint256 _amount): (Assumed typo, should be store) Stores the amount provided.
retrieve(): Retrieves the stored amount.
addDebtor(string memory _name, uint256 _amount): Adds a debtor for John’s list.
3. DebtorsFactory
This contract allows the creation of multiple Debtors contracts. Each contract can be individually managed for storing and retrieving debtor amounts.

Functions:
createDebtorsContract(): Creates a new Debtors contract.
dfStore(uint256 _debtorsIndex, uint256 _newDebtorsNumber): Stores a new debtor amount in a specific debtor contract by index.
dfGet(uint256 _debtorsIndex): Retrieves the debtor amount from a specific debtor contract by index.
How to Use
Deploy the DebtorsFactory contract.
Use createDebtorsContract() to create a new debtor contract.
Use dfStore() to store a debtor amount in a specific contract.
Use dfGet() to retrieve the debtor amount from a specific contract.
License
This project is licensed under the MIT License. See the LICENSE file for details.

