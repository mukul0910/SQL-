Query the list of CITY names from STATION that do not start with vowels and do not end with vowels. Your result cannot contain duplicates.
Input Format
The STATION table is described as follows:
where LAT_N is the northern latitude and LONG_W is the western longitude.

solution:
SELECT DISTINCT CITY FROM STATION WHERE SUBSTRING(CITY,1,1)NOT IN ('A','E','I','O','U') AND  SUBSTRING(CITY,-1,1) NOT IN ('A','E','I','O','U');
