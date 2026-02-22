---
layout: description
title: Data Science
permalink: /datascience/
background-color: "#d7d7ff"
text-color: "#292121"
highlight-color: "#c47ee9"
font: "monospace"
---

# <center>DATA SCIENCE</center>

{:refdef: style="text-align: center;"}
![I'm doing data science](/images/me-datascience.png){: width="200px"}
{: refdef}

I’ve been working professionally in data science since 2021, mostly working on traditional Natural Language Processing, Transformer models, and more recently Diffusion models. Currently, I am the Machine Learning Engineer at QUT’s GenAI Lab [link]. I previously worked for the Australian government, and before that, livestreamed funerals (nothing to do with AI or data science, just some fun trivia).

CV Available here: LINK

---

## <center>HIGHLIGHT PROJECTS</center>

### BriX
One of the first projects I worked on at the QUT GenAI Lab - this is an API endpoint that takes your social media feed (twitter, facebook, or instagram) and then reranks the returned posts, with a few post injections, to make your feed more pro-social and less polarising (think left wing vs right wing social media feeds). This was a finalist in the Centre for Human AI ProSocial Ranking Challenge (LINK) in 2024. I didn’t design the actual algorithm(s) it/themselves, but I productionised the research code into a multi-container API endpoint that returned a post request in (generally) less than 500ms whilst running all algorithms on fairly cheap, air-gapped AWS instances (so no cheating with fancy expensive API calls to ChatGPT). Code available here

### Stable diffusion tutorial
A series of (hopefully) accessible jupyter notebook tutorials on the basic concepts of a latent diffusion model, specifically focusing on Stable Diffusion 1.4. This goes into each component (the text embedding, the denoising UNet, and the variational autoencoder) in great detail before mushing them all together into an image generation model. This is targeted to a non-technical audience, so hopefully it’s interesting to most people! Accessible here: (link)

### RAG Workshop and software
I put my hand up to run a RAG workshop for communications studies Post-graduate research students and early career researchers for the ADM+S and DMRC in 2025. At the time, there weren’t any particularly user-friendly build-it-yourself RAG softwares, especially for non-technical people (e.g. media and communications researchers). So, I decided to build a RAG GUI myself that ran entirely on-device so that I didn’t have to worry about scaling servers, API calls to third parties, and/or data sovereignty issues, since these students and ECRs would have come from all over the world. I ended up building this software: LINK, which runs from a standalone executable compiled by pyinstaller. The frontend is built in streamlit, the vector database backend is a local install of chromaDB, and the only external install requirement is an on-device install of Ollama. Code available here: LINK

### GenAI Arcade
A collab across the whole of QUT’s GenAI Lab, headed by Dr. Kevin Witzenberger and myself (specifically on the technical aspects). This is a self-guided learning website targeted towards non-technical people who are keen to know more about how GenAI works on the inside, not just prompting techniques and other commercial tips and tricks. We break down concepts like attention, system prompts, reinforcement learning context windows and the like, to help the average ChatGPT user understand why their chatbots might “behave” a certain way, or what they could be good and bad at. The frontend of this is built in Jekyll, and the backend currently sits across multiple huggingface spaces, although a move to serverless is currently in the works. Website viewable here: 

### Little Freaks
This is a silly offshoot of a project I made for QUT’s woodford folk festival stall in early 2025 as part of the Data Donation Project at the DMRC. Essentially the way it works is, it uses an unCLIP-like latent diffusion model (specifically karlo), and mixes the image embeddings of several images together using a weighted summation of each embedding, and then generates an output based on that weighted sum of embeddings. For the woodford folk festival, we mixed several pre-determined “persona” images into a single image based on how much your social media usage data reflects a “persona”. In the little freaks generator, I’ve just drawn 11 little freaks, and every time you hit generate, you get a random mixture of all 11. It’s surprisingly consistent, and very fun. Currently running on a CPU space on huggingface, so it’s extremely slow to generate anything - feel free to steal the code, I promise it’s fun, and runs pretty easily locally (if you have a GPU). Space viewable here: LINK. Code available here: LINK.

