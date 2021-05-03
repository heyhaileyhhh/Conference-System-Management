LOGIN SYSTEM INSTRUCTIONS:
Note: if a new user is using the program, he or she needs to first sign-up. The user can choose whether to sign up as an
Attendee or an Organizer, then type in their username and password accordingly. The username is case-insensitive.
If the account is successfully created, then the user needs to log-in using the newly-created account.

The LoginSystem also deals with the second option shown on the main menu: 2.  View account settings/Create account if
you are an organizer.
As user chooses this option, the LoginSystem will call the corresponding run() method that display menu options specific
 to the type of the user.
If the user is an Attendee or a Speaker, he or she would be able to see 3 options:
1. Change password: this allows the user to change password if they wish. It asks the user to enter the old password
to verify their identity and then asks them to enter the new password.
2. Log out: this allows the user to log out of the program. Once they are logged out, the program will display
the initial menu:
	1. Sign up
	2. Log in
	3. Quit
   to allow another user to use the program.
3. Return to the main menu: this allows the user to return to the main menu and choose what they want to do.

If the user is an Organizer, he or she can choose from the same options as above, with an additional option of
creating an account for a Speaker. The menu options are listed as below:
1. Create account for the speaker
2. Change password
3. Log out
4. Return to the main menu

Mandatory Extension-specific Instructions:
1. VIP user:
- I think we overthought about this, but we allow the user to be upgraded to a VIP user if he/she has attended at least
5 events, instead of just allowing a new user to sign up as a VIPUser.
- The organizer is allowed to create a vip user account, which is an "upgraded" attendee account.
- so it would be easy to test the functionality to let the organizer create a vip account then log in using this account.

Organizer creates all types of account in the system:
- after logging in, click 2: "View options for account settings/user-specific tasks.". Then the first option should
allow you to create different user account.


Optional Extension-specific Instructions:
1. User Request:
   Description: Allow the system to support additional user requests (e.g. dietary restrictions,
   accessibility requirements) where organizers can tag a request as "pending" or "addressed".
   All organizers see the same list of requests, so if one tags a request as addressed, all other organizers can log in
   and see that.
- you need to log in as an Attendee. After logging in, go to option 2: "View options for account settings/user-specific
tasks." Then there is an option for you to send requests.
- organizers can log in and click the same menu option(option 2). Then you should see options of "see the list of
addressed requests" and "see the list of pending requests". After clicking
one of these two options, follow-up instructions will pop up to ask whether you want to address or pend the request.
- if the organizer wants to address the request, you can enter the identifier for the request. Same process applied
to re-pending an addressed request.
- All addressed and pending requests are immediately added to the addressed/pending-requests lists after the operations
mentioned above, and could be viewed by Organizers.

-------------------------------------------------------------------------------------------------
EVENT MANAGEMENT PAGE INSTRUCTIONS:
There are 3 different menu screens of event management page for each type of user. Listed are all the different
possible menu options.

-Viewing the list of all events, available events for yourself, and events you are signed up for
To view any of these lists, simply input the valid number menu option.


-Signing up and cancelling your spot from an event(Attendee and Organizer only)
Enter the sign up or cancel spot number option. To sign up for an event or cancel
your spot from an event, you must enter the unique identifier of the event you wish to sign up
for or remove yourself from. You will not be signed up for that event if you are already in it,
the event is full, if you entered an identifier that is not associated with an event, or if you are
attempting to sign up for a VIP event as a non VIP-user. Please note speakers cannot sign up for an
event and must create an attendee account to do so. Press the enter key to return to the Event Management
Menu if you decide not to sign up/cancel your spot.


-Adding a room into the system(Organizer only)
Enter the add room number option. To add a room into the system, you must enter an integer number that is 3 digits long.
The room will not be added if it already exists in the system, or if your input is not an integer 3 digits long.
Press the enter key to return to the Event Management Menu if you decide not to add a room.

-Adding resources to a room(Organizer only)
Enter the add resource to the room menu number option. Input the room you would like to add resources to.
Then simply follow the prompts to add certain resources to the room. You will not be able to add resources
to a room that does not exist.

-Finding a room with certain resources(Organizer only)
Enter the find a room with resources menu number option. Simply follow the prompts to decide what room
with what resources you wish to find. If such room does not exist, no rooms will be listed for you.

