--REMOVING MISSSING VALUES--

--FROM DAILYACTIVITY TABLE
SELECT * 
FROM dailyActivity_merged
WHERE Id IS NULL OR ActivityDate IS NULL OR TotalSteps IS NULL OR Calories IS NULL;

DELETE FROM dailyActivity_merged
WHERE Id IS NULL OR ActivityDate IS NULL OR TotalSteps IS NULL OR Calories IS NULL;

--FROM HEARTRATE TABLE
SELECT * 
FROM heartrate_seconds_merged
WHERE Id IS NULL OR Time IS NULL OR Value IS NULL;

DELETE FROM heartrate_seconds_merged
WHERE Id IS NULL OR Time IS NULL OR Value IS NULL;

--FROM CALORIES TABLE
SELECT * 
FROM hourlyCalories_merged
WHERE Id IS NULL OR ActivityHour IS NULL OR Calories IS NULL;

DELETE hourlyCalories_merged
WHERE Id IS NULL OR ActivityHour IS NULL OR Calories IS NULL;

--FROM INTENSITIES TABLE
SELECT * 
FROM hourlyIntensities_merged
WHERE Id IS NULL OR ActivityHour IS NULL OR TotalIntensity IS NULL OR AverageIntensity IS NULL;

DELETE hourlyIntensities_merged
WHERE Id IS NULL OR ActivityHour IS NULL OR TotalIntensity IS NULL OR AverageIntensity IS NULL;

--FROM STEPS TABLE
SELECT * 
FROM hourlySteps_merged
WHERE Id IS NULL OR ActivityHour IS NULL OR StepTotal IS NULL;

DELETE hourlySteps_merged
WHERE Id IS NULL OR ActivityHour IS NULL OR StepTotal IS NULL;

--FROM WEIGHT-INFO TABLE
SELECT * 
FROM weightLogInfo_merged
WHERE Id IS NULL OR ActivityHour IS NULL OR StepTotal IS NULL;

DELETE hourlySteps_merged
WHERE Id IS NULL OR ActivityHour IS NULL OR StepTotal IS NULL;


--Identifying Duplicates
SELECT Id, ActivityDate, COUNT(*)
FROM dailyActivity_merged
GROUP BY Id, ActivityDate
HAVING COUNT(*) > 1;

SELECT Id, COUNT(*)
FROM heartrate_seconds_merged
GROUP BY Id
HAVING COUNT(*) > 1;

SELECT Id, COUNT(*)
FROM hourlyCalories_merged
GROUP BY Id
HAVING COUNT(*) > 1;

SELECT Id, COUNT(*)
FROM hourlyIntensities_merged
GROUP BY Id
HAVING COUNT(*) > 1;

SELECT Id, COUNT(*)
FROM hourlySteps_merged
GROUP BY Id
HAVING COUNT(*) > 1;

SELECT Id, COUNT(*)
FROM weightLogInfo_merged
GROUP BY Id
HAVING COUNT(*) > 1;

--Removing Duplicates

DELETE FROM dailyActivity_merged
WHERE Id NOT IN (
    SELECT MIN(Id)
    FROM dailyActivity_merged
 GROUP BY Id, ActivityDate);

DELETE FROM heartrate_seconds_merged
WHERE Id NOT IN (
    SELECT MIN(Id)
    FROM heartrate_seconds_merged
 GROUP BY Id);

DELETE FROM hourlyCalories_merged
WHERE Id NOT IN (
    SELECT MIN(Id)
    FROM hourlyCalories_merged
 GROUP BY Id);

DELETE FROM hourlyIntensities_merged
WHERE Id NOT IN (
    SELECT MIN(Id)
    FROM hourlyIntensities_merged
 GROUP BY Id);

DELETE FROM hourlySteps_merged
WHERE Id NOT IN (
    SELECT MIN(Id)
    FROM hourlySteps_merged
 GROUP BY Id);

DELETE FROM weightLogInfo_merged
WHERE Id NOT IN (
    SELECT MIN(Id)
    FROM weightLogInfo_merged
 GROUP BY Id);


--Exporting the cleaned data

SELECT * FROM dailyActivity_merged;
SELECT * FROM heartrate_seconds_merged;
SELECT * FROM hourlyCalories_merged;
SELECT * FROM hourlyIntensities_merged;
SELECT * FROM hourlySteps_merged;
SELECT * FROM weightLogInfo_merged;
