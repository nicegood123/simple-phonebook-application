<b>GraphQL Playground Link</b>: BASE_URL/graphql-playground

<br>
<br>
<br>

<b>HTTP HEADERS</b>
{
	"Accept": "application/json",
	"Authorization": "Bearer 1|ijAbVzl23mqtVclvdGC2HZLZoKrTDWhQECKPgVqGe3fbf77d"
}

<br>
<br>
<br>

<b>MODULE NAME: AUTH</b>

<br>

LOGIN:
	Mutation:
		 mutation {
		 	login(
		     email:"gisangeff@gmail.com", 
		     password: "Gisangeff321!",
		     device: "web"
		   )
		 }

<br>
<br>


REGISTER:
	Mutation:
	mutation {
		register(
	    name: "Gisan Geff Raniego"
	    email:"gisangeff@gmail.com", 
	    password: "Bambu123!",
	    device: "web"
	  )
	}

<br>
<be>
<br>


MODULE NAME: USER

RETRIVE ALL USERS:
	Query:
		query {
		  listUsers {
		    id
		    name
		    email
		    created_at
		    updated_at
		  }
		}

 
RETRIEVE USER:
	Query:
		query {
		  viewUser(id: 1) {
		    id
		    name
		    email
		    created_at
		    updated_at
		  }
		}


ADD USER:
	Mutation:
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



DELETE USER:
	Mutation:
		mutation {
		  deleteUser(id: 1) {
		    id
		    name
		    email
		  }
		}

=========================================================================================
MODULE NAME: CONTACT

RETRIVE ALL CONTACTS:
	Query:
   		query {
		  listContacts {
		    id
		    name
		    contact_no
		    created_at
		    updated_at
		  }
		}

 
RETRIEVE CONTACT:
	Query:
		query {
		  viewContact(id: 1) {
		    id
		    name
		    contact_no
		    created_at
		    updated_at
		  }
		}

ADD CONTACT:
	Mutation:
		mutation {
		  createContact(
				  name: "Janice",
				  contact_no: "+639678123674"
		  ) {
		    id
		    name
		    contact_no
		    created_at
		    updated_at
		  }
		}



UPDATE CONTACT:
	Mutation:
		mutation {
		  updateContact(
		     	id: 1,
				  name: "Recca Rance",
				  contact_no: "+639487776849"
		  ) {
		    id
		    name
		    contact_no
		    created_at
    		updated_at
		  }
		}	



DELETE CONTACT:
	Mutation:
		mutation {
		  deleteContact(id: 3) {
		    id
		    name
		    contact_no
        created_at
        updated_at
		  }
		}
