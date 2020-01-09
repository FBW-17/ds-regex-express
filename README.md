# Validation Exercise #6 - RegEx with Express Validator

We now want to write a password check using the matches() function and a regular expression.

Basic way to perform a regular expression match on a field in Express Validator:
`check('password', '<custom error message>').matches(/regex/)`

## Password check rules

* The sent Password should start with letters (case insensitive), minimum 4
* Then exactly one special character should follow. It can be any of these: *+-/$
* Afterwards the password should end by at least one number or more

Example of valid passwords:
`
Hello+123
GoodMorning$55
`

Invalid passwords:
`
Hi-10
Hello_2020
`