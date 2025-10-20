# PrinterDemo
A sample .NET application demonstrating the producer-consumer pattern, using a print spooler as an example.

For a single app (producer) going to a single print spooler (consumer), a basic FIFO queue would be sufficient. However, in a more complex scenario with multiple applications sending print jobs to multiple print spoolers ("fan-out"), via various intensive transformation functions, a more sophisticated approach is needed.

This demo illustrates how to implement such a system using [.NET's Dataflow (TPL) library](https://learn.microsoft.com/en-us/dotnet/standard/parallel-programming/dataflow-task-parallel-library).