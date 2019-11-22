# RSVP [Répondez S’il Vous Plaît - (R)afael (S)ubía (V)aldez (P)resets] 
State Saving System for Pure Data

RSVP is a state saving system for Pure Data (http://puredata.info/). It was created to offer Pure Data users a way to record presets for the GUI objects inside patches.

RSVP stands for two things Répondez S’il Vous Plaît and my initials Rafael Subía Valdez Presets. The goal of an RSVP invitation, is to confirm assistance to an event, effectively reserving a place to that event. This translated to the preset system is a space and time "reserved" for a certain value.

This version of RSVP is completely developed with Pure Data vanilla 0.50 which makes the system more robust by dropping all third party dependencies. Like previous versions of RSVP, the library is a collection of abstractions that wrap around Pure Data's own GUI. The [msc_pre] object can be used to store states from none vanilla objects. 

The system is designed to use the abstractions as templates to modify and create personalized GUIs. More explanation and tutorials to come.

## HISTORY
### Version 1
RSVP was developed in 2016 when working on my PhD at The University of Edinburgh. Initially it was designed to simplify state saving in Pure Data as an alternative to more extensive State Saving methods like "Kollabs". The first version of RSVP made use of planty of externals and libraries from the Pure Data community. This made RSVP easier to use, but increased its dependence of external code. The saving and recalling mechanism was complex and made use of the [coll] object avialable in the "Cyclone" library. Its development started with Pure Data 0.46 which did not include the now used text object. This version of RSVP was presented in the LAC2018 - Berlin.

### Version 2
Version 2 of RSVP was never made public and wrapped the [param] object from the "tof" library. This simplified the system but used a library which had not been updated nor had any further support or development. This version showed a new way of working with presets as it recorded a file for each preset, unlike Version 1 which recorded all presets in a large text file. It works extremly well and my PhD project made use of this version extensively, however concerns of using a library that was not getting updated were still there and I decided to continue developing an idea to create an RSVP version completely compatible with Pure Data vanilla. Fortunately, PD 47 incorporated the [text] object and offered a solution. 

### Version 3
With the incorporation of the [text] object in Pure Data vanilla and understanding how the [param] object divided each preset into its own text file, I decided to adapt version 1 wrapping solutions to record states into text files useing the [text] object. As a result, RSVP version 3 is now working and completely vanilla friendly. 


![](rsvp1.gif)

# IMPORTANT 
## (RSVP breaks backwards compatability)
Because RSVP is designed as a local library, it is better to leave projects done with previous versions with their own local version. 


