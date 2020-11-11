# F#  Hello World tutorial

### Create F# project from the command line with:
```cmd
dotnet new console -lang F# -o myFSharpApp
```

Move to your new app
```cmd
cd myFSharpApp
```

The main file in the myFSharpApp folder is Program.fs. By default, it already contains the necessary code to write "Hello World from F#!" to the Console.

```fsharp
open System

[<EntryPoint>]
let main argv =
    printfn "Hello World from F#!"
    0 // return an integer exit code
```

Define a new function to print a name.

```fsharp
let printGreeting name =
    printfn "Hello %s from F#!" name
```

Call the function

```fsharp
printGreeting "Ana"
```

the entire piece of code will look like the following:

```fsharp
open System

let printGreeting name =
    printfn "Hello %s from F#!" name

[<EntryPoint>]
let main argv =
    printGreeting "Ana"
    0 // return an integer exit code
```