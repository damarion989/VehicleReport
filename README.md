# Vehicle Report Generator

A simple Java Template Method project for the Automated Report Generator assignment.

## Run

Requires a JDK (Java 17 or newer works). From the repository root:

```bash
mkdir -p out
javac -d out src/*.java
java -cp out Main
```

In IntelliJ, open the project, select a JDK, mark `src` as Sources Root if needed, and run `Main.main()`.

## Expected output

```text
Truck Report:
Fetching GPS data...
Formatting heavy cargo dimensions.
Performing standard maintenance check.
Log entry created.

Bike Report:
Fetching GPS data...
Formatting lightweight parcel dimensions.
Log entry created.
```

## How it works

`VehicleReport.generateReport()` is final and controls the order. Shared collection and logging steps live in the base class. Both subclasses implement abstract formatting. The maintenance hook defaults to false; TruckReport overrides it to return true.

## Assignment progress

Each phase was implemented, compiled, executed, and committed before moving on. Phase 1 used a temporary subclass outside the repository because VehicleReport is abstract. Journal.md contains assistant-recorded verification notes and spaces for the student's own reflections. Complete those reflections before submitting.
