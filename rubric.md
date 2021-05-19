# CS50 Final Project rubric

This is an *initial rubric* and we reserve the right to update it based on things that come up after posting the rubric.
This page provides detail on the published grade breakdown.

## Design spec (15%)

### Teams of 3 students:

We grade this section out of 36 points.

#### Presentation (12 points)

"In 10 minutes you must present an *overview* of your design decisions and how your group will divide the work; the design document provides more detail. Be prepared to answer questions and receive feedback."

* (4) Good overview of the design.
* (4) Decomposition and data structures.
* (4) Plan for division of the work.

#### Document (24 points)

"Your design document (written in Markdown) shall describe the major design decisions, plan for testing, and the roles of each member of your group."

**Server (24):**

* (4) User interface
* (4) Inputs and outputs
* (4) Functional decomposition into functions/modules
* (4) Major data structures
* (4) High-level pseudo code (plain English-like language) for logic/algorithmic flow
* (4) Testing plan, including unit tests, integration tests, system tests

### Teams of 4 students:

We grade this section out of 50 points.

#### Presentation (12 points)

"In 10 minutes you must present an *overview* of your design decisions and how your group will divide the work; the design document provides more detail. Be prepared to answer questions and receive feedback."

* (4) Good overview of the design.
* (4) Decomposition and data structures.
* (4) Plan for division of the work.

#### Document (38 points)

"Your design document (written in Markdown) shall describe the major design decisions, plan for testing, and the roles of each member of your group."

**Client (14):**

* (2) User interface
* (2) Inputs and outputs
* (4) Functional decomposition into functions/modules
* (2) Major data structures
* (2) High-level pseudo code (plain English-like language) for logic/algorithmic flow
* (2) Testing plan, including unit tests, integration tests, system tests

**Server (24):**

* (4) User interface
* (4) Inputs and outputs
* (4) Functional decomposition into functions/modules
* (4) Major data structures
* (4) High-level pseudo code (plain English-like language) for logic/algorithmic flow
* (4) Testing plan, including unit tests, integration tests, system tests

## Implementation spec (15%)

We asked for "a summary of your approach to implementing the server (and client, for teams of 4) and any modules, providing the prototype and brief description of each function, and specifics of the data structure(s) you plan to use."
The "implementation spec should describe all of your implementation's units (other than those we provide), provide pseudo code for each unit's functions (including prototypes and their parameters), and describe every major data structure," and 

We're looking for a clear, modular structure with well-chosen data structures, function names, and function interfaces.

We grade this section out of 30 points.

**Teams of 3 students:**

  * (6) module structure, cohesion, coupling
  * (8) function prototypes (server)
  * (8) function descriptions & pseudocode(server)
  * (8) data structures (server)

**Teams of 4 students:**

  * (6) module structure, cohesion, coupling
  * (5) function prototypes (server)
  * (5) function descriptions & pseudocode (server)
  * (5) data structures (server)
  * (3) function prototypes & pseudocode (client)
  * (3) function descriptions (client)
  * (3) data structures (client)


## Code style and quality (15%)

See *[CS50 coding standards](https://www.cs.dartmouth.edu/~cs50/Labs/CodingStyle.html)*.

* code should be well-organized with sensible filenames and subdirectories
* brief `README.md` in each directory
* clear Makefile for clean and build
* clear and consistent style
* clear code design, functional decomposition, naming
* clear code logic and flow
* at most one global variable in each program
* good choice of, and use of, data structures
* good modularity (strong cohesion, loose coupling)
* good in-code documentation (comments)
* code is consistent with documentation (IMPLEMENTATION.md)
* defensive programming (error checking, malloc, etc.)
* no compiler warnings
* no memory leaks/errors caused by student code
* no output to stdout other than what is required to play the game
* handles errors gracefully

## Final presentation (15%)

We grade this section out of 15 points.

* (2) organized and efficient
* (2) all members have meaningful speaking role
* (2) identify known limitations of implementation
* (1) show a new, nontrivial map
* (8) game runs smoothly, demonstrating that the core requirements work:
	* spectator mode
	* multiple players
	* visibility - "known" and "sees"
	* gold collection
	* game over

## Scrum and Git practices (10%)

Your repo *must* have a git branch `submit-final`.
We will grade the contents of that branch as it appears on GitHub at the moment of the deadline; if you want us to grade a later commit, despite the lateness penalty, let us know.

We grade this section out of 20 points.

  * (4) GitHub wiki shows good use of Sprint retrospectives
  * (4) GitHub Project Board shows good use of Scrum planning
  * (4) git commit history - logical groupings of changes in each commit, and meaningful commit messages.
  * (4) git commit history - good use of branches and [git-flow](https://www.cs.dartmouth.edu/~cs50/Lectures/units/git-flow.html).
  * (4) no executable files, object files, core dump files, editor backup files, or extraneous files existing in any directory.

## Functionally correct and complete (30%)

(details tba)   

## Lateness (-10%)

If the `submit-final` branch appears late, we take
**10 points per hour**, prorated by the minute, *off the top.*
This means that you lose (10/60 x minutesPastDeadline) points off your total project grade.
