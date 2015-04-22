#Operator Precedence

## "||" has a greater precedence than "or"

$val = false || true; // $val : true [ $val = (false || true)]

$val = false or true; // $val : false [ ($val = false ) || true]



##"&&" has a greater precedence than "and"

$val = true && false; // $val: false [ $val = (true && false) ]

$val = true and false; // $val : true [ ($val = true ) and false ]

#Evaluations
Evaluation of logical expressions is stopped as soon as the result is known.

$foo = null;
if (is_object($var) && $var->getId()) # $var->getId() is never called
