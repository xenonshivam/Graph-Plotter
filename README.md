# Graph-plotter
A simple javascript graph plotter that can plot polynomial and trigonometric expressions. 
This graph plotter show a full screen graph.User can zoomin or zoomout the graph.User can easily get the value of y by counting the no of small boxes for any values of x.

"polynomial and trigonometric" file is the actual code for this graph plotter.And "polynomial" file is created initially.
Some important point about this graph plotter:
  1. Input expression must be parenthesized correctly i.e. use sin(x) instead of sin x or use 10*(x-2)^2+45*x and x is always in lower-case.Don't use whitespace in the expression. 
  2.            To use:                 use:
  
                sin x                : sin(x)
                sin x+5              : sin(x+5)
                cos x                : cos(x)
                cos x-2              : cos(x-2)
                tan x                : tan(x)
                tan x/5              : tan(x/5)
                sin^(-1) x+5         : asin(x+5)
                cos^(-1) x/5         : acos(x/5)
                tan^(-1) x/3         : atan(x/3)
                sinh x-5             : sinh(x-5)
                arsinh x*2           : arsinh(x*2)
                cosh x/5             : cosh(x/5)
                arcosh x*2           : arcosh(x*2)
                tanh x+2*x           : tanh(x+2*x)
                artanh x-19          : artanh(x-19)
                csch x*5             : csch(x*5)
                arcsch x*5           : arcsch(x*5)
                sech 2*x             : sech(2*x)
                arsech 3*(x-2)       : arsech(3*(x-2))
                coth 5*x             : coth(5*x)
                arcoth 3*x           : arcoth(3*x)
                log x (base e)       : log(x)
                log10 x+5 (base 10)  : log10(x+5)
                log1p x              : log1p(x)
                log2 x (base 2)      : log2(x)
                |x|                  : abs(x)
  3. This graph plotter does not show infinity.
  
  Process:
    Getting the infix expression, the infix expression is transformed to postfix expression. Evaluate the postfix expression for every pixel and plot the value. Each small unit=5px.In trigonometric graph x is in degree.
