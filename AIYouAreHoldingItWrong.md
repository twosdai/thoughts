# AI: Are We Holding It Wrong?

Articles, Videos, Thought-Pieces and other content around the web spend too much time on the same topic about AI. They focus on how AI is going to do one of the following:

- Take our jobs
- Threaten our humanity
- Bring about the singularity

These topics spawn an argument which comes to one of two conclusions depending on your philosophical stance.

1. "It's too dumb to do anything of _real_ value"
2. "AI is the singularity. _All praise the Basilisk_"

I fundamentally believe we are incorrectly discussing AI. We are not dispassionately thinking about AI as a tool, but as an eldrich horror bent on replacing us. I am not trying to convince you if AI will or will not replace our jobs, but I am trying to convince you we _collectively_ are talking about the wrong things. In essance it leads to us "holding it wrong". By missing the real use cases for it and then just moving on.

## AI is a tool

I was once asked to explain how AI will make the life of a salesperson or a teacher obsolete. To which I responded:

_"That is like asking how does a shovel find gold"_

The shovel is a tool, and it is not going to replace the gold miner. The shovel makes the gold miner more efficient, maybe at some point the shovel will be so efficient that the gold miner will not have to be deeply involved in the process, but the shovel will not, on its own, find gold. To elaborate further, AI cannot come up with new or novel ideas on its own. It can perform work, transform text or images, but it cannot fundementally create. In a recent Marques Brownlee video about Open AI's new generative video model `Sora` he said: 

_"I do not want to use the word Create here. These (AI Videos) are artifically generated from source material."_ - [Source](https://youtu.be/OY2x0TyKzIQ?si=YmCDyzhN49xSpOBT&t=285)

In essance, AI on its own cannot create. Only Transform. Will a system be built with AI that can handle our jobs in the future? No idea. Its not important. AI is a tool and when I realized its nothing more, I realized its real power and limitations. I began ignoring the "AI is going to replace us" argument, and instead focused on how to use AI in products I build and in my daily life. In this vein, I want to provide the two most powerful use cases I have found for AI as a tool. 

I believe there to be two core classifications of AI as a tool, which _feel_ functionally different. Even though they do the same underlying work.

1. AI as a transformer (Literally in the name for ChatGPT)
2. AI as a domain specific companion / assistant.

### AI as a transformer

Sometimes I have odd bits of text, data, or information I need categorized, processed, or otherwise transformed. AI is a great tool to reach for in this case. For example, If I have the raw HTML of a Job Posting. I can use AI to extract the text, and then use AI to transform it into a structured data format, such as JSON. See the following basic example where I use AI to create structured data from a Job Posting.

- [Job Posting Extraction](https://chatgpt.com/share/675905c9-6cd0-8007-a986-fadc14233b7a)
- [Segmenting a list of links](https://chatgpt.com/share/67590e9a-0818-8007-97cc-3eea4ccc0577)

Admittedly, these are very simple examples, but they show the power of AI as a tool, when given a good prompt, and some simple pre / post processing. Powerful applications can be built over a base layer of this tool. Frequently I use this case whenever I need to take in unstructured/semi-structured data, and transform it or classify it in some way. Typically beforehand pre-processing (Removing known noise, or formatting) is needed, and afterwards post processing (Validating the output, formatting the output, etc) is needed.

In the above cases, I manually did the pre processing, by only getting the relevant text from the webpage, and then post processing, by manually validating the output. But this reasonably could be programmed into a system.

### AI as a domain specific companion / assistant

My father is an educator, and has been experimenting with AI. He began using AI, by treating it like a companion. He would ask ChatGPT nicely to help him with his work, provide context, and then carry on a conversation with the model. While initially not wrong, he soon found that the model had hidden limitations. Such as a context window, or hallucinations. In the short term, it worked really well. The idea of an AI as a companion / assistant is a great use case for AI.

I am not an educator, but I have used AI in "Companion" mode. I have used it to help me with my work, such as the below example, where I was trying to understand the bcrypt npm library to a greater degree.

- [AI as a companion](https://chatgpt.com/share/67590689-f9a4-8007-a799-c90611b2683e)
- [Another case with DocumentDB Shard Questions](https://chatgpt.com/share/67590e4b-6cdc-8007-8846-995325a0fe47)
- [AI explaining some legal issue to me](https://chatgpt.com/share/67591073-1288-8007-9740-b0c2f78477ab)

I believe companion mode is fundamentally different from the general purpose transformer case above. In companion mode I am trying to learn something, read digestible information, and get sources for information. No longer do I need to dive through docs for hours, or spend time trying to understand a library. I can ask the AI to help me, and it will give me a good enough overview, and then provide sources for me to verify and dive deeper. The frequent case where I have the model go through websites, provide links and summarize information makes this case feel more like a companion than a transformer.

In companion mode, the best tips I can provide, are to be explicit that you want source references, and to provide enough domain context for the model. So if you have a few sentances on the type of researcher you are, or the type of devlopment you do. Drop it in at the beginning of your prompt.

For example I always start devlopment problems with:

`You are a ____ Expert. You understand the ____ domain. I am currently working on ____`
Then I will provide my actual question and ask explicitly for sources. Finally I end with:  `Provide links and sources for your answers.`

I know other people have written to death about prompt engineering, and prompt structure. But I feel like these simple two cases are the most important to understand.
## Conclusion

There might be other use cases, but after using it for a while, I believe that the two cases above are the most common. Beyond these two cases, if you draw the conclusion that AI is going to take your job, or that AI is going to cause a cataclysm, that is your conclusion. I don't think its really helpful. But I am not you.  

**Takeaway**: AI is just a tool, like a shovel. Let’s focus on when and how to use it effectively and then move on.


# Post Script Thoughts

### Aren't you afraid of an AI system taking your job?

 Deep down, I don't care if my job is replaced. I will leave my job someday and I will be fine. Priveledged take. I know. But really, I cannot control the future, but I can control how I react to it. So the question for my life is not if AI will take my job or if AI will cause an uncontrolable cataclysm, but how can I use AI to make me better and more efficient. Wasting headspace on fears about uncontrolable futures is a waste of time.

### Copilot

Another popular case I feel like I need to mention, which I used even to write this article, is to use AI as an "Autocomplete" tool.

- [Cursor](https://www.cursor.com/).
- [Github Copilot](https://github.com/features/copilot)

These tools work well; ultimately it's the same two cases as above in a more "ergonomic" form factor. I either have it transform some text, by giving it a general outline as I write. Or I ask it explicitly to explain / summarize / etc.
