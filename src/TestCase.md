## Test Case: Admin Authentication

| Step | Description                                                | Expected Result                                                    | Status |
|------|------------------------------------------------------------|--------------------------------------------------------------------|--------|
| 1    | Go to the application login page.                          | The application login page opens.                                  | N/A    |
| 2    | Locate the admin login form                                | The login form is located successfully.                            | N/A    |
| 3    | Verify that the admin can input data into the form fields. | The admin can input data to complete the form.                     | N/A    |   
| 3    | Enter valid admin credentials                              | The fields are completed successfully.                             | N/A    |
| 4    | Locate the login button                                    | The login button is successfully located.                          | N/A    |
| 5    | Click on the login button.                                 | The admin is successfully redirected to the page intended for him. | N/A    |

## Test Case: Admin Profile Administration

| Preconditions                     | Step   | Description                                           | Expected Result                                                                    | Status |
|-----------------------------------|--------|-------------------------------------------------------|------------------------------------------------------------------------------------|--------|
| Admin is logged in to the system. | 1      | Access the admin profile section.                     | The admin profile section opens.                                                   | N/A    |
|                                   | 2      | Verify if only admin functionalities appear.          | Only the basic functionalities accessible to admin appear.                         | N/A    |
|                                   | 3      | Verify if the profile update functionality exists.    | The profile update functionality is present.                                       | N/A    |
|                                   | 4      | Update the admin's profile information.               | The admin's profile information (e.g., name, email, etc.) is updated successfully. | N/A    |
|                                   | 5      | Save the changes.                                     | The changes are saved successfully.                                                | N/A    |


## Test Case: Deauthentication Admin

| Preconditions                           | Step | Description                                          | Expected Result                                            | Status |
|-----------------------------------------|------|------------------------------------------------------|------------------------------------------------------------|--------|
| Admin is logged in to the system.       | 1    | Locate the admin logout button.                      | The admin logout button is successfully located.           | N/A    |
|                                         | 2    | Click on the admin logout button.                    | The logout button is clickable.                            | N/A    |
|                                         | 3    | Verify if the admin is logged out.                   | The admin is successfully logged out.                      | N/A    |
|                                         | 4    | Verify if the admin is redirected to the login page. | The admin is redirected to the login page successfully.    | N/A    |


## Test Case: Authentication with Invalid Data

| Preconditions                                                                                   | Step | Description                                                                          | Expected Result                                                                                                                                   | Status |
|-------------------------------------------------------------------------------------------------|------|--------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|--------|
| The application login page is available and the form is functional.                             | 1    | Access the application login page.                                                   | The login page is accessed successfully.                                                                                                          | N/A    |
|                                                                                                 | 2    | Leave the username field empty and enter a correct password. Click the login button. | An error message is generated: "The username field is required!"                                                                                  | N/A    |
|                                                                                                 | 3    | Enter a valid username and leave the password field empty. Click the login button.   | An error message is generated: "The password field is required!"                                                                                  | N/A    |
|                                                                                                 | 4    | Enter an invalid username and a correct password. Click the login button.            | An error message is generated: "The username must contain only letters, for example!"                                                             | N/A    |
|                                                                                                 | 5    | Enter an existing username and an incorrect password. Click the login button.        | An error message is generated: "Password must contain at least 8 characters, at least one letter, one digit, one special character, for example." | N/A    |


## Test Case: Create New Theme

| Preconditions                      | Step | Description                                                              | Expected Result                                                               | Status |
|------------------------------------|------|--------------------------------------------------------------------------|-------------------------------------------------------------------------------|--------|
| User is logged into the system.    | 1    | Click on the three dots in the upper right corner.                       | The options menu opens.                                                       | N/A    |
|                                    | 2    | Verify that the option to create a new topic exists.                     | The option to create a new topic is present.                                  | N/A    |
|                                    | 3    | Click on 'CREATE TOPIC'.                                                 | The page for creating topics opens.                                           | N/A    |
|                                    | 4    | Verify that the fields can be filled out.                                | The fields are editable.                                                      | N/A    |
|                                    | 5    | Enter a unique name for the topic, a description, and add a photo/video. | The information is successfully entered.                                      | N/A    |
|                                    | 6    | Click on the 'SAVE' button.                                              | A confirmation message appears: "New topic saved successfully."               | N/A    |
|                                    | 7    | Verify that the created topic is saved.                                  | The topic is successfully saved and accessible in the user's account.         | N/A    |
|                                    | 8    | Click on the 'POST' button.                                              | A confirmation message appears: "New topic created successfully."             | N/A    |
|                                    | 9    | Verify that the new topic appears in the list of topics.                 | The new topic is visible in the list of topics and accessible to other users. | N/A    |


## Test Case: Validation of the newly created theme

