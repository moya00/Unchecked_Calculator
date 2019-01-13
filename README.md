# Unchecked_Calculator
vb.net version of unchecked keyword in c#

## Design
In vb.net, there is no equivalent keyword like 'unchecked' in c#. <br>
This class overrides OverflowException and implemented in vb.net.

## How to use
```vb.net
Imports UncheckedCalculator

Module TestModule

    Sub Main()

        Dim newUncheckedPlus As Integer = Unchecked.Plus(2147483647, 1)
        Dim newUncheckedMinus As Integer = Unchecked.Minus(0, 1)
        Dim newUncheckedMultiply As Integer = Unchecked.Multiply(2147483647, 2)

        Console.WriteLine("2147483647 + 1 = {0}", newUncheckedPlus)
        Console.WriteLine("0 - 1 = {0}", newUncheckedMinus)
        Console.WriteLine("2147483647 * 2 = {0}", newUncheckedMultiply)

    End Sub

End Module
```
Before using it, you should add the project or compiled binaries from the reference.
