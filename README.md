# Assert Action

## Inputs
- comparison:
  - The kind of comparison to be done, where valid values are in the set { `>`, `<`, `==`, `>=`, `<=`, `!=` }
- expected
- actual


If `${expected} ${comparison} ${actual}` evaluates to false, the action will fail

## Examples:
- comparison: `>`
  - `${expected} == ${actual}` ==> FAIL
  - `${expected} > ${actual}` ==> PASS
  - `${expected} < ${actual}` ==> FAIL
- comparison: `<`
  - `${expected} == ${actual}` ==> FAIL
  - `${expected} > ${actual}` ==> FAIL
  - `${expected} < ${actual}` ==> PASS
- comparison: `==`
  - `${expected} == ${actual}` ==> PASS
  - `${expected} > ${actual}` ==> FAIL
  - `${expected} < ${actual}` ==> FAIL
- comparison: `>=`
  - `${expected} == ${actual}` ==> PASS
  - `${expected} > ${actual}` ==> PASS
  - `${expected} < ${actual}` ==> FAIL
- comparison: `<=`
  - `${expected} == ${actual}` ==> PASS
  - `${expected} > ${actual}` ==> FAIL
  - `${expected} < ${actual}` ==> PASS
- comparison: `!=`
  - `${expected} == ${actual}` ==> FAIL
  - `${expected} > ${actual}` ==> PASS
  - `${expected} < ${actual}` ==> PASS