| Preconditions                                                                       | Step | Description                                                                         | Expected Result                                                                                        | Status |
|-------------------------------------------------------------------------------------|------|-------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|--------|
| User is logged into the system and the form for creating a new topic is functional. | 1    | Leave the fields blank and click the button 'POST'.                                 | An error message is generated: "All fields must be completed!"                                         | N/A    |
|                                                                                     | 2    | Create a topic with an existing name. Click the button 'POST'.                      | An error message is generated: "The topic name already exists. Try another name!"                      | N/A    |
|                                                                                     | 3    | Create a topic without a name. Click the button 'POST'.                             | An error message is generated: "The topic name is required. Try again!"                                | N/A    |
|                                                                                     | 4    | Create a topic with special characters. Click the button 'POST'.                    | An error message is generated: "The topic name must not contain special characters. Try another name!" | N/A    |
|                                                                                     | 5    | Create a topic with a length exceeding the allowed limit.  Click the button 'POST'. | An error message is generated: "The topic name exceeds the permissible length!"                        | N/A    |
|                                                                                     | 6    | Create a topic without a description. Click the button 'POST'.                      | An error message is generated: "The topic description is required. Try again!"                         | N/A    |
|                                                                                     | 7    | Add a photo that does not match the format. Click the button 'POST'.                | An error message is generated: "The photo does not match the format!"                                  | N/A    |
|                                                                                     | 8    | Add a photo that exceeds the size limit. Click the button 'POST'.                   | An error message is generated: "The photo exceeds the size of…!"                                       | N/A    |
|                                                                                     | 9    | Add a video that exceeds the size limit. Click the button 'POST'.                   | An error message is generated: "The video exceeds the size of…!"                                       | N/A    |


## Test Case: Editing the theme by the user

| Preconditions                                                | Step   | Description                                                          | Expected Result                                           | Status |
|--------------------------------------------------------------|--------|----------------------------------------------------------------------|-----------------------------------------------------------|--------|
| The user is logged into the system and is in the user panel. | 1      | Select the 'TOPICS' option.                                          | The topics created by the user are displayed.             | N/A    |
|                                                              | 2      | Click on the three dots on the right side of the topic to be edited. | Options for editing and deleting appear.                  | N/A    |
|                                                              | 3      | Click on the edit button for the topic.                              | The user is directed to the edit page for the topic.      | N/A    |
|                                                              | 4      | Modify the topic's name/description/photo/video.                     | The changes are successfully made.                        | N/A    |
|                                                              | 5      | Click on the cancel button.                                          | The topic remains unchanged.                              | N/A    |
|                                                              | 6      | Click on the save button.                                            | The modifications are successfully saved.                 | N/A    |
|                                                              | 7      | Verify if the changes are reflected in the system.                   | The modifications to the topic are visible in the system. | N/A    |


## Test Case: Deleting the theme by the user

| Preconditions                                                | Step | Description                                                          | Expected Result                                         | Status |
|--------------------------------------------------------------|------|----------------------------------------------------------------------|---------------------------------------------------------|--------|
| The user is logged into the system and is in the user panel. | 1    | Select the 'TOPICS' option.                                          | The topics created by the user are displayed.           | N/A    |
|                                                              | 2    | Click on the three dots on the right side of the topic to be edited. | Options for editing and deleting appear.                | N/A    |
|                                                              | 3    | Click on the delete button for the topic.                            | A confirmation message appears.                         | N/A    |
|                                                              | 4    | Click on the cancel button.                                          | The topic remains unchanged.                            | N/A    |
|                                                              | 5    | Click on the confirm button.                                         | The topic is successfully deleted.                      | N/A    |
|                                                              | 6    | Verify if the topic is removed from the list.                        | The topic is no longer present in the list.             | N/A    |


## Test Case: Administration of themes by the admin

| Preconditions                                                        | Step | Description                                              | Expected Result                                          | Status |
|----------------------------------------------------------------------|------|----------------------------------------------------------|----------------------------------------------------------|--------|
| The admin is logged into the system and is in the admin panel.       | 1    | Choose the topic to be edited.                           | The topic is successfully selected.                      | N/A    |
|                                                                      | 2    | Locate the option to edit the topic.                     | The option to edit the topic is successfully located.    | N/A    |
|                                                                      | 3    | Click on the edit button for the topic.                  | The system allows the admin to edit the selected topic.  | N/A    |
|                                                                      | 4    | Modify the topic's name/description/photo/video.         | The details of the topic can be changed successfully.    | N/A    |
|                                                                      | 5    | Click on the cancel button.                              | The topic remains unchanged.                             | N/A    |
|                                                                      | 6    | Click on the save button.                                | The details of the topic are successfully updated.       | N/A    |
|                                                                      | 7    | Verify if the modifications are reflected in the system. | The modifications to the topic can be seen successfully. | N/A    |


## Test Case: Content Moderation

| Preconditions                                | Step   | Description                                                      | Expected Result                                                                       | Status |
|----------------------------------------------|--------|------------------------------------------------------------------|---------------------------------------------------------------------------------------|--------|
| The admin is logged into the system.         | 1      | Access the admin control panel.                                  | The admin control panel opens.                                                        | N/A    |
|                                              | 2      | Locate the options to modify and delete the desired content.     | The options to modify and delete are present on the page.                             | N/A    |
|                                              | 3      | Click on the delete button.                                      | A confirmation message appears.                                                       | N/A    |
|                                              | 4      | Click on the cancel button.                                      | The content remains unchanged.                                                        | N/A    |
|                                              | 5      | Click on the confirmation button.                                | The content is successfully deleted.                                                  | N/A    |
|                                              | 6      | Click on the modify button.                                      | The content can be modified.                                                          | N/A    |
|                                              | 7      | Introduce the desired changes.                                   | The admin can input the desired changes.                                              | N/A    |
|                                              | 8      | Click on the cancel button.                                      | The content remains unchanged.                                                        | N/A    |
|                                              | 9      | Click on the save changes button.                                | The modifications are successfully saved and can be viewed in the system.             | N/A    |


