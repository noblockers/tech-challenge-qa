# Time Tracker Bug Defects
__________
__________


- Special Characters can be used, included and saved as session name titles

![image](https://user-images.githubusercontent.com/60823603/122279080-918e8f00-cedf-11eb-8928-685ec9d2bc27.png)

## STEPS TO REPRODUCE:
Enter special characters in the input field > click `Start` > click `Stop` > click `Save` > Navigate to `Viewed Saved Sessions`

Actual result(s)
Special characters are saved on the time tracker 

Expected result(s)
Special characters must not be saved as part of a session name
__________
__________

- Duplicate session names can be saved and seen in the `"Viewed Saved Sessions"` section by the user 

![image](https://user-images.githubusercontent.com/60823603/122279240-bbe04c80-cedf-11eb-873e-81053de7bb5e.png)

## STEPS TO REPRODUCE:
Enter input in the input field > click `Start` > click `Stop` > click `Stop` > click `Save` > Repeat and then Navigate to `Viewed Saved Sessions` identical input

Actual result(s)
Duplicate sessions names are saved

Expected result(s)
Duplicate sessions names must not be saved as these will lead to confusion for the user and will prevet search accuracy 
__________
__________

- Buttons should not be enabled until a session name has been added to the "Form Control" input field
![image](https://user-images.githubusercontent.com/60823603/122279688-3dd07580-cee0-11eb-82a8-63edcacc9355.png)

During the User Experience, I would expect them to be enabled after the start buton has been activated and a session name entered into the input field

## STEPS TO REPRODUCE:
Enter input in the input field > click `Start` > click `Stop` > click `Stop` > click `Reset`

Actual result(s)
All three buttons are enabled during the testing flow 

Expected result(s)
Buttons must be disabled until the user has entered a session name, clicked play, and then clicked stop 
__________
__________

- No SignIn option for freelancers to access their personal accounts 

## STEPS TO REPRODUCE:
Navigate to the Time Tracker form > Inspect the Page

Actual result(s)
No signIn form for the user to sign in to in order to view their personal accounts 

Expected result(s)
There must be a signIn option for users so that they are able to view their personal accounts  
__________
__________
- Error message of "`TypeError: Cannot read property 'then' of undefined" appears on the UI after the user selects "OK"` on the localhost prompt message
![image](https://user-images.githubusercontent.com/60823603/122286919-4d53bc80-cee8-11eb-97c6-357ed4244c34.png)

Click `"OK"`

![image](https://user-images.githubusercontent.com/60823603/122287388-ce12b880-cee8-11eb-8ac4-e001b27229c0.png)

## STEPS TO REPRODUCE:
Enter input in the input field > click `Start` > click `Stop` > click `Stop` > click `Save`

Actual result(s)
Error message of "`TypeError: Cannot read property 'then' of undefined" appears on the UI after the user selects "OK"` on the localhost prompt message

Expected result(s)
After the user has clicked `Stop` > click `Stop` > click `Save`, I would expect them to be naviagted back to the Time Tracker so they can attempt another entry. 
__________
__________
- No character limit on the `"Enter Session"` `"Form Control"` input field
![image](https://user-images.githubusercontent.com/60823603/122283232-3ca14780-cee4-11eb-8b10-6e71be3e0483.png)

There is no character limit or minimum / maximum input for the `"Enter Session"` input field. 

## STEPS TO REPRODUCE:
Enter input in the input field > click `Start` > click `Stop` > click `Stop` > click `Save`

Actual result(s)
Error message of "`TypeError: Cannot read property 'then' of undefined" appears on the UI after the user selects "OK"` on the localhost prompt message

Expected result(s)
After the user has clicked `Stop` > click `Stop` > click `Save`, I would expect them to be naviagted back to the Time Tracker so they can attempt another entry. 
__________
__________

- The `Reset` button only resets the timer, not the content of the `Form Control` input field 

The `Reset` button only appears to reset the timer and doesn't clear the content in the input field.  

## STEPS TO REPRODUCE:
Enter input in the input field > click `Start` > click `Stop` > click `Stop` > click `Save` > click `Reset`

Actual result(s)
The `Reset` button only resets the timer

Expected result(s)
The `Reset` button must reset the timer and clear the content of the input field 
__________
__________ 
- Click events are not being detected in the console 

Each individual click event is not detected in the Console. 

## STEPS TO REPRODUCE:
Click `Start` > click `Stop` > click `Save` > click `Reset` > open console and inspect

Actual result(s)
No click events are detected by the console 

Expected result(s)
Click events must be detected in the console
__________
__________ 
- There is no `x` clear icon in the "Form Control" input field 

No 'x' icon is visible in the search input field 

## STEPS TO REPRODUCE:
Populate the saerch input field with text / characters 

Actual result(s)
No 'x' icon is visible in the search input field

Expected result(s)
There must be an 'x' icon is visible in the search input field

__________
__________ __________
__________ 

# New Features 
## _Updating the the time tracker tool for freelancers_
__________
__________ 
We want to allow users to edit and delete existing sessions. Regarding the editing functionality, they should be able to do the following: 

1. Change an existing session name and duration.
2. We want to allow users to search for sessions in the list. They should be able to search by name or duration.

## Acceptance Criteria

_**1. Change an existing session name and duration.**_

**Given** - The user has created a new session 

**And**  - Saved the session 

**When** - The user navigates to the `Viewed Saved Sessions` section 

**Then** - The user will have the option to Delete the session

**And** - Edit the session name

**And** - Edit the session duration


_**2. We want to allow users to search for sessions in the list. They should be able to search by name or duration.**_
 
**Given** - The user has created a new session 

**And**  - Saved the session 

**Then** - The user must have the option to Search for their saved sessions in the `Viewed Saved Sessions` section list 

**And** - Search by the session name

**And** - Search by the session duration
