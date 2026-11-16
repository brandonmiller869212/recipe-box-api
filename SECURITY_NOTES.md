# Open API security baseline – 2026-11-15

- Anonymous GET /recipes -> 200, returns all recipes including non-public ones.
- Anonymous PATCH /recipes/3 -> 200, was able to change the title of recipe 3.
- Anonymous DELETE /recipes/3 -> 204, recipe 3 was removed from the list.
- No login, token, or authentication is required for any of these operations.
- Any requester who can reach the API and knows the paths can read, change, or delete recipes.

