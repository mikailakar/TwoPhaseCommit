# Two-Phase Commit (2PC) Project

This project demonstrates the implementation of the Two-Phase Commit (2PC) protocol in .NET. The Two-Phase Commit protocol is a distributed algorithm used to ensure that all participants in a distributed transaction either commit or roll back their changes, maintaining the atomicity of the transaction.

## Features

- **Two-Phase Commit Protocol**: Implementation of the 2PC protocol for managing distributed transactions.
- **Distributed Transaction Handling**: Coordination between multiple services to ensure consistency.
- **ASP.NET Core Web API**: Provides a web API for initiating and managing transactions.
- **Entity Framework Core**: Used for data access and management.

## API Documentation

### Transaction Management

- `POST /api/Transactions/initiate`: Initiate a new distributed transaction.
- `POST /api/Transactions/commit`: Commit an ongoing transaction.
- `POST /api/Transactions/rollback`: Roll back a transaction if an error occurs.

### API STATE
  0: Ready
  1: Pending
  2: Unready

### TRANSACTION STATE
  0: Done
  1: Pending
  2: Abort (Rollback)
