# Multiplication

Scenario: Signs of the numbers
 Given The Calculator is on
 When I Typed in "Positive Number"
 and I press "Multiply"
 And I type in "Negative number"
 And I press "equals"
 Then I see the "Multiplied number" as the result with negative sign

Scenario: Zero value multiplication
 Given The Calculator is on
 When I Typed in "Number"
 and I press "Multiply"
 And I type in "Zero"
 And I press "equals"
 Then I see the "Zero" as the result

Scenario: Multiplication by 1
 Given The Calculator is on
 When I Typed in "Number"
 and I press "Multiply"
 And I type in "One"
 And I press "equals"
 Then I see the "Nymber" as the result

Scenario: Decimal value multiplication
 Given The Calculator is on
 When I Typed in "Decimal Number 1"
 and I press "Multiply"
 And I type in "Decimal Number 2"
 And I press "equals"
 Then I see the "Multiplied Decimal Number" as the result

Scenario: Irrational value multiplication
 Given The Calculator is on
 When I Typed in "Irrational Number 1"
 and I press "Multiply"
 And I type in "Irrational Number 2"
 And I press "equals"
 Then I see the "Multiplied Number" as the result

Scenario: Simple multiplication
 Given The Calculator is on
 When I Typed in "Number 1"
 and I press "Multiply"
 And I type in "Number 2"
 And I press "equals"
 Then I see the "Multiplied Number" as the result

Scenario: Rational multiplication
 Given The Calculator is on
 When I Typed in "Rational Number 1"
 and I press "Multiply"
 And I type in "Rational Number 2"
 And I press "equals"
 Then I see the "Multiplied Number" as the result

Scenario: Decimal & integer multiplication
 Given The Calculator is on
 When I Typed in "Decimal Number"
 and I press "Multiply"
 And I type in "Integer Number"
 And I press "equals"
 Then I see the "Multiplied Decimal Number" as the result
 
Scenario: More than two numbers multiplication
 Given The Calculator is on
 When I Typed in "Number 1"
 and I press "Multiply"
 And I type in "Number 2"
 And I press "Multiply"
 And I type in "Number 3"
 And I press "equals"
 Then I see the "Multiplied number" as the result

Scenario: Range of operand exceeds allowed limit
 Given The Calculator is on
 When I Typed in "Number 1"
 and I press "Multiply"
 And I type in "Number 2"
 And I press "equals"
 Then I see the "Range Error" as the result

Scenario: Pressing "multiply button" multiple times
 Given The Calculator is on
 When I Typed in "Number 1"
 and I press "Multiply"
 and I press "Multiply"
 And I type in "Number 2"
 And I press "equals"
 Then I see the "Error" as the result

Scenario: Interleaving operators
 Given The Calculator is on
 When I Typed in "Number 1"
 and I press "Multiply"
 and I press "Addition"
 And I type in "Number 2"
 And I press "equals"
 Then I see the "Error" as the result

Scenario: Decimal value capping
 Given The Calculator is on
 When I Typed in "Number 1"
 and I press "Multiply"
 And I type in "Number 2"
 And I press "equals"
 Then I see the "Multiplied Number" as the result upto two decimal place
