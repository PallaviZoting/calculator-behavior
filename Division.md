# Division

Scenario: Division by 0 when operand 1 is any number
 Given The calculator is on
 When I type in "number"
 And I press "Divide"
 And I type in "Zero"
 And I press "equals"
 Then I see the "Cannot divide by zero" as the result

Scenario: Divide 0 by any number
 Given The calculator is on
 When I type in "Zero"
 And I press "Divide"
 And I type in "Number"
 And I press "equals"
 Then I see the "Zero" as the result

Scenario: Sign rules for operands
 Given The calculator is on
 When I type in "positive number"
 And I press "Divide"
 And I type in "negative number"
 And I press "equals"
 Then I see the "Divided negative number" as the result

Scenario: Division isn't symmetric
 Given The calculator is on
 When I type in "Number 1"
 And I press "Divide"
 And I type in "Number 2"
 And I press "equals"
 And I press "Clear"
 And I type "Number 2"
 And I press "Divide"
 And I type "Number 1"
 And I press "equals"
 Then I see the both results are different

Scenario: Division when both operands are 0
 Given The calculator is on
 When I type in "Zero"
 And I press "Divide"
 And I type in "Zero"
 And I press "equals"
 Then I see the "Undefined" as the result

Scenario: Recurring decimal case
 Given The calculator is on
 When I type in "recurrring number 1"
 And I press "Divide"
 And I type in "recurring number 2"
 And I press "equals"
 Then I see the "Divided number" as the result rounded off to two decimal place

Scenario: Multiple times "/" is pressed
 Given The calculator is on
 When I type in "number 1"
 And I press "Divide"
 And I press "Divide"
 And I type in "number 2"
 And I press "equals"
 Then I see the "Divided Number" as the result

Scenario: Interleaving of multiple operators
 Given The calculator is on
 When I type in "number 1"
 And I press "Divide"
 And I press "Addition"
 And I type in "number 2"
 And I press "equals"
 Then I see the "Error" as the result

Scenario: When operand 2 is not present
 Given The calculator is on
 When I type in "number 1"
 And I press "Divide"
 And I press "equals"
 Then I see the "one" as the result

Scenario: Division of multiple numbers (eg: 4/5/6/7)
 Given The calculator is on
 When I type in "number 1"
 And I press "Divide"
 And I type in "number 2"
 And I press "Divide"
 And I type "number 3"
 And I press "Divide"
 And I type "number 4"
 And I press "equals"
 Then I see the "Divided" as the result (left to right division)
