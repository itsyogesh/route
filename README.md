route
=====
Route keeps all your events in place.

Database Schema (Rough Sketch)

Database for Event 

all_members_count     The number of invitees to the event
unsigned int32	

attending_count	      The number of invitees who have accepted the event invite
unsigned int32 	

can_invite_friends	  Whether the viewer can invite friends to the event
bool	

creator *	            Creator of the event
id	

declined_count	      The number of invitees who have declined the invite
unsigned int32	

description	          Description of the event
string	

eid *	                Event id
id	

end_time	           End time of the event UNIX timestamp
string	

event_header_pic	    Cover photo for the event
string	

host	               Host id of the event
string	

Location	           Lcation of the event
dict/hash table	

name 	               Name of the event
string	

privacy	             privacy of the event
string	

start_time	          Start time of the event UNIX timestamp
string	

unsure_count	      The number of invitees who have responded in maybe
unsigned int32	

Checkin Database

author_uid        The id of the user who has made the checkin
id	

checkin_id	       The id of checkin
id	

coords	           The latitude and longitude of the location
struct	

message	           The message the author posted with the checkin
string	

place_id	         The id of the place representing the location
id	

tagged_uids	       The ids of users tagged in with that checkin
struct	

photos_list	       list of photos tagged in with that checkin
struct	           if not present, add the photo of the location

target_event_id	    The id of the event the user checked into
id	

target_type	        Type of checkin location or event
string	

timestamp	         A UNIX timestamp for the checkin
string	

User Database
Well I need to think about this.
General data like the facebook ones can be accquired from facebook only.
