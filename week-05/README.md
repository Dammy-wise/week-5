# Week 05 — Exceptions, logging and test discipline

The final API defines `NotFoundException`, `ConflictException` and `InsufficientStockException`, plus a centralized `@RestControllerAdvice` with stable error codes and field validation details. Service logging records operational order identifiers and totals only; it must never log passwords, card details, credentials or unnecessary personal information. File examples use try-with-resources in `SafeCsvReader`.

The JUnit suite contains more than 15 test methods across pricing, collection analytics, CSV validation and order-state boundaries. Capture the real `mvn test` output for the submission.
