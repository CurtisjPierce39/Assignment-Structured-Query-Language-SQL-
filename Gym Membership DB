CREATE DATABASE Gym_Membership_DB;
CREATE TABLE Members (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255) NOT NULL,
    age INT
);
CREATE TABLE WorkoutSessions (
    session_id INT AUTO_INCREMENT PRIMARY KEY,
    member_id INT,
    session_date DATE,
    session_time VARCHAR(50),
    activity VARCHAR(255),
    FOREIGN KEY (member_id) REFERENCES Members(id)
);
INSERT INTO Members (name, age)
VALUE('Bob Belcher', 25),
	('Linda Belcher', 27),
    ('John Doe', 32),
    ('Jane Doe', 21),
	('John Smith', '30');
    
INSERT INTO WorkoutSessions (session_date, session_time, activity, member_id)
VALUES('2021-02-15', '08:00 AM', 'Cardio', 5),
	('2022-08-14', '09:30 AM', 'Strength Training', 8),
    ('2021-09-15', '10:30 AM', 'Yoga', 6),
    ('2024-09-15', '12:00 PM', 'Swim Training', 7);

UPDATE WorkoutSessions
SET session_time = '09:30 PM'
WHERE member_id = 8;

SET SQL_SAFE_UPDATES = 0;
DELETE FROM Members
WHERE name = 'John Smith';
SET SQL_SAFE_UPDATES = 1;

SELECT * FROM Members;
SELECT * FROM WorkoutSessions;
