Alexa and GPT-3 Experiment
===
This is an experimental project showing how to use OpenAI's GPT-3 API (https://openai.com/api/) under the covers of an Alexa skill to produce "intelligent" responses to user prompts. This is the code created in the video at https://youtu.be/4g_rY451bxM.

Before this code was committed to GitHub, it was scrubbed to remove the Alexa skill ID, AWS Lambda URNs, and OpenAI keys. You'll need to provide your own skill ID and OpenAI keys. The Lambda URNs should be created for you once you deploy your Alexa skill.

To do this, I recommend the following steps:

1. Clone this repository to your local machine.
2. Create a new Alexa-hosted skill using `ask new`. Be sure to create it in a separate directory from where you cloned this repository.
3. Selectively copy interaction model JSON and lambda Node.js code from the clone directory over your newly created Alexa skill directory. **WARNING!** Do not copy the `skill-package/skill.json` file over your skill project's corresponding file. Doing so will remove your skill's AWS Lambda URNs.
4. Register for an OpenAI key at https://openai.com/api/ and paste it into the `lambda/Keys.js` file as the value for `OPEN_AI_KEY`.
5. Deploy your skill and try it out by committing and pushing the Alexa-hosted skill.

If you are new to developing Alexa skills or need further understanding of these suggested instructions, you can learn a lot about Alexa skill development by reading [Build Talking Apps for Alexa](https://pragprog.com/titles/cwalexa/build-talking-apps-for-alexa/), or post an issue in the issue tracker and I'll try to help out.

That said, this is a personal and experimental project and is not in any way officially supported. I'll try to help out when I have time, but no promises of support should be expected.
