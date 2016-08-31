# ThriftCompatibilityTest
Test thrift versions intercompatibility

## How to test:
1. Start server 0.9.3 Test with Client 0.9.3
2. Start server 0.9.3 Test with Client 0.7.0
3. Start server 0.7.0 Test with Client 0.7.0 (Need to figure out how to return correctly)
4. Start server 0.7.0 Test with Client 0.9.3 (Need to figure out how to return correctly)

## Findings
1. No problem related to Transport
2. Need to figure out how to return correctly for some functions in my thrift file. This shouldn't be a problem with what we have in ele codebase because returns from the thrift server were taken care of (i.e there was an extra null for no error as first argument of result(success in the case of ele)).

## Overall result
Good to deploy. 
