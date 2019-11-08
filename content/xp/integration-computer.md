<!-- TODO: translate this -->
Dedicated Integration Computer

A single computer dedicated to sequential releases works really well when the development team is co-located. This computer acts as a physical token to control releasing. There is also an objective last word on what the current build contains. Developers have a source for final arbitration on integration problems. The computer allows developers to see who is releasing and when. When the release computer is occupied no other changes can be released, stability is ensured.
The latest combined unit test suite can be run before releasing. Because a single computer is used the test suite is always up to date. If the unit tests run at 100% the changes are committed, if they fail the changes  are  debugged  or  backed	out and debugged at the developers own workstation.
It can be very tempting to substitute automated build software for an integration computer. Sharing a vital resource helps build a sense of community. Team members can't become isolated from each other if they share. Seeing who is releasing and how often helps keep continuous integration happening often. Having one programming pair integrate at a time limits the scope of debugging if the build fails.