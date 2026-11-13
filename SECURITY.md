# Leaked secret?

1. Tell your supervisor **immediately**. Do not try to hide it.
2. Revoke / rotate the secret (change the password, regenerate the key).
   Deleting it from Git is not enough: it stays in history.
3. Remove it from history with your supervisor's help (e.g. `git filter-repo`).
