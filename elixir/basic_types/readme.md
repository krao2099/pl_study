# Primatives

Elixir basic types: integers, floats, booleans, atoms, and strings

1          # integer
0x1F       # integer
1.0        # float (support scientific notation, 64 bits)
true       # boolean
:atom      # atom / symbol
"elixir"   # string
[1, 2, 3]  # list
{1, 2, 3}  # tuple

nil        # null val (Consider falsly)


# Arithetic

operators: +,-,*,/

/ always returns a float. div() will return an int (rounds down)

functions: div,rem, round, trunc (cut off bits)

type checks: is_integer, is_float, is_number (either or types), is_boolean, is_atom, is_binary

Boolean arithetic: or, and, not (cannot be overloaded)(Short-circuit)

Logical operators: ||, &&, and ! (can be overload)
example: 1 || true -> 1

# Function signatures
Functions in Elixir are identified by both their name and their arity. Uses the notion {func_name}/{arity}

Access man pages with h {namespace}.{funcation signature}

All functions in the Kernel module are automatically imported into our namespace.

# Atom
An atom is a constant whose value is its own name. Some other languages call these symbols. example ':apple'
Used for status. Boolean are consider atoms

# String

delimated by "". UTF-8.
<> concatenation operator
String interpolation ex: ```"hello #{string}!```. Interpolated var must be string convertable

Print with IO.puts/1

Represented as byte sequences so is_binary return true
Length with String.length/1
Uppercase with String.upcase/1

# Structural comparison
==,!=,<=,>=,<,>, and strict === !==
