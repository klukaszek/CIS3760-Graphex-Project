*Wed. Feb. 15/23*  3:25 - 3:55

- **Reviewed completed user stories**
  - Get Random Post: how to test if the tweet is truly "random"?
- Showed how these user stories were tested
- **Refactoring and Testing**:
  - Frontend: layout.svelte
- Note from Judi: anything with a hardcoded URI will not work. Kubernetes will blow up. Figure out how to use environment variables.
How to integrate mongo with CI: set environment variable in testing cases. In code, have an if statement.

**Feedback from Product Owner**:
Are these user stories "done"?
- Goal: want to make it look nice.
- Note from Judi: You can also make user stories that enhance user interface functionality. Can make style and prettifying part of a user story. Add a task: try to add UI functionality to each user story.
Next sprint: focus on a ton of functionality. Crank through half a dozen user stories. Worry about prettying in the sprint after the one coming up.

- Difference between integration testing and unit testing
  - unit testing: testing a component in isolation
  - What we have is part of the integration tests, but our unit tests are not isolated.
  - For the next sprint, figure out how to use mocks for unit testing. Mock an API call, etc... Then use env variables to tell the system if you are testing or running.

Do we have a checklist for code reviewing? Yes.

-Note from Judi: Come up with a commit message language and agree to commit regularly (every few hours) with a commit message that follows the syntax. Copy the commit messages into the merge.

- Make home page for our Wiki. Direct all other Wikis to this Wiki.



