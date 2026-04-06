# Testing Guide

## Test Types Covered

### 1. Status Code Tests
Verify API returns correct HTTP status codes.

### 2. Response Structure Tests
Ensure response has required fields and correct types.

### 3. Data Validation Tests
Verify data values are correct and consistent.

### 4. Performance Tests
Check response times are within acceptable range.

### 5. Error Handling Tests
Verify API handles invalid requests gracefully.

## Running Tests

```bash
npm test              # All tests
npm run test:products # Specific suite
npm run test:verbose  # Detailed output
```

## Interpreting Results

Green ✓ = Test passed
Red ✗ = Test failed
Details in HTML report: `results/api-test-report.html`
