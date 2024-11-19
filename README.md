# RAG-chatbot-with-bedrock-knowledgebase
a 𝗥𝗔𝗚 𝗖𝗵𝗮𝘁𝗯𝗼𝘁 𝗹𝗲𝘃𝗲𝗿𝗮𝗴𝗶𝗻𝗴 𝗯𝗼𝘁𝗵 𝗔𝗺𝗮𝘇𝗼𝗻 𝗕𝗲𝗱𝗿𝗼𝗰𝗸 𝗸𝗻𝗼𝘄𝗹𝗲𝗱𝗴𝗲 𝗯𝗮𝘀𝗲/𝗦𝟯 𝗯𝘂𝗰𝗸𝗲𝘁 and user-uploaded documents to provide accurate, context-aware responses. It also 𝗽𝗿𝗼𝘃𝗶𝗱𝗲𝘀 𝘁𝗵𝗲 𝘀𝗼𝘂𝗿𝗰𝗲𝘀 𝗼𝗳 𝘁𝗵𝗲 𝗿𝗲𝘀𝗽𝗼𝗻𝘀𝗲 and 𝗺𝗮𝗶𝗻𝘁𝗮𝗶𝗻𝘀 𝗰𝗵𝗮𝘁 𝗵𝗶𝘀𝘁𝗼𝗿𝘆. 

🔍 Key Features:
- 𝗗𝗼𝗰𝘂𝗺𝗲𝗻𝘁 𝗨𝗽𝗹𝗼𝗮𝗱 𝗖𝗮𝗽𝗮𝗯𝗶𝗹𝗶𝘁𝘆: Support for PDF and TXT files allows users to enrich the chatbot's knowledge base with personal or proprietary documents.
- 𝗘𝗳𝗳𝗶𝗰𝗶𝗲𝗻𝘁 𝗥𝗲𝘁𝗿𝗶𝗲𝘃𝗮𝗹 𝗠𝗲𝗰𝗵𝗮𝗻𝗶𝘀𝗺: Utilizes FAISS for vector-based similarity searches.
-𝗦𝗼𝘂𝗿𝗰𝗲𝘀 𝗳𝗼𝗿 𝗥𝗲𝘀𝗽𝗼𝗻𝘀𝗲𝘀: Ensures transparency and reliability by providing references to the original sources from which information was retrieved. This feature allows users to verify and delve deeper into the provided answers.
- 𝗖𝗵𝗮𝘁 𝗛𝗶𝘀𝘁𝗼𝗿𝘆 𝗠𝗮𝗻𝗮𝗴𝗲𝗺𝗲𝗻𝘁: Maintains a well-organized chat history.
- 𝗖𝗹𝗲𝗮𝗿 𝗖𝗵𝗮𝘁 𝗙𝘂𝗻𝗰𝘁𝗶𝗼𝗻𝗮𝗹𝗶𝘁𝘆: Users can easily reset their conversation history

🛠️ 𝗗𝗶𝗿𝗲𝗰𝘁 𝗞𝗻𝗼𝘄𝗹𝗲𝗱𝗴𝗲 𝗕𝗮𝘀𝗲 𝗜𝗻𝘁𝗲𝗴𝗿𝗮𝘁𝗶𝗼𝗻 𝗘𝘅𝗽𝗹𝗮𝗶𝗻𝗲𝗱: 
One of the standout features of my RAG Chatbot is it's ability to dynamically retrieve and integrate information directly from Amazon Bedrock knowledge base. Here's how it works:

𝗤𝘂𝗲𝗿𝘆 𝗘𝗺𝗯𝗲𝗱𝗱𝗶𝗻𝗴: When a user submits a question, the system first converts the query into a high-dimensional vector using Amazon Bedrock's fully managed bedrock-runtime Embedding API. Leveraging this fully managed API ensures seamless scalability and reliability without the need for manual infrastructure management.

𝗩𝗲𝗰𝘁𝗼𝗿-𝗕𝗮𝘀𝗲𝗱 𝗥𝗲𝘁𝗿𝗶𝗲𝘃𝗮𝗹: This vector is then used to perform a similarity search against the knowledge base stored in FAISS, identifying the most relevant documents or passages based on cosine similarity. This is achieved through the 𝗯𝗲𝗱𝗿𝗼𝗰𝗸_𝗮𝗴𝗲𝗻𝘁_𝗿𝘂𝗻𝘁𝗶𝗺𝗲.𝗿𝗲𝘁𝗿𝗶𝗲𝘃𝗲 method, which takes the 𝗸𝗻𝗼𝘄𝗹𝗲𝗱𝗴𝗲𝗕𝗮𝘀𝗲𝗜𝗱 and a 𝗿𝗲𝘁𝗿𝗶𝗲𝘃𝗮𝗹𝗤𝘂𝗲𝗿𝘆 containing the user's question. By utilizing this method, the chatbot efficiently fetches pertinent information directly from the knowledge base, thereby enhancing performance and reducing latency.

𝗖𝗼𝗻𝘁𝗲𝘅𝘁𝘂𝗮𝗹 𝗥𝗲𝘀𝗽𝗼𝗻𝘀𝗲 𝗚𝗲𝗻𝗲𝗿𝗮𝘁𝗶𝗼𝗻: The retrieved information serves as contextual input for the large language model (LLM), specifically Amazon Bedrock's fully managed Titan-TG1 Large LLM services, which generate a coherent and accurate response tailored to the user's query. 

If you're interested in seeing this in action or exploring collaboration opportunities, feel free to reach out or try it out yourself!
🔗 Live App: https://lnkd.in/gVEJzM9c
