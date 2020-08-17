# Subtraction

Scenario: Subtraction of two positive numbers
 Given The calculator is on
 When I type in "positive number"
 And I press "minus"
 And I type in "positive number"
 And I press "equals"
 Then I see the "subtracted number" as the result

Scenario: Subtraction of two negative numbers
 Given The calculator is on
 When I type in "negative number"
 And I press "minus"
 And I type in "negative number"
 And I press "equals"
 Then I second number is added to first negative number and I see
 the "subtracted number" as the result with appropriate sign

Scenario: Subtraction of fractions
 Given The calculator is on and I am able to enter the fraction number
 When I type in "fraction number 1"
 And I press "minus"
 And I type in "fraction number 2"
 And I press "equals"
 Then I see the "subtracted number" as the result in fraction form
 with appropriate sign

Scenario: Subtraction of positive and negative numbers
 Given The calculator is on
 When I type in "positive number"
 And I press "minus"
 And I type in "negative number"
 And I press "equals"
 Then I see the "subtracted number" as the result and
 addition of two numbers takes place

Scenario: Subtraction of decimals
 Given The calculator is on and able to enter decimal number
 When I type in "decimal number 1"
 And I press "minus"
 And I type in "decimal number 2"
 And I press "equals"
 Then I see the "Subtracted number" as the result in decimal form
 with appropriate sign

Scenario: Typing operator more than once
 Given The calculator is on
 When I type in "number 1"
 And I press "minus"
 And I press "other operator"
 And I type in "number 2"
 And I press "equals"
 Then I see the "Error" as the result

Scenario: Subtraction of more than two numbers
 Given The calculator is on
 When I type in "number 1"
 And I press "minus"
 And I type in "number 2"
 And I press "minus"
 And I type in "number 3"
 And I press "equals"
 Then I see the "subtracted number" as the result
 with appropriate sign

Scenario: Converse operation
 Given The calculator is on
 When I type in "number 1"
 And I press "minus"
 And I type in "number 2"
 And I press "equals"
 And I press "Clear"
 And I type in "number 2"
 And I press "minus"
 And I type in "number 1"
 And I press "equals"
 Then I see the result of both cases need not be same
