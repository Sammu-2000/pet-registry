# Pet Registry Smart Contract

A Clarity smart contract for registering pets and allowing users to adopt them on the Stacks blockchain.

## Features

- **Register Pets:** Add new pets with a name and breed.
- **Adopt Pets:** Users can adopt available pets.
- **Event Logging:** Emits events for pet registration and adoption.
- **Read Functions:** Query pet details and total registered pets.

## Contract Functions

### Public Functions

- `register-pet (name, breed)`  
  Registers a new pet with the given name and breed. Returns the new pet's ID.

- `adopt-pet (pet-id)`  
  Allows a user to adopt a pet by its ID. Returns a success message or error.

### Read-Only Functions

- `get-pet (pet-id)`  
  Returns the pet's details (name, breed, adopter) for the given ID.

- `get-total-pets`  
  Returns the total number of registered pets.

## Events

- **pet-registered:** Emitted when a new pet is registered.
- **pet-adopted:** Emitted when a pet is adopted.

## Usage

1. **Clone the repository:**
   ```sh
   git clone https://github.com/your-username/pet-registry.git
   cd pet-registry
   ```

2. **Deploy the contract:**  
   Use the [Stacks CLI](https://docs.stacks.co/docs/cli-usage) or your preferred Stacks development environment.

3. **Interact with the contract:**  
   Use Clarity tools or a frontend to call contract functions.

## File Structure

- `contracts/pet-registry.clar` — Main smart contract source code.
- `tests/` — Test cases for the contract.

## Requirements

- [Stacks Blockchain](https://www.stacks.co/)
- [Clarity Language](https://docs.stacks.co/docs/clarity-overview)