## Test case: Writing comments to posts

| Preconditions                                                    | Step | Description                                                      | Expected Result                                                | Status |
|------------------------------------------------------------------|------|------------------------------------------------------------------|----------------------------------------------------------------|--------|
| The user is logged in and has posting and commenting privileges. | 1    | Access the post for which you want to write a comment.           | The post is accessed and visible on the screen.                | N/A    |
|                                                                  | 2    | Check if there is an option to write comments on posts.          | The option to write comments is present.                       | N/A    |
|                                                                  | 3    | Click on the "ADD A COMMENT" field.                              | The user is able to input text.                                | N/A    |
|                                                                  | 4    | Write a comment.                                                 | The user can input a comment.                                  | N/A    |
|                                                                  | 5    | Click on the cancel button.                                      | The comment is not posted.                                     | N/A    |
|                                                                  | 6    | Click on the save button.                                        | The comment is successfully posted.                            | N/A    |
|                                                                  | 7    | Click on the save button.                                        | The comment is successfully posted and visible under the post. | N/A    |


## Test case: Validating comments

| Preconditions                                                   | Step | Description                                                      | Expected Result                                                                                                         | Status |
|-----------------------------------------------------------------|------|------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------|--------|
| The user is logged in and has selected the comment to reply to. | 1    | Click on the "ADD A COMMENT" field.                              | The user is able to input text.                                                                                         | N/A    |
|                                                                 | 2    | Leave the comment field empty and click on the post button.      | The user cannot click on the post button until they input a comment.                                                    | N/A    |
|                                                                 | 3    | Attempt to post a comment exceeding the maximum character limit. | An error message appears: "Your comment exceeds the maximum character limit. Please write a new comment and try again." | N/A    |


## Test case: Writing a reply to another comment

| Preconditions                                                                                  | Step  | Description                                                                         | Expected Result                                                                                      | Status |
|------------------------------------------------------------------------------------------------|-------|-------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|--------|
| The user is logged in and has posting and commenting privileges.                               | 1     | Locate the arrow indicating a reply to a comment.                                   | The arrow is successfully located.                                                                   | N/A    |
|                                                                                                | 2     | Click on the arrow.                                                                 | A field appears allowing the user to write a reply to that comment.                                  | N/A    |
|                                                                                                | 3     | Enter a comment.                                                                    | The user can input a comment.                                                                        | N/A    |
|                                                                                                | 4     | Click on the cancel button.                                                         | The comment is not posted.                                                                           | N/A    |
|                                                                                                | 5     | Click on the post button.                                                           | The comment is successfully posted.                                                                  | N/A    |
|                                                                                                | 6     | Verify if the comment is displayed under the commented comment.                     | The comment is displayed correctly and it is clearly identified as a reply to the commented comment. | N/A    |


## Test case: Editing a comment by the user

| Preconditions                                                                                      | Step | Description                                 | Expected Result                                           | Status |
|----------------------------------------------------------------------------------------------------|------|---------------------------------------------|-----------------------------------------------------------|--------|
| The user is logged in and has a comment on a post that they want to edit.                          | 1    | Click on the three dots on the right side   | A menu with options appears.                              | N/A    |
|                                                                                                    | 2    | Look for the edit option.                   | Find the option to edit the comment.                      | N/A    |
|                                                                                                    | 3    | Click on the "Edit" button.                 | The system allows the user to edit the comment.           | N/A    |
|                                                                                                    | 4    | Edit the comment.                           | The comment can be edited.                                | N/A    |
|                                                                                                    | 5    | Click on the "Cancel" button.               | The original comment remains unchanged.                   | N/A    |
|                                                                                                    | 6    | Click on the "Save" button.                 | The edited comment appears in place of the original one.  | N/A    |


## Test case: User deleting a comment

| Preconditions                                                                                           | Step | Description                                           | Expected Result                                               | Status |
|---------------------------------------------------------------------------------------------------------|------|-------------------------------------------------------|---------------------------------------------------------------|--------|
| The user is logged in and has a comment on a post that they want to delete.                             | 1    | Click on the three dots on the right side             | A menu with options appears.                                  | N/A    |
|                                                                                                         | 2    | Look for the delete option.                           | Find the option to delete the comment.                        | N/A    |
|                                                                                                         | 3    | Click on the "DELETE" button.                         | A confirmation message appears: "Permanently delete comment?" | N/A    |
|                                                                                                         | 4    | Click on the "Cancel" button.                         | The original comment remains unchanged.                       | N/A    |
|                                                                                                         | 5    | Click on the "DELETE" button again.                   | The comment is deleted.                                       | N/A    |
|                                                                                                         | 6    | Check if the deleted comment still exists.            | The comment cannot be found.                                  | N/A    |


## Test case: Deleting a comment by an admin

