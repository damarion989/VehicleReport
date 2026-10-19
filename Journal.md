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
