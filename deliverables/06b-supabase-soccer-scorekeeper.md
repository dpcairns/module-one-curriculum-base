
# Deliverable 06 - Supabase Soccer Scorekeeper

### Live Example:
https://dpcairns.github.io/soccer-scorekeeper/

| User should be able to . . .                                                         |             |
| :----------------------------------------------------------------------------------- | ----------: |
| Visit the deployed pages on GitHub pages, with link in the About section of the Github repo|        1 |
| On the home page (`'/'`), Login and Signup using the login and signup form. On success, redirect to the `/games` page   |        1 |
| Logout by clicking the logout button                                                       |        1 |
| If a non-logged-in user tries to visit the games page, redirect them to the login page | 1 |
| On the games page load, see a form and empty current game div                              |        1 |
| On the games page load, fetch all past games and render them to the past games div         |        1 |
| On submit, add the team names to the current game div                                      |        1 |
| On clicking add or subtract, increment and decrement the correct score in the current game div|     1 |
| On clicking finish, empty the current game div, and use supabase to add the current game to the database. |1|
| On clicking finish, clear the past games div, then fetch all past games from supabase and render them in the past games div. |1|

| Functions                                                              |             |
| :----------------------------------------------------------------------------------- | ----------: |
| IMPURE: `updateCurrentGameEl()` | 1|
| IMPURE: `renderAllGames()` : clears out and appends to games div | 1|
| PURE: `renderGame(game)` : returns DOM node | 1|
| PURE: `renderTeam(name, score)` :  return DOM node | 1|
| AUTH: `getUser()` : return currently logged in user |1|
| AUTH: `checkAuth()` : redirect the user to login if nobody is currently not logged in |1|
| ASYNC AUTH: `signupUser()` : create a new user in superbase and return user |1|
| ASYNC AUTH: `signinUser()` : log into superbase and return currently logged in user |1|
| ASYNC: `createGame(game)` : creates a game for currently logged in user in supabase |1|
| ASYNC: `getGames()` : returns games for currently logged in user from supabase |1|