| Preconditions                                                                                        | Step | Description                                            | Expected Result                                               | Status |
|------------------------------------------------------------------------------------------------------|------|--------------------------------------------------------|---------------------------------------------------------------|--------|
| The admin is logged in and has selected the comment they want to delete.                             | 1    | Locate the option to delete the comment.               | The option to delete the comment is successfully located.     | N/A    |
|                                                                                                      | 2    | Click on the "DELETE" button.                          | A confirmation message appears: "Permanently delete comment?" | N/A    |
|                                                                                                      | 3    | Click on the "Cancel" button.                          | The original comment remains unchanged.                       | N/A    |
|                                                                                                      | 4    | Click on the "DELETE" button again.                    | The comment is deleted.                                       | N/A    |
|                                                                                                      | 5    | Check if the deleted comment still exists.             | The comment cannot be found.                                  | N/A    |


## Test case: Search functionality

| Preconditions                                                                                                 | Step | Description                                                       | Expected Result                                                    | Status |
|---------------------------------------------------------------------------------------------------------------|------|-------------------------------------------------------------------|--------------------------------------------------------------------|--------|
| The user is logged in to the system.                                                                          | 1    | Locate the search bar.                                            | The search bar is successfully located.                            | N/A    |
|                                                                                                               | 2    | Click on the search bar.                                          | The user can type something in the search bar.                     | N/A    |
|                                                                                                               | 3    | Enter the information you want to search.                         | The user can input text into the search bar.                       | N/A    |
|                                                                                                               | 4    | Press the "Enter" key.                                            | The searched information appears.                                  | N/A    |
|                                                                                                               | 5    | Leave the search bar empty and press Enter.                       | A notification appears indicating that no search term was entered. | N/A    |
|                                                                                                               | 6    | Enter irrelevant information into the search bar and press Enter. | A message appears: "No results found for the searched term."       | N/A    |


## Test case: Search functionality using filters

| Preconditions                                  | Step | Description                                         | Expected Result                                                                                            | Status |
|------------------------------------------------|------|-----------------------------------------------------|------------------------------------------------------------------------------------------------------------|--------|
| The user is logged in to the system.           | 1    | Locate the filtering tool.                          | The filtering tool is successfully located.                                                                | N/A    |
|                                                | 2    | Click on the arrow next to the 'FILTER' button.     | A list of filters appears.                                                                                 | N/A    |
|                                                | 3    | Select the desired filters.                         | The filters are successfully selected.                                                                     | N/A    |
|                                                | 4    | Check the displayed result.                         | The desired information appears according to the selected filters.                                         | N/A    |


## Test case: Light theme

| Preconditions                                                                                 | Step | Description                                      | Expected Result                                                                                           | Status |
|-----------------------------------------------------------------------------------------------|------|--------------------------------------------------|-----------------------------------------------------------------------------------------------------------|--------|
| The user is logged in.                                                                        | 1    | Locate the menu icon at the top right corner.    | The menu icon is successfully located.                                                                    | N/A    |
|                                                                                               | 2    | Click on the menu icon.                          | A menu appears.                                                                                           | N/A    |
|                                                                                               | 3    | Find the 'LIGHT MODE' button.                    | The 'LIGHT MODE' button is successfully located.                                                          | N/A    |
|                                                                                               | 4    | Click on the theme change button.                | The user interface elements are changed to the light theme, offering a coherent and pleasant experience.  | N/A    |


## Test case: Dark theme

| Preconditions                                                                               | Step | Description                                          | Expected Result                                                                                         | Status |
|---------------------------------------------------------------------------------------------|------|------------------------------------------------------|---------------------------------------------------------------------------------------------------------|--------|
| The user is logged in and has access.                                                       | 1    | Locate the menu icon at the top right corner.        | The menu icon is successfully located.                                                                  | N/A    |
|                                                                                             | 2    | Click on the menu icon.                              | A menu appears.                                                                                         | N/A    |
|                                                                                             | 3    | Find the 'DARK MODE' button.                         | The 'DARK MODE' button is successfully located.                                                         | N/A    |
|                                                                                             | 4    | Click on the theme change button.                    | The user interface elements are changed to the dark theme, offering a coherent and pleasant experience. | N/A    |

## Test case: Popup window functionality

| Preconditions                                             | Step  | Description                                                                      | Expected Result                                                                                                                                                                                                            | Status |
|-----------------------------------------------------------|-------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------|
| The user is logged into the system.                       | 1     | Access the website.                                                              | The website is successfully accessed.                                                                                                                                                                                      | N/A    |
| The popup window has not been previously viewed.          | 2     | Wait for the page to fully load.                                                 | The page has fully loaded.                                                                                                                                                                                                 | N/A    |
|                                                           | 3     | Check if the popup window is displayed.                                          | The popup window is successfully displayed.                                                                                                                                                                                | N/A    |
|                                                           | 4     | Click on the "Privacy Policy" link in the popup window.                          | The corresponding privacy policy page is successfully opened.                                                                                                                                                              | N/A    |
|                                                           | 5     | Close the privacy policy page.                                                   | The privacy policy page closes successfully, and the user is returned to the main page.                                                                                                                                    | N/A    |
|                                                           | 6     | Click on the "Terms of Use" link in the popup window.                            | The corresponding terms of use page is successfully opened.                                                                                                                                                                | N/A    |
|                                                           | 7     | Close the terms of use page.                                                     | The terms of use page closes successfully, and the user is returned to the main page.                                                                                                                                      | N/A    |
|                                                           | 8     | Click on the "Cookie Policy" link in the popup window.                           | The corresponding cookie policy page is successfully opened.                                                                                                                                                               | N/A    |
|                                                           | 9     | Close the cookie policy page.                                                    | The cookie policy page closes successfully, and the user is returned to the main page.                                                                                                                                     | N/A    |
|                                                           | 10    | Click outside the popup window, in an area outside it, but within the main page. | The popup window remains open, and the user can return to it if desired. Interacting with the area outside the popup does not close the popup.                                                                             | N/A    |
|                                                           | 11    | Click on the "X" button to close the popup window.                               | The popup window closes correctly, and the user is returned to the main page of the site.                                                                                                                                  | N/A    |
|                                                           | 12    | Reload the main page of the website.                                             | The popup window for the cookie policy appears again on the screen, requesting user consent. The user remains on the main page of the website and can interact again with the popup to accept or reject the cookie policy. | N/A    |
|                                                           | 13    | Reject the cookie policy.                                                        | The popup window closes correctly, and the user is returned to the main page of the site.                                                                                                                                  | N/A    |
|                                                           | 14    | Reload the main page of the website.                                             | The popup window for the cookie policy appears again on the screen, requesting user consent.                                                                                                                               | N/A    |
|                                                           | 15    | Accept the cookie policy from the popup.                                         | The popup window closes, and it no longer appears repeatedly on subsequent visits to the website. The user remains on the main page of the website.                                                                        | N/A    |

