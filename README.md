# alexa-skill-template
This is an example alexa skill repository. The skill uses Python. It is configured to be used with Visual Studio Code in a debuggable way. There are two functions for sending requests to a third-party API
in the `lambda_function.py`. 

* When a skill is created with `ask cli`, a repository is created automatically on the AWS servers. This repository is not publicly available.
* If you make a change on the *alexa skill console* on the intents part, you might need to pull those changes before pushing anything to the server since you can override them.

* An example command for getting the actual interaction-model that is altered on the console to the local is `ask smapi get-interaction-model -s <SKILL ID> --locale en-US > skill-package/interactionModels/custom/en-US.json`
After this you can push your repo that might include changes on the `lambda_function.py` or more(of course you can also change your interaction-model on local) without overriding the changes 
on the console.
