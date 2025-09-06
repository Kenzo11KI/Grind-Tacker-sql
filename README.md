# Grind-Tacker-sql
A personal grind tracker database project built in PostgreSQL. Tracks hours spent on gym, study, family, faith, and relationships
 DROP TABLE IF EXISTS grind_tracker;

CREATE TABLE grind_tracker (
id SERIAL PRIMARY KEY,
date DATE NOT NULL,
category TEXT NOT NULL,
hours INT,
notes TEXT,
quality TEXT
);
INSERT INTO grind_tracker (date,category,hours,notes ,quality)
VALUES
('2025-07-01','gym',1,'focus on chest,shoulders and arms','average'),
('2025-07-02','study' ,8,'sql gringind','good'),
('2025-07-03','family',6,'spend time with my son','better'),
('2025-07-04','faith',1,'quality time with GOD','great'),
('2025-07-05','relationship',4,'spend time with my girlfriend','good');
