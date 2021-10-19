# Event-Driven Architecture

- What's the difference between a FIFO and a standard queue?

*None. Stacks are LIFO by design and queues are FIFO by design.*

- How can the server be assured a message was properly received?

*We can add a function after the response firing action, which means we've proceeded through the code and reached the final function in the action, verifying the .emit or .send was received by the client/socket.*

- What classic design pattern is best represented by event driven programming?

*Asynchronous architecture (promise-like actions and req/res responses).*

- How do you test an event driven system?

*Service tests, Unit tests, and SUT tests.*

Term | Definition
---- | ----
FIFO Queue | A queue based on the first in, first out principle.
Pub/Sub | Publishers and Subscribers that communicate through asynchronous events.