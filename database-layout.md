# Database layout
It is assumed that mySql will be the database used and all SQL will be mysql compatible. Things are always subject to change!

## Tables

### Company
	id
	name
	street
	phone
	ts

### City
	id
	name
	stateId
	ts

### State
	id
	fullname
	shortname
	ts

### Zipcode
	id
	code
	stateId
	cityId
	ts

### JobType
	id
	name
	ts

### People
	id
	firstname
	lastname
	street
	phone
	cityId
	stateId
	zipId
	classId
	ts

### Classes
	id
	className (recruiter, jobseeker, indicidual)
	ts

### RecruiterCompany
	id
	companyName
	ts

### Employees
	id
	companyId
	peopleId
	ts

### Jobs
	id
	position
	jobTypeId
	ts

### JobLists
	id
	jobsId
	postedDate
	removedDate
	filled (y/n)
	ts

This is a preliminry idea and will be adjusted. this document should be kept up to date.
