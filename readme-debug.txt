
debug UnlockAccount


(dlv) bt
 0  0x0000000000ca7a0b in github.com/ethereum/go-ethereum/console.(*bridge).UnlockAccount
    at /mwp/work/study/economy/ethereum/go-ethereum-master/build/_workspace/src/github.com/ethereum/go-ethereum/console/bridge.go:134
 1  0x0000000000cafa5a in github.com/ethereum/go-ethereum/console.(*bridge).UnlockAccount-fm
    at /mwp/work/study/economy/ethereum/go-ethereum-master/build/_workspace/src/github.com/ethereum/go-ethereum/console/console.go:186
 2  0x0000000000c67b9d in github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto.(*_object).call
    at /mwp/work/study/economy/ethereum/go-ethereum-master/build/_workspace/src/github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto/type_function.go:161
 3  0x0000000000bf7eae in github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto.(*_runtime).cmpl_evaluate_nodeCallExpression
    at /mwp/work/study/economy/ethereum/go-ethereum-master/build/_workspace/src/github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto/cmpl_evaluate_expression.go:244
 4  0x0000000000bf6304 in github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto.(*_runtime).cmpl_evaluate_nodeExpression
    at /mwp/work/study/economy/ethereum/go-ethereum-master/build/_workspace/src/github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto/cmpl_evaluate_expression.go:44
 5  0x0000000000bfbd8d in github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto.(*_runtime).cmpl_evaluate_nodeStatement
    at /mwp/work/study/economy/ethereum/go-ethereum-master/build/_workspace/src/github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto/cmpl_evaluate_statement.go:62
 6  0x0000000000bfc1f5 in github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto.(*_runtime).cmpl_evaluate_nodeStatementList
    at /mwp/work/study/economy/ethereum/go-ethereum-master/build/_workspace/src/github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto/cmpl_evaluate_statement.go:121
 7  0x0000000000bf5171 in github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto.(*_runtime).cmpl_evaluate_nodeProgram
    at /mwp/work/study/economy/ethereum/go-ethereum-master/build/_workspace/src/github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto/cmpl_evaluate.go:17
 8  0x0000000000c7f894 in github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto.(*_runtime).cmpl_runOrEval.func1
    at /mwp/work/study/economy/ethereum/go-ethereum-master/build/_workspace/src/github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto/runtime.go:671
 9  0x0000000000c0614c in github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto.catchPanic
    at /mwp/work/study/economy/ethereum/go-ethereum-master/build/_workspace/src/github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto/error.go:250
10  0x0000000000c5f996 in github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto.(*_runtime).cmpl_runOrEval
    at /mwp/work/study/economy/ethereum/go-ethereum-master/build/_workspace/src/github.com/ethereum/go-ethereum/vendor/github.com/robertkrimen/otto/runtime.go:672
(dlv) 

