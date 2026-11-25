# MC/DC tool qualification test cases

This document provides test cases that show that the tool satisfies the
requirements listed in [requirements](requirements.md).

## MCDC-BASICS-001

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** Test coverage of various combinations for a Boolean
“OR” operation.

**Input data:** [Test source code](../../tests/qual/basics-001.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows 100% coverage for the Boolean
expression inside the `test_simple_or()` function.

## MCDC-BASICS-002

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that partial coverage for a Boolean OR operation
is reported correctly, taking into account C’s short-circuit evaluation
of Boolean expressions.

**Input data:** [Test source code](../../tests/qual/basics-002.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows that only the first part of the
Boolean expression inside the `test_simple_or()` function was sensitized
for True and False values.

## MCDC-BASICS-003

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that partial coverage for a Boolean OR operation
is reported correctly.

**Input data:** [Test source code](../../tests/qual/basics-003.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows that only the first part of the
Boolean expression inside the `test_simple_or()` function was sensitized
for the False value, while the second part was sensitized for both True
and False values.

## MCDC-BASICS-004

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that a simple Boolean “AND” operation is handled
and provides full coverage.

**Input data:** [Test source code](../../tests/qual/basics-004.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows 100% coverage for the Boolean
expression inside the `test_simple_and()` function.

## MCDC-BASICS-005

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that a simple Boolean “AND” operation is handled
and MC/DC metric is correctly calculated for partial coverage.

**Input data:** [Test source code](../../tests/qual/basics-005.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows 50% coverage for the Boolean
expression inside the `test_simple_and()` function; the first part of
the expression is not sensitized.

## MCDC-BASICS-006

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that a simple Boolean “AND” operation is handled
and MC/DC metric is correctly calculated for partial coverage.

**Input data:** [Test source code](../../tests/qual/basics-006.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows 0% coverage for the Boolean
expression inside the `test_simple_and()` function.

## MCDC-BASICS-007

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that a simple Boolean “NOT EQUAL” operation is
handled and MC/DC metric is calculated correctly.

**Input data:** [Test source code](../../tests/qual/basics-007.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows 100% coverage for the Boolean
expression inside the `test_neq()` function.

## MCDC-BASICS-008

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that a simple Boolean “NOT” operation is handled
and MC/DC metric is calculated correctly.

**Input data:** [Test source code](../../tests/qual/basics-008.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows 100% coverage for the Boolean
expression inside the `test_not()` function.

## MCDC-BASICS-009

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that a simple “LESS THAN” operation is handled
and MC/DC metric is calculated correctly.

**Input data:** [Test source code](../../tests/qual/basics-009.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows complete coverage for all comparison
expressions inside the `test_lt()` function, except the expression
`a < 65538`.

## MCDC-BASICS-010

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that a simple “LESS THAN OR EQUAL” operation is
handled and MC/DC metric is calculated correctly.

**Input data:** [Test source code](../../tests/qual/basics-010.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows complete coverage for all comparison
expressions inside the `test_lte()` function, except the expression
`a <= 65538`.

## MCDC-BASICS-011

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that a simple “GREATER THAN” operation is handled
and MC/DC metric is calculated correctly.

**Input data:** [Test source code](../../tests/qual/basics-011.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows complete coverage for all comparison
expressions inside the `test_gt()` function, except the expression
`a > 65538`.

## MCDC-BASICS-012

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that a simple “GREATER THAN OR EQUAL” operation is
handled and MC/DC metric is calculated correctly.

**Input data:** [Test source code](../../tests/qual/basics-012.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows complete coverage for all comparison
expressions inside the `test_gte()` function, except the expression
`a >= 65538`.

## MCDC-BASICS-013

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that a simple “EQUAL” operation on integer
variables is handled and MC/DC metric is calculated correctly.

**Input data:** [Test source code](../../tests/qual/basics-013.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows complete coverage for the Boolean
expression inside the `test_eq()` function.

## MCDC-BASICS-014

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that a simple “NOT EQUAL” operation on integer
variables is handled and MC/DC metric is calculated correctly.

**Input data:** [Test source code](../../tests/qual/basics-014.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows complete coverage for the Boolean
expression inside the `test_neq()` function.

## MCDC-COMPLEX-001

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that a complex Boolean OR expression is handled
and the tool correctly calculates full MC/DC coverage based on a minimal
set of tests.

**Input data:** [Test source code](../../tests/qual/complex-001.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows complete coverage for the Boolean
expression inside the `test_or()` function.

## MCDC-COMPLEX-002

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that a complex Boolean AND expression is handled
and the tool correctly calculates full MC/DC coverage based on a minimal
set of tests.

**Input data:** [Test source code](../../tests/qual/complex-002.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows complete coverage for the Boolean
expression inside the `test_and()` function.

## MCDC-COMPLEX-003

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that a complex Boolean expression is handled and
the tool correctly calculates full MC/DC coverage based on a minimal set
of tests.

**Input data:** [Test source code](../../tests/qual/complex-003.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows complete coverage for the Boolean
expression inside the `test_func()` function.

## MCDC-COMPLEX-004

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that a complex Boolean expression is handled and
the tool correctly calculates full MC/DC coverage based on a minimal set
of tests.

**Input data:** [Test source code](../../tests/qual/complex-004.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows complete coverage for the Boolean
expression inside the `test_func()` function.

## MCDC-COMPLEX-005

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that a complex Boolean expression is handled and
the tool correctly calculates MC/DC coverage based on an excessive but
incomplete set of tests.

**Input data:** [Test source code](../../tests/qual/complex-005.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows incomplete coverage for the Boolean
expression inside the `test_func()` function: variables “b” and “d” do
not show independence.

## MCDC-PARSING-001

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`
  - `MCDC~SREQ~HandleComplexConstructs~1`

**Objective:** To verify that the tool handles Boolean expressions that
access global variables.

**Input data:** [Test source code](../../tests/qual/parsing-001.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** Report shows complete coverage for the Boolean
expression inside the `test_global_var()` function.

## MCDC-PARSING-002

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~Outcomes~1`
  - `MCDC~SREQ~HandleComplexConstructs~1`

**Objective:** To verify that the tool handles multiple nested Boolean
expressions.

**Input data:** [Test source code](../../tests/qual/parsing-002.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** The tool is able to parse the source file and
generate a report successfully. Report shows incomplete MC/DC coverage.

## MCDC-PARSING-003

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`
  - `MCDC~SREQ~HandleComplexConstructs~1`

**Objective:** To verify that the tool handles pointer comparisons.

**Input data:** [Test source code](../../tests/qual/parsing-003.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** The tool is able to parse the source file and
generate a report successfully. Report shows incomplete MC/DC coverage.

## MCDC-PARSING-004

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`
  - `MCDC~SREQ~HandleComplexConstructs~1`

**Objective:** To verify that the tool handles `sizeof()` expressions.

**Input data:** [Test source code](../../tests/qual/parsing-004.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** The tool is able to parse the source file and
generate a report successfully. Report shows incomplete MC/DC coverage.

## MCDC-PARSING-005

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~HandleDoubleNot~1`
  - `MCDC~SREQ~Outcomes~1`
  - `MCDC~SREQ~HandleComplexConstructs~1`

**Objective:** To verify that the tool handles `__builtin_expect()`
expressions wrapped inside macros.

**Input data:** [Test source code](../../tests/qual/parsing-005.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** The tool is able to parse the source file and
generate a report successfully. Report shows incomplete MC/DC coverage.

## MCDC-PARSING-006

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`
  - `MCDC~SREQ~HandleComplexConstructs~1`

**Objective:** To verify that the tool handles complex macros that contain
Boolean expressions.

**Input data:** [Test source code](../../tests/qual/parsing-006.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** The tool is able to parse the source file and
generate a report successfully. Report shows incomplete MC/DC coverage.

## MCDC-PARSING-007

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~HandleConstants~1`
  - `MCDC~SREQ~HandleComplexConstructs~1`

**Objective:** To verify that the tool handles simple fully constant
expressions.

**Input data:** [Test source code](../../tests/qual/parsing-007.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** The tool is able to parse the source file, but no
report is generated, as the source file has no non-constant Boolean
expressions.

## MCDC-PARSING-008

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~HandleConstants~1`
  - `MCDC~SREQ~HandleComplexConstructs~1`

**Objective:** To verify that the tool handles complex fully constant
expressions.

**Input data:** [Test source code](../../tests/qual/parsing-008.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** The tool is able to parse the source file, but no
report is generated, as the source file has no non-constant Boolean
expressions.

## MCDC-PARSING-009

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~HandleConstants~1`
  - `MCDC~SREQ~HandleComplexConstructs~1`

**Objective:** To verify that the tool handles Boolean expressions that
provide a constant result.

**Input data:** [Test source code](../../tests/qual/parsing-009.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** The tool is able to parse the source file, but no
report is generated, as the source file has no non-constant Boolean
expressions.

## MCDC-PARSING-010

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`
  - `MCDC~SREQ~HandleComplexConstructs~1`

**Objective:** To verify that the tool handles comparisons with
enumerations.

**Input data:** [Test source code](../../tests/qual/parsing-010.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** The tool is able to parse the source file and
generate a report successfully. Report shows incomplete MC/DC coverage.

## MCDC-PARSING-011

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~Outcomes~1`

**Objective:** To verify that the tool handles Boolean expressions that
include function call return values.

**Input data:** [Test source code](../../tests/qual/parsing-011.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** The tool is able to parse the source file and
generate a report successfully. Report shows incomplete MC/DC coverage.

## MCDC-PARSING-012

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`
  - `MCDC~SREQ~HandleComplexConstructs~1`

**Objective:** To verify that the tool handles code that uses `goto` labels.

**Input data:** [Test source code](../../tests/qual/parsing-012.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** The tool is able to parse the source file and
generate a report successfully. Report shows incomplete MC/DC coverage.

## MCDC-PARSING-013

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`
  - `MCDC~SREQ~HandleComplexConstructs~1`

**Objective:** To verify that the tool handles ternary expressions inside
macros.

**Input data:** [Test source code](../../tests/qual/parsing-013.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** The tool is able to parse the source file and
generate a report successfully. Report shows incomplete MC/DC coverage.

## MCDC-PARSING-014

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`
  - `MCDC~SREQ~HandleComplexConstructs~1`

**Objective:** To verify that the tool handles statement expressions inside
macros.

**Input data:** [Test source code](../../tests/qual/parsing-014.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** The tool is able to parse the source file and
generate a report successfully. Report shows incomplete MC/DC coverage.

## MCDC-PARSING-015

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~Outcomes~1`
  - `MCDC~SREQ~HandleComplexConstructs~1`

**Objective:** To verify that the tool handles Boolean expressions that do
not provide a resulting value.

**Input data:** [Test source code](../../tests/qual/parsing-015.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** The tool is able to parse the source file and
generate a report successfully. Report shows incomplete MC/DC coverage.

## MCDC-PARSING-016

**Covers:**
  - `MCDC~SREQ~UseClang~1`
  - `MCDC~SREQ~FindBoolExpr~1`
  - `MCDC~SREQ~IdentifyCond~1`
  - `MCDC~SREQ~ShortCircuit~1`
  - `MCDC~SREQ~Outcomes~1`
  - `MCDC~SREQ~HandleComplexConstructs~1`

**Objective:** To verify that the tool handles assignment of a Boolean
expression’s value to a variable.

**Input data:** [Test source code](../../tests/qual/parsing-016.c)

**Test procedure:** Run the provided test program and collect MC/DC
metric with the MC/DC tool according to the procedure described in the
tool manual.

**Expected results:** The tool is able to parse the source file and
generate a report successfully. Report shows incomplete MC/DC coverage.
