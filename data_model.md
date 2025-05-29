
# Data Model - Wealthy Singles Matchmaking Platform

## User Entity
- UserID (string, PK)
- Age (integer)
- Gender (string)
- Ethnicity (string)
- IncomeLevel (float)
- NetWorth (float)
- RelationshipIntent (string)
- InterracialPreference (boolean)
- BackgroundCheckStatus (string)
- InterestsHobbies (list of strings)

## Event Entity
- EventID (string, PK)
- EventType (string)
- EventDate (date)
- Attendees (list of UserIDs)

## Match Entity
- MatchID (string, PK)
- User1ID (string, FK)
- User2ID (string, FK)
- MatchDate (date)
- MatchOutcome (string: Matched, Dated, Engaged, Married)
