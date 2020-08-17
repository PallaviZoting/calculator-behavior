# Addition

Scenario: Addition of two positive numbers
 Given The calculator is on
 When I type in "positive number"
 And I press "plus"
 And I type in "positive number"
 And I press "equals"
 Then I see the "added number" as the result

Scenario: Addition of two negative numbers
 Given The calculator is on
 When I type in "negative number"
 And I press "plus"
 And I type in "negative number"
 And I press "equals"
 Then I see the "added number" as the result

Scenario: Addition of fractions
 Given The calculator is on and I am able to enter the fraction number
 When I type in "fraction number 1"
 And I press "plus"
 And I type in "fraction number 2"
 And I press "equals"
 Then I see the "added number" as the result in fraction form

Scenario: Addition of positive and negative numbers
 Given The calculator is on
 When I type in "positive number"
 And I press "plus"
 And I type in "negative number"
 And I press "equals"
 Then I see the "added number" as the result

Scenario: Addition of decimals
 Given The calculator is on and able to enter decimal number
 When I type in "decimal number 1"
 And I press "plus"
 And I type in "decimal number 2"
 And I press "equals"
 Then I see the "added number" as the result in decimal form

Scenario: Typing operator more than once
 Given The calculator is on
 When I type in "number 1"
 And I press "plus"
 And I press "other operator"
 And I type in "number 2"
 And I press "equals"
 Then I see the "Error" as the result

Scenario: Addition of more than two numbers
 Given The calculator is on
 When I type in "number 1"
 And I press "plus"
 And I type in "number 2"
 And I press "plus"
 And I type in "number 3"
 And I press "equals"
 Then I see the "added number" as the result

Scenario: Adding numbers where the result goes out of range
 Given The calculator is on
 When I type in "Large number 1"
 And I press "plus"
 And I type in "Large number 2"
 And I press "equals"
 Then I see the "Range Error" as the result

Scenario: 6+* is provided as input
 Given The calculator is on
 When I type in "positive number"
 And I press "plus"
 And I press "multiply"
 And I type in "positive number"
 And I press "equals"
 Then I see the "Error" as the result

Scenario: Identify operation
 Given The calculator is on
 When I press operator
 Then I am able to identify operation

Scenario: Converse operation
 Given The calculator is on
 When I type in "number 1"
 And I press "plus"
 And I type in "number 2"
 And I press "equals"
 And I press "Clear"
 And I type in "number 2"
 And I press "plus"
 And I type in "number 1"
 And I press "equals"
 Then I see the "added number" as the result for both cases
