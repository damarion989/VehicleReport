# Process Journal

Implementation and verification notes below were recorded by the AI assistant. Add your own reflections before submitting; these notes do not describe your personal experience.

## Phase 1
Implemented an abstract VehicleReport with a final generateReport method, shared collection/logging, and abstract formatting.
Verification: compiled the base class and a temporary subclass outside the repository. Output was collection, temporary formatting, logging, in that order.
Reflection: In your own words, how does the base class control when subclass methods run (the Hollywood Principle)? What challenges did you encounter?

Your reflection: [Write here.]

## Phase 2
Added TruckReport and BikeReport, each overriding formatReport, plus a Main runner using VehicleReport references.
Verification: compiled all source files and ran Main. Both reports printed collection, their own formatting, then logging.
Reflection: Which class drove execution? What felt intuitive or tricky about abstract inheritance?

Your reflection: [Write here.]

## Phase 3
Added a default false maintenance hook, a shared maintenance step, and a TruckReport override returning true. The template evaluates the hook immediately after formatting.
Verification: compiled and ran Main. Truck maintenance appeared between formatting and logging. BikeReport skipped maintenance without an override.
Reflection: How does a hook with a default differ from an abstract method that subclasses must implement? How did seeing the output affect your understanding?

Your reflection: [Write here.]

## Phase 4
Final verification: compiled all four source files and ran Main again. Inspected the output: truck collection -> heavy cargo formatting -> maintenance -> logging; bike collection -> parcel formatting -> logging. No errors occurred in the final compilation or run.
AI review: the assistant checked that generateReport is final, formatting is abstract, the hook defaults to false, and only TruckReport opts in. The beginner implementation matches the required pattern. Collection and logging intentionally remain dummy console messages, as allowed by the assignment.
Reflection: What issues or misunderstandings did YOU find when running it? What did you learn from the AI feedback above?

Your reflection: [Write here.]