## Test case: User authentication using existing Google account

| Preconditions                       | Step | Description                                                | Expected Result                                                      | Status |
|-------------------------------------|------|------------------------------------------------------------|----------------------------------------------------------------------|--------|
| The user is registered on the site. | 1    | Locate the 'OR LOG IN WITH GOOGLE ACCOUNT' button.         | The 'OR LOG IN WITH GOOGLE ACCOUNT' button is successfully located.  | N/A    |
|                                     | 2    | Click on the 'OR LOG IN WITH GOOGLE ACCOUNT' button.       | The button is clickable.                                             | N/A    |
|                                     | 3    | Check if a window with the user's Google accounts appears. | A window opens displaying all of the user's Google accounts.         | N/A    |
|                                     | 4    | Select the account you want to use.                        | The user is successfully logged into the system.                     | N/A    |


## Test case: User authentication with a new Google account

| Preconditions                                                          | Step | Description                                                                   | Expected Result                                                   | Status |
|------------------------------------------------------------------------|------|-------------------------------------------------------------------------------|-------------------------------------------------------------------|--------|
| The user is registered on the site.                                    | 1    | Click on the 'USE ANOTHER ACCOUNT' button.                                    | A window opens to authenticate the user.                          | N/A    |
|                                                                        | 2    | Locate the field responsible for entering the email.                          | The email field is successfully located.                          | N/A    |
|                                                                        | 3    | Enter the desired email.                                                      | The email is entered.                                             | N/A    |
|                                                                        | 4    | Click on the 'Next' button.                                                   | The button is clickable.                                          | N/A    |
|                                                                        | 5    | Check if the field to enter the password appears.                             | The password field appears.                                       | N/A    |
|                                                                        | 6    | Enter the password.                                                           | The password is entered.                                          | N/A    |
|                                                                        | 7    | Click on the 'Next' button.                                                   | The button is clickable.                                          | N/A    |
|                                                                        | 8    | Check if the user is redirected to the main page of the site.                 | The user is successfully redirected to the main page of the site. | N/A    |
|                                                                        | 9    | Log out.                                                                      | The user is successfully logged out.                              | N/A    |
|                                                                        | 10   | Check if the Google account you logged in with appears in the account window. | The Google account appears in the account window.                 | N/A    |

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Test case: User Registration

### Purpose: Verify the functionality of registering a new user in the system.
### Requirement: The user should be able to register a new user.

| Step | Description of the Step                                                                                  | Expected Result                                               | Final Expected Result                                                                                | Status |
|------|----------------------------------------------------------------------------------------------------------|---------------------------------------------------------------|------------------------------------------------------------------------------------------------------|--------|
| 1    | Access the user registration page.                                                                       | The registration page is opened.                              | The user is successfully registered in the system and can log in using the registration credentials. | N/A    |
| 2    | Verify the appearance of basic functionalities on the registration page.                                 | Basic functionalities on the registration page are displayed. |                                                                                                      | N/A    |
| 3    | Check if all input fields are accessible and clickable.                                                  | All input fields can be accessed and filled.                  |                                                                                                      | N/A    |
| 4    | Fill in all mandatory fields with valid data (name, surname, email address, password, confirm password). | Fields are filled with valid data.                            |                                                                                                      | N/A    |
| 5    | Click on the "Register" button.                                                                          | User is successfully registered, and the page is displayed.   |                                                                                                      | N/A    |

---

## Test case: Negative User Registration

### Purpose: Verify the system behavior when a user attempts to register using invalid or missing data.
### Requirement: The username must be at least 8 characters long, and the password must be maximum 12 characters long.

