# Addition

Scenario: Addition of two positive numbers

 Given The calculator is turned on

 When I type in "positive number"
 And I press "plus"
 And I type in "positive number"
 And I press "equals"

 Then I see the "added number" as the result

Scenario: Addition of two negative numbers

 Given The calculator is turned on

 When I type in "neagtive number"
 And I press "plus"
 And I type in "neagtive number"
 And I press "equals"

 Then I see the "added number" as the result

Scenario: Addition of fractions

 Given The calculator is turned on

 When I type in "fraction number"
 And I press "plus"
 And I type in "fraction number"
 And I press "equals"

 Then I see the "added number" as the result

Scenario: Addition of +ve and -ve number

 Given The calculator is turned on

 When I type in "positive number"
 And I press "plus"
 And I type in "negative number"
 And I press "equals"

 Then I see the "added number" as the result

Scenario: Addition of decimals

Given The calculator is turned on

 When I type in "decimal number"
 And I press "plus"
 And I type in "decimal number"
 And I press "equals"

 Then I see the "added number" as the result

Scenario: Typing operator more than once

Given The calculator is turned on

 When I type in "number"
 And I press "plus"
 And I press "plus"
 And I type in "number"
 And I press "equals"

 Then I see the "added number" as the result

Scenario: Addition of more than 2 numbers

 Given The calculator is turned on

 When I type in "positive number"
 And I press "plus"
 And I type in "positive number"
 And I press "plus"
 And I type in "positive number"
 And I press "equals"

 Then I see the "added number" as the result

Scenario: Adding numbers where the result goes out of range
 Given The calculator is turned on

 When I type in "positive number"
 And I press "plus"
 And I type in "positive number"
 And I press "equals"

 Then I see the "added number" as the result
  Given The calculator is turned on

 When I type in "positive number"
 And I press "plus"
 And I type in "positive number"
 And I press "equals"

 Then I see the "added number" as the result

Scenario: 6+* is provided as input?
 Given The calculator is turned on

 When I type in "positive number"
 And I press "plus"
 And I type in "positive number"
 And I press "equals"

 Then I see the "added number" as the result

Scenario: Identify operation
 Given The calculator is turned on

 When I type in "positive number"
 And I press "plus"
 And I type in "positive number"
 And I press "equals"

 Then I see the "added number" as the result

Scenario: Converse operation
 Given The calculator is turned on

 When I type in "positive number"
 And I press "plus"
 And I type in "positive number"
 And I press "equals"

 Then I see the "added number" as the result
