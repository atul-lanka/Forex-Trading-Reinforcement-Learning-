# Forex-Trading-Reinforcement-Learning-
This project describes the implementation of a Deep Reinforcement Learning based system that is capable of automatically trading on the Foreign Exchange Market (Euro-Dollar Exchanges).

## Method and Data

In designing this project it was determined there would be 3 areas to explore, the custom environment, the neural network, and the reinforcement learning model. The custom environment would include aspects such as the actions the agent could take, the method of introducing rewards, and the way observation was output to the neural network. The neural network would include the architecture of the model’s decision making process, and would explore the benefits of models such as a dense neural network, convolutional neural network, and Long Short Term Memory (LSTM) networks. LSTMs are very powerful in sequence prediction problems because they're able to store past information and have feedback connections. Finally, the modifications to the DQN reinforcement learning model would explore how the policy, window size, and dueling architecture modified the results.

The data being used in this experimental process consisted of foreign exchange data collected between January 2017 and March 2021 in increments of 10 minutes, 1 hour, and 4 hours for the EURO/USD currency pair. To test the functionality of our models simulated data manually generated from a repeating sine wave was also used.

The environment was designed in a way that only one trade could be going on at any given time. Every step, the agent could make the decision to enter a short or a long trade, wait, or exit an existing trade. If the action selected by the agent was invalid in the current state, the environment would default to waiting until the next step. This would happen, for example, if the agent tried to enter a new trade when another trade was still active. Once a trade was exited, the episode would end. Below is a list of the efforts made to modify the environment in the hopes of improving performance.

<img width="655" alt="Screen Shot 2023-02-06 at 1 44 32 PM" src="https://user-images.githubusercontent.com/74167574/217058671-21824850-0c3a-4a77-b7c5-34f0df82bae0.png">
<img width="667" alt="Screen Shot 2023-02-06 at 1 44 44 PM" src="https://user-images.githubusercontent.com/74167574/217058684-49014bbf-9f53-47ef-a375-7b716d3d62a4.png">

## Results
<img width="515" alt="Screen Shot 2023-02-06 at 1 46 08 PM" src="https://user-images.githubusercontent.com/74167574/217058747-3452c73b-f457-4feb-be48-e48e2b8c827b.png">
<img width="497" alt="Screen Shot 2023-02-06 at 1 46 18 PM" src="https://user-images.githubusercontent.com/74167574/217058750-fb229bb6-1f18-4214-bfe0-2c90dd45860f.png">
<img width="498" alt="Screen Shot 2023-02-06 at 1 46 25 PM" src="https://user-images.githubusercontent.com/74167574/217058752-cea96905-e6f2-4b18-97f1-f651d0dfd293.png">
<img width="496" alt="Screen Shot 2023-02-06 at 1 46 31 PM" src="https://user-images.githubusercontent.com/74167574/217058754-6f994b35-01a5-40e7-8b88-743b6eff978b.png">
<img width="507" alt="Screen Shot 2023-02-06 at 1 46 37 PM" src="https://user-images.githubusercontent.com/74167574/217058757-bdef9fb5-aa99-4178-a3b8-9e6517533e4f.png">
<img width="532" alt="Screen Shot 2023-02-06 at 1 46 43 PM" src="https://user-images.githubusercontent.com/74167574/217058762-dcec37f9-de08-46e7-8cba-bda26be13b60.png">
<img width="508" alt="Screen Shot 2023-02-06 at 1 46 49 PM" src="https://user-images.githubusercontent.com/74167574/217058766-71f16f85-3306-4aa1-80ce-5148a8c2fee1.png">
