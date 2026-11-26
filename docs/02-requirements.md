# Requirements and acceptance Criteria

## Accounts and permissions
|ID| Requirement | Acceptance criteria|
|--|-------------|--------------------|
|R1 | A student can register with name, email and password | Given a new email and a valid password,when the form is submitted, then an account is created and the password is stored hashed |
|R2|A Student can login in with email and password|Given valid credentials when login form is submitted,then a ssesion token is issued|
|R3| A logged-in students can post a lost or found item| Given a logged-in student,when they click logout,then the session ends and the protected pages are longer accessible|
|R4| Only logged-in students can post a lost or found item| Given avisitor who is not logged in when they try to post an item,then they are redirected to the login page|
|R5| An admin can remove in appropriate posts| Given a logged-in admin when they delete a post, then it is removed and nolonger shown in the item list|
| R6 | The system rejects a login with a wrong password | Given a wrong password, when the login form is submitted, then an error message is shown and no session is created |
| R7 | A logged-in student can post a lost item with title, description, location and date | Given a logged-in student, when the lost item form is submitted with all required fields, then the item is saved and appears in the lost items list |
| R8 | A logged-in student can post a found item with title, description, location and date | Given a logged-in student, when the found item form is submitted with all required fields, then the item is saved and appears in the found items list |
| R9 | A student can upload a photo with a post | Given a post form, when a valid image under the size limit is attached, then the photo is stored and shown with the item |
| R10 | Anyone can browse and view all items | Given the items page, when it loads, then all active lost and found items are listed with their title, location and date |
| R11 | A student can search and filter items by keyword, category or status | Given a list of items, when a keyword or filter is applied, then only matching items are shown |
| R12 | The owner of a post can mark it as claimed or resolved | Given a post owned by the logged-in student, when they mark it resolved, then its status changes and it is no longer shown as active |
| R13 | A post cannot be submitted with missing required fields | Given the item form, when a required field is empty, then an error message is shown and nothing is saved |