## WEEK 7 ASSIGNMENT

Using the two-step commit process presented in the beginning of this chapter, describe how to avoid assigning one seat to two people, as in the airline example.  That is, list precisely which steps the database manager should follow in assigning passengers to seats.  Provide at least one other example of a real-world scenario in which you would want to follow the two-step commit process and why you'd want to do so (you can pick an example from school, business, etc.)
    - First you have to use the intent phase which begins with the check of a "commit-flag" if there is no set "commit-flag" then the database system proceeds to check for the corresponding values or in this case seats on the plane. This is would be done by assigning temporary values to all data sets, so in this example it would be the seat number/id and the passenger name/id.
    - Next these temporary values are set as a "commit-flag" and are no longer marked as temporary values. Then the "commit-flag" is unset in order to update the database. 
    - Any other database that has multiple incoming data streams would use this system in order to avoid incorrect data assigning. So any online ticketing system would do this, really any system that will have multiple tickets at the same time that could want to change the exact same data should have this. 

Can a database contain two identical records without a negative effect on the integrity of the database?  Why or why not? Provide examples to support your response
    - Yes a database can contain identical records but it is entirely dependant on the database on whether or not this would have a negative effect. For most databases this would have a greatly negative effect and is not recommended to be allowed by the constraints of the system. The only way in which it would be okay to have duplicate records is if there is a link between them that updates them to match so that data is not out of sync but then what is the purpose of the duplicate? So its better to not allow it and just create a second that demands different information. 

Disclosure of the sum of all financial aid for students in Smith dorm is not sensitive because no individual student is associated with an amount.  Similarly, a list of names of students receiving financial aid is not sensitive because no amounts are specified.
  
However, the combination of these two lists reveals the amount for an individual student if only one student in Smith dorm receives aid.  What computation would a database management system have to perform to determine that the list of names might reveal sensitive data? What records would the database management system have to maintain on what different users know in order to determine that the list of names might reveal sensitive data?
    - The database system could use the rule of "n items over k percent" which allows data to be withheld if certain items represent more then is allowed of the results reported. Access to information can overall be tracked and controlled to all the users that access the database. This would enable limitations on data that could be pulled/complied from the system. So as shown in the example list A is not sensitive and list B is not sensitive, but having A + B = C which is sensitive data. This could be over the allowed percentaged of data and be restricted. 
    - Also simple user access permissions could be put in place so that only certain higher level users have access to both lists or sections of the database. This would be the easier method. Also encryption over some of the values so that the only high level database managers have access to the real data could come in handy as well. 

Is the response "sensitive value: response suppressed"  itself a disclosure?  Why or why not?  What other ways could you suppress responses that reveal sensitive information without informing the user that the response to their query is sensitive?
    - Simple response suppression controls and values in the database could achieve this. Also user permissions to execute could also achieve this where if a user doesn't have the permission the quire is refused without executing and no message or result is shown. 