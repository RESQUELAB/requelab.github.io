# Submitted to EMSE Journal

## A Comparative Study on Reward Models for UI Adaptation with Reinforcement Learning

### Daniel Gaspar-Figueired, Silvia Abrahão, Marta Fernández-Diego and Emilio Insfran

## Experiment Replication:

**Server Side (Windows only):**

1. Download the Server side app: [Server App](https://drive.google.com/file/d/1C3x5ya6PPGzHzRcfveD03rkuFntV1XQr/view?usp=drive_link)
2. Execute the RL-SERVER (tested with Python version 3.6.3):
   - (OpenAI Gym Dependency) - Go to [RL-UIAdaptation GitHub](https://github.com/RESQUELAB/RL-UIAdaptation), download and install the package. Follow these steps:

     

    ```python 
    conda create -n UIrlhf python==3.6.3

     conda activate UIrlhf
     
     cd RL-based-UIAdaptation
     
     pip install -e .
     ```

   - Execute the Server: `python server.py`

3. Extract the zip and execute “AdaptiveUI_Server.exe”
4. Wait till clients connect. (Click on Refresh to see the connected clients)
   - Give the clients your:

     - Address
     - PORT
     - Password

5. Once a client is connected, you can:
   - Change the System/Domain:

     - Sports
     - Trips
     - Courses

   - Assign an Adaptation Method:

     - Non-Adaptive (NA) - Assigns a random UI to the client.
     - Using Predictive HCI models (HCI) – Requires the RL-Server.
     - Using Predictive HCI models with HF (HCI-HF) - Requires the RL-Server.

   - Assign the Learning method (LEARN) to train the HCI-HF models.

**Client Side (Windows only):**

1. Download the Client side app: [Client App](https://drive.google.com/file/d/1KChAqqDx94inN7kgAA_GUafroBOuFO1C/view?usp=drive_link)
2. Extract the zip.
3. Execute “proxy-win.exe”:
   - Enter the SERVER’S IP (press enter to continue)
   - Enter the SERVER’S PORT (press enter to continue)
   - Allow access (if needed)
   - Comment: Now the client and the server can keep the connection. Don’t close this console.
4. Execute “adaptiveapp.exe”
5. Click on the refresh button.
6. “Connected” and a Green circle should appear. If not:
   - “Server is down. Try again later”: Launch the Server app and repeat from step 3 (Client side).
   - “Proxy is off. Launch it first.”: Restart the proxy and repeat from step 3 (Client side).
7. Log in with the following data:
   - Username: (free of choice)
   - Password: (check the Server UI to see the password) – Default: uiadapt
8. Use the application.

To create the RLHF model, follow the steps in [RL-Teacher-UIAdaptation GitHub](https://github.com/RESQUELAB/RL-Teacher-UIAdaptation).

## Data is yet to be uploaded.

## Manuscript

To be uploaded.
