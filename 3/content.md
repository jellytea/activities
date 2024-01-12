# 2024.1.12
## What have I done today？

### Fixed bugs
- *cee/parser.Parser.ExpectOperator* returns the next token.
- *cee/token.IsOperator* range was incorrect.

### Implementations
- Implemented *cee/parser.ExpectBinaryExpr*
- Tried to implement binary operator precedence:
  1) Sort precedences of the operators.
  2) Reduce expressions with operator between, begin from highest precedence.
  3) Reduce until no more expression available.
  4) Return the reduction.
- Dropped binary operator precedence lang spec, because the implementation will slow the efficiency of parser down.
