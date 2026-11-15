# house-watch

Checks every 5 minutes that home.rkhuntjr.com reaches the house. When it
can't, it opens an issue assigned to the owner, which GitHub sends as an email
and a phone notification. When the house answers again it closes the issue.

The probe path is the one the edge gate passes through; a 404 from the app
means the house answered.

`keepalive` is touched once a month because GitHub turns off scheduled
workflows in a public repository after 60 days with no commits.
