# The-Standard-FAQ
1. I was looking otripleS solution you are directly exposing  domain entities but in my development career I was using viewmodel or DTO’s can you explain us when to use ViewModel or DTO?

DTO approaches assume that the APIs are responsible for populating audit fields, ids ... etc.

But in reality there are scenarios where you want to let the consumer control these fields. Like a migration scenario for instance. You can't force maintaining certain audit fields like created and updated dates without Hacking into the database and by passing your API because of the DTO model.