| Step | Description of the Step                                                                                                                             | Expected Result                                                                                                       | Final Expected Result                                                                                                                                                                                             | Status |
|------|-----------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------|
| 1    | Access the user registration page.                                                                                                                  | The registration page is opened.                                                                                      | The system displays appropriate error messages for incorrectly completed or missing fields. The user is not registered in the system and is redirected back to the registration page to correct the entered data. | N/A    |
| 2    | Verify the appearance of basic functionalities on the registration page.                                                                            | Basic functionalities on the registration page are displayed.                                                         |                                                                                                                                                                                                                   | N/A    |
| 3    | Check if all input fields are accessible and clickable.                                                                                             | All input fields can be accessed and filled.                                                                          |                                                                                                                                                                                                                   | N/A    |
| 4    | Fill in the mandatory username field with invalid data or leave fields blank, such as "Maadwuh3", "manhqbc3", "MANTHSL3", "MANYYWBD N", "15785155". | Error message appears for incorrect username.                                                                         |                                                                                                                                                                                                                   | N/A    |
| 5    | Fill in the mandatory password field with invalid data or leave fields blank.                                                                       | Error message appears for incorrect password.                                                                         |                                                                                                                                                                                                                   | N/A    |
| 6    | Click on the "Register" button.                                                                                                                     | The user is not registered in the system and is redirected back to the registration page to correct the entered data. |                                                                                                                                                                                                                   | N/A    |

---

### Test case: User Login

#### Purpose: Verify the functionality of user login in the system.
#### Requirements: The user should be able to log in with valid credentials.

| Step | Description of the Step                                                                                   | Expected Result                                          | Final Expected Result                                                                                                                                       | Status |
|------|-----------------------------------------------------------------------------------------------------------|----------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|--------|
| 1    | Access the user login page.                                                                               | The login page is opened.                                | User is successfully logged into the system and has access to role-specific functionalities (e.g., profile management, viewing personal information, etc.). | N/A    |
| 2    | Fill in the login fields (email address and password) with valid data of a registered user in the system. | User is successfully logged in.                          |                                                                                                                                                             | N/A    |
| 3    | Test with minimum length for username and password.                                                       | Checkmark turns green, data matches system expectations. |                                                                                                                                                             | N/A    |
| 4    | Test with alphanumeric and numeric characters for username and password, respectively.                    | Green checkmark appears.                                 |                                                                                                                                                             | N/A    |
| 5    | Click on the "Log in" button.                                                                             | User is successfully authenticated.                      |                                                                                                                                                             | N/A    |

---

### Test case: Negative User Login

#### Purpose: Verify the system behavior when a user attempts to log in using invalid login credentials.
#### Requirements: Username must be at least 8 characters long, password maximum 12 characters.

| Step | Description of the Step                                                                                                                                                                           | Expected Result                                         | Final Expected Result                                                                                                                                                                | Status |
|------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------|
| 1    | Access the user login page.                                                                                                                                                                       | The login page is opened.                               | The system displays an appropriate error message for incorrect login credentials. User is not authenticated in the system and remains on the login page to correct the entered data. | N/A    |
| 2    | Fill in the login username field with invalid or nonexistent email addresses or leave fields blank for a registered user in the system (e.g., "3postaMold@.48", "postaMOLD.48", "52258585@.com"). | Error message displayed.                                | User is not authenticated in the system and remains on the login page to correct the entered data.                                                                                   | N/A    |
| 3    | Fill in the login password field with invalid data or leave fields blank.                                                                                                                         | Error message appears.                                  |                                                                                                                                                                                      | N/A    |
| 4    | Click on the "Log in" button.                                                                                                                                                                     | Error message displayed and returned to the login page. |                                                                                                                                                                                      | N/A    |

---

### Test Case: Post Voting System

#### Purpose: Verify the functionality of posting and voting on posts in the system.
#### Requirements: Posts should be accessible and allow comments.

| Step | Description of the Step                                             | Expected Result                                                | Final Expected Result                                                      | Status |
|------|---------------------------------------------------------------------|----------------------------------------------------------------|----------------------------------------------------------------------------|--------|
| 1    | Log in to the system as a valid user.                               | General page is opened.                                        | Post is successfully created by the user and can be viewed by other users. | N/A    |
| 2    | Access the post creation section in the selected theme.             | Comment window is available.                                   |                                                                            | N/A    |
| 3    | Fill in the mandatory fields for the title.                         | Title field is accessible.                                     |                                                                            | N/A    |
| 4    | Fill in the mandatory fields for the content.                       | Content field is accessible.                                   |                                                                            | N/A    |
| 5    | Fill in the fields for other details such as file import, stickers. | Details field is accessible, files are successfully accessed.  |                                                                            | N/A    |
| 6    | Click on the "Post" button.                                         | Post is created and can be viewed.                             |                                                                            | N/A    |

---

### Test Case: Successful Voting on User-Created Posts

#### Purpose: Verify successful voting on user-created posts.
#### Requirements: The post must exist and be votable.

| Step | Description of the Step                                                          | Expected Result                                   | Final Expected Result                                                                                                                       | Status |
|------|----------------------------------------------------------------------------------|---------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|--------|
| 1    | Log in to the system as a valid user.                                            | User exists, entry to the main page.              | Post can be upvoted or downvoted, the system must correctly calculate the positive or negative vote and display it for other users to view. | N/A    |
| 2    | Access an existing post in the selected theme. - Post can be accessed.           | Post can be accessed.                             |                                                                                                                                             | N/A    |
| 3    | Give a positive vote (upvote) to the post.                                       | Positive vote is placed, +1 to post's vote count. |                                                                                                                                             | N/A    |
| 4    | Give a negative vote (downvote) to the post.                                     | Negative vote is placed, -1 to post's vote count. |                                                                                                                                             | N/A    |
| 5    | Verify that the system allows only one vote per post and updates the vote count. | User can only place one vote, not two.            |                                                                                                                                             | N/A    |---

