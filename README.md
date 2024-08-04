-- Database Design as Below:

Tables:
table 1 - Users

1  user_id (Primary Key)
2  email (Unique)
3  name

table 2 - Rooms

1 room_id (Primary Key)
2 room_name (Unique)

table 3 - Meetings

meeting_id (Primary Key)
day
start_time
end_time
room_id (Foreign Key)
creator_id (Foreign Key referencing Users)

table 4 - MeetingParticipants

meeting_id (Foreign Key)
user_id (Foreign Key)
Composite Primary Key: (meeting_id, user_id)
