## Core Activity Steps (6 minutes)

- **Enable Streaming:**
  - In the API Connector, modify the existing API call to enable streaming by adding `"stream": true` to the JSON body and changing the Data type to **Stream**.
<p align="center"> <img src="https://github.com/Sasishivaran/API_images/blob/main/enable_streaming.png" width="900"> </p>

- **After ReIntializing call make the necessary changes and click save:**
<p align="center"> <img src="https://github.com/Sasishivaran/API_images/blob/main/build_streaming.png" width="900"> </p>


- **Build the Streaming Workflow**
  - Create a new workflow that triggers on the "An API request has finished" event. Use this event to append the incoming text chunk to a custom state. Connect this custom state to the response text element on the page to display the text in real time.

<p align="center">
  <img src="https://github.com/Sasishivaran/API_images/blob/main/open_AI_workflow.png" width="900">
</p>

- **Implement the Cancel Button:**
  -  Add a "Stop" button to the UI. Create a workflow for this button that uses the "Cancel an API request" action, targeting the correct API Request ID to terminate the stream.
<p align="center">
  <img src="https://github.com/Sasishivaran/API_images/blob/main/implement_workfow.png" width="900">
</p>    

<p align="center">
  <img src="https://github.com/Sasishivaran/API_images/blob/main/stop_button.png" width="900">
</p> 
