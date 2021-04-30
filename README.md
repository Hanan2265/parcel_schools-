# Volusia.parcel_schools 
Nearest School Name and distance 

The zipped file has two files the first one is parcel_schools.txt to download the file and create the parcel_schools table

the seconed one is scdistance (school distance) 

load parcel_schools table (download zip file in repository, extract to c:\temp\cs540) 

COPY volusia.parcel_schools from 'C:\temp\cs540\parcel_schools.txt' WITH (FORMAT 'csv', DELIMITER E'\t', NULL '', HEADER);

load scdistance (download zip file in repository, extract to c:\temp\cs540)

copy (select parid, scdistance from volusia.parcel where geom is not null ) to 'c:\temp\cs540\scdistance.txt'
with (format 'csv',DELIMITER E'\t', NULL '',HEADER); 

To konw more about Nearest School Name and to find the distance see the PDF

https://github.com/Hanan2265/parcel_schools-/blob/main/Student%20Presentation%20CS540.pdf



