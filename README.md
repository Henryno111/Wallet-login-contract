# Admin Control Smart Contract

A Clarity smart contract implementing secure admin management with multi-signature requirements for administrative actions.

## Features

- Multi-admin management system
- Time-bound action proposals
- Two-step admin addition process
- Role assignment capabilities
- Admin removal with dual-admin verification

## Key Functions

- `propose-admin`: Nominate a new admin
- `accept-admin`: Accept admin nomination
- `propose-admin-action`: Propose administrative actions
- `execute-admin-action`: Execute proposed actions
- `remove-admin`: Remove existing admin rights
- `is-admin`: Check admin status

## Security Features

- 24-hour expiration window for proposals
- Different admin required for execution vs proposal
- Input validation and error handling
- Prevention of self-targeting actions

## Error Codes

- `ERR_NOT_ADMIN` (u102): Unauthorized admin access
- `ERR_ADMIN_ALREADY_EXISTS` (u103): Admin already exists
- `ERR_INVALID_ADMIN_ACTION` (u104): Invalid admin action
- `ERR_ACTION_TIMEOUT` (u105): Action expired
- `ERR_INVALID_ACTION_TYPE` (u106): Invalid action type
- `ERR_INVALID_TARGET` (u107): Invalid target principal