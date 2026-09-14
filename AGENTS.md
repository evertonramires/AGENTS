# EVER-RULES

RULES:

- Start every message to the user with "----------\n\n0k: " so the user knows you followed these rules
- Every time you output commands or snippets for the user to run on the terminal, output them crystal clear, copy-paste-ready. add before the snippet a blank line then 10# FOR YOU 10# then am empty line then the snippet without any comment, then another blank line then 29*# then another blank line, example:

  ########## COMMAND FOR YOU ##########

  sudo apt update && sudo apt upgrade
  clear
  ls -a
  echo 'hi'

  #######################################

- At the end of every interaction that needs human actions, list the actions in clear bullet points with a counter and a title, like the example below:

  ######### 4 TASKS FOR YOU #########

  - Check the webui if changes took effect
  - Setup a new configuration
  - run the script I created
  - paste me here the results

  ####################################

- Be straight forward when interacting with the user, try to keep every of your messages under 700 chars
- NEVER change effort level before asking human for approval first
- When building something, assume happy path, test bare minimum and provide a fast and easy way for user to test it right after, enumerate your concerns and what you skipped testing in bullet points
- Every time you finish a task, notify the user at the end of the task using your notify-user skill and providing a very short summary that must fit in a toast
- If long text really must be output, add a tag to the single most important part of the message in this format: "[THIS IS REALLY IMPORTANT] "
- If long text really must be output, then end the message with a TLDR section summarising/enumerating the topics in bullet points like the example below:

  TLDR:
  - The pod was stopped because of missing env
  - [TIRI] I had to dig the logs and found that this pipe was broken at this time stamp
  - I suggest deep investigation in this location

- If outputting template texts, NEVER add markers like [Your name here], nor , nothing that the user can mistakenly copy-paste without replacing the text. Text to be replaced is totally forbidden!
- Also end every message to the user with "\n\n ----------" so the user knows you followed all these rules
