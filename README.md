# RSVP [Répondez S’il Vous Plaît - (R)afael (S)ubía (V)aldez (P)resets] 
State Saving System for Pure Data

RSVP is a state saving system for Pure Data (http://puredata.info/). It was created to offer Pure Data users a way to record presets for the GUI objects inside patches.

RSVP stands for two things Répondez S’il Vous Plaît and my initials Rafael Subía Valdez Presets. The concept of RSVP in an invitation is to confirm assistance to an event, so this translated to the preset system is that that space and time is reserved for a certain value, it is "reserved".

This version of RSVP is completely developed with Pure Data vanilla 0.50 which makes the system more robust by dropping all third party dependencies. Like previous versions of RSVP, the library is a collection of abstractions that wrap around Pure Data's own GUI. The [msc_pre] object can be used to store states from none vanilla objects. 

The system is designed to use the wrappers as templates to modify and create personalized GUIs. More explanation and tutorials to come.

![](rsvp1.gif)

# IMPORTANT 
## (RSVP breaks backwards compatability)
Because RSVP is designed as a local library, it is better to leave projects done with previous versions with their own local version. 


