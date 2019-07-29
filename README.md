# SortingHat.org
Sort students into classes with this cutting edge interface. 


## Instructions

### Step 1: Upload the Students File
Click the "Choose file" button under the students tab to upload a csv containing information about students. This 
file must have the following headers (order does not matter):

* "ID" - a unique identifier for a student
* "Gender" - the student's gender. Must be one of "M" or "F" (Working on adding additional options)
* "Athlete" - indicates if the student is involved with an athletics program. Should be "Y" if the student is an athlete
* "Sport" - a list of the sports the student is involved in. The list should be space-separated and each sport should
be a single word. Ex: if a student plays basketball and baseball, this section would look like "basketball baseball". 
* "Choice 1" - the ID of the student's top class choice
* "Choice 2", "Choice 3", ..., "Choice 6" - the student's 2nd through 6th class choices. All different columns.

Additionally, the following headers are also supported:
* "Placement" - the ID of a section for which the student is to be allocated. This allows the user to make course 
allocations prior to running SortingHat.
* "Previous Instructor" - the ID of a previous instructor (used to prevent students from taking a class with a 
previous instructor of theirs).
* "Illegal Sections" - a list of sections that the student is not allowed to take. If "Previous Instructor" is specified,
this includes all the courses the instructor is teaching by default. If additional courses are specified, these are added
to the student's list of illegal course allocations. It is highly unlikely that a student will be placed in an illegal 
section.

Other headers and columns are permitted to be in the student csv file, but the program will not be able to use data 
from columns that have headers named something other than what is specified above.

