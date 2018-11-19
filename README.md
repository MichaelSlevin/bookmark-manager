# Bookmark Manager

## User stories
* Show a list of bookmarks
* Add new bookmarks
* Delete bookmarks
* Update bookmarks
* Comment on bookmarks
* Tag bookmarks into categories
* Filter bookmarks by tag
* Users manage their bookmarks

#### Show a list of bookmarks

As a user of the app
So that I can revisit my booked-marked sites
I should be able to see a list my bookmarks
`

![image of US1]
(./Images/US1.png)
```sequence'
Title: US1: List bookmarks
Controller->Model: Request list_bookmarks
Model->Database: Retrieve_bookmarks(user)
Database->Model: return query results
Model->Controller: return booksmarks as array
Controller->View: initiate erb with bookmarks
```
`
