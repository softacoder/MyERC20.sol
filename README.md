# MyERC20.sol

This is a custom ERC20 token contract with access control using OpenZeppelin's libraries:

Inheritance:

ERC20: Standard token functionality (transfers, balances, etc.).
AccessControl: Role-based permissions (admin/minter roles).
Roles:

DEFAULT_ADMIN_ROLE: Granted to the deployer (can manage roles).
MINTER_ROLE: Granted to the deployer (can mint new tokens).
Key Functions:

constructor(): Sets token name (My Cyfrin CLF Token) and symbol (CLF).
mint(): Only callable by MINTER_ROLE; creates new tokens and assigns them to to.
Security:

Uses OpenZeppelin’s audited contracts.
Role checks prevent unauthorized minting.
