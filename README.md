**OpenAI Computer Use Agent Code Demo**

This is an experimental demo of OpenAI's new computer use agent. It enables you to run a simple computer use agent task, and to observe the actions the agent takes, and analyse the API call logs.

This agent has been designed to work within the constraints of Google colab, yet still provide a simple UI to monitor agent actions.

**Access the notebook here:** https://github.com/smartaces/OpenAI_Computer_Use_Agents_Google_Colab_Demo/blob/main/OpenAI_Computer_Use_Agents_Colab_Demo_Github_Shared.ipynb

**Or in Google colab:** https://colab.research.google.com/github/smartaces/OpenAI_Computer_Use_Agents_Google_Colab_Demo/blob/main/OpenAI_Computer_Use_Agents_Colab_Demo_Github_Shared.ipynb

![image](https://github.com/user-attachments/assets/3fce12a1-cca8-4aac-82bc-adc42db1982f)

**Watch The Video Walkthrough:** https://www.youtube.com/watch?v=T88s6IB0hQI

![image](https://github.com/user-attachments/assets/74bd214c-847b-4bda-9290-3f62be658621)

**Important - Please Read**

Helpful guidance:

- Computer use agents processes text, images and actions, and can consume a lot of tokens

- To complete actions, the agents have to be passed historical actions as context. To make these agents work in Colab with a UI, I have had to build in ways to pass history as context. This includes the last 10 messages in the context, so potentially incurs a chunky number of tokens. Monitor your spend

- To manage for this, I recommend keeping sessions short, or that you optimise the code more as you wish.

- Sometimes computer use agents get stuck in loops, or act erratically, this can mean they take longer than they should to complete a simple action.

- I have designed the notebook so that API requests and responses are logged in the API logs folder, the full agent history is also stored in the conversation_history.json, this can be useful for understanding how these agents work, and where they fail.

- All agent screenshots are saved in the screenshots folder, again for you to check back through as you need.

- Generally the AI works pretty well, giving you a view of the screen the agent is working on, the chat interaction history, and the current agent action/ logs.

- This notebook uses a mix of the previous_response_id to pass historic agent actions back the computer use model, and chat history. I find this mix works best in colab, and overall it helps the agent stay on track
