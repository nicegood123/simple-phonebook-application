# Simple Phonebook Application Guide

## GraphQL Playground Link: BASE_URL/graphql-playground

## HTTP Headers

```
{
	"Accept": "application/json",
	"Authorization": "Bearer 1|ijAbVzl23mqtVclvdGC2HZLZoKrTDWhQECKPgVqGe3fbf77d"
}

NOTE: Change Bearer token with your generated access token
```

## Auth Module
### *Login User*

```
mutation {
  login(email: "gisangeff@gmail.com", password: "Bambu123!", device: "web")
}
```

### *Register User*

```
mutation {
  register(
    name: "Gisan Geff Raniego"
    email: "gisangeff@gmail.com"
    password: "Bambu123!"
    device: "web"
  )
}
```



## User Module
### *Get list of users*

```
query {
  listUsers {
    id
    name
    email
    created_at
    updated_at
  }
}
```


### *View a user*

```
query {
  viewUser(id: 1) {
    id
    name
    email
    created_at
    updated_at
  }
}
```


### *Create a user*

```
mutation {
  createUser(
    name: "Gisan Geff Raniego",
    email: "gisangeff@gmail.com",
    password: "gisangeff123*"
  ) {
    id
    name
    email
    created_at
    updated_at
  }
}
```


### *Delete a specific user*

```
mutation {
  deleteUser(id: 1) {
    id
    name
    email
  }
}
```



## Contact Module
### *Get list of contacts*

```
query {
  listContacts {
    id
    name
    contact_no
    created_at
    updated_at
  }
}
```


### *View a contact*

```
query {
  viewContact(id: 1) {
    id
    name
    contact_no
    created_at
    updated_at
  }
}
```


### *Create a contact*

```
mutation {
  createContact(name: "Janice", contact_no: "+639678123674") {
    id
    name
    contact_no
    created_at
    updated_at
  }
}
```


### *Edit a specific contact*

```
mutation {
  updateContact(id: 1, name: "Recca Rance", contact_no: "+639487776849") {
    id
    name
    contact_no
    created_at
    updated_at
  }
}
```


### *Delete a specific contact*

```
mutation {
  deleteContact(id: 3) {
    id
    name
    contact_no
    created_at
    updated_at
  }
}
```
