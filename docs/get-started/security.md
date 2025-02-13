# Security Best Practices for Linea Developers

Security is a critical aspect of smart contract development on Linea. Below are best practices to help developers build secure applications.

## 1. Use Proper Access Controls
- Implement role-based permissions using `Ownable` or `AccessControl`.
- Restrict critical functions to specific accounts or contract logic.

## 2. Avoid Reentrancy Attacks
- Use the **Checks-Effects-Interactions** pattern.
- Utilize Reentrancy Guards (`nonReentrant` modifier in OpenZeppelin).

## 3. Prevent Integer Overflows and Underflows
- Use `SafeMath` or Solidity 0.8+ built-in overflow protection.

## 4. Secure Private Keys and Environment Variables
- Store secrets in `.env` files and **never hardcode private keys**.
- Use secure wallet infrastructure like **hardware wallets** for deployments.

## 5. Be Cautious with External Calls
- Validate and sanitize all user input.
- Avoid making state-changing calls to unknown contracts.

## 6. Regularly Audit and Test Your Smart Contracts
- Write comprehensive unit tests and use **fuzzing techniques**.
- Consider third-party **smart contract audits** before deployment.

For additional resources, visit [Ethereum Security Best Practices](https://ethereum.org/en/developers/docs/smart-contracts/security/).
