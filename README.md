[![Build Status](https://travis-ci.org/christos312/moodle-local_get_user_cohorts.svg?branch=master)](https://travis-ci.org/christos312/moodle-local_get_user_cohorts)
# Get User cohorts

## Description
This plugin can be used to retrieve the cohorts of a given user in Moodle by providing the USER ID

## How it works
1. Install plugin in Moodle
2. Enable WebServices
3. Assign the function to the web service user
4. Send a request to the server
> http://[moodleurl]/webservice/rest/server.php?wstoken=[YOURTOKEN]&wsfunction=local_wsgetusercohorts&userid=18&moodlewsrestformat=json

### Parameters
```php
int  Default to "null" //The ID of the user"
```
### Returns
```php
object {
    cohorts list of (
        object {
            cohortid int   //Cohort ID
            idnumber string   //Cohort id number
            name string   //Cohort name
        }
    )
}
```
### Change log


#### [1.0] (2017-07-26)
Fixed PHP LINT errors

#### [1.1] (2017-09-19)
**Closed issues:**
-  [\#1](https://github.com/christos312/moodle-local_get_user_cohorts/issues/1)
-  [\#2](https://github.com/christos312/moodle-local_get_user_cohorts/issues/2)
-  [\#3](https://github.com/christos312/moodle-local_get_user_cohorts/issues/3)
