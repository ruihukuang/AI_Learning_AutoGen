# AI_Learning_AutoGen  

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
<img width="991" height="583" alt="image" src="https://github.com/user-attachments/assets/094878f5-2616-4b9d-978a-6cdd120deac1" />  


## lab 3  

Context  

This lab focuses on standalone runtime: the *SingleThreadedAgentRuntime*, a local embedded agent runtime implementation. In this example, there are 3 agents including player 1, player 2 and an agent providing instructions for players and judgements of who wins. The instructions are about playing rock, paper, scissors.  

The screenshot belows show results.   
<img width="908" height="210" alt="image" src="https://github.com/user-attachments/assets/f1766153-8ce7-484d-887f-9aa54d785433" />  


## lab 4     

Context  

This lab focuses on distributed runtime. In this example, there are 3 agents including player 1, player 2 and an agent providing instructions for players and making a decision on whether to use AutoGen for a project. The instructions are about discussing pros and cons for AutoGen.  

The screenshot belows show results.  
<img width="877" height="574" alt="image" src="https://github.com/user-attachments/assets/1539132c-8c8b-4885-a6a3-9dc2416f712b" />  

## App folder   

Context  
There are 3 agents in this workflow. One agent is a creator who could creates agents. 2 agents are created based on a python code template provided in agent.py. These two agents come up with a new business idea. If a randomly generated number is lower than a defined percentage, an agent will act on refining the idea and make it better. This workflow uses distributed runtime and distributed runtime and coroutines, enabling agents to run asynchronous tasks concurrently.   

The screenshot below shows progress in steps in this workflow.  
<img width="1725" height="284" alt="image" src="https://github.com/user-attachments/assets/5555ea17-97db-4772-98ea-821a5d3255fd" />  

2 newly created templates for 2 agents who propose a new business idea could be found in https://github.com/ruihukuang/AI_Learning_AutoGen/blob/main/app/agent1.py and https://github.com/ruihukuang/AI_Learning_AutoGen/blob/main/app/agent2.py.  

Ideas that are proposed by 2 agents could be found in https://github.com/ruihukuang/AI_Learning_AutoGen/blob/main/app/idea1.md and https://github.com/ruihukuang/AI_Learning_AutoGen/blob/main/app/idea2.md.  

This process is not reliable. 3 Attemps were made before generating outputs. 












