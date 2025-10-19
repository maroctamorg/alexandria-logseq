- The principle deals with a key issue in a system: how do we decompose or partition the system into separate units, that can be developed and changed independently of each other. What are the criteria that we use to decide what each unit is responsible for in fulfilling the system’s mission?
  
  The principle states the following:
- A program is divided into [[modules]] that hide from other modules an aspect of implementation that is *likely to change*.
- A module exposes a* stable abstract interface* that does not reveal details about its implementation.