---

### Test Case: Visibility and Ranking

#### Purpose: Visibility and Ranking
#### Requirements: Posts must be visible and ranked by the number of votes.

| Step | Description of the Step                                                                                                                        | Expected Result                                                          | Final Expected Result                                                                                               | Status |
|------|------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|--------|
| 1    | Access the post viewing section in the selected theme.                                                                                         | The section is successfully opened.                                      | Posts are visible to users and sorted in the sorting section according to the total number of votes the post holds. | N/A    |
| 2    | Verify that the button leading to the sorted posts display is present on the page and clickable.                                               | The button is found successfully and is clickable.                       |                                                                                                                     | N/A    |
| 3    | Verify that the button to access the post visibility section is clickable.                                                                     | The button is clickable.                                                 |                                                                                                                     | N/A    |
| 4    | Verify that the posts are present on the posts viewing page.                                                                                   | Posts are successfully displayed on the posts page.                      |                                                                                                                     | N/A    |
| 5    | Verify that the posts are displayed in the correct order based on the total number of votes, with the most voted posts at the top of the list. | Posts are displayed successfully according to the total number of votes. |                                                                                                                     | N/A    |
---

### Test Case: Editing and Deleting Posts

#### Purpose: Editing and Deleting Posts
#### Requirements: Posts can be edited and deleted.

| Step | Description of the Step                                                                    | Expected Result                                                                                                        | Final Expected Result                                                                                                             | Status |
|------|--------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|--------|
| 1    | Log in to the system as a valid user or as an administrator.                               | Existing user, existing admin, successful login.                                                                       | Posts can be edited by the post owner, deleted by the post owner and by the admin if the post violates the general writing rules. | N/A    |
| 2    | Access your own post or the posts in the topics for which you have edit and delete rights. | Post can be accessed by the post owner and the admin responsible for the topic.                                        |                                                                                                                                   | N/A    |
| 3    | Attempt to Edit the post content and verify that the changes are saved correctly.          | unsuccessful                                                                                                           |                                                                                                                                   | N/A    |
| 4    | Attempt to Delete a post and verify that it no longer appears in the list of posts.        | unsuccessful.                                                                                                          |                                                                                                                                   | N/A    |
| 5    | Log in to the system as a valid user or as an administrator.                               | successful                                                                                                             |                                                                                                                                   | N/A    |
| 6    | Access your own post or the posts in the topics for which you have edit and delete rights. | Post can be accessed by the post owner and the admin responsible for the topic.                                        |                                                                                                                                   | N/A    |
| 7    | Edit the post content and verify that the changes are saved correctly.                     | Content can be modified and saved successfully by the user, the admin does not have the right to modify user posts.    |                                                                                                                                   | N/A    |
| 8    | Delete a post and verify that it no longer appears in the list of posts.                   | Post is successfully deleted and no longer appears in the list of posts.                                               |                                                                                                                                   | N/A    |
| 9    | Log in to the system as a valid user or as an administrator.                               | User/Administrator is successfully logged in.                                                                          |                                                                                                                                   | N/A    |
| 10   | Access your own post or the posts in the topics for which you have edit and delete rights. | Post can be accessed by the post owner and the admin responsible for the topic.                                        |                                                                                                                                   | N/A    |
| 11   | Edit the post content and verify that the changes are saved correctly.                     | Content can be modified and saved successfully by the user, the admin does not have the right to modify user posts.    |                                                                                                                                   | N/A    |
| 12   | Delete a post and verify that it no longer appears in the list of posts.                   | Post can be deleted by the post owner and the admin of the topic, and the post no longer appears in the list of posts. |                                                                                                                                   | N/A    |

---

### Test Case: Managing Post Votes

#### Purpose: Managing Votes
#### Requirements: The total number of votes is correctly counted by the system.

| Step | Description of the Step                                                                                                              | Expected Result                                                                                                                                                                                         | Final Expected Result                                                                                                                                                                             | Status |
|------|--------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------|
| 1    | Log in to the system as a valid user or as an administrator.                                                                         | The voting system for posts works correctly, allowing users to view and vote on posts based on the number of votes. When accessing upvote or downvote, the total number of votes is correctly modified. | Posts can be managed and viewed by existing users and administrators, and the total number of votes for each post is displayed correctly and can be updated by giving positive or negative votes. | N/A    |
| 2    | Access the post votes management section.                                                                                            | Successful access to the section with posts.                                                                                                                                                            |                                                                                                                                                                                                   | N/A    |
| 3    | Verify that the system allows viewing and managing votes given to posts (upvotes and downvotes).                                     | The post can be viewed, and positive or negative votes can be added.                                                                                                                                    |                                                                                                                                                                                                   | N/A    |
| 4    | Verify that the total number of votes for each post is displayed correctly and can be updated.                                       | Pressing the upvote button adds +1 vote to the total; Pressing the downvote button subtracts -1 vote from the total votes.                                                                              |                                                                                                                                                                                                   | N/A    |
| 5    | Verify that posts with a higher number of votes are placed higher in the list of posts, and those with fewer votes are placed lower. | Posts are sorted based on the total number of votes. Posts with a higher number of votes are displayed above those with a lower number of votes.                                                        |                                                                                                                                                                                                   | N/A    |
---