-Scheduling a new event(Organizer only)
Enter the schedule an event number option and follow the prompts the system asks. There are several restrictions of
scheduling a new event.
	- Identifier: Your input must be exactly 4 characters long
	- Event Name: Your input may be any value
	- VIP Status: Your input should be 'yes' or 'no'
	- Max Capacity: Your input should be an integer greater than 0
	- Room: The room you enter must already exist inside the system. If not, you will be prompted again for a
	        room. Press enter to return to the Event Menu if you forgot to add a room into the system.
	- Speaker username: Input a speaker user name and press Enter. You may add as many speakers as you like.
	                    Once you are finished adding speakers, enter 'none.' You may also have no speaker
	                    events, in which case enter 'none' upon the first prompt. Note if any one of the
	                    speakers are double booked, the event will fail to be created.
	- Duration: Your input will be how long the event lasts in minutes
	- Date: Your date must follow the format MM/DD/YYYY where the month, day, and year are valid
	- Time: Your time must follow the 24 hour clock and follow the format HH:MM. You must input exactly 2 digits for
	        the hour and 2 digits for the minute

Failure to meet any of these restrictions will result in the event not being created. In addition, if you attempt to
schedule the new event in a room where another event is already taking place, the new event will not be created.

-Cancel an event(Organizer only)
Input the Event menu option to cancel an event and enter the event identifier you would like to cancel.
It will not be cancelled if the event identifier does not exist. Note all organizers have the power to
cancel any event.

-Change the maximum capacity of an event(Organizer only)
Input the Event menu option to change the maximum capacity of an event. Enter the event identifier number
and input an integer you would like to change the maximum capacity to. Please note you cannot lower the
maximum capacity of an event to prevent the maximum capacity from being less than number of signed up
attendees.

-Print the schedule of events
Input the Event menu number option to print a schedule of all events. An html file called schedule.html
will be created in the phase2 folder. Right click the file and click open in browser. A neatly generated
schedule of all the events with their information will be outputted in a table.

-Viewing list of events you are speaking at(Speaker only)
Simply input the number menu option to view the list of events you are speaking at.


Returning to the Main Menu
-To return to the main menu, simply input the number option to return.

-------------------------------------------------------------------------------------------------
MESSAGING SYSTEM INSTRUCTIONS:
All users registered in the conference can use the messaging system to message other users. The messaging system is
represented as a Message Management Page with different menu options for different types of users
(i.e. Attendees/Organizers/Speakers).

All Attendees/Organizers/Speakers can:
- View their conversations
    A list of the user's conversations with other users is listed under ***My conversations***. Each conversation is
    represented as "- username (Unread/Read)". If there is nothing under ***My conversations***,
    the user currently doesn't have any conversations with other users. From here, the user can:
        1. View their conversation with another user.
        2. Mark a conversation as Unread.
        3. Mark a conversation as Read.
        4. Delete your conversation with another user.
        5. Archive a conversation.
        6. Undo conversation archive.
        7. View your archived conversations.
        8. Return to previous page.

    - For options 1-6: Select the corresponding menu option, then simply input the other user's username.
    - For option 7: A list of the user's archived conversations is presented under ***My conversations***. The user can
                    input the other user's username to view the archived conversation.

- Send a message to another user
    To send a message to another user, simply input the other user's username.

- View my favorite contacts
    Select the menu option to view the user's favorite contacts.

- Add a user to my favorite contacts
    Simply enter the other user's username to add to the favorite contacts list.

- Return to Main Menu
    Input the menu option to return to the main menu.


On top of the above options,
1) an Organizer can:
- Send a message to all Attendees attending an event.
    Enter the event identifier to send a message to all the attendees signed up for that event.

- Send a message to all Attendees registered for the conference.
    Simply input the message and it will be automatically sent to all Attendees registered in the conference.

- Send a message to all Speakers registered for the conference.
    Simply input the message and it will be automatically sent to all Speakers registered in the conference.

- Send a message to all Attendees AND Speakers registered for the conference.
    Simply input the message and it will be automatically sent to all Attendees and Speakers registered in the
    conference.

2) a Speaker can:
- Send a message to all Attendees attending the Speaker's event.
    Enter the event identifier to send a message to all the attendees signed up for the Speaker's event.


Optional Extensions:
- Mark a conversation as Read/Unread
    A conversation is automatically marked as Read/Unread, for example,
    1) when user1 send a message to user2, the conversation is automatically marked as Unread for user2;
    2) when user2 views the conversation with user1, the status of the conversation is automatically changed to Read.

    The users can also manually mark a conversation as Read/Unread. Please see the instructions above for more
    information.
- Delete a conversation
    The user can delete their conversation with another user using the menu option described above.
    The conversation with another user will disappear from the user's conversation list once it is deleted.
- Archive a conversation/Undo archive
    The user can choose to archive a conversation using the menu option described above. The archived conversation
    with be added to the user's archived conversation list. On the other hand, the user can undo the archive by
    selecting the corresponding menu option described above. The conversation will disappear from the user's archived
    conversation list once the archive is undone.