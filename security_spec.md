# Security Spec

## Data Invariants
- Every user must have a valid role ('admin', 'technician', 'doctor').
- Only admins can change roles.
- Users can only read their own profile, or admins can read everything.

## The "Dirty Dozen" Payloads (Examples)
1. { "role": "admin" } // Unauthorized role setting
2. { "role": "hacker" } // Invalid role
...

## Test Runner
(To be implemented in firestore.rules.test.ts)