### Test Case: Managing Votes for Comments on Posts

#### Purpose: Managing Votes for Comments on Posts
#### Requirements: The total number of votes for comments must match the number of clicks recorded in the system
#### Preconditions: The user is logged in

| Step | Description of the Step                                                                          | Expected Result                                                                   | Final Expected Result                                                                                     | Status |
|------|--------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|--------|
| 1    | Access the section for viewing a post with comments.                                             | The post and comments are visible.                                                | The post and comments are visible, and the total number of votes for each comment is displayed correctly. | N/A    |
| 2    | Verify that the upvote and downvote buttons for comments are clickable.                          | The upvote and downvote buttons are active.                                       |                                                                                                           | N/A    |
| 3    | Give a positive vote (upvote) to a comment.                                                      | The total number of votes for the comment increases by 1.                         |                                                                                                           | N/A    |
| 4    | Give a negative vote (downvote) to a comment.                                                    | The total number of votes for the comment decreases by 1.                         |                                                                                                           | N/A    |
| 5    | Verify that the system does not allow more than one vote for the same comment by the same user.  | No additional votes are added for the same comment from the same user.            |                                                                                                           | N/A    |
| 6    | Verify that the total number of votes for each comment is updated correctly after giving a vote. | The total number of votes for the comment is updated according to the given vote. |                                                                                                           | N/A    |

---

### Test Case for Recommendation System Based on Number of Likes (Upvotes):

#### Purpose: Verifying the Recommendation System
#### Requirements: The system must recommend posts based on the number of upvotes.
#### Preconditions: The user is successfully logged in

| Step | Description of the Step                                                               | Expected Result                                                        | Final Expected Result                                             | Status |
|------|---------------------------------------------------------------------------------------|------------------------------------------------------------------------|-------------------------------------------------------------------|--------|
| 1    | Access the recommendations section for posts.                                         | The recommendations section is opened successfully.                    | Posts are recommended to the user based on the number of upvotes. | N/A    |
| 2    | Verify that the list of recommendations is displayed correctly and contains posts.    | The list of recommendations is displayed correctly and contains posts. |                                                                   | N/A    |
| 3    | Access one of the recommended posts.                                                  | The recommended post is accessed successfully.                         |                                                                   | N/A    |
| 4    | Verify that the accessed post has a high number of upvotes.                           | The accessed post has a high number of upvotes.                        |                                                                   | N/A    |
| 5    | Access the section for viewing posts.                                                 | The section for viewing posts is opened successfully.                  |                                                                   | N/A    |
| 6    | Verify that the viewed posts contain the most upvotes.                                | The viewed posts contain the most upvotes.                             |                                                                   | N/A    |


---

### Test Case: User Logout

#### Purpose: User Logout
#### Requirements: The user successfully logs out of the system
#### Preconditions: Authenticated User

| Step | Description of the Step                                                        | Expected Result                                             | Status |
|------|--------------------------------------------------------------------------------|-------------------------------------------------------------|--------|
| 1    | Locate the logout button in the user menu.                                     | The logout button is successfully located in the user menu. | N/A    |
| 2    | Verify that we can click on the logout button.                                 | The logout button is clickable.                             | N/A    |
| 3    | Verify if the user is logged out.                                              | The user is successfully logged out.                        | N/A    |
| 4    | Verify if the user is redirected to the login page after logout.               | The user is redirected to the login page after logout.      | N/A    |

---

## Test Case: Forgot Password
### Purpose: Verify the functionality of password recovery for a registered user in the system.

### Requirements: The user must have a valid account in the system. The user must have access to the "Forgot Password" option on the login page.

| Step | Description of the Step                                                                                              | Expected Result                                                                           | Final Expected Result                                        | Status |
|------|----------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------|--------------------------------------------------------------|--------|
| 1    | The user accesses the system's login page.                                                                           | The login page is opened successfully.                                                    | The user has access to the "Forgot Password" link or button. | N/A    |
| 2    | The user identifies and clicks on the "Forgot Password" link or button for password recovery.                        | The user is redirected to the password recovery page.                                     |                                                              | N/A    |
| 3    | The user enters their email address associated with their account in the dedicated field.                            | The email address is entered.                                                             |                                                              | N/A    |
| 4    | The user clicks the button or link to submit the password recovery request.                                          | The user receives a confirmation message for the password recovery request.               |                                                              | N/A    |
| 5    | The system sends an email to the email address associated with the account with instructions for password recovery.  | The password recovery email is successfully sent.                                         |                                                              | N/A    |
| 6    | The user accesses the email and follows the received instructions to reset their password.                           | The user can access the email and receives clear instructions for resetting the password. |                                                              | N/A    |
| 7    | The user enters a new password according to the system's security requirements.                                      | The user enters a new password.                                                           |                                                              | N/A    |
| 8    | The user completes the password recovery process by confirming the new password.                                     | The user confirms the new password.                                                       |                                                              | N/A    |
| 9    | The user can access their account using the newly set password.                                                      | The user can access the account with the new password.                                    |                                                              | N/A    |

---
