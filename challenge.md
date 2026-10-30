The values of PATH, LANG and PWD, using printenv | grep three times.
STUDENT_NAME, STUDENT_ROLL_NUMBER and STUDENT_SEMESTER created with export, shown with printenv | grep '^STUDENT_', and proven gone after a new login.
The same three variables made permanent in ~/.bashrc, proven after a new login.
Ping blocked, proven, then allowed again. Use the handout hints: back up /etc/ufw/before.rules, change ACCEPT to DROP on the first echo-request line, run sudo ufw reload, then undo it
