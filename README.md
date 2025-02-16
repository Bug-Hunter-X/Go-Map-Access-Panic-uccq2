# Go Map Access Panic

This repository demonstrates a common error in Go: panicking when accessing a nil map.  The `bug.go` file shows the problematic code, and `bugSolution.go` provides a safe solution.

## Bug

Attempting to access a map value before checking if the map is initialized can lead to a runtime panic. This is because Go will attempt to access a `nil` pointer, which is not allowed.

## Solution

The solution is to check if the map is nil before accessing any values, or to initialize the map if it is nil.