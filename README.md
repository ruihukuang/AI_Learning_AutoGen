# AI_learning_AutoGen  

## lab 1  

Context  
Create a database file locally with round trip prices for different cities. Define a tool to get a price for a city bassed on this database file. AutoGen uses a model, an agent with system messages and the tool to provide an answer based on a user message related to a price for a city. 

The user message in this example is *I'd like to go to London*.  
The screenshot below shows an answer provided by AutoGen.  
<img width="1021" height="262" alt="image" src="https://github.com/user-attachments/assets/9c7b2e92-5fbc-4df1-9070-e992c1f6c803" />  


## lab 2    

Context  
There are four topics in this lab using AutoGen. 

The first one is to use AutoGen to read an image from a provided link and then to use MultiModalMessage to create a user message so that a response could be provided for a defined agent. The user message in this example is *Describe the content of this image in detail*.  

The screenshot below shows the response.  
<img width="1004" height="592" alt="image" src="https://github.com/user-attachments/assets/ff9de295-abc2-4c96-a994-ac872c3e0def" />  


The second one is to create a structured/defined output based on the same setup as the first topic. The output should include *scene*, *message*, *style* , and *orientation*.  

The screenshot below shows the output.  
<img width="943" height="401" alt="image" src="https://github.com/user-attachments/assets/766288a0-12a6-407b-90d6-573e721e1092" />  


The third one is to integrate LangChain tools with AutoGen.   
In this example, LangChain tools include google serper API to search webs and file management tool kits to write outputs into a file. The file could be found in the link https://github.com/ruihukuang/AI_learning_AutoGen/blob/main/sandbox/flights.md.   


The fourth one is to use RoundRobinGroupChat to enable multiple agents to share the same context.   
In this example, there are 2 agents. One agent acts as a research assistant to uses google serper API, a LangChain tool to look for promising deals on flights. Another agent acts as an evaluator to provide feedback and approval for the research assistant agent. The user message is *Find a one-way non-stop flight from JFK to LHR in June 2025*.  

The screenshot below shows outputs.  



