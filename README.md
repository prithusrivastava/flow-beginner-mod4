# SomeContract - Access Modifiers Guide

## Overview

`SomeContract` demonstrates the usage of access modifiers for variables and functions within a contract.

## Access Modifiers

### 1. `pub` (Public)

- **Usage**: `pub var`, `pub struct`, `pub fun`, `pub resource`
- **Description**: Public entities are accessible from any scope, including external contracts and modules.

### 2. `pub(set)` (Public Set)

- **Usage**: `pub(set) var`
- **Description**: Allows external contracts to read the variable but restricts write access to the defining contract.

### 3. `access(contract)` (Contract-level Access)

- **Usage**: `access(contract) var`, `access(contract) fun`
- **Description**: Restricted to access within the current contract and any contracts that inherit from it.

### 4. `access(self)` (Private to Self)

- **Usage**: `access(self) var`, `access(self) fun`
- **Description**: Accessible only within the current struct or contract, ensuring privacy within the defining entity